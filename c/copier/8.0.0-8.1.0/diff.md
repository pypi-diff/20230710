# Comparing `tmp/copier-8.0.0.tar.gz` & `tmp/copier-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copier-8.0.0.tar", max compression
+gzip compressed data, was "copier-8.1.0.tar", max compression
```

## Comparing `copier-8.0.0.tar` & `copier-8.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1076 2023-06-04 15:59:42.226863 copier-8.0.0/LICENSE
--rw-r--r--   0        0        0     6143 2023-06-04 15:59:42.226863 copier-8.0.0/README.md
--rw-r--r--   0        0        0      189 2023-06-04 15:59:56.982921 copier-8.0.0/copier/__init__.py
--rw-r--r--   0        0        0      198 2023-06-04 15:59:42.226863 copier-8.0.0/copier/__main__.py
--rw-r--r--   0        0        0    11786 2023-06-04 15:59:42.226863 copier-8.0.0/copier/cli.py
--rw-r--r--   0        0        0     3745 2023-06-04 15:59:42.226863 copier-8.0.0/copier/errors.py
--rw-r--r--   0        0        0    38198 2023-06-04 15:59:42.226863 copier-8.0.0/copier/main.py
--rw-r--r--   0        0        0     2476 2023-06-04 15:59:42.226863 copier-8.0.0/copier/subproject.py
--rw-r--r--   0        0        0    16594 2023-06-04 15:59:42.226863 copier-8.0.0/copier/template.py
--rw-r--r--   0        0        0     6234 2023-06-04 15:59:42.226863 copier-8.0.0/copier/tools.py
--rw-r--r--   0        0        0     2243 2023-06-04 15:59:42.226863 copier-8.0.0/copier/types.py
--rw-r--r--   0        0        0    17020 2023-06-04 15:59:42.226863 copier-8.0.0/copier/user_data.py
--rw-r--r--   0        0        0     6730 2023-06-04 15:59:42.226863 copier-8.0.0/copier/vcs.py
--rw-r--r--   0        0        0     3509 2023-06-04 15:59:56.978921 copier-8.0.0/pyproject.toml
--rw-r--r--   0        0        0     7718 1970-01-01 00:00:00.000000 copier-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-10 18:54:55.303518 copier-8.1.0/LICENSE
+-rw-r--r--   0        0        0     6148 2023-07-10 18:54:55.303518 copier-8.1.0/README.md
+-rw-r--r--   0        0        0      189 2023-07-10 18:55:10.196069 copier-8.1.0/copier/__init__.py
+-rw-r--r--   0        0        0      198 2023-07-10 18:54:55.303518 copier-8.1.0/copier/__main__.py
+-rw-r--r--   0        0        0    11797 2023-07-10 18:54:55.303518 copier-8.1.0/copier/cli.py
+-rw-r--r--   0        0        0     3745 2023-07-10 18:54:55.303518 copier-8.1.0/copier/errors.py
+-rw-r--r--   0        0        0    38292 2023-07-10 18:54:55.303518 copier-8.1.0/copier/main.py
+-rw-r--r--   0        0        0     2476 2023-07-10 18:54:55.303518 copier-8.1.0/copier/subproject.py
+-rw-r--r--   0        0        0    16376 2023-07-10 18:54:55.303518 copier-8.1.0/copier/template.py
+-rw-r--r--   0        0        0     6426 2023-07-10 18:54:55.303518 copier-8.1.0/copier/tools.py
+-rw-r--r--   0        0        0     2243 2023-07-10 18:54:55.303518 copier-8.1.0/copier/types.py
+-rw-r--r--   0        0        0    16678 2023-07-10 18:54:55.303518 copier-8.1.0/copier/user_data.py
+-rw-r--r--   0        0        0     6730 2023-07-10 18:54:55.303518 copier-8.1.0/copier/vcs.py
+-rw-r--r--   0        0        0     3512 2023-07-10 18:55:10.192069 copier-8.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7726 1970-01-01 00:00:00.000000 copier-8.1.0/PKG-INFO
```

### Comparing `copier-8.0.0/LICENSE` & `copier-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `copier-8.0.0/README.md` & `copier-8.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 ```
 
 To generate a project from the template:
 
 -   On the command-line:
 
     ```shell
-    copier path/to/project/template path/to/destination
+    copier copy path/to/project/template path/to/destination
     ```
 
 -   Or in Python code, programmatically:
 
     ```python
     from copier import run_copy
```

### Comparing `copier-8.0.0/copier/cli.py` & `copier-8.1.0/copier/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     )
     quiet = cli.Flag(["-q", "--quiet"], help="Suppress status output")
     prereleases = cli.Flag(
         ["-g", "--prereleases"],
         help="Use prereleases to compare template VCS tags.",
     )
     unsafe = cli.Flag(
-        ["--UNSAFE"],
+        ["--UNSAFE", "--trust"],
         help=(
             "Allow templates with unsafe features (Jinja extensions, migrations, tasks)"
         ),
     )
 
     @cli.switch(
         ["-d", "--data"],
```

### Comparing `copier-8.0.0/copier/errors.py` & `copier-8.1.0/copier/errors.py`

 * *Files identical despite different names*

### Comparing `copier-8.0.0/copier/main.py` & `copier-8.1.0/copier/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     CopierAnswersInterrupt,
     ExtensionNotFoundError,
     UnsafeTemplateError,
     UserMessageError,
 )
 from .subproject import Subproject
 from .template import Task, Template
-from .tools import Style, TemporaryDirectory, printf, readlink
+from .tools import OS, Style, TemporaryDirectory, printf, readlink
 from .types import (
     MISSING,
     AnyByStrDict,
     JSONSerializable,
     Literal,
     OptStr,
     RelativePath,
@@ -163,15 +163,15 @@
 
         quiet:
             When `True`, disable all output.
 
             See [quiet][].
 
         conflict:
-            One of "rej" (default), "inline" (still experimental).
+            One of "inline" (default), "rej".
 
         context_lines:
             Lines of context to consider when solving conflicts in updates.
 
             With more lines, context resolution is more accurate, but it will
             also produce more conflicts if your subproject has evolved.
 
@@ -194,18 +194,20 @@
     skip_if_exists: StrSeq = ()
     cleanup_on_error: bool = True
     defaults: bool = False
     user_defaults: AnyByStrDict = field(default_factory=dict)
     overwrite: bool = False
     pretend: bool = False
     quiet: bool = False
-    conflict: str = "inline"
+    conflict: Literal["inline", "rej"] = "inline"
     context_lines: PositiveInt = 3
     unsafe: bool = False
 
+    answers: AnswersMap = field(default_factory=AnswersMap, init=False)
+
     def __enter__(self):
         """Allow using worker as a context manager."""
         return self
 
     def __exit__(self, type, value, traceback):
         """Clean up garbage files after worker usage ends."""
         if value is not None:
@@ -251,14 +253,15 @@
             if value is not None:
                 answers[key] = value
         # Other data goes next
         answers.update(
             (str(k), v)
             for (k, v) in self.answers.combined.items()
             if not k.startswith("_")
+            and k not in self.answers.hidden
             and k not in self.template.secret_questions
             and k in self.template.questions_data
             and isinstance(k, JSONSerializable)
             and isinstance(v, JSONSerializable)
         )
         return answers
 
@@ -294,14 +297,15 @@
         conf = asdict(self)
         conf.update(
             {
                 "answers_file": self.answers_relpath,
                 "src_path": self.template.local_abspath,
                 "vcs_ref_hash": self.template.commit_hash,
                 "sep": os.sep,
+                "os": OS,
             }
         )
 
         return dict(
             DEFAULT_DATA,
             **self.answers.combined,
             _copier_answers=self._answers_to_remember(),
@@ -403,41 +407,38 @@
                 style=Style.IGNORE,
                 quiet=self.quiet,
                 file_=sys.stderr,
             )
             return True
         return self._solve_render_conflict(dst_relpath)
 
-    @cached_property
-    def answers(self) -> AnswersMap:
-        """Container of all answers to the questionary.
-
-        It asks the user the 1st time it is called, if running interactively.
-        """
+    def _ask(self) -> None:
+        """Ask the questions of the questionary and record their answers."""
         result = AnswersMap(
-            default=self.template.default_answers,
             user_defaults=self.user_defaults,
             init=self.data,
             last=self.subproject.last_answers,
             metadata=self.template.metadata,
         )
 
         for var_name, details in self.template.questions_data.items():
             question = Question(
                 answers=result,
                 jinja_env=self.jinja_env,
                 var_name=var_name,
                 **details,
             )
-            # Skip a question when the skip condition is met and remove any data
-            # from the answers map, so no answer for this question is recorded
-            # in the answers file.
+            # Skip a question when the skip condition is met.
             if not question.get_when():
-                result.remove(var_name)
-                continue
+                # Omit its answer from the answers file.
+                result.hide(var_name)
+                # Skip immediately to the next question when it has no default
+                # value.
+                if question.default is MISSING:
+                    continue
             if var_name in result.init:
                 # Try to parse the answer value.
                 answer = question.parse_answer(result.init[var_name])
                 # Try to validate the answer value if the question has a
                 # validator.
                 question.validate_answer(answer)
                 # At this point, the answer value is valid. Do not ask the
@@ -449,21 +450,22 @@
             try:
                 if self.defaults:
                     new_answer = question.get_default()
                     if new_answer is MISSING:
                         raise ValueError(f'Question "{var_name}" is required')
                 else:
                     new_answer = unsafe_prompt(
-                        [question.get_questionary_structure()], answers=result.combined
+                        [question.get_questionary_structure()],
+                        answers={question.var_name: question.get_default()},
                     )[question.var_name]
             except KeyboardInterrupt as err:
                 raise CopierAnswersInterrupt(result, question, self.template) from err
             result.user[var_name] = new_answer
 
-        return result
+        self.answers = result
 
     @cached_property
     def answers_relpath(self) -> Path:
         """Obtain the proper relative path for the answers file.
 
         It comes from:
 
@@ -724,14 +726,15 @@
         created. Otherwise, `src_path` be rendered
         directly into it, without worrying about evolving what was there
         already.
 
         See [generating a project][generating-a-project].
         """
         self._check_unsafe("copy")
+        self._ask()
         was_existing = self.subproject.local_abspath.exists()
         src_abspath = self.template_copy_root
         try:
             if not self.quiet:
                 # TODO Unify printing tools
                 print(
                     f"\nCopying from template version {self.template.version}",
@@ -852,15 +855,15 @@
                     diff = diff_cmd("--inter-hunk-context=0")
             # Run pre-migration tasks
             self._execute_tasks(
                 self.template.migration_tasks("before", self.subproject.template)
             )
             # Clear last answers cache to load possible answers migration
             with suppress(AttributeError):
-                del self.answers
+                self.answers = AnswersMap()
             with suppress(AttributeError):
                 del self.subproject.last_answers
             # Do a normal update in final destination
             self.run_copy()
             # Render with the same answers in an empty dir to avoid pollution
             new_worker = replace(
                 self,
@@ -876,15 +879,14 @@
             with local.cwd(subproject_top):
                 apply_cmd = git["apply", "--reject", "--exclude", self.answers_relpath]
                 for skip_pattern in chain(
                     self.skip_if_exists, self.template.skip_if_exists
                 ):
                     apply_cmd = apply_cmd["--exclude", skip_pattern]
                 (apply_cmd << diff)(retcode=None)
-                # TODO Test more, remove from experimental, make default
                 if self.conflict == "inline":
                     status = git("status", "--porcelain").strip().splitlines()
                     for line in status:
                         # Find merge rejections
                         if not (line.startswith("?? ") and line.endswith(".rej")):
                             continue
                         # FIXME Test with a file named '`â ñ"', see it fail, fix it
```

### Comparing `copier-8.0.0/copier/subproject.py` & `copier-8.1.0/copier/subproject.py`

 * *Files identical despite different names*

### Comparing `copier-8.0.0/copier/template.py` & `copier-8.1.0/copier/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,19 +278,14 @@
         """
         result = filter_config(self._raw_config)[0]
         with suppress(KeyError):
             verify_copier_version(result["min_copier_version"])
         return result
 
     @cached_property
-    def default_answers(self) -> AnyByStrDict:
-        """Get default answers for template's questions."""
-        return {key: value.get("default") for key, value in self.questions_data.items()}
-
-    @cached_property
     def envops(self) -> Mapping:
         """Get the Jinja configuration specified in the template, or default values.
 
         See [envops][].
         """
         result = self.config_data.get("envops", {})
         if "keep_trailing_newline" not in result:
```

### Comparing `copier-8.0.0/copier/tools.py` & `copier-8.1.0/copier/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Some utility functions."""
 
 import errno
 import os
+import platform
 import shutil
 import stat
 import sys
 import tempfile
 import warnings
 from contextlib import suppress
 from pathlib import Path
 from types import TracebackType
-from typing import Any, Callable, Optional, TextIO, Tuple, Union
+from typing import Any, Callable, Optional, TextIO, Tuple, Union, cast
 
 import colorama
 from packaging.version import Version
 from pydantic import StrictBool
 
-from .types import IntSeq
+from .types import IntSeq, Literal
 
 # TODO Remove condition when dropping python 3.8 support
 if sys.version_info < (3, 8):
     from importlib_metadata import version
 else:
     from importlib.metadata import version
 
@@ -36,15 +37,22 @@
     DANGER: IntSeq = [colorama.Fore.RED, colorama.Style.BRIGHT]
     RESET: IntSeq = [colorama.Fore.RESET, colorama.Style.RESET_ALL]
 
 
 INDENT = " " * 2
 HLINE = "-" * 42
 
-NO_VALUE: object = object()
+OS: Optional[Literal["linux", "macos", "windows"]] = cast(
+    Any,
+    {
+        "Linux": "linux",
+        "Darwin": "macos",
+        "Windows": "windows",
+    }.get(platform.system()),
+)
 
 
 def copier_version() -> Version:
     """Get closest match for the installed copier version."""
     # Importing __version__ at the top of the module creates a circular import
     # ("cannot import name '__version__' from partially initialized module 'copier'"),
     # so instead we do a lazy import here
```

### Comparing `copier-8.0.0/copier/types.py` & `copier-8.1.0/copier/types.py`

 * *Files identical despite different names*

### Comparing `copier-8.0.0/copier/user_data.py` & `copier-8.1.0/copier/user_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,62 +99,51 @@
             Data used to be able to reproduce the template.
 
             It comes from [copier.template.Template.metadata][].
 
         last:
             Data from [the answers file][the-copier-answersyml-file].
 
-        default:
-            Default data from the template.
-
-            See [copier.template.Template.default_answers][].
-
         user_defaults:
             Default data from the user e.g. previously completed and restored data.
 
             See [copier.main.Worker][].
     """
 
     # Private
-    removed: Set[str] = field(default_factory=set, init=False)
+    hidden: Set[str] = field(default_factory=set, init=False)
 
     # Public
     user: AnyByStrDict = field(default_factory=dict)
     init: AnyByStrDict = field(default_factory=dict)
     metadata: AnyByStrDict = field(default_factory=dict)
     last: AnyByStrDict = field(default_factory=dict)
     user_defaults: AnyByStrDict = field(default_factory=dict)
-    default: AnyByStrDict = field(default_factory=dict)
 
     @property
     def combined(self) -> Mapping[str, Any]:
         """Answers combined from different sources, sorted by priority."""
-        combined = dict(
+        return dict(
             ChainMap(
                 self.user,
                 self.init,
                 self.metadata,
                 self.last,
                 self.user_defaults,
-                self.default,
                 DEFAULT_DATA,
             )
         )
-        for key in self.removed:
-            if key in combined:
-                del combined[key]
-        return combined
 
     def old_commit(self) -> OptStr:
         """Commit when the project was updated from this template the last time."""
         return self.last.get("_commit")
 
-    def remove(self, key: str) -> None:
+    def hide(self, key: str) -> None:
         """Remove an answer by key."""
-        self.removed.add(key)
+        self.hidden.add(key)
 
 
 @dataclass(config=AllowArbitraryTypes)
 class Question:
     """One question asked to the user.
 
     All attributes are init kwargs.
```

### Comparing `copier-8.0.0/copier/vcs.py` & `copier-8.1.0/copier/vcs.py`

 * *Files identical despite different names*

### Comparing `copier-8.0.0/pyproject.toml` & `copier-8.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "copier"
 # This version is a placeholder autoupdated by poetry-dynamic-versioning
-version = "8.0.0"
+version = "8.1.0"
 description = "A library for rendering project templates."
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -35,15 +35,15 @@
 funcy = ">=1.17"
 importlib-metadata = { version = ">=3.4,<7.0", python = "<3.8" }
 jinja2 = ">=3.1.1"
 jinja2-ansible-filters = ">=1.3.1"
 packaging = ">=23.0"
 pathspec = ">=0.9.0"
 plumbum = ">=1.6.9"
-pydantic = ">=1.10.2"
+pydantic = ">=1.10.2,<2"
 pygments = ">=2.7.1"
 pyyaml = ">=5.3.1"
 pyyaml-include = ">=1.2"
 questionary = ">=1.8.1"
 typing-extensions = { version = ">=3.7.4,<5.0.0", python = "<3.8" }
 
 [tool.poetry.group.dev]
@@ -127,12 +127,12 @@
 ]
 
 [tool.commitizen]
 annotated_tag = true
 changelog_incremental = true
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "8.0.0"
+version = "8.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `copier-8.0.0/PKG-INFO` & `copier-8.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copier
-Version: 8.0.0
+Version: 8.1.0
 Summary: A library for rendering project templates.
 Home-page: https://github.com/copier-org/copier
 License: MIT
 Author: Ben Felder
 Author-email: ben@felder.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,15 @@
 Requires-Dist: funcy (>=1.17)
 Requires-Dist: importlib-metadata (>=3.4,<7.0) ; python_version < "3.8"
 Requires-Dist: jinja2 (>=3.1.1)
 Requires-Dist: jinja2-ansible-filters (>=1.3.1)
 Requires-Dist: packaging (>=23.0)
 Requires-Dist: pathspec (>=0.9.0)
 Requires-Dist: plumbum (>=1.6.9)
-Requires-Dist: pydantic (>=1.10.2)
+Requires-Dist: pydantic (>=1.10.2,<2)
 Requires-Dist: pygments (>=2.7.1)
 Requires-Dist: pyyaml (>=5.3.1)
 Requires-Dist: pyyaml-include (>=1.2)
 Requires-Dist: questionary (>=1.8.1)
 Requires-Dist: typing-extensions (>=3.7.4,<5.0.0) ; python_version < "3.8"
 Project-URL: Bug Tracker, https://github.com/copier-org/copier/issues
 Project-URL: Repository, https://github.com/copier-org/copier
@@ -100,15 +100,15 @@
 ```
 
 To generate a project from the template:
 
 -   On the command-line:
 
     ```shell
-    copier path/to/project/template path/to/destination
+    copier copy path/to/project/template path/to/destination
     ```
 
 -   Or in Python code, programmatically:
 
     ```python
     from copier import run_copy
```

