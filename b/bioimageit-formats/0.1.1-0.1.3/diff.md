# Comparing `tmp/bioimageit_formats-0.1.1.tar.gz` & `tmp/bioimageit_formats-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageit_formats-0.1.1.tar", last modified: Thu Jul 28 14:39:59 2022, max compression
+gzip compressed data, was "bioimageit_formats-0.1.3.tar", last modified: Mon Jul 10 10:58:30 2023, max compression
```

## Comparing `bioimageit_formats-0.1.1.tar` & `bioimageit_formats-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 14:39:59.643378 bioimageit_formats-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 14:39:59.635378 bioimageit_formats-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 14:39:59.635378 bioimageit_formats-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2801 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-07-28 14:39:59.643378 bioimageit_formats-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 14:39:59.639377 bioimageit_formats-0.1.1/bioimageit_formats/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/bioimageit_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/bioimageit_formats/_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     5087 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/bioimageit_formats/_formats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 14:39:59.639377 bioimageit_formats-0.1.1/bioimageit_formats/_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/bioimageit_formats/_plugins/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/bioimageit_formats/_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/bioimageit_formats/_plugins/_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/bioimageit_formats/_plugins/_imagetiff.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/bioimageit_formats/_plugins/_imagezarr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/bioimageit_formats/_plugins/_movietxt.py
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/bioimageit_formats/_plugins/_trackmate.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/bioimageit_formats/_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 14:39:59.639377 bioimageit_formats-0.1.1/bioimageit_formats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-07-28 14:39:59.000000 bioimageit_formats-0.1.1/bioimageit_formats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-07-28 14:39:59.000000 bioimageit_formats-0.1.1/bioimageit_formats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-28 14:39:59.000000 bioimageit_formats-0.1.1/bioimageit_formats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-28 14:39:59.000000 bioimageit_formats-0.1.1/bioimageit_formats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-28 14:39:59.000000 bioimageit_formats-0.1.1/bioimageit_formats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-28 14:39:59.643378 bioimageit_formats-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 14:39:59.639377 bioimageit_formats-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1055 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/tests/formats.json
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/tests/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-07-28 14:39:41.000000 bioimageit_formats-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:58:30.799692 bioimageit_formats-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:58:30.795692 bioimageit_formats-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:58:30.795692 bioimageit_formats-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-10 10:58:30.799692 bioimageit_formats-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:58:30.795692 bioimageit_formats-0.1.3/bioimageit_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/bioimageit_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/bioimageit_formats/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/bioimageit_formats/_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:58:30.799692 bioimageit_formats-0.1.3/bioimageit_formats/_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/bioimageit_formats/_plugins/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/bioimageit_formats/_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/bioimageit_formats/_plugins/_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/bioimageit_formats/_plugins/_imagetiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/bioimageit_formats/_plugins/_imagezarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/bioimageit_formats/_plugins/_movietxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/bioimageit_formats/_plugins/_pythonscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/bioimageit_formats/_plugins/_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/bioimageit_formats/_plugins/_trackmate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/bioimageit_formats/_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:58:30.795692 bioimageit_formats-0.1.3/bioimageit_formats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-10 10:58:30.000000 bioimageit_formats-0.1.3/bioimageit_formats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-10 10:58:30.000000 bioimageit_formats-0.1.3/bioimageit_formats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:58:30.000000 bioimageit_formats-0.1.3/bioimageit_formats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 10:58:30.000000 bioimageit_formats-0.1.3/bioimageit_formats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 10:58:30.000000 bioimageit_formats-0.1.3/bioimageit_formats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:58:30.799692 bioimageit_formats-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:58:30.799692 bioimageit_formats-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/tests/formats.json
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/tests/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-10 10:58:12.000000 bioimageit_formats-0.1.3/tox.ini
```

### Comparing `bioimageit_formats-0.1.1/.github/workflows/test_and_deploy.yml` & `bioimageit_formats-0.1.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `bioimageit_formats-0.1.1/LICENSE` & `bioimageit_formats-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageit_formats-0.1.1/PKG-INFO` & `bioimageit_formats-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bioimageit_formats
-Version: 0.1.1
+Version: 0.1.3
 Summary: Manage data formats for BioImageIT project
 Home-page: https://github.com/bioimageit/bioimageit_formats
-Author: Sylvain Prigent
-Author-email: sylvain.prigent@inria.fr
+Author: Sylvain Prigent and BioImageIT team
+Author-email: bioimageit@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bioimageit_formats-0.1.1/README.md` & `bioimageit_formats-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bioimageit_formats-0.1.1/bioimageit_formats/_factory.py` & `bioimageit_formats-0.1.3/bioimageit_formats/_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 RunnerServiceProvider
 
 """
 from ._plugins._csv import (TableCSVServiceBuilder, ArrayCSVServiceBuilder, NumberCSVServiceBuilder)
 from ._plugins._imagetiff import ImagetiffServiceBuilder
 from ._plugins._imagezarr import ImagezarrServiceBuilder
 from ._plugins._movietxt import MovietxtServiceBuilder
+from ._plugins._raw import RawServiceBuilder
 from ._plugins._trackmate import TrackmateModelServiceBuilder
 
 
 class ObjectFactory:
     """Agnostic factory
 
     Implements the factory design pattern
@@ -46,7 +47,8 @@
 formatsServices.register_builder('imagetiff', ImagetiffServiceBuilder())
 formatsServices.register_builder('imagezarr', ImagezarrServiceBuilder())
 formatsServices.register_builder('movietxt', MovietxtServiceBuilder())
 formatsServices.register_builder('tablecsv', TableCSVServiceBuilder())
 formatsServices.register_builder('arraycsv', ArrayCSVServiceBuilder())
 formatsServices.register_builder('numbercsv', NumberCSVServiceBuilder())
 formatsServices.register_builder('trackmatemodel', TrackmateModelServiceBuilder())
+formatsServices.register_builder('raw', RawServiceBuilder())
```

### Comparing `bioimageit_formats-0.1.1/bioimageit_formats/_formats.py` & `bioimageit_formats-0.1.3/bioimageit_formats/_formats.py`

 * *Files identical despite different names*

### Comparing `bioimageit_formats-0.1.1/bioimageit_formats/_plugins/_csv.py` & `bioimageit_formats-0.1.3/bioimageit_formats/_plugins/_csv.py`

 * *Files identical despite different names*

### Comparing `bioimageit_formats-0.1.1/bioimageit_formats/_plugins/_imagetiff.py` & `bioimageit_formats-0.1.3/bioimageit_formats/_plugins/_imagetiff.py`

 * *Files identical despite different names*

### Comparing `bioimageit_formats-0.1.1/bioimageit_formats/_plugins/_imagezarr.py` & `bioimageit_formats-0.1.3/bioimageit_formats/_plugins/_imagezarr.py`

 * *Files identical despite different names*

### Comparing `bioimageit_formats-0.1.1/bioimageit_formats/_plugins/_movietxt.py` & `bioimageit_formats-0.1.3/bioimageit_formats/_plugins/_movietxt.py`

 * *Files identical despite different names*

### Comparing `bioimageit_formats-0.1.1/bioimageit_formats/_plugins/_trackmate.py` & `bioimageit_formats-0.1.3/bioimageit_formats/_plugins/_trackmate.py`

 * *Files identical despite different names*

### Comparing `bioimageit_formats-0.1.1/bioimageit_formats/_reader.py` & `bioimageit_formats-0.1.3/bioimageit_formats/_reader.py`

 * *Files identical despite different names*

### Comparing `bioimageit_formats-0.1.1/bioimageit_formats.egg-info/PKG-INFO` & `bioimageit_formats-0.1.3/bioimageit_formats.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bioimageit-formats
-Version: 0.1.1
+Version: 0.1.3
 Summary: Manage data formats for BioImageIT project
 Home-page: https://github.com/bioimageit/bioimageit_formats
-Author: Sylvain Prigent
-Author-email: sylvain.prigent@inria.fr
+Author: Sylvain Prigent and BioImageIT team
+Author-email: bioimageit@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bioimageit_formats-0.1.1/bioimageit_formats.egg-info/SOURCES.txt` & `bioimageit_formats-0.1.3/bioimageit_formats.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,11 +15,13 @@
 bioimageit_formats.egg-info/top_level.txt
 bioimageit_formats/_plugins/.gitignore
 bioimageit_formats/_plugins/__init__.py
 bioimageit_formats/_plugins/_csv.py
 bioimageit_formats/_plugins/_imagetiff.py
 bioimageit_formats/_plugins/_imagezarr.py
 bioimageit_formats/_plugins/_movietxt.py
+bioimageit_formats/_plugins/_pythonscript.py
+bioimageit_formats/_plugins/_raw.py
 bioimageit_formats/_plugins/_trackmate.py
 tests/__init__.py
 tests/formats.json
 tests/test_csv.py
```

### Comparing `bioimageit_formats-0.1.1/setup.py` & `bioimageit_formats-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bioimageit_formats",
-    version="0.1.1",
-    author="Sylvain Prigent",
-    author_email="sylvain.prigent@inria.fr",
+    version="0.1.3",
+    author="Sylvain Prigent and BioImageIT team",
+    author_email="bioimageit@gmail.com",
     description="Manage data formats for BioImageIT project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bioimageit/bioimageit_formats",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `bioimageit_formats-0.1.1/tests/formats.json` & `bioimageit_formats-0.1.3/tests/formats.json`

 * *Files identical despite different names*

### Comparing `bioimageit_formats-0.1.1/tests/test_csv.py` & `bioimageit_formats-0.1.3/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `bioimageit_formats-0.1.1/tox.ini` & `bioimageit_formats-0.1.3/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 platform =
     macos: darwin
     linux: linux
     windows: win32
 passenv =
     CI
     GITHUB_ACTIONS
-    DISPLAY XAUTHORITY
+    DISPLAY
+    XAUTHORITY
     NUMPY_EXPERIMENTAL_ARRAY_FUNCTION
     PYVISTA_OFF_SCREEN
 deps =
     pytest  # https://docs.pytest.org/en/latest/contents.html
     pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
     pytest-xvfb ; sys_platform == 'linux'
     numpy
-commands = pytest -v --color=yes --cov=bioimageit_formats --cov-report=xml
+commands = pytest -v --color=yes --cov=bioimageit_formats --cov-report=xml
```

