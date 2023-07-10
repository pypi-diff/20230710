# Comparing `tmp/bvhio-1.3.2.tar.gz` & `tmp/bvhio-1.3.3.tar.gz`

## Comparing `bvhio-1.3.2.tar` & `bvhio-1.3.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bvhio-1.3.2/.flake8
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 bvhio-1.3.2/CITATION.cff
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bvhio-1.3.2/changelog.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 bvhio-1.3.2/requirements.txt
--rw-r--r--   0        0        0    16571 2020-02-02 00:00:00.000000 bvhio-1.3.2/test.ipynb
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 bvhio-1.3.2/.github/workflows/build_main.yml
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 bvhio-1.3.2/.github/workflows/build_preview.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bvhio-1.3.2/bvhio/__init__.py
--rw-r--r--   0        0        0    13640 2020-02-02 00:00:00.000000 bvhio-1.3.2/bvhio/lib/Parser.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bvhio-1.3.2/bvhio/lib/bvh/BvhContainer.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bvhio-1.3.2/bvhio/lib/bvh/BvhJoint.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bvhio-1.3.2/bvhio/lib/bvh/__init__.py
--rw-r--r--   0        0        0    17687 2020-02-02 00:00:00.000000 bvhio-1.3.2/bvhio/lib/hierarchy/Joint.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bvhio-1.3.2/bvhio/lib/hierarchy/__init__.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 bvhio-1.3.2/bvhio/tests/example.bvh
--rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 bvhio-1.3.2/bvhio/tests/test_bvh.py
--rw-r--r--   0        0        0    22186 2020-02-02 00:00:00.000000 bvhio-1.3.2/bvhio/tests/test_hierarchy.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 bvhio-1.3.2/bvhio/tests/test_io.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 bvhio-1.3.2/bvhio/tests/utils.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bvhio-1.3.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bvhio-1.3.2/LICENSE
--rw-r--r--   0        0        0    18002 2020-02-02 00:00:00.000000 bvhio-1.3.2/README.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 bvhio-1.3.2/pyproject.toml
--rw-r--r--   0        0        0    18545 2020-02-02 00:00:00.000000 bvhio-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bvhio-1.3.3/.flake8
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 bvhio-1.3.3/CITATION.cff
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bvhio-1.3.3/changelog.txt
+-rw-r--r--   0        0        0    16571 2020-02-02 00:00:00.000000 bvhio-1.3.3/test.ipynb
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 bvhio-1.3.3/.github/workflows/build_main.yml
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 bvhio-1.3.3/.github/workflows/build_preview.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/__init__.py
+-rw-r--r--   0        0        0    13640 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/lib/Parser.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/lib/bvh/BvhContainer.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/lib/bvh/BvhJoint.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/lib/bvh/__init__.py
+-rw-r--r--   0        0        0    17687 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/lib/hierarchy/Joint.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/lib/hierarchy/__init__.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/tests/example.bvh
+-rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/tests/test_bvh.py
+-rw-r--r--   0        0        0    22186 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/tests/test_hierarchy.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/tests/test_io.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 bvhio-1.3.3/bvhio/tests/utils.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bvhio-1.3.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bvhio-1.3.3/LICENSE
+-rw-r--r--   0        0        0    18002 2020-02-02 00:00:00.000000 bvhio-1.3.3/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 bvhio-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0    18643 2020-02-02 00:00:00.000000 bvhio-1.3.3/PKG-INFO
```

### Comparing `bvhio-1.3.2/test.ipynb` & `bvhio-1.3.3/test.ipynb`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.2/.github/workflows/build_main.yml` & `bvhio-1.3.3/.github/workflows/build_main.yml`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,15 @@
       - name: Install environment dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install flake8
           python -m pip install build
 
       - name: Install project dependencies
-        run: if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+        run: python -m pip install .
 
       - name: Lint with flake8
         run: |
           # stop the build if there are Python syntax errors or undefined names
           flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
           # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
           flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
```

### Comparing `bvhio-1.3.2/.github/workflows/build_preview.yml` & `bvhio-1.3.3/.github/workflows/build_preview.yml`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,15 @@
       - name: Install environment dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install flake8
           python -m pip install build
 
       - name: Install project dependencies
-        run: if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+        run: python -m pip install .
 
       - name: Lint with flake8
         run: |
           # stop the build if there are Python syntax errors or undefined names
           flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
           # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
           flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
```

### Comparing `bvhio-1.3.2/bvhio/lib/Parser.py` & `bvhio-1.3.3/bvhio/lib/Parser.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.2/bvhio/lib/bvh/BvhContainer.py` & `bvhio-1.3.3/bvhio/lib/bvh/BvhContainer.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.2/bvhio/lib/bvh/BvhJoint.py` & `bvhio-1.3.3/bvhio/lib/bvh/BvhJoint.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.2/bvhio/lib/hierarchy/Joint.py` & `bvhio-1.3.3/bvhio/lib/hierarchy/Joint.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.2/bvhio/tests/example.bvh` & `bvhio-1.3.3/bvhio/tests/example.bvh`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.2/bvhio/tests/test_bvh.py` & `bvhio-1.3.3/bvhio/tests/test_bvh.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.2/bvhio/tests/test_hierarchy.py` & `bvhio-1.3.3/bvhio/tests/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.2/bvhio/tests/test_io.py` & `bvhio-1.3.3/bvhio/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.2/bvhio/tests/utils.py` & `bvhio-1.3.3/bvhio/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.2/LICENSE` & `bvhio-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.2/README.md` & `bvhio-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.2/pyproject.toml` & `bvhio-1.3.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-dynamic = ["dependencies"]
 name = "bvhio"
-version = "1.3.2"
+version = "1.3.3"
 authors = [ { name="Wasserwecken", email="author@example.com" }, ]
 description = "Read, write, edit and create .bvh files with hierarchical 3D transforms."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-[tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
+dependencies = [
+    'numpy==1.23.1',
+    'PyGLM==2.7.0',
+    'spatial-transform==1.2.13',
+]
 
 [project.urls]
 "Homepage" = "https://github.com/Wasserwecken/bvhio"
 "Bug Tracker" = "https://github.com/Wasserwecken/bvhio/issues"
```

### Comparing `bvhio-1.3.2/PKG-INFO` & `bvhio-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: bvhio
-Version: 1.3.2
+Version: 1.3.3
 Summary: Read, write, edit and create .bvh files with hierarchical 3D transforms.
 Project-URL: Homepage, https://github.com/Wasserwecken/bvhio
 Project-URL: Bug Tracker, https://github.com/Wasserwecken/bvhio/issues
 Author-email: Wasserwecken <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: numpy==1.23.1
+Requires-Dist: pyglm==2.7.0
+Requires-Dist: spatial-transform==1.2.13
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/bvhio.svg)](https://pypi.python.org/pypi/bvhio/)
 [![PyPI download month](https://img.shields.io/pypi/dm/bvhio.svg)](https://pypi.python.org/pypi/bvhio/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Build Main](https://github.com/Wasserwecken/bvhio/actions/workflows/build_main.yml/badge.svg?branch=main)](https://github.com/Wasserwecken/bvhio/actions)
 [![Build Preview](https://github.com/Wasserwecken/bvhio/actions/workflows/build_preview.yml/badge.svg?branch=preview)](https://test.pypi.org/project/bvhio/)
```

#### html2text {}

```diff
@@ -1,47 +1,49 @@
-Metadata-Version: 2.1 Name: bvhio Version: 1.3.2 Summary: Read, write, edit and
+Metadata-Version: 2.1 Name: bvhio Version: 1.3.3 Summary: Read, write, edit and
 create .bvh files with hierarchical 3D transforms. Project-URL: Homepage,
 https://github.com/Wasserwecken/bvhio Project-URL: Bug Tracker, https://
 github.com/Wasserwecken/bvhio/issues Author-email: Wasserwecken
 example.com> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
-markdown [![PyPI version](https://badge.fury.io/py/bvhio.svg)](https://
-pypi.python.org/pypi/bvhio/) [![PyPI download month](https://img.shields.io/
-pypi/dm/bvhio.svg)](https://pypi.python.org/pypi/bvhio/) [![License: MIT]
-(https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/
-licenses/MIT) [![Build Main](https://github.com/Wasserwecken/bvhio/actions/
-workflows/build_main.yml/badge.svg?branch=main)](https://github.com/
-Wasserwecken/bvhio/actions) [![Build Preview](https://github.com/Wasserwecken/
-bvhio/actions/workflows/build_preview.yml/badge.svg?branch=preview)](https://
-test.pypi.org/project/bvhio/) [https://www.buymeacoffee.com/assets/img/
-custom_images/orange_img.png] # bvhio Lightweight libary for reading, editing
-and creating [Biovision .bvh](https://research.cs.wisc.edu/graphics/Courses/cs-
-838-1999/Jeff/BVH.html) files. Deserializes files into a hierarchical spatial
-structure like transforms in Unity or Unreal. Data for each joint is provided
-in local and world space and does support modifing the hierarchy itself without
-losing the keyframe data. The spatial structure does also allow for editing the
-motion or rest pose data. This libary supports also deserializing and
-serialising .bvh files into a simplified structure that represents the key data
-from the file. ## Install ``` batch pip install bvhio ``` ## Why and intention
-This libary is a side product of my master thesis, in order to extract
-conveniently local and world data features from a humanoid skeleton hierarchy.
-I could not find any libary that could do that, without bloat or the features I
-required for extraction or modification. ## Notes - The package [spatial-
-transform](https://github.com/Wasserwecken/spatial-transform) is used as base
-object for joints and provides the most properties and methods. - The package
-[PyGLM](https://github.com/Zuzu-Typ/PyGLM) is used for matrix, quaternion and
-vector calculations. - Same coordination space as [openGL and GLM](https://
-www.evl.uic.edu/ralph/508S98/coordinates.html) is used. Which is: Right-Handed,
-- Y+ is up, Z- is forward and positive rotations are counter clockwise. ##
-Features - Read/Write/Edit - Read and write .bvh files as simplified structure
-(`BvhJoint`). - Read and write .bvh files as transform hierarchy (`Joint`). -
-Animation data can be modified with both methods. - The transform hierarchy
-allows for easy modifications of rest and motion data. - Animation - Supports
-modifing keyframe, rest positon and final pose data. - Supports joint special
+Language :: Python :: 3 Requires-Python: >=3.7 Requires-Dist: numpy==1.23.1
+Requires-Dist: pyglm==2.7.0 Requires-Dist: spatial-transform==1.2.13
+Description-Content-Type: text/markdown [![PyPI version](https://badge.fury.io/
+py/bvhio.svg)](https://pypi.python.org/pypi/bvhio/) [![PyPI download month]
+(https://img.shields.io/pypi/dm/bvhio.svg)](https://pypi.python.org/pypi/bvhio/
+) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https:
+//opensource.org/licenses/MIT) [![Build Main](https://github.com/Wasserwecken/
+bvhio/actions/workflows/build_main.yml/badge.svg?branch=main)](https://
+github.com/Wasserwecken/bvhio/actions) [![Build Preview](https://github.com/
+Wasserwecken/bvhio/actions/workflows/build_preview.yml/
+badge.svg?branch=preview)](https://test.pypi.org/project/bvhio/) [https://
+www.buymeacoffee.com/assets/img/custom_images/orange_img.png] # bvhio
+Lightweight libary for reading, editing and creating [Biovision .bvh](https://
+research.cs.wisc.edu/graphics/Courses/cs-838-1999/Jeff/BVH.html) files.
+Deserializes files into a hierarchical spatial structure like transforms in
+Unity or Unreal. Data for each joint is provided in local and world space and
+does support modifing the hierarchy itself without losing the keyframe data.
+The spatial structure does also allow for editing the motion or rest pose data.
+This libary supports also deserializing and serialising .bvh files into a
+simplified structure that represents the key data from the file. ## Install ```
+batch pip install bvhio ``` ## Why and intention This libary is a side product
+of my master thesis, in order to extract conveniently local and world data
+features from a humanoid skeleton hierarchy. I could not find any libary that
+could do that, without bloat or the features I required for extraction or
+modification. ## Notes - The package [spatial-transform](https://github.com/
+Wasserwecken/spatial-transform) is used as base object for joints and provides
+the most properties and methods. - The package [PyGLM](https://github.com/Zuzu-
+Typ/PyGLM) is used for matrix, quaternion and vector calculations. - Same
+coordination space as [openGL and GLM](https://www.evl.uic.edu/ralph/508S98/
+coordinates.html) is used. Which is: Right-Handed, - Y+ is up, Z- is forward
+and positive rotations are counter clockwise. ## Features - Read/Write/Edit -
+Read and write .bvh files as simplified structure (`BvhJoint`). - Read and
+write .bvh files as transform hierarchy (`Joint`). - Animation data can be
+modified with both methods. - The transform hierarchy allows for easy
+modifications of rest and motion data. - Animation - Supports modifing
+keyframe, rest positon and final pose data. - Supports joint special
 modifications, like changing the joint-roll - Keyframes are stored in local
 space and as difference to the rest pose. - Keyframes support Position,
 Rotation and Scale. - Python - Every method is documented in code with
 docstrings. - Every method has type hinting. - ([Fluent Interface](https://
 de.wikipedia.org/wiki/Fluent_Interface)) design. ## Examples ### Read bvh as
 transform hierarchy ```python import bvhio # Reads the file into a transform
 tree structure and converts all data to build proper local and world spaces. #
```

