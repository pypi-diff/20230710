# Comparing `tmp/env_logger-0.2.0.tar.gz` & `tmp/env_logger-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env_logger-0.2.0.tar", max compression
+gzip compressed data, was "env_logger-0.3.0.tar", max compression
```

## Comparing `env_logger-0.2.0.tar` & `env_logger-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-07-09 14:41:17.266011 env_logger-0.2.0/LICENSE
--rw-r--r--   0        0        0      927 2023-07-09 14:41:17.266011 env_logger-0.2.0/README.md
--rw-r--r--   0        0        0      526 2023-07-09 14:41:17.270011 env_logger-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4344 2023-07-09 14:41:17.270011 env_logger-0.2.0/src/env_logger/__init__.py
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 env_logger-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-10 20:13:35.375587 env_logger-0.3.0/LICENSE
+-rw-r--r--   0        0        0      791 2023-07-10 20:13:35.375587 env_logger-0.3.0/README.md
+-rw-r--r--   0        0        0      526 2023-07-10 20:13:35.407587 env_logger-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3667 2023-07-10 20:13:35.407587 env_logger-0.3.0/src/env_logger/__init__.py
+-rw-r--r--   0        0        0     4336 2023-07-10 20:13:35.407587 env_logger-0.3.0/src/env_logger/_handlers.py
+-rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 env_logger-0.3.0/PKG-INFO
```

### Comparing `env_logger-0.2.0/LICENSE` & `env_logger-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `env_logger-0.2.0/pyproject.toml` & `env_logger-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "env_logger"
-version = "0.2.0"
+version = "0.3.0"
 description = "The easy way to configure logging"
 license = "MIT"
 authors = ["AP Ljungquist <ap@ljungquist.eu>"]
 readme = "README.md"
 homepage = "https://github.com/apljungquist/env_logger_py"
```

### Comparing `env_logger-0.2.0/src/env_logger/__init__.py` & `env_logger-0.3.0/src/env_logger/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,19 @@
 from __future__ import annotations
 
 import argparse
-import json
 import logging
 import os
 import sys
-from typing import Optional, List, Callable, Any, Dict
+from typing import TYPE_CHECKING
 
-import colorama
+from . import _handlers
 
-logger = logging.getLogger(__name__)
-
-STYLES = {
-    logging.DEBUG: colorama.Fore.RESET + colorama.Style.DIM,
-    logging.INFO: colorama.Fore.RESET + colorama.Style.NORMAL,
-    logging.WARNING: colorama.Fore.YELLOW + colorama.Style.NORMAL,
-    logging.ERROR: colorama.Fore.RED + colorama.Style.NORMAL,
-    logging.CRITICAL: colorama.Fore.RED + colorama.Style.BRIGHT,
-}
-
-
-class Handler(logging.StreamHandler):
-    def __init__(self, *args, **kwargs) -> None:
-        self.style_output = kwargs.pop("style_output", True)
-        super().__init__(*args, **kwargs)
-
-    def format(self, record: logging.LogRecord) -> str:
-        default = super().format(record)
-        # TODO: Consider making configurable
-        escaped = json.dumps(default)[1:-1]
-        # TODO: Consider styling unnamed levels
-        colored = (
-            STYLES.get(record.levelno, "") + escaped + colorama.Style.RESET_ALL
-            if self.style_output
-            else escaped
-        )
-        return colored
+if TYPE_CHECKING:
+    from typing import Optional, List, Callable, Any, Dict
 
 
 def _resolve(
     kwargs: Dict[str, Any],
     key: str,
     from_env: Callable[[], Any],
     default: Callable[[], Any],
@@ -74,24 +48,38 @@
 
 
 def _valid_handlers(text: Optional[str]) -> Optional[List[logging.Handler]]:
     if text is None:
         return None
     if text == "rich":
         try:
-            import rich.logging
+            import rich.logging  # type: ignore
 
             return [rich.logging.RichHandler()]
         except ImportError as e:
             raise ValueError(
                 f"Invalid log handler: {text} (install rich to enable this handler)"
             ) from e
+    if text == "sparse":
+        return [_handlers.SparseColorHandler()]
     raise ValueError(f"Invalid log handler: {text}")
 
 
+def _default_format() -> str:
+    return "%(asctime)s %(levelname)s %(message)s"
+
+
+def _default_level() -> str:
+    return "INFO"
+
+
+def _default_handlers() -> List[logging.Handler]:
+    return [_handlers.Handler(style_output=_style_output())]
+
+
 def _style_output() -> bool:
     # Inspired by https://clig.dev/#output
     # But I disagree with the authors on using stderr for logging.
     if not sys.stderr.isatty():
         return False
     if os.environ.get("NO_COLOR", "0") != "0":
         return False
@@ -101,46 +89,47 @@
 
 
 def configure(**kwargs) -> None:
     _resolve(
         kwargs,
         "format",
         lambda: _valid_format(os.environ.get("LOG_FORMAT")),
-        lambda: "%(asctime)s %(levelname)s %(message)s",
+        _default_format,
     )
     _resolve(
         kwargs,
         "level",
         lambda: _valid_level(os.environ.get("LOG_LEVEL")),
-        lambda: "INFO",
+        _default_level,
     )
     _resolve(
         kwargs,
         "handlers",
         lambda: _valid_handlers(os.environ.get("LOG_HANDLER")),
-        lambda: [Handler(style_output=_style_output())],
+        _default_handlers,
     )
     logging.basicConfig(**kwargs)
 
 
-def _demo() -> None:
+def _log_samples(logger: logging.Logger) -> None:
     logger.debug("A debug message")
     logger.info("An info message")
-    logger.info(
-        "Another info message. This one contains special characters: \n\t\r\b\f\v\a..."
-    )
     logger.warning("A warning message")
     logger.error("An error message")
     logger.critical("A critical message")
     try:
         raise Exception("Oops")
     except Exception:
         logger.exception("A exception message")
 
 
+def _demo() -> None:
+    _log_samples(logging.getLogger(__name__))
+
+
 def _parser() -> argparse.ArgumentParser:
     root_parser = argparse.ArgumentParser(
         "env_logger",
         "Utility for configuring the Python logging module via environment variables.",
     )
     subparsers = root_parser.add_subparsers(required=True)
```

### Comparing `env_logger-0.2.0/PKG-INFO` & `env_logger-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-logger
-Version: 0.2.0
+Version: 0.3.0
 Summary: The easy way to configure logging
 Home-page: https://github.com/apljungquist/env_logger_py
 License: MIT
 Author: AP Ljungquist
 Author-email: ap@ljungquist.eu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -46,10 +46,7 @@
 import env_logger
 import rich.logging
 
 env_logger.configure(handlers=[rich.logging.RichHandler()])
 logging.getLogger(__name__).info("Hello!")
 ```
 
-The reason why `rich` not used by default is because it defaults to
-* writing to `stdout` instead of `stderr`
-* always printing colors.
```

