# Comparing `tmp/robotcode_plugin-0.46.0.tar.gz` & `tmp/robotcode_plugin-0.47.0.tar.gz`

## Comparing `robotcode_plugin-0.46.0.tar` & `robotcode_plugin-0.47.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 robotcode_plugin-0.46.0/src/robotcode/plugin/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_plugin-0.46.0/src/robotcode/plugin/__version__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 robotcode_plugin-0.46.0/src/robotcode/plugin/manager.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_plugin-0.46.0/src/robotcode/plugin/py.typed
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 robotcode_plugin-0.46.0/src/robotcode/plugin/specs.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 robotcode_plugin-0.46.0/src/robotcode/plugin/click_helper/aliases.py
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 robotcode_plugin-0.46.0/src/robotcode/plugin/click_helper/options.py
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 robotcode_plugin-0.46.0/src/robotcode/plugin/click_helper/types.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_plugin-0.46.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_plugin-0.46.0/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_plugin-0.46.0/README.md
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 robotcode_plugin-0.46.0/pyproject.toml
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 robotcode_plugin-0.46.0/PKG-INFO
+-rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.0/src/robotcode/plugin/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.0/src/robotcode/plugin/__version__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.0/src/robotcode/plugin/manager.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.0/src/robotcode/plugin/py.typed
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.0/src/robotcode/plugin/specs.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.0/src/robotcode/plugin/click_helper/aliases.py
+-rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.0/src/robotcode/plugin/click_helper/options.py
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.0/src/robotcode/plugin/click_helper/types.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.0/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.0/README.md
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.0/pyproject.toml
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.0/PKG-INFO
```

### Comparing `robotcode_plugin-0.46.0/src/robotcode/plugin/__init__.py` & `robotcode_plugin-0.47.0/src/robotcode/plugin/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -216,15 +216,15 @@
             )
             click.echo(text, color=color if color is not None else self.colored)
         else:
             click.echo_via_pager(text_or_generator, color=color if color is not None else self.colored)
 
     def keyboard_interrupt(self) -> None:
         self.verbose("Aborted!", file=sys.stderr)
-        raise SystemExit(253)
+        sys.exit(253)
 
     def exit(self, code: int = 0) -> None:
         self.verbose(f"Exit with code {code}")
-        raise SystemExit(code)
+        sys.exit(code)
 
 
 pass_application = click.make_pass_decorator(Application, ensure=True)
```

### Comparing `robotcode_plugin-0.46.0/src/robotcode/plugin/manager.py` & `robotcode_plugin-0.47.0/src/robotcode/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.46.0/src/robotcode/plugin/click_helper/aliases.py` & `robotcode_plugin-0.47.0/src/robotcode/plugin/click_helper/aliases.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.46.0/src/robotcode/plugin/click_helper/options.py` & `robotcode_plugin-0.47.0/src/robotcode/plugin/click_helper/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Sequence, Set, Tuple
+from typing import List, Optional, Sequence, Set, Tuple
 
 import click
 from robotcode.core.types import ServerMode
 from robotcode.plugin import Application
 from robotcode.plugin.click_helper.types import (
     AddressesPort,
     AddressParamType,
@@ -11,19 +11,21 @@
     MutuallyExclusiveOption,
     NameParamType,
     PortParamType,
 )
 
 from .types import FC
 
+# mypy: disable-error-code="attr-defined"
+
 
 def server_options(
     default_server_mode: ServerMode, default_port: int, allowed_server_modes: Optional[Set[ServerMode]] = None
 ) -> Sequence[FC]:
-    result = []
+    result: List[FC] = []
 
     def exclusive(option_name: str, *args: ServerMode) -> Sequence[str]:
         return (
             [option_name]
             if not allowed_server_modes or any(True for arg in args if arg in allowed_server_modes)
             else []
         )
```

### Comparing `robotcode_plugin-0.46.0/src/robotcode/plugin/click_helper/types.py` & `robotcode_plugin-0.47.0/src/robotcode/plugin/click_helper/types.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.46.0/.gitignore` & `robotcode_plugin-0.47.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.46.0/LICENSE.txt` & `robotcode_plugin-0.47.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.46.0/README.md` & `robotcode_plugin-0.47.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.46.0/pyproject.toml` & `robotcode_plugin-0.47.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.46.0/PKG-INFO` & `robotcode_plugin-0.47.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-plugin
-Version: 0.46.0
+Version: 0.47.0
 Summary: Some classes for RobotCode plugin management
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
 Author-email: Daniel Biehl <dbiehl@live.de>
```

