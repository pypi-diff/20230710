# Comparing `tmp/flynt-0.78.tar.gz` & `tmp/flynt-1.0.0.tar.gz`

## Comparing `flynt-0.78.tar` & `flynt-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,36 @@
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/__init__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/__main__.py
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/api.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/ast_chunk.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/cli.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/cli_messages.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/exceptions.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/format.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/module.py
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/process.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/pyproject_finder.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/state.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/utils.py
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/lexer/Chunk.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/lexer/PyToken.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/lexer/__init__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/lexer/context.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/lexer/split.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/linting/__init__.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/linting/fstr_lint.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/static_join/__init__.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/static_join/candidates.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/static_join/transformer.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/static_join/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/string_concat/__init__.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/string_concat/candidates.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/string_concat/string_in_string.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/string_concat/transformer.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/transform/FstringifyTransformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/transform/__init__.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/transform/format_call_transforms.py
--rw-r--r--   0        0        0     7984 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/transform/percent_transformer.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/transform/transform.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 flynt-0.78/src/flynt/transform/util.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 flynt-0.78/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flynt-0.78/LICENSE
--rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 flynt-0.78/README.md
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 flynt-0.78/pyproject.toml
--rw-r--r--   0        0        0     9041 2020-02-02 00:00:00.000000 flynt-0.78/PKG-INFO
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/__init__.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/__main__.py
+-rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/api.py
+-rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/cli.py
+-rw-r--r--   0        0        0     9634 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/code_editor.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/exceptions.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/candidates/__init__.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/candidates/ast_call_candidates.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/candidates/ast_chunk.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/candidates/ast_percent_candidates.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/linting/__init__.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/linting/fstr_lint.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/static_join/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/static_join/candidates.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/static_join/transformer.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/static_join/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/string_concat/__init__.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/string_concat/candidates.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/string_concat/string_in_string.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/string_concat/transformer.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/transform/FstringifyTransformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/transform/__init__.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/transform/format_call_transforms.py
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/transform/percent_transformer.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/transform/transform.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/transform/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/utils/__init__.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/utils/format.py
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/utils/pyproject_finder.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/utils/utils.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 flynt-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flynt-1.0.0/LICENSE
+-rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 flynt-1.0.0/README.md
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 flynt-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9357 2020-02-02 00:00:00.000000 flynt-1.0.0/PKG-INFO
```

### Comparing `flynt-0.78/src/flynt/api.py` & `flynt-1.0.0/src/flynt/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import ast
 import codecs
 import dataclasses
 import logging
 import os
 import sys
 import time
+import traceback
 from difflib import unified_diff
 from typing import Collection, List, Optional, Tuple
 
 import astor
 
-from flynt.cli_messages import farewell_message
-from flynt.process import (
+from flynt.code_editor import (
     fstringify_code_by_line,
     fstringify_concats,
     fstringify_static_joins,
 )
 from flynt.state import State
 
 log = logging.getLogger(__name__)
@@ -43,15 +43,15 @@
     with open(filename, encoding=encoding, newline="") as f:
         try:
             contents = f.read()
         except UnicodeDecodeError:
             log.error(f"Exception while reading {filename}", exc_info=True)
             return None
 
-    result = fstringify_content(
+    result = fstringify_code(
         contents=contents,
         state=state,
         filename=filename,
     )
 
     if result is None:
         return None
@@ -70,19 +70,20 @@
         with open(filename, "wb") as outf:
             if bom is not None:
                 outf.write(bom)
             outf.write(new_code.encode(encoding))
     return result
 
 
-def fstringify_content(
+def fstringify_code(
     contents: str,
     state: State,
     filename: str = "<code>",
 ) -> Optional[FstringifyResult]:
+    """transform given string, assuming it's python code."""
     try:
         ast_before = ast.parse(contents)
     except SyntaxError:
         log.exception(f"Can't parse {filename} as a python file.")
         return None
 
     try:
@@ -90,27 +91,39 @@
         changes = 0
         if state.transform_percent or state.transform_format:
             new_code, changes = fstringify_code_by_line(
                 contents,
                 state=state,
             )
         if state.transform_concat:
-            new_code, concat_changes = fstringify_concats(
-                new_code,
-                state=state,
-            )
-            changes += concat_changes
-            state.concat_changes += concat_changes
+            try:
+                new_code, concat_changes = fstringify_concats(
+                    new_code,
+                    state=state,
+                )
+            except Exception:
+                msg = traceback.format_exc()
+                log.error("Transforming concatenation of literal strings failed")
+                log.error(msg)
+            else:
+                changes += concat_changes
+                state.concat_changes += concat_changes
         if state.transform_join:
-            new_code, join_changes = fstringify_static_joins(
-                new_code,
-                state=state,
-            )
-            changes += join_changes
-            state.join_changes += join_changes
+            try:
+                new_code, join_changes = fstringify_static_joins(
+                    new_code,
+                    state=state,
+                )
+            except Exception:
+                msg = traceback.format_exc()
+                log.error("Transforming concatenation of literal strings failed")
+                log.error(msg)
+            else:
+                changes += join_changes
+                state.join_changes += join_changes
 
     except Exception as e:
         msg = str(e) or e.__class__.__name__
         log.warning(
             f"Skipping fstrings transform of file {filename} due to {msg}.",
             exc_info=True,
         )
@@ -144,14 +157,15 @@
     return result
 
 
 def fstringify_files(
     files: List[str],
     state: State,
 ) -> int:
+    """apply transforms to sequence of files, keep shared stats."""
     changed_files = 0
     total_charcount_original = 0
     total_charcount_new = 0
     total_expressions = 0
     start_time = time.time()
     for path in files:
         result = _fstringify_file(
@@ -180,14 +194,21 @@
             total_expressions,
             total_time,
         )
 
     return changed_files
 
 
+farewell_message = (
+    "Please run your tests before committing. Did flynt get a perfect conversion? give it a star at: "
+    "\n~ https://github.com/ikamensh/flynt ~"
+    "\nThank you for using flynt. Upgrade more projects and recommend it to your colleagues!\n"
+)
+
+
 def _print_report(
     state: State,
     found_files: int,
     changed_files: int,
     total_cc_new: int,
     total_cc_original: int,
     total_expr: int,
```

### Comparing `flynt-0.78/src/flynt/ast_chunk.py` & `flynt-1.0.0/src/flynt/candidates/ast_chunk.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Uses py3.8 AST to define a chunk of code as an AST node."""
 
 import ast
 
-from flynt.format import QuoteTypes
-
 
 class AstChunk:
     def __init__(self, node: ast.AST) -> None:
         self.node = node
 
     @property
     def start_line(self) -> int:
@@ -30,23 +28,19 @@
         return lineno - 1
 
     @property
     def n_lines(self) -> int:
         return 1 + self.end_line - self.start_line
 
     @property
-    def string_in_string(self) -> bool:
-        return False
-
-    @property
     def quote_type(self) -> str:
-        return QuoteTypes.double
+        raise NotImplementedError
 
     def __str__(self) -> str:
-        from flynt.utils import ast_to_string
+        from flynt.utils.utils import ast_to_string
 
         src = ast_to_string(self.node)
         if src.startswith("(") and src.endswith(")"):
             src = src[1:-1]
         return src
 
     def __repr__(self) -> str:
```

### Comparing `flynt-0.78/src/flynt/cli.py` & `flynt-1.0.0/src/flynt/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import logging
 import os
 import sys
 import warnings
 from typing import List, Optional
 
 from flynt import __version__
-from flynt.api import fstringify, fstringify_content
-from flynt.pyproject_finder import find_pyproject_toml, parse_pyproject_toml
+from flynt.api import fstringify, fstringify_code
 from flynt.state import State
+from flynt.utils.pyproject_finder import find_pyproject_toml, parse_pyproject_toml
 
 
 def main():
     return sys.exit(run_flynt_cli())
 
 
 def run_flynt_cli(arglist: Optional[List[str]] = None) -> int:
@@ -52,14 +52,15 @@
         "-ll",
         "--line-length",
         action="store",
         help="for expressions spanning multiple lines, convert only if "
         "the resulting single line will fit into the line length limit. "
         "Default value is 88 characters.",
         default=88,
+        type=int,
     )
 
     group = parser.add_mutually_exclusive_group()
     group.add_argument(
         "-d",
         "--dry-run",
         action="store_true",
@@ -194,24 +195,24 @@
 
     state = state_from_args(args)
     if args.verbose:
         logging.getLogger("flynt").setLevel(logging.DEBUG)
 
     if args.string:
         content = " ".join(args.src)
-        result = fstringify_content(
+        result = fstringify_code(
             content,
             state,
         )
         print(result.content if result else content)
         return 0
     if "-" in args.src:
         if len(args.src) > 1:
             parser.error("Cannot use '-' with a list of other paths")
-        result = fstringify_content(
+        result = fstringify_code(
             sys.stdin.read()[: -len(os.linesep)],
             state,
             filename="<stdin>",
         )
         if not result:
             return 1
         print(result.content)
```

### Comparing `flynt-0.78/src/flynt/process.py` & `flynt-1.0.0/src/flynt/code_editor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 import logging
 import re
 import string
 import sys
-from functools import partial
-from typing import Callable, List, Optional, Tuple, Union
+from functools import lru_cache, partial
+from typing import Callable, List, Optional, Tuple
 
-from flynt.ast_chunk import AstChunk
+from flynt.candidates.ast_call_candidates import call_candidates
+from flynt.candidates.ast_chunk import AstChunk
+from flynt.candidates.ast_percent_candidates import percent_candidates
 from flynt.exceptions import FlyntException
-from flynt.format import QuoteTypes as qt
-from flynt.format import get_quote_type
-from flynt.lexer import split
-from flynt.lexer.Chunk import Chunk
 from flynt.state import State
 from flynt.static_join.candidates import join_candidates
 from flynt.static_join.transformer import transform_join
 from flynt.string_concat.candidates import concat_candidates
 from flynt.string_concat.transformer import transform_concat
 from flynt.transform.transform import transform_chunk
+from flynt.utils.format import QuoteTypes as qt
+from flynt.utils.format import get_quote_type
+from flynt.utils.utils import contains_comment
 
 noqa_regex = re.compile("#[ ]*noqa.*flynt")
 
 log = logging.getLogger(__name__)
 
 
-class JoinTransformer:
-    """JoinTransformer fills up the resulting code by tracking
-    the last line number and char index. Failed transformations do not need to do anything -
-    not adding results is safe, as original code will be filled in."""
+class CodeEditor:
+    """CodeEditor applies local edits, and keeps most of the original code.
+
+    As parsing and unparsing a file risks unintended changes ( escaped chars,
+    formatting quirks, etc.), we try to keep most characters of the original,
+    and only inject our edits on relevant locations.
+
+    This class uses variable functions to identify candidate edit locations,
+    tries to apply edits on candidates. The candidates factory must return candidates in
+    the same order as they occur in the code (first line to last line, left to right chars).
+    Given this property, whenever we decide to transform each candidate or not, we can
+    add all code to the left of candidate to the result as there will be no edits there;
+    and then append the optionally transformed candidate expression. After processing last
+    candidate, we can add the rest of the file.
+    """
 
     def __init__(
         self,
         code: str,
         len_limit: Optional[int],
         candidates_iter_factory: Callable,
         transform_func: Callable,
@@ -45,26 +57,52 @@
 
         self.results: List[str] = []
         self.count_expressions = 0
 
         self.last_line = 0
         self.last_idx = 0
         self.used_up = False
+        self.output: Optional[str] = None
 
-    def fstringify_code_by_line(self) -> Tuple[str, int]:
+    def edit(self) -> Tuple[str, int]:
+        """Apply edits to the original code."""
         assert not self.used_up, "Tried to use JT twice."
         for chunk in self.candidates_iter:
             self.fill_up_to(chunk)
             self.try_chunk(chunk)
 
         self.add_rest()
         self.used_up = True
-        return "".join(self.results)[:-1], self.count_expressions
+        self.output = "".join(self.results)[:-1]
+        return self.output, self.count_expressions
+
+    def code_between(
+        self, start_line: int, start_idx: int, end_line: int, end_idx: int
+    ) -> str:
+        """get source code in the original between two locations."""
+        assert end_line >= start_line
+        result = []
+        if start_line == end_line:
+            assert end_idx >= start_idx
+            result.append(self.src_lines[start_line][start_idx:end_idx])
+        else:
+            result.append(self.src_lines[start_line][start_idx:])
+            full_lines = range(start_line + 1, end_line)
+            for line in full_lines:
+                result.append(self.src_lines[line])
+            result.append(self.src_lines[end_line][:end_idx])
+        return "\n".join(result)
+
+    @lru_cache(None)
+    def code_in_chunk(self, chunk: AstChunk):
+        return self.code_between(
+            chunk.start_line, chunk.start_idx, chunk.end_line, chunk.end_idx
+        )
 
-    def fill_up_to(self, chunk: Union[Chunk, AstChunk]) -> None:
+    def fill_up_to(self, chunk: AstChunk) -> None:
         start_line, start_idx, _ = (chunk.start_line, chunk.start_idx, chunk.end_idx)
         if start_line == self.last_line:
             self.results.append(
                 self.src_lines[self.last_line][self.last_idx : start_idx],
             )
         else:
             self.results.append(self.src_lines[self.last_line][self.last_idx :] + "\n")
@@ -72,55 +110,69 @@
             line = self.src_lines[start_line]
 
             self.fill_up_to_line(start_line)
             self.results.append(line[:start_idx])
 
         self.last_idx = start_idx
 
-    def fill_up_to_line(self, start_line: int) -> None:
-        while self.last_line < start_line:
+    def fill_up_to_line(self, line: int) -> None:
+        while self.last_line < line:
             self.results.append(self.src_lines[self.last_line] + "\n")
             self.last_line += 1
 
-    def try_chunk(self, chunk: Union[Chunk, AstChunk]) -> None:
+    def try_chunk(self, chunk: AstChunk) -> None:
+        """Try applying a transform to a chunk of code.
+
+        Transformation function is free to decide to refuse conversion,
+        e.g. in edge cases that are not supported."""
 
-        for line in self.src_lines[chunk.start_line : chunk.start_line + chunk.n_lines]:
+        # if a chunk has a comment in it, we should abort.
+        if contains_comment(self.code_in_chunk(chunk)):
+            return
+
+        # skip raw strings
+        if self.code_in_chunk(chunk)[0] == "r":
+            return
+
+        # skip lines with # noqa comment
+        for line in self.src_lines[chunk.start_line : chunk.end_line + 1]:
             if noqa_regex.findall(line):
-                # user does not wish for this line to be converted.
                 return
 
         try:
-            quote_type = (
-                qt.double
-                if chunk.string_in_string and chunk.n_lines == 1
-                else chunk.quote_type
-            )
+            quote_type = get_quote_type(self.code_in_chunk(chunk))
         except FlyntException:
             quote_type = qt.double
 
-        converted, changed = self.transform_func(str(chunk), quote_type=quote_type)
+        converted, changed = self.transform_func(chunk.node, quote_type=quote_type)
         if changed:
             contract_lines = chunk.n_lines - 1
             if contract_lines == 0:
                 line = self.src_lines[chunk.start_line]
                 rest = line[chunk.end_idx :]
             else:
                 next_line = self.src_lines[chunk.start_line + contract_lines]
                 rest = next_line[chunk.end_idx :]
             self.maybe_replace(chunk, contract_lines, converted, rest)
 
     def maybe_replace(
         self,
-        chunk: Union[Chunk, AstChunk],
+        chunk: AstChunk,
         contract_lines: int,
         converted: str,
         rest: str,
     ) -> None:
+        """Given a possible edit, see if we want to apply it.
+
+        For example, we might not want to change multiple lines."""
         if contract_lines:
-            if get_quote_type(str(chunk)) in (qt.triple_double, qt.triple_single):
+            if get_quote_type(self.code_in_chunk(chunk)) in (
+                qt.triple_double,
+                qt.triple_single,
+            ):
                 lines = converted.split("\\n")
                 lines[-1] += rest
                 lines_fit = all(
                     len(line) <= self.len_limit - chunk.start_idx for line in lines
                 )
                 converted = converted.replace("\\n", "\n")
             else:
@@ -170,19 +222,26 @@
         self.last_line += 1
 
         while len(self.src_lines) > self.last_line:
             self.results.append(self.src_lines[self.last_line] + "\n")
             self.last_line += 1
 
 
+def fstring_candidates(code, state):
+    chunks = percent_candidates(code, state) + call_candidates(code, state)
+    chunks.sort(key=lambda c: (c.start_line, c.start_idx))
+    return chunks
+
+
 def fstringify_code_by_line(code: str, state: State) -> Tuple[str, int]:
     """returns fstringified version of the code and amount of lines edited."""
+
     return _transform_code(
         code,
-        partial(split.get_fstringify_chunks, lexer_context=state.lexer_context),
+        partial(fstring_candidates, state=state),
         partial(transform_chunk, state=state),
         state,
     )
 
 
 def fstringify_concats(code: str, state: State) -> Tuple[str, int]:
     """replace string literal concatenations with f-string expressions."""
@@ -207,13 +266,13 @@
 def _transform_code(
     code: str,
     candidates_iter_factory: Callable,
     transform_func: Callable,
     state: State,
 ) -> Tuple[str, int]:
     """returns fstringified version of the code and amount of lines edited."""
-    return JoinTransformer(
+    return CodeEditor(
         code,
         state.len_limit,
         candidates_iter_factory,
         transform_func,
-    ).fstringify_code_by_line()
+    ).edit()
```

### Comparing `flynt-0.78/src/flynt/pyproject_finder.py` & `flynt-1.0.0/src/flynt/utils/pyproject_finder.py`

 * *Files identical despite different names*

### Comparing `flynt-0.78/src/flynt/utils.py` & `flynt-1.0.0/src/flynt/utils/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import ast
-from typing import Optional
+import io
+import tokenize
+from typing import Optional, Union
 
 import astor
 from astor.string_repr import pretty_string
 
 from flynt.exceptions import ConversionRefused
-from flynt.format import QuoteTypes, set_quote_type
 from flynt.linting.fstr_lint import FstrInliner
+from flynt.utils.format import QuoteTypes, set_quote_type
 
 
 def nicer_pretty_string(
     s,
     embedded,
     current_line,
     uni_lit=False,
@@ -31,33 +33,67 @@
 
 
 def is_str_literal(node: ast.AST) -> bool:
     """Returns True if a node is a string literal. f-string is also a string literal."""
     return isinstance(node, (ast.Str, ast.JoinedStr))
 
 
+class StringInStringVisitor(ast.NodeVisitor):
+    def __init__(self):
+        self.string_in_string = False
+        self.in_fmt_value = False
+
+    def visit_FormattedValue(self, node):
+        if self.in_fmt_value:
+            self.generic_visit(node.value)
+            return
+
+        self.in_fmt_value = True
+        self.generic_visit(node.value)
+        self.in_fmt_value = False
+
+    def visit_JoinedStr(self, node):
+        if self.in_fmt_value:
+            self.string_in_string = True
+        self.generic_visit(node)
+
+    def visit_Str(self, node):
+        if self.in_fmt_value:
+            self.string_in_string = True
+
+
+def str_in_str(node: ast.AST) -> bool:
+    sisv = StringInStringVisitor()
+    sisv.visit(node)
+    return sisv.string_in_string
+
+
 def ast_formatted_value(
     val: ast.AST,
     fmt_str: Optional[str] = None,
     conversion: Optional[str] = None,
-) -> ast.FormattedValue:
+) -> Union[ast.FormattedValue, ast.Str]:
     if isinstance(val, ast.FormattedValue):
         return val
 
     if ast_to_string(val).startswith("{"):
         raise ConversionRefused(
             "values starting with '{' are better left not transformed.",
         )
 
     if fmt_str:
         format_spec = ast.JoinedStr([ast_string_node(fmt_str)])
     else:
         format_spec = None
 
     conversion_val = -1 if conversion is None else ord(conversion.replace("!", ""))
+
+    if format_spec is None and isinstance(val, ast.Str):
+        return val
+
     return ast.FormattedValue(
         value=val,
         conversion=conversion_val,
         format_spec=format_spec,
     )
 
 
@@ -73,7 +109,15 @@
         if new_code[:4] == 'f"""' or new_code[:3] == "'''" or new_code[:3] == '"""':
             quote_type = QuoteTypes.double
     if quote_type is not None:
         new_code = set_quote_type(new_code, quote_type)
     new_code = new_code.replace("\n", "\\n")
     new_code = new_code.replace("\t", "\\t")
     return new_code
+
+
+def contains_comment(code: str) -> bool:
+    tokens = tokenize.generate_tokens(io.StringIO(code).readline)
+    for token in tokens:
+        if token.type == tokenize.COMMENT:
+            return True
+    return False
```

### Comparing `flynt-0.78/src/flynt/linting/fstr_lint.py` & `flynt-1.0.0/src/flynt/linting/fstr_lint.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ast
 from typing import List
 
-from flynt.ast_chunk import AstChunk
+from flynt.candidates.ast_chunk import AstChunk
 
 
 class FstringFinder(ast.NodeVisitor):
     def __init__(self) -> None:
         super().__init__()
         self.victims: List[AstChunk] = []
```

### Comparing `flynt-0.78/src/flynt/static_join/candidates.py` & `flynt-1.0.0/src/flynt/static_join/candidates.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ast
 from typing import List
 
-from flynt.ast_chunk import AstChunk
+from flynt.candidates.ast_chunk import AstChunk
 from flynt.state import State
 from flynt.static_join.utils import get_static_join_bits
 
 
 class JoinHound(ast.NodeVisitor):
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `flynt-0.78/src/flynt/static_join/transformer.py` & `flynt-1.0.0/src/flynt/static_join/transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ast
 from typing import List, Tuple
 
 from flynt.static_join.utils import get_static_join_bits
-from flynt.utils import ast_formatted_value, ast_string_node, fixup_transformed
+from flynt.utils.utils import ast_formatted_value, ast_string_node, fixup_transformed
 
 
 class JoinTransformer(ast.NodeTransformer):
     def __init__(self):
         super().__init__()
         self.counter = 0
 
@@ -35,14 +35,13 @@
                     for arg in args_with_interleaved_joiner
                     if isinstance(arg, ast.Str)
                 ),
             )
         return ast.JoinedStr(args_with_interleaved_joiner)
 
 
-def transform_join(code: str, *args, **kwargs) -> Tuple[str, bool]:
-    tree = ast.parse(f"({code})")
+def transform_join(tree: ast.AST, *args, **kwargs) -> Tuple[str, bool]:
 
     jt = JoinTransformer()
     jt.visit(tree)
     new_code = fixup_transformed(tree)
     return new_code, jt.counter > 0
```

### Comparing `flynt-0.78/src/flynt/static_join/utils.py` & `flynt-1.0.0/src/flynt/static_join/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ast
 from typing import List, Optional, Sequence, Tuple
 
-from flynt.utils import is_str_literal
+from flynt.utils.utils import is_str_literal
 
 
 def get_joiner_from_static_join(func: ast.AST) -> Optional[str]:
     if (
         isinstance(func, ast.Attribute)
         and func.attr == "join"
         and is_str_literal(func.value)
```

### Comparing `flynt-0.78/src/flynt/string_concat/candidates.py` & `flynt-1.0.0/src/flynt/string_concat/candidates.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
-from typing import Generator, List
+from typing import Iterable, List
 
-from flynt.ast_chunk import AstChunk
+from flynt.candidates.ast_chunk import AstChunk
 from flynt.state import State
-from flynt.utils import is_str_literal
+from flynt.utils.utils import is_str_literal
 
 
 def is_string_concat(node: ast.AST) -> bool:
     """Returns True for nodes representing a string concatenation."""
     if is_str_literal(node):
         return True
     if isinstance(node, ast.BinOp) and isinstance(node.op, ast.Add):
@@ -26,16 +26,16 @@
         """
         if is_string_concat(node):
             self.victims.append(AstChunk(node))
         else:
             self.generic_visit(node)
 
 
-def concat_candidates(code: str, state: State) -> Generator[AstChunk, None, None]:
+def concat_candidates(code: str, state: State) -> Iterable[AstChunk]:
     tree = ast.parse(code)
 
     ch = ConcatHound()
     ch.visit(tree)
 
     state.concat_candidates += len(ch.victims)
 
-    yield from ch.victims
+    return ch.victims
```

### Comparing `flynt-0.78/src/flynt/string_concat/string_in_string.py` & `flynt-1.0.0/src/flynt/string_concat/string_in_string.py`

 * *Files identical despite different names*

### Comparing `flynt-0.78/src/flynt/string_concat/transformer.py` & `flynt-1.0.0/src/flynt/string_concat/transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
 from typing import List, Tuple
 
 from flynt.string_concat.candidates import is_string_concat
 from flynt.string_concat.string_in_string import check_sns_depth
-from flynt.utils import ast_formatted_value, ast_string_node, fixup_transformed
+from flynt.utils.utils import ast_formatted_value, ast_string_node, fixup_transformed
 
 
 def unpack_binop(node: ast.BinOp) -> List[ast.AST]:
     assert isinstance(node, ast.BinOp)
     result = []
 
     if isinstance(node.left, ast.BinOp):
@@ -57,15 +57,14 @@
                 segments.append(ast_string_node(p.value))
             else:
                 segments.append(ast_formatted_value(p))
 
         return ast.JoinedStr(segments)
 
 
-def transform_concat(code: str, *args, **kwargs) -> Tuple[str, bool]:
-    tree = ast.parse(f"({code})")
+def transform_concat(tree: ast.AST, *args, **kwargs) -> Tuple[str, bool]:
 
     ft = ConcatTransformer()
-    ft.visit(tree)
-    new_code = fixup_transformed(tree)
+    new = ft.visit(tree)
+    new_code = fixup_transformed(new)
 
     return new_code, ft.counter > 0
```

### Comparing `flynt-0.78/src/flynt/transform/FstringifyTransformer.py` & `flynt-1.0.0/src/flynt/transform/FstringifyTransformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 import ast
 from typing import Tuple
 
+from flynt.candidates.ast_call_candidates import is_call_format
 from flynt.linting.fstr_lint import FstrInliner
 from flynt.state import State
-from flynt.transform.format_call_transforms import joined_string, matching_call
+from flynt.transform.format_call_transforms import joined_string
 from flynt.transform.percent_transformer import is_percent_stringify, transform_binop
 
 
 class FstringifyTransformer(ast.NodeTransformer):
     def __init__(
         self,
         state: State,
     ) -> None:
         super().__init__()
         self.state = state
         self.counter = 0
-        self.string_in_string = False
 
     def visit_Call(self, node: ast.Call) -> ast.AST:
         """
         Convert `ast.Call` to `ast.JoinedStr` f-string.
         """
-        if self.state.transform_format and matching_call(node):
+        if self.state.transform_format and is_call_format(node):
             self.state.call_candidates += 1
 
             # bail in these edge cases...
             if any(isinstance(arg, ast.Starred) for arg in node.args):
                 return node
 
-            result_node, str_in_str = joined_string(
+            result_node = joined_string(
                 node,
                 aggressive=self.state.aggressive,
             )
-            self.string_in_string = str_in_str
             self.visit(result_node)
             self.counter += 1
             self.state.call_transforms += 1
             return result_node
 
         return node
 
@@ -66,29 +65,28 @@
                 # f-string expression part cannot include a backslash
                 if isinstance(ch, ast.Str) and (
                     any(x in ch.s for x in ("\n", "\t", "\r", "'", '"', "%s", "%%"))
                     or "\\" in ch.s
                 ):
                     return node
 
-            result_node, str_in_str = transform_binop(
+            result_node = transform_binop(
                 node,
                 aggressive=self.state.aggressive,
             )
-            self.string_in_string = str_in_str
             self.counter += 1
             self.state.percent_transforms += 1
             return result_node
 
         return node
 
 
 def fstringify_node(
     node: ast.AST,
     state: State,
-) -> Tuple[ast.AST, bool, bool]:
+) -> Tuple[ast.AST, bool]:
     ft = FstringifyTransformer(state)
     result = ft.visit(node)
     il = FstrInliner()
     il.visit(result)
 
-    return result, ft.counter > 0, ft.string_in_string
+    return result, ft.counter > 0
```

### Comparing `flynt-0.78/src/flynt/transform/percent_transformer.py` & `flynt-1.0.0/src/flynt/transform/percent_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ast
 import re
 from collections import deque
-from typing import List, Tuple
+from typing import List, Union
 
 from flynt.exceptions import ConversionRefused, FlyntException
 from flynt.transform.format_call_transforms import ast_formatted_value, ast_string_node
 
 FORMATS = "diouxXeEfFgGcrsa"
 
 FORMAT_GROUP = f"[hlL]?[{FORMATS}]"
@@ -44,15 +44,15 @@
 
 def formatted_value(
     fmt_prefix: str,
     fmt_spec: str,
     val: ast.AST,
     *,
     aggressive: bool = False,
-) -> ast.FormattedValue:
+) -> Union[ast.FormattedValue, ast.Str]:
     if fmt_spec in integer_specificers:
         fmt_prefix = fmt_prefix.replace(".", "0")
 
     if fmt_spec in conversion_methods:
         if not aggressive and fmt_prefix:
             raise ConversionRefused(
                 "Default text alignment has changed between percent fmt and fstrings. "
@@ -182,15 +182,15 @@
 
     return ast.JoinedStr(segments)
 
 
 def transform_generic(
     node: ast.BinOp,
     aggressive: bool = False,
-) -> Tuple[ast.JoinedStr, bool]:
+) -> ast.JoinedStr:
     """Convert a `BinOp` `%` formatted str with a unknown name on the `node.right` to an f-string.
 
     When `node.right` is a Name since we don't know if it's a single var or a dict so we sniff the string.
 
     Sniffs the left string for Dict style usage
     e.g. `"val: %(key_name1)s val2: %(key_name2)s" % some_dict`
 
@@ -198,23 +198,21 @@
     Borrow the core logic by injecting the name into a ast.Tuple
 
     Returns ast.JoinedStr (f-string), bool: str-in-str
     """
     assert isinstance(node.left, ast.Str)
     has_dict_str_format = DICT_PATTERN.findall(node.left.s)
     if has_dict_str_format:
-        return transform_dict(node, aggressive=aggressive), True
+        return transform_dict(node, aggressive=aggressive)
 
-    # if it's just a name then pretend it's tuple to use that code
-    str_in_str = any(
-        isinstance(n, (ast.Str, ast.JoinedStr)) for n in ast.walk(node.right)
-    )
+    any(isinstance(n, (ast.Str, ast.JoinedStr)) for n in ast.walk(node.right))
 
+    # if it's just a name then pretend it's tuple to use that code
     node.right = ast.Tuple(elts=[node.right])
-    return transform_tuple(node, aggressive=aggressive), str_in_str
+    return transform_tuple(node, aggressive=aggressive)
 
 
 supported_operands = [
     ast.Name,
     ast.Attribute,
     ast.Str,
     ast.Subscript,
@@ -224,22 +222,19 @@
 ]
 
 
 def transform_binop(
     node: ast.BinOp,
     *,
     aggressive: bool = False,
-) -> Tuple[ast.JoinedStr, bool]:
+) -> ast.JoinedStr:
     if isinstance(node.right, tuple(supported_operands)):
         return transform_generic(node, aggressive=aggressive)
 
     if isinstance(node.right, ast.Tuple):
-        return (
-            transform_tuple(node, aggressive=aggressive),
-            any(isinstance(n, (ast.Str, ast.JoinedStr)) for n in ast.walk(node.right)),
-        )
+        return transform_tuple(node, aggressive=aggressive)
 
     if isinstance(node.right, ast.Dict):
         # todo adapt transform dict to Dict literal
-        return transform_dict(node, aggressive=aggressive), False
+        return transform_dict(node, aggressive=aggressive)
 
     raise ConversionRefused(f"Unsupported `node.right` class: {type(node.right)}")
```

### Comparing `flynt-0.78/src/flynt/transform/util.py` & `flynt-1.0.0/src/flynt/transform/util.py`

 * *Files identical despite different names*

### Comparing `flynt-0.78/LICENSE` & `flynt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flynt-0.78/README.md` & `flynt-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,39 +31,44 @@
 
 ### Command line options
 
 From the output of `flynt -h`:
 
 <!-- begin-options -->
 ```
-usage: flynt [-h] [-v | -q] [--no-multiline | -ll LINE_LENGTH] [-d]
-             [-s] [--no-tp] [--no-tf] [-tc] [-tj] [-f] [-a]
-             [-e EXCLUDE [EXCLUDE ...]] [--version]
+usage: flynt [-h] [-v | -q] [--no-multiline | -ll LINE_LENGTH]
+             [-d | --stdout] [-s] [--no-tp] [--no-tf] [-tc] [-tj]
+             [-f] [-a] [-e EXCLUDE [EXCLUDE ...]] [--version]
              [src ...]
 
-flynt v.0.77-beta
+flynt v.0.78
 
 positional arguments:
   src                   source file(s) or directory (or a single `-`
                         to read stdin and output to stdout)
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -v, --verbose         run with verbose output
-  -q, --quiet           run without stdout output
+  -q, --quiet           run without outputting statistics to stdout
   --no-multiline        convert only single line expressions
   -ll LINE_LENGTH, --line-length LINE_LENGTH
                         for expressions spanning multiple lines,
                         convert only if the resulting single line
                         will fit into the line length limit. Default
                         value is 88 characters.
   -d, --dry-run         Do not change the files in-place and print
                         the diff instead. Note that this must be
                         used in conjunction with '--fail-on-change'
                         when used for linting purposes.
+  --stdout              Do not change the files in-place and print
+                        the result instead. This argument implies
+                        --quiet, i.e. no statistics are printed to
+                        stdout, only the resulting code. It is
+                        incompatible with --dry-run and --verbose.
   -s, --string          Interpret the input as a Python code snippet
                         and print the converted version. The snippet
                         must use single quotes or escaped double
                         quotes.
   --no-tp, --no-transform-percent
                         Don't transform % formatting to f-strings
                         (default: do so)
```

#### html2text {}

```diff
@@ -9,44 +9,48 @@
 using flynt.* To run: `flynt {source_file_or_directory}` * Given a single file,
 it will 'f-stringify' it: replace all applicable string formatting in this file
 (file will be modified). * Given a folder, it will search the folder
 recursively and f-stringify all the .py files it finds. It skips some hard-
 coded folder names: `blacklist = {'.tox', 'venv', 'site-packages', '.eggs'}`.
 It turns the code it runs on into Python 3.6+, since 3.6 is when "f-strings"
 were introduced. ### Command line options From the output of `flynt -h`:  ```
-usage: flynt [-h] [-v | -q] [--no-multiline | -ll LINE_LENGTH] [-d] [-s] [--no-
-tp] [--no-tf] [-tc] [-tj] [-f] [-a] [-e EXCLUDE [EXCLUDE ...]] [--version] [src
-...] flynt v.0.77-beta positional arguments: src source file(s) or directory
-(or a single `-` to read stdin and output to stdout) options: -h, --help show
-this help message and exit -v, --verbose run with verbose output -q, --quiet
-run without stdout output --no-multiline convert only single line expressions -
-ll LINE_LENGTH, --line-length LINE_LENGTH for expressions spanning multiple
-lines, convert only if the resulting single line will fit into the line length
-limit. Default value is 88 characters. -d, --dry-run Do not change the files
-in-place and print the diff instead. Note that this must be used in conjunction
-with '--fail-on-change' when used for linting purposes. -s, --string Interpret
-the input as a Python code snippet and print the converted version. The snippet
-must use single quotes or escaped double quotes. --no-tp, --no-transform-
-percent Don't transform % formatting to f-strings (default: do so) --no-tf, --
-no-transform-format Don't transform .format formatting to f-strings (default:
-do so) -tc, --transform-concats Replace string concatenations (defined as +
-operations involving string literals) with f-strings. Available only if flynt
-is installed with 3.8+ interpreter. -tj, --transform-joins Replace static joins
-(where the joiner is a string literal and the joinee is a static- length list)
-with f-strings. Available only if flynt is installed with 3.8+ interpreter. -f,
---fail-on-change Fail when changing files (for linting purposes) -a, --
-aggressive Include conversions with potentially changed behavior. -e EXCLUDE
-[EXCLUDE ...], --exclude EXCLUDE [EXCLUDE ...] ignore files with given strings
-in it's absolute path. --version Print the current version number and exit. ```
-### Sample output of a successful run: ``` 38f9d3a65222:~ ikkamens$ git clone
-https://github.com/pallets/flask.git Cloning into 'flask'... ... Resolving
-deltas: 100% (12203/12203), done. 38f9d3a65222:open_source ikkamens$ flynt
-flask Running flynt v.0.40 Flynt run has finished. Stats: Execution time:
-0.789s Files modified: 21 Character count reduction: 299 (0.06%) Per expression
-type: Old style (`%`) expressions attempted: 40/42 (95.2%) `.format(...)` calls
+usage: flynt [-h] [-v | -q] [--no-multiline | -ll LINE_LENGTH] [-d | --stdout]
+[-s] [--no-tp] [--no-tf] [-tc] [-tj] [-f] [-a] [-e EXCLUDE [EXCLUDE ...]] [--
+version] [src ...] flynt v.0.78 positional arguments: src source file(s) or
+directory (or a single `-` to read stdin and output to stdout) optional
+arguments: -h, --help show this help message and exit -v, --verbose run with
+verbose output -q, --quiet run without outputting statistics to stdout --no-
+multiline convert only single line expressions -ll LINE_LENGTH, --line-length
+LINE_LENGTH for expressions spanning multiple lines, convert only if the
+resulting single line will fit into the line length limit. Default value is 88
+characters. -d, --dry-run Do not change the files in-place and print the diff
+instead. Note that this must be used in conjunction with '--fail-on-change'
+when used for linting purposes. --stdout Do not change the files in-place and
+print the result instead. This argument implies --quiet, i.e. no statistics are
+printed to stdout, only the resulting code. It is incompatible with --dry-run
+and --verbose. -s, --string Interpret the input as a Python code snippet and
+print the converted version. The snippet must use single quotes or escaped
+double quotes. --no-tp, --no-transform-percent Don't transform % formatting to
+f-strings (default: do so) --no-tf, --no-transform-format Don't transform
+.format formatting to f-strings (default: do so) -tc, --transform-concats
+Replace string concatenations (defined as + operations involving string
+literals) with f-strings. Available only if flynt is installed with 3.8+
+interpreter. -tj, --transform-joins Replace static joins (where the joiner is a
+string literal and the joinee is a static- length list) with f-strings.
+Available only if flynt is installed with 3.8+ interpreter. -f, --fail-on-
+change Fail when changing files (for linting purposes) -a, --aggressive Include
+conversions with potentially changed behavior. -e EXCLUDE [EXCLUDE ...], --
+exclude EXCLUDE [EXCLUDE ...] ignore files with given strings in it's absolute
+path. --version Print the current version number and exit. ``` ### Sample
+output of a successful run: ``` 38f9d3a65222:~ ikkamens$ git clone https://
+github.com/pallets/flask.git Cloning into 'flask'... ... Resolving deltas: 100%
+(12203/12203), done. 38f9d3a65222:open_source ikkamens$ flynt flask Running
+flynt v.0.40 Flynt run has finished. Stats: Execution time: 0.789s Files
+modified: 21 Character count reduction: 299 (0.06%) Per expression type: Old
+style (`%`) expressions attempted: 40/42 (95.2%) `.format(...)` calls
 attempted: 26/33 (78.8%) F-string expressions created: 48 Out of all attempted
 transforms, 7 resulted in errors. To find out specific error messages, use --
 verbose flag. _-_._-_._-_._-_._-_._-_._-_._-_._-_._-_._-_._-_._-_._-_._-_._-
 _._-_._-_._-_._-_._-_._-_._-_._-_._-_. Please run your tests before committing.
 Did flynt get a perfect conversion? give it a star at: ~ https://github.com/
 ikamensh/flynt ~ Thank you for using flynt. Upgrade more projects and recommend
 it to your colleagues! 38f9d3a65222:~ ikkamens$ ``` ### Pre-commit hook To make
```

### Comparing `flynt-0.78/pyproject.toml` & `flynt-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 keywords = [
     "strings",
     "utility",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
@@ -51,17 +50,46 @@
 path = "src/flynt/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/src",
 ]
 
-[tool.bandit]
-exclude_dirs = ["test"]
-skips = ["B101"]
-
 [tool.mypy]
 exclude = "test/integration/(actual|expected|samples).*"
 
 [[tool.mypy.overrides]]
 module = "astor"
 ignore_missing_imports = true
+
+[tool.ruff]
+extend-select = [
+    "C9",
+    "I",
+    "PLR091",
+    "S",
+]
+extend-ignore = [
+    "S101",
+]
+line-length = 141
+target-version = "py37"
+
+[tool.ruff.mccabe]
+max-complexity = 22
+
+[tool.ruff.pylint]
+max-args = 7
+max-branches = 18
+max-statements = 67
+
+[tool.ruff.per-file-ignores]
+"test/*" = ["I"]
+"test/integration/*" = [
+    "F523",
+    "F821",
+    "F841",
+    "I",
+ ]
+"test/test_lexer.py" = ["F841"]
+"test/test_pyproject.py" = ["E712"]
+"test/test_styles.py" = ["S311"]
```

### Comparing `flynt-0.78/PKG-INFO` & `flynt-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: flynt
-Version: 0.78
+Version: 1.0.0
 Summary: CLI tool to convert a python project's %-formatted strings to f-strings.
 Project-URL: Homepage, https://github.com/ikamensh/flynt
 Author: Ilya Kamenshchikov
 License-Expression: MIT
 License-File: LICENSE
 Keywords: strings,utility
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
@@ -60,39 +59,44 @@
 
 ### Command line options
 
 From the output of `flynt -h`:
 
 <!-- begin-options -->
 ```
-usage: flynt [-h] [-v | -q] [--no-multiline | -ll LINE_LENGTH] [-d]
-             [-s] [--no-tp] [--no-tf] [-tc] [-tj] [-f] [-a]
-             [-e EXCLUDE [EXCLUDE ...]] [--version]
+usage: flynt [-h] [-v | -q] [--no-multiline | -ll LINE_LENGTH]
+             [-d | --stdout] [-s] [--no-tp] [--no-tf] [-tc] [-tj]
+             [-f] [-a] [-e EXCLUDE [EXCLUDE ...]] [--version]
              [src ...]
 
-flynt v.0.77-beta
+flynt v.0.78
 
 positional arguments:
   src                   source file(s) or directory (or a single `-`
                         to read stdin and output to stdout)
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -v, --verbose         run with verbose output
-  -q, --quiet           run without stdout output
+  -q, --quiet           run without outputting statistics to stdout
   --no-multiline        convert only single line expressions
   -ll LINE_LENGTH, --line-length LINE_LENGTH
                         for expressions spanning multiple lines,
                         convert only if the resulting single line
                         will fit into the line length limit. Default
                         value is 88 characters.
   -d, --dry-run         Do not change the files in-place and print
                         the diff instead. Note that this must be
                         used in conjunction with '--fail-on-change'
                         when used for linting purposes.
+  --stdout              Do not change the files in-place and print
+                        the result instead. This argument implies
+                        --quiet, i.e. no statistics are printed to
+                        stdout, only the resulting code. It is
+                        incompatible with --dry-run and --verbose.
   -s, --string          Interpret the input as a Python code snippet
                         and print the converted version. The snippet
                         must use single quotes or escaped double
                         quotes.
   --no-tp, --no-transform-percent
                         Don't transform % formatting to f-strings
                         (default: do so)
```

#### html2text {}

```diff
@@ -1,66 +1,70 @@
-Metadata-Version: 2.1 Name: flynt Version: 0.78 Summary: CLI tool to convert a
+Metadata-Version: 2.1 Name: flynt Version: 1.0.0 Summary: CLI tool to convert a
 python project's %-formatted strings to f-strings. Project-URL: Homepage,
 https://github.com/ikamensh/flynt Author: Ilya Kamenshchikov License-
 Expression: MIT License-File: LICENSE Keywords: strings,utility Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Topic :: Utilities Requires-Python:
->=3.7 Requires-Dist: astor Requires-Dist: tomli>=1.1.0; python_version < '3.11'
-Provides-Extra: dev Requires-Dist: build; extra == 'dev' Requires-Dist: pre-
-commit; extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist:
-pytest-cov; extra == 'dev' Requires-Dist: twine; extra == 'dev' Description-
-Content-Type: text/markdown # flynt - string formatting converter
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Utilities Requires-Python: >=3.7 Requires-Dist: astor Requires-Dist:
+tomli>=1.1.0; python_version < '3.11' Provides-Extra: dev Requires-Dist: build;
+extra == 'dev' Requires-Dist: pre-commit; extra == 'dev' Requires-Dist: pytest;
+extra == 'dev' Requires-Dist: pytest-cov; extra == 'dev' Requires-Dist: twine;
+extra == 'dev' Description-Content-Type: text/markdown # flynt - string
+formatting converter
     [Actions_Status] [License:_MIT] [PyPI] [Downloads] [Code_style:_black]
 `flynt` is a command line tool to automatically convert a project's Python code
 from old "%-formatted" and .format(...) strings into Python 3.6+'s "f-strings".
 F-Strings: > Not only are they more readable, more concise, and less prone to
 error than other ways of formatting, but they are also faster! ### Installation
 `pip install flynt`. It requires Python version 3.7+. ### Usage *Flynt will
 modify the files it runs on. Add your project to version control system before
 using flynt.* To run: `flynt {source_file_or_directory}` * Given a single file,
 it will 'f-stringify' it: replace all applicable string formatting in this file
 (file will be modified). * Given a folder, it will search the folder
 recursively and f-stringify all the .py files it finds. It skips some hard-
 coded folder names: `blacklist = {'.tox', 'venv', 'site-packages', '.eggs'}`.
 It turns the code it runs on into Python 3.6+, since 3.6 is when "f-strings"
 were introduced. ### Command line options From the output of `flynt -h`:  ```
-usage: flynt [-h] [-v | -q] [--no-multiline | -ll LINE_LENGTH] [-d] [-s] [--no-
-tp] [--no-tf] [-tc] [-tj] [-f] [-a] [-e EXCLUDE [EXCLUDE ...]] [--version] [src
-...] flynt v.0.77-beta positional arguments: src source file(s) or directory
-(or a single `-` to read stdin and output to stdout) options: -h, --help show
-this help message and exit -v, --verbose run with verbose output -q, --quiet
-run without stdout output --no-multiline convert only single line expressions -
-ll LINE_LENGTH, --line-length LINE_LENGTH for expressions spanning multiple
-lines, convert only if the resulting single line will fit into the line length
-limit. Default value is 88 characters. -d, --dry-run Do not change the files
-in-place and print the diff instead. Note that this must be used in conjunction
-with '--fail-on-change' when used for linting purposes. -s, --string Interpret
-the input as a Python code snippet and print the converted version. The snippet
-must use single quotes or escaped double quotes. --no-tp, --no-transform-
-percent Don't transform % formatting to f-strings (default: do so) --no-tf, --
-no-transform-format Don't transform .format formatting to f-strings (default:
-do so) -tc, --transform-concats Replace string concatenations (defined as +
-operations involving string literals) with f-strings. Available only if flynt
-is installed with 3.8+ interpreter. -tj, --transform-joins Replace static joins
-(where the joiner is a string literal and the joinee is a static- length list)
-with f-strings. Available only if flynt is installed with 3.8+ interpreter. -f,
---fail-on-change Fail when changing files (for linting purposes) -a, --
-aggressive Include conversions with potentially changed behavior. -e EXCLUDE
-[EXCLUDE ...], --exclude EXCLUDE [EXCLUDE ...] ignore files with given strings
-in it's absolute path. --version Print the current version number and exit. ```
-### Sample output of a successful run: ``` 38f9d3a65222:~ ikkamens$ git clone
-https://github.com/pallets/flask.git Cloning into 'flask'... ... Resolving
-deltas: 100% (12203/12203), done. 38f9d3a65222:open_source ikkamens$ flynt
-flask Running flynt v.0.40 Flynt run has finished. Stats: Execution time:
-0.789s Files modified: 21 Character count reduction: 299 (0.06%) Per expression
-type: Old style (`%`) expressions attempted: 40/42 (95.2%) `.format(...)` calls
+usage: flynt [-h] [-v | -q] [--no-multiline | -ll LINE_LENGTH] [-d | --stdout]
+[-s] [--no-tp] [--no-tf] [-tc] [-tj] [-f] [-a] [-e EXCLUDE [EXCLUDE ...]] [--
+version] [src ...] flynt v.0.78 positional arguments: src source file(s) or
+directory (or a single `-` to read stdin and output to stdout) optional
+arguments: -h, --help show this help message and exit -v, --verbose run with
+verbose output -q, --quiet run without outputting statistics to stdout --no-
+multiline convert only single line expressions -ll LINE_LENGTH, --line-length
+LINE_LENGTH for expressions spanning multiple lines, convert only if the
+resulting single line will fit into the line length limit. Default value is 88
+characters. -d, --dry-run Do not change the files in-place and print the diff
+instead. Note that this must be used in conjunction with '--fail-on-change'
+when used for linting purposes. --stdout Do not change the files in-place and
+print the result instead. This argument implies --quiet, i.e. no statistics are
+printed to stdout, only the resulting code. It is incompatible with --dry-run
+and --verbose. -s, --string Interpret the input as a Python code snippet and
+print the converted version. The snippet must use single quotes or escaped
+double quotes. --no-tp, --no-transform-percent Don't transform % formatting to
+f-strings (default: do so) --no-tf, --no-transform-format Don't transform
+.format formatting to f-strings (default: do so) -tc, --transform-concats
+Replace string concatenations (defined as + operations involving string
+literals) with f-strings. Available only if flynt is installed with 3.8+
+interpreter. -tj, --transform-joins Replace static joins (where the joiner is a
+string literal and the joinee is a static- length list) with f-strings.
+Available only if flynt is installed with 3.8+ interpreter. -f, --fail-on-
+change Fail when changing files (for linting purposes) -a, --aggressive Include
+conversions with potentially changed behavior. -e EXCLUDE [EXCLUDE ...], --
+exclude EXCLUDE [EXCLUDE ...] ignore files with given strings in it's absolute
+path. --version Print the current version number and exit. ``` ### Sample
+output of a successful run: ``` 38f9d3a65222:~ ikkamens$ git clone https://
+github.com/pallets/flask.git Cloning into 'flask'... ... Resolving deltas: 100%
+(12203/12203), done. 38f9d3a65222:open_source ikkamens$ flynt flask Running
+flynt v.0.40 Flynt run has finished. Stats: Execution time: 0.789s Files
+modified: 21 Character count reduction: 299 (0.06%) Per expression type: Old
+style (`%`) expressions attempted: 40/42 (95.2%) `.format(...)` calls
 attempted: 26/33 (78.8%) F-string expressions created: 48 Out of all attempted
 transforms, 7 resulted in errors. To find out specific error messages, use --
 verbose flag. _-_._-_._-_._-_._-_._-_._-_._-_._-_._-_._-_._-_._-_._-_._-_._-
 _._-_._-_._-_._-_._-_._-_._-_._-_._-_. Please run your tests before committing.
 Did flynt get a perfect conversion? give it a star at: ~ https://github.com/
 ikamensh/flynt ~ Thank you for using flynt. Upgrade more projects and recommend
 it to your colleagues! 38f9d3a65222:~ ikkamens$ ``` ### Pre-commit hook To make
```

