# Comparing `tmp/streamlit-binary-tree-0.1.5.tar.gz` & `tmp/streamlit-binary-tree-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-binary-tree-0.1.5.tar", last modified: Sun Jul  9 22:24:47 2023, max compression
+gzip compressed data, was "streamlit-binary-tree-0.1.6.tar", last modified: Sun Jul  9 22:29:06 2023, max compression
```

## Comparing `streamlit-binary-tree-0.1.5.tar` & `streamlit-binary-tree-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 22:24:47.741945 streamlit-binary-tree-0.1.5/
--rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      346 2023-07-09 22:24:47.741945 streamlit-binary-tree-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.1.5/README.md
--rw-rw-rw-   0        0        0       86 2023-07-09 22:24:47.742946 streamlit-binary-tree-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      803 2023-07-09 22:24:39.000000 streamlit-binary-tree-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 22:24:47.707936 streamlit-binary-tree-0.1.5/streamlit_binary_tree/
--rw-rw-rw-   0        0        0    11392 2023-07-09 22:24:28.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 22:24:47.689931 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-09 22:24:47.720939 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/
--rw-rw-rw-   0        0        0      879 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0     2186 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-09 22:24:47.690931 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-09 22:24:47.722940 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/css/
--rw-rw-rw-   0        0        0     6342 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css
--rw-rw-rw-   0        0        0    12587 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-09 22:24:47.740946 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/
--rw-rw-rw-   0        0        0   666670 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js
--rw-rw-rw-   0        0        0     3049 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2405628 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.map
--rw-rw-rw-   0        0        0     3474 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js
--rw-rw-rw-   0        0        0    11295 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
--rw-rw-rw-   0        0        0     8383 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
-drwxrwxrwx   0        0        0        0 2023-07-09 22:24:47.718939 streamlit-binary-tree-0.1.5/streamlit_binary_tree.egg-info/
--rw-rw-rw-   0        0        0      346 2023-07-09 22:24:47.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1068 2023-07-09 22:24:47.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 22:24:47.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-09 22:24:47.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-09 22:24:47.000000 streamlit-binary-tree-0.1.5/streamlit_binary_tree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 22:29:06.536711 streamlit-binary-tree-0.1.6/
+-rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      346 2023-07-09 22:29:06.536711 streamlit-binary-tree-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.1.6/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-09 22:29:06.538711 streamlit-binary-tree-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-07-09 22:28:58.000000 streamlit-binary-tree-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:29:06.505702 streamlit-binary-tree-0.1.6/streamlit_binary_tree/
+-rw-rw-rw-   0        0        0    11392 2023-07-09 22:24:28.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:29:06.497700 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-09 22:29:06.522707 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/
+-rw-rw-rw-   0        0        0      879 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     2186 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-09 22:29:06.498700 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-09 22:29:06.524707 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/css/
+-rw-rw-rw-   0        0        0     6342 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css
+-rw-rw-rw-   0        0        0    12587 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-09 22:29:06.535710 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   666670 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js
+-rw-rw-rw-   0        0        0     3049 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2405628 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.map
+-rw-rw-rw-   0        0        0     3474 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js
+-rw-rw-rw-   0        0        0    11295 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
+-rw-rw-rw-   0        0        0     8383 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
+drwxrwxrwx   0        0        0        0 2023-07-09 22:29:06.520706 streamlit-binary-tree-0.1.6/streamlit_binary_tree.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-07-09 22:29:06.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-07-09 22:29:06.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 22:29:06.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 22:29:06.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-09 22:29:06.000000 streamlit-binary-tree-0.1.6/streamlit_binary_tree.egg-info/top_level.txt
```

### Comparing `streamlit-binary-tree-0.1.5/LICENSE` & `streamlit-binary-tree-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.5/setup.py` & `streamlit-binary-tree-0.1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-binary-tree",
-    version="0.1.5",
+    version="0.1.6",
     author="Abhishek Sharma",
     author_email="abhishek1995sharma@gmail.com",
     description="Interactive Binary Tree as a Streamlit component",
     long_description="Interactive Binary Tree as a Streamlit component",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
@@ -16,12 +16,9 @@
     install_requires=[
         # By definition, a Custom Component depends on Streamlit.
         # If your component has other Python dependencies, list
         # them here.
         "streamlit >= 0.63",
         "scikit-learn >= 1.3.0",
         "numpy",
-        "math",
-        "os",
-        "typing",
     ],
 )
```

### Comparing `streamlit-binary-tree-0.1.5/streamlit_binary_tree/__init__.py` & `streamlit-binary-tree-0.1.6/streamlit_binary_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/asset-manifest.json` & `streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/index.html` & `streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css` & `streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css.map` & `streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js` & `streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.LICENSE.txt` & `streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.map` & `streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js` & `streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js.map` & `streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js` & `streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.5/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map` & `streamlit-binary-tree-0.1.6/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.5/streamlit_binary_tree.egg-info/SOURCES.txt` & `streamlit-binary-tree-0.1.6/streamlit_binary_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

