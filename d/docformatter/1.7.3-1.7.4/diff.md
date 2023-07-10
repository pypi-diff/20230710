# Comparing `tmp/docformatter-1.7.3.tar.gz` & `tmp/docformatter-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docformatter-1.7.3.tar", max compression
+gzip compressed data, was "docformatter-1.7.4.tar", max compression
```

## Comparing `docformatter-1.7.3.tar` & `docformatter-1.7.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.7.3/LICENSE
--rw-r--r--   0        0        0     6864 2023-06-06 14:28:12.772135 docformatter-1.7.3/README.rst
--rw-r--r--   0        0        0     6343 2023-06-23 01:50:08.112575 docformatter-1.7.3/pyproject.toml
--rw-r--r--   0        0        0     1614 2023-06-06 14:28:12.798136 docformatter-1.7.3/src/docformatter/__init__.py
--rwxr-xr-x   0        0        0     6417 2023-06-23 01:50:08.112575 docformatter-1.7.3/src/docformatter/__main__.py
--rw-r--r--   0        0        0     1191 2023-06-23 01:50:08.113575 docformatter-1.7.3/src/docformatter/__pkginfo__.py
--rw-r--r--   0        0        0    13592 2023-06-07 03:06:35.282648 docformatter-1.7.3/src/docformatter/configuration.py
--rw-r--r--   0        0        0     3717 2023-06-23 01:50:08.113575 docformatter-1.7.3/src/docformatter/encode.py
--rw-r--r--   0        0        0    21057 2023-06-23 01:50:08.113575 docformatter-1.7.3/src/docformatter/format.py
--rw-r--r--   0        0        0     6998 2023-06-06 14:28:12.821136 docformatter-1.7.3/src/docformatter/strings.py
--rw-r--r--   0        0        0    28407 2023-06-23 01:50:08.114575 docformatter-1.7.3/src/docformatter/syntax.py
--rw-r--r--   0        0        0     4573 2023-04-28 16:27:48.980570 docformatter-1.7.3/src/docformatter/util.py
--rw-r--r--   0        0        0     8257 1970-01-01 00:00:00.000000 docformatter-1.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.7.4/LICENSE
+-rw-r--r--   0        0        0     6864 2023-06-06 14:28:12.772135 docformatter-1.7.4/README.rst
+-rw-r--r--   0        0        0     6352 2023-07-10 13:44:42.178415 docformatter-1.7.4/pyproject.toml
+-rw-r--r--   0        0        0     1614 2023-06-06 14:28:12.798136 docformatter-1.7.4/src/docformatter/__init__.py
+-rwxr-xr-x   0        0        0     6417 2023-06-23 16:31:57.338250 docformatter-1.7.4/src/docformatter/__main__.py
+-rw-r--r--   0        0        0     1191 2023-07-10 13:44:42.178415 docformatter-1.7.4/src/docformatter/__pkginfo__.py
+-rw-r--r--   0        0        0    13592 2023-06-07 03:06:35.282648 docformatter-1.7.4/src/docformatter/configuration.py
+-rw-r--r--   0        0        0     3717 2023-06-23 17:25:42.338248 docformatter-1.7.4/src/docformatter/encode.py
+-rw-r--r--   0        0        0    21006 2023-07-07 02:43:16.864063 docformatter-1.7.4/src/docformatter/format.py
+-rw-r--r--   0        0        0     6998 2023-06-06 14:28:12.821136 docformatter-1.7.4/src/docformatter/strings.py
+-rw-r--r--   0        0        0    28451 2023-07-10 13:44:42.178415 docformatter-1.7.4/src/docformatter/syntax.py
+-rw-r--r--   0        0        0     4573 2023-04-28 16:27:48.980570 docformatter-1.7.4/src/docformatter/util.py
+-rw-r--r--   0        0        0     8266 1970-01-01 00:00:00.000000 docformatter-1.7.4/PKG-INFO
```

### Comparing `docformatter-1.7.3/LICENSE` & `docformatter-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.3/README.rst` & `docformatter-1.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.3/pyproject.toml` & `docformatter-1.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "docformatter"
-version = "1.7.3"
+version = "1.7.4"
 description = "Formats docstrings to follow PEP 257"
 authors = ["Steven Myint"]
 maintainers = [
     "Doyle Rowland <doyle.rowland@reliaqual.com>",
 ]
 license = "Expat"
 readme = "README.rst"
 homepage = "https://github.com/PyCQA/docformatter"
 repository = "https://github.com/PyCQA/docformatter"
-documentation = "https://github.com/PyCQA/docformatter"
+documentation = "https://docformatter.readthedocs.io/en/latest/"
 keywords = [
     "PEP 257", "pep257", "style", "formatter", "docstrings",
 ]
 classifiers=[
           'Intended Audience :: Developers',
           'Environment :: Console',
           'Programming Language :: Python :: 3',
```

### Comparing `docformatter-1.7.3/src/docformatter/__init__.py` & `docformatter-1.7.4/src/docformatter/__init__.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.3/src/docformatter/__main__.py` & `docformatter-1.7.4/src/docformatter/__main__.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.3/src/docformatter/__pkginfo__.py` & `docformatter-1.7.4/src/docformatter/__pkginfo__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Package information for docformatter."""
 
-__version__ = "1.7.3"
+__version__ = "1.7.4"
```

### Comparing `docformatter-1.7.3/src/docformatter/configuration.py` & `docformatter-1.7.4/src/docformatter/configuration.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.3/src/docformatter/encode.py` & `docformatter-1.7.4/src/docformatter/encode.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.3/src/docformatter/format.py` & `docformatter-1.7.4/src/docformatter/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -475,15 +475,14 @@
         if not self.args.force_wrap and (
             _syntax.is_some_sort_of_list(
                 summary,
                 self.args.non_strict,
                 self.args.rest_section_adorns,
                 self.args.style,
             )
-            or _syntax.do_find_directives(summary)
             or _syntax.do_find_links(summary)
         ):
             # Something is probably not right with the splitting.
             return docstring
 
         # Compensate for textwrap counting each tab in indentation as 1
         # character.
```

### Comparing `docformatter-1.7.3/src/docformatter/strings.py` & `docformatter-1.7.4/src/docformatter/strings.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.3/src/docformatter/syntax.py` & `docformatter-1.7.4/src/docformatter/syntax.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 OPTION_REGEX = r"^-{1,2}[\S ]+ {2}\S+"
 """Regular expression to use for finding option lists."""
 
 REST_REGEX = r"((\.{2}|`{2}) ?[\w.~-]+(:{2}|`{2})?[\w ]*?|`[\w.~]+`)"
 """Regular expression to use for finding reST directives."""
 
-SPHINX_REGEX = r":[a-zA-Z0-9_\-() ]*:"
+SPHINX_REGEX = r":(param|raises|return|rtype|type)[a-zA-Z0-9_\-.() ]*:"
 """Regular expression to use for finding Sphinx-style field lists."""
 
 URL_PATTERNS = (
     "afp|"
     "apt|"
     "bitcoin|"
     "chrome|"
@@ -272,15 +272,18 @@
     is_directive : bool
         Whether the docstring is a reST directive.
     """
     _rest_iter = re.finditer(REST_REGEX, text)
     return bool([(_rest.start(0), _rest.end(0)) for _rest in _rest_iter])
 
 
-def do_find_field_lists(text: str, style: str):
+def do_find_field_lists(
+    text: str,
+    style: str,
+):
     r"""Determine if docstring contains any field lists.
 
     Parameters
     ----------
     text : str
         The docstring description to check for field list patterns.
     style : str
```

### Comparing `docformatter-1.7.3/src/docformatter/util.py` & `docformatter-1.7.4/src/docformatter/util.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.3/PKG-INFO` & `docformatter-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docformatter
-Version: 1.7.3
+Version: 1.7.4
 Summary: Formats docstrings to follow PEP 257
 Home-page: https://github.com/PyCQA/docformatter
 License: Expat
 Keywords: PEP 257,pep257,style,formatter,docstrings
 Author: Steven Myint
 Maintainer: Doyle Rowland
 Maintainer-email: doyle.rowland@reliaqual.com
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Provides-Extra: tomli
 Requires-Dist: charset_normalizer (>=3.0.0,<4.0.0)
 Requires-Dist: tomli (>=2.0.0,<3.0.0) ; (python_version < "3.11") and (extra == "tomli")
 Requires-Dist: untokenize (>=0.1.1,<0.2.0)
-Project-URL: Documentation, https://github.com/PyCQA/docformatter
+Project-URL: Documentation, https://docformatter.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/PyCQA/docformatter
 Description-Content-Type: text/x-rst
 
 ============
 docformatter
 ============
```

