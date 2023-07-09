# Comparing `tmp/streamlit-binary-tree-0.1.7.tar.gz` & `tmp/streamlit-binary-tree-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-binary-tree-0.1.7.tar", last modified: Sun Jul  9 22:34:54 2023, max compression
+gzip compressed data, was "streamlit-binary-tree-0.1.8.tar", last modified: Sun Jul  9 22:38:51 2023, max compression
```

## Comparing `streamlit-binary-tree-0.1.7.tar` & `streamlit-binary-tree-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 22:34:54.782384 streamlit-binary-tree-0.1.7/
--rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      346 2023-07-09 22:34:54.782384 streamlit-binary-tree-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.1.7/README.md
--rw-rw-rw-   0        0        0       86 2023-07-09 22:34:54.784395 streamlit-binary-tree-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-07-09 22:34:49.000000 streamlit-binary-tree-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 22:34:54.753548 streamlit-binary-tree-0.1.7/streamlit_binary_tree/
--rw-rw-rw-   0        0        0    11392 2023-07-09 22:24:28.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 22:34:54.745554 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-09 22:34:54.766925 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/
--rw-rw-rw-   0        0        0      879 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0     2186 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-09 22:34:54.746548 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-09 22:34:54.768926 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/css/
--rw-rw-rw-   0        0        0     6342 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css
--rw-rw-rw-   0        0        0    12587 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-09 22:34:54.781384 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/
--rw-rw-rw-   0        0        0   666670 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js
--rw-rw-rw-   0        0        0     3049 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2405628 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.map
--rw-rw-rw-   0        0        0     3474 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js
--rw-rw-rw-   0        0        0    11295 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
--rw-rw-rw-   0        0        0     8383 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
-drwxrwxrwx   0        0        0        0 2023-07-09 22:34:54.765925 streamlit-binary-tree-0.1.7/streamlit_binary_tree.egg-info/
--rw-rw-rw-   0        0        0      346 2023-07-09 22:34:54.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1068 2023-07-09 22:34:54.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 22:34:54.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 22:34:54.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-09 22:34:54.000000 streamlit-binary-tree-0.1.7/streamlit_binary_tree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 22:38:51.420993 streamlit-binary-tree-0.1.8/
+-rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      346 2023-07-09 22:38:51.420993 streamlit-binary-tree-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.1.8/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-09 22:38:51.421994 streamlit-binary-tree-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-07-09 22:38:45.000000 streamlit-binary-tree-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:38:51.391645 streamlit-binary-tree-0.1.8/streamlit_binary_tree/
+-rw-rw-rw-   0        0        0    11388 2023-07-09 22:38:38.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:38:51.372761 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-09 22:38:51.406062 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/
+-rw-rw-rw-   0        0        0      879 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     2186 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-09 22:38:51.373761 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-09 22:38:51.408990 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/css/
+-rw-rw-rw-   0        0        0     6342 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css
+-rw-rw-rw-   0        0        0    12587 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-09 22:38:51.419993 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   666670 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js
+-rw-rw-rw-   0        0        0     3049 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2405628 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.map
+-rw-rw-rw-   0        0        0     3474 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js
+-rw-rw-rw-   0        0        0    11295 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
+-rw-rw-rw-   0        0        0     8383 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
+drwxrwxrwx   0        0        0        0 2023-07-09 22:38:51.404052 streamlit-binary-tree-0.1.8/streamlit_binary_tree.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-07-09 22:38:51.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-07-09 22:38:51.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 22:38:51.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 22:38:51.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-09 22:38:51.000000 streamlit-binary-tree-0.1.8/streamlit_binary_tree.egg-info/top_level.txt
```

### Comparing `streamlit-binary-tree-0.1.7/LICENSE` & `streamlit-binary-tree-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.7/setup.py` & `streamlit-binary-tree-0.1.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-binary-tree",
-    version="0.1.7",
+    version="0.1.8",
     author="Abhishek Sharma",
     author_email="abhishek1995sharma@gmail.com",
     description="Interactive Binary Tree as a Streamlit component",
     long_description="Interactive Binary Tree as a Streamlit component",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-binary-tree-0.1.7/streamlit_binary_tree/__init__.py` & `streamlit-binary-tree-0.1.8/streamlit_binary_tree/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
-import streamlit.components.v1 as components
+import math
+import numpy as np
 from typing import List
+import streamlit as st
+import streamlit.components.v1 as components
 from sklearn.tree import _tree
 from sklearn.tree._classes import DecisionTreeClassifier as DCTClass
-import math
-import numpy as np
 
 _RELEASE = True
 _DEBUG = False
 _NAME = "streamlit_binary_tree"
 
 if _RELEASE:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
@@ -343,15 +344,14 @@
         style=style,
     )
 
     return component_value
 
 
 if _DEBUG:
-    import streamlit as st
     from sklearn.datasets import load_iris
     from sklearn import tree
 
     st.set_page_config(layout="wide")
 
     clf = tree.DecisionTreeClassifier(class_weight={0: 1, 1: 10}, random_state=42)
     iris = load_iris()
```

### Comparing `streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/asset-manifest.json` & `streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/index.html` & `streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css` & `streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css.map` & `streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js` & `streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.LICENSE.txt` & `streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.map` & `streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js` & `streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js.map` & `streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js` & `streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.7/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map` & `streamlit-binary-tree-0.1.8/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.7/streamlit_binary_tree.egg-info/SOURCES.txt` & `streamlit-binary-tree-0.1.8/streamlit_binary_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

