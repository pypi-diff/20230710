# Comparing `tmp/pyolin-0.0.2.tar.gz` & `tmp/pyolin-0.0.3.tar.gz`

## Comparing `pyolin-0.0.2.tar` & `pyolin-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pyolin-0.0.2/__main__.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 pyolin-0.0.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pyolin-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/__init__.py
--rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/field.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/header_detector.py
--rw-r--r--   0        0        0    16373 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/ioformat.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/parser.py
--rw-r--r--   0        0        0     7752 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/pyolin.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/record.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/util.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/__init__.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_addresses.csv
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_addresses_unix.csv
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_addresses_with_header.csv
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_amazon_reviews.tsv
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_colors.json
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_files.txt
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_files_with_header.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_formatting.txt
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_grades_simple_csv.csv
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_grades_with_header.csv
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_nba.txt
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_news_decline.csv
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_news_decline.tsv
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_onerow.csv
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/data_pickle
--rw-r--r--   0        0        0    64009 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/test_pyolin.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyolin/test/utils.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pyolin-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyolin-0.0.2/LICENSE
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 pyolin-0.0.2/README.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 pyolin-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 pyolin-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 pyolin-0.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pyolin-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/__init__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/__main__.py
+-rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/field.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/header_detector.py
+-rw-r--r--   0        0        0    16373 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/ioformat.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/parser.py
+-rw-r--r--   0        0        0     7752 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/pyolin.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/record.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/util.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/__init__.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_addresses.csv
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_addresses_unix.csv
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_addresses_with_header.csv
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_amazon_reviews.tsv
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_colors.json
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_files.txt
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_files_with_header.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_formatting.txt
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_grades_simple_csv.csv
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_grades_with_header.csv
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_nba.txt
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_news_decline.csv
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_news_decline.tsv
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_onerow.csv
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/data_pickle
+-rw-r--r--   0        0        0    64009 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/test_pyolin.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyolin/test/utils.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pyolin-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyolin-0.0.3/LICENSE
+-rw-r--r--   0        0        0     8781 2020-02-02 00:00:00.000000 pyolin-0.0.3/README.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 pyolin-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 pyolin-0.0.3/PKG-INFO
```

### Comparing `pyolin-0.0.2/.github/workflows/python-package.yml` & `pyolin-0.0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.2/pyolin/field.py` & `pyolin-0.0.3/pyolin/field.py`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.2/pyolin/header_detector.py` & `pyolin-0.0.3/pyolin/header_detector.py`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.2/pyolin/ioformat.py` & `pyolin-0.0.3/pyolin/ioformat.py`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.2/pyolin/parser.py` & `pyolin-0.0.3/pyolin/parser.py`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.2/pyolin/pyolin.py` & `pyolin-0.0.3/pyolin/pyolin.py`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.2/pyolin/record.py` & `pyolin-0.0.3/pyolin/record.py`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.2/pyolin/util.py` & `pyolin-0.0.3/pyolin/util.py`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.2/pyolin/test/data_amazon_reviews.tsv` & `pyolin-0.0.3/pyolin/test/data_amazon_reviews.tsv`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.2/pyolin/test/data_grades_with_header.csv` & `pyolin-0.0.3/pyolin/test/data_grades_with_header.csv`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.2/pyolin/test/test_pyolin.py` & `pyolin-0.0.3/pyolin/test/test_pyolin.py`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.2/pyolin/test/utils.py` & `pyolin-0.0.3/pyolin/test/utils.py`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.2/LICENSE` & `pyolin-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyolin-0.0.2/README.md` & `pyolin-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Pyolin
 
 ![CI](https://github.com/mauricelam/pyolin/actions/workflows/python-package.yml/badge.svg)
+[![PyPI](https://img.shields.io/pypi/v/pyolin.svg?color=%230073b7)](https://pypi.org/project/pyolin/)
 
 Tool to easily write Python one-liners
 
 Pyolin processes data from stdin or a given file, evaluates the given input `prog` and prints the result.
 
 Example:
 ```sh
```

### Comparing `pyolin-0.0.2/pyproject.toml` & `pyolin-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyolin"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Maurice Lam", email="mauriceprograms@gmail.com" },
 ]
 description = "Tool to easily write Python one-liners"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyolin-0.0.2/PKG-INFO` & `pyolin-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyolin
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool to easily write Python one-liners
 Project-URL: Homepage, https://github.com/mauricelam/pyolin
 Project-URL: Bug Tracker, https://github.com/mauricelam/pyolin/issues
 Author-email: Maurice Lam <mauriceprograms@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Requires-Python: >=3.8
 Requires-Dist: hashbang>=0.1.14
 Description-Content-Type: text/markdown
 
 # Pyolin
 
 ![CI](https://github.com/mauricelam/pyolin/actions/workflows/python-package.yml/badge.svg)
+[![PyPI](https://img.shields.io/pypi/v/pyolin.svg?color=%230073b7)](https://pypi.org/project/pyolin/)
 
 Tool to easily write Python one-liners
 
 Pyolin processes data from stdin or a given file, evaluates the given input `prog` and prints the result.
 
 Example:
 ```sh
```

