# Comparing `tmp/bvhio-1.3.3.tar.gz` & `tmp/bvhio-1.3.4.tar.gz`

## Comparing `bvhio-1.3.3.tar` & `bvhio-1.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bvhio-1.3.3/.flake8
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 bvhio-1.3.3/CITATION.cff
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bvhio-1.3.3/changelog.txt
--rw-r--r--   0        0        0    16571 2020-02-02 00:00:00.000000 bvhio-1.3.3/test.ipynb
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 bvhio-1.3.3/.github/workflows/build_main.yml
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 bvhio-1.3.3/.github/workflows/build_preview.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/__init__.py
--rw-r--r--   0        0        0    13640 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/lib/Parser.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/lib/bvh/BvhContainer.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/lib/bvh/BvhJoint.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/lib/bvh/__init__.py
--rw-r--r--   0        0        0    17687 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/lib/hierarchy/Joint.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/lib/hierarchy/__init__.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/tests/example.bvh
--rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/tests/test_bvh.py
--rw-r--r--   0        0        0    22186 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/tests/test_hierarchy.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/tests/test_io.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/tests/utils.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bvhio-1.3.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bvhio-1.3.3/LICENSE
--rw-r--r--   0        0        0    18002 2020-02-02 00:00:00.000000 bvhio-1.3.3/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 bvhio-1.3.3/pyproject.toml
--rw-r--r--   0        0        0    18643 2020-02-02 00:00:00.000000 bvhio-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bvhio-1.3.4/.flake8
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 bvhio-1.3.4/CITATION.cff
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bvhio-1.3.4/changelog.txt
+-rw-r--r--   0        0        0    16571 2020-02-02 00:00:00.000000 bvhio-1.3.4/test.ipynb
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 bvhio-1.3.4/.github/workflows/build_main.yml
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 bvhio-1.3.4/.github/workflows/build_preview.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/__init__.py
+-rw-r--r--   0        0        0    13640 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/lib/Parser.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/lib/bvh/BvhContainer.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/lib/bvh/BvhJoint.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/lib/bvh/__init__.py
+-rw-r--r--   0        0        0    17687 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/lib/hierarchy/Joint.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/lib/hierarchy/__init__.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/tests/example.bvh
+-rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/tests/test_bvh.py
+-rw-r--r--   0        0        0    22186 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/tests/test_hierarchy.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/tests/test_io.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/tests/utils.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bvhio-1.3.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bvhio-1.3.4/LICENSE
+-rw-r--r--   0        0        0    18002 2020-02-02 00:00:00.000000 bvhio-1.3.4/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 bvhio-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0    18635 2020-02-02 00:00:00.000000 bvhio-1.3.4/PKG-INFO
```

### Comparing `bvhio-1.3.3/test.ipynb` & `bvhio-1.3.4/test.ipynb`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/.github/workflows/build_main.yml` & `bvhio-1.3.4/.github/workflows/build_main.yml`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/.github/workflows/build_preview.yml` & `bvhio-1.3.4/.github/workflows/build_preview.yml`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/bvhio/lib/Parser.py` & `bvhio-1.3.4/bvhio/lib/Parser.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/bvhio/lib/bvh/BvhContainer.py` & `bvhio-1.3.4/bvhio/lib/bvh/BvhContainer.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/bvhio/lib/bvh/BvhJoint.py` & `bvhio-1.3.4/bvhio/lib/bvh/BvhJoint.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/bvhio/lib/hierarchy/Joint.py` & `bvhio-1.3.4/bvhio/lib/hierarchy/Joint.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/bvhio/tests/example.bvh` & `bvhio-1.3.4/bvhio/tests/example.bvh`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/bvhio/tests/test_bvh.py` & `bvhio-1.3.4/bvhio/tests/test_bvh.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/bvhio/tests/test_hierarchy.py` & `bvhio-1.3.4/bvhio/tests/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/bvhio/tests/test_io.py` & `bvhio-1.3.4/bvhio/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/bvhio/tests/utils.py` & `bvhio-1.3.4/bvhio/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/LICENSE` & `bvhio-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/README.md` & `bvhio-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.3/pyproject.toml` & `bvhio-1.3.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bvhio"
-version = "1.3.3"
+version = "1.3.4"
 authors = [ { name="Wasserwecken", email="author@example.com" }, ]
 description = "Read, write, edit and create .bvh files with hierarchical 3D transforms."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    'numpy==1.23.1',
+    'numpy',
     'PyGLM==2.7.0',
     'spatial-transform==1.2.13',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Wasserwecken/bvhio"
 "Bug Tracker" = "https://github.com/Wasserwecken/bvhio/issues"
```

### Comparing `bvhio-1.3.3/PKG-INFO` & `bvhio-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bvhio
-Version: 1.3.3
+Version: 1.3.4
 Summary: Read, write, edit and create .bvh files with hierarchical 3D transforms.
 Project-URL: Homepage, https://github.com/Wasserwecken/bvhio
 Project-URL: Bug Tracker, https://github.com/Wasserwecken/bvhio/issues
 Author-email: Wasserwecken <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: numpy==1.23.1
+Requires-Dist: numpy
 Requires-Dist: pyglm==2.7.0
 Requires-Dist: spatial-transform==1.2.13
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/bvhio.svg)](https://pypi.python.org/pypi/bvhio/)
 [![PyPI download month](https://img.shields.io/pypi/dm/bvhio.svg)](https://pypi.python.org/pypi/bvhio/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: bvhio Version: 1.3.3 Summary: Read, write, edit and
+Metadata-Version: 2.1 Name: bvhio Version: 1.3.4 Summary: Read, write, edit and
 create .bvh files with hierarchical 3D transforms. Project-URL: Homepage,
 https://github.com/Wasserwecken/bvhio Project-URL: Bug Tracker, https://
 github.com/Wasserwecken/bvhio/issues Author-email: Wasserwecken
 example.com> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Requires-Python: >=3.7 Requires-Dist: numpy==1.23.1
-Requires-Dist: pyglm==2.7.0 Requires-Dist: spatial-transform==1.2.13
-Description-Content-Type: text/markdown [![PyPI version](https://badge.fury.io/
-py/bvhio.svg)](https://pypi.python.org/pypi/bvhio/) [![PyPI download month]
-(https://img.shields.io/pypi/dm/bvhio.svg)](https://pypi.python.org/pypi/bvhio/
-) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https:
-//opensource.org/licenses/MIT) [![Build Main](https://github.com/Wasserwecken/
+Language :: Python :: 3 Requires-Python: >=3.7 Requires-Dist: numpy Requires-
+Dist: pyglm==2.7.0 Requires-Dist: spatial-transform==1.2.13 Description-
+Content-Type: text/markdown [![PyPI version](https://badge.fury.io/py/
+bvhio.svg)](https://pypi.python.org/pypi/bvhio/) [![PyPI download month](https:
+//img.shields.io/pypi/dm/bvhio.svg)](https://pypi.python.org/pypi/bvhio/) [!
+[License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
+opensource.org/licenses/MIT) [![Build Main](https://github.com/Wasserwecken/
 bvhio/actions/workflows/build_main.yml/badge.svg?branch=main)](https://
 github.com/Wasserwecken/bvhio/actions) [![Build Preview](https://github.com/
 Wasserwecken/bvhio/actions/workflows/build_preview.yml/
 badge.svg?branch=preview)](https://test.pypi.org/project/bvhio/) [https://
 www.buymeacoffee.com/assets/img/custom_images/orange_img.png] # bvhio
 Lightweight libary for reading, editing and creating [Biovision .bvh](https://
 research.cs.wisc.edu/graphics/Courses/cs-838-1999/Jeff/BVH.html) files.
```

