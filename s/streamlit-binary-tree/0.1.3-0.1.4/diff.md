# Comparing `tmp/streamlit-binary-tree-0.1.3.tar.gz` & `tmp/streamlit-binary-tree-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-binary-tree-0.1.3.tar", last modified: Sun Jul  9 21:52:04 2023, max compression
+gzip compressed data, was "streamlit-binary-tree-0.1.4.tar", last modified: Sun Jul  9 22:15:04 2023, max compression
```

## Comparing `streamlit-binary-tree-0.1.3.tar` & `streamlit-binary-tree-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 21:52:04.909314 streamlit-binary-tree-0.1.3/
--rw-rw-rw-   0        0        0     2340 2023-06-07 13:55:36.000000 streamlit-binary-tree-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      346 2023-07-09 21:52:04.909314 streamlit-binary-tree-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-09 21:52:04.909314 streamlit-binary-tree-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-07-09 21:52:01.000000 streamlit-binary-tree-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 21:52:04.860906 streamlit-binary-tree-0.1.3/streamlit_binary_tree/
--rw-rw-rw-   0        0        0    11391 2023-07-09 21:40:13.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 21:52:04.855907 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-09 21:52:04.894285 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/
--rw-rw-rw-   0        0        0      879 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0     2186 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-09 21:52:04.856906 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-09 21:52:04.897286 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/css/
--rw-rw-rw-   0        0        0     6342 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css
--rw-rw-rw-   0        0        0    12587 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-09 21:52:04.908313 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/
--rw-rw-rw-   0        0        0   666670 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js
--rw-rw-rw-   0        0        0     3049 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2405628 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.map
--rw-rw-rw-   0        0        0     3474 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js
--rw-rw-rw-   0        0        0    11295 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
--rw-rw-rw-   0        0        0     8383 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
-drwxrwxrwx   0        0        0        0 2023-07-09 21:52:04.892285 streamlit-binary-tree-0.1.3/streamlit_binary_tree.egg-info/
--rw-rw-rw-   0        0        0      346 2023-07-09 21:52:04.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2023-07-09 21:52:04.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 21:52:04.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-09 21:52:04.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-09 21:52:04.000000 streamlit-binary-tree-0.1.3/streamlit_binary_tree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 22:15:04.274663 streamlit-binary-tree-0.1.4/
+-rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      346 2023-07-09 22:15:04.275662 streamlit-binary-tree-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.1.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-09 22:15:04.276663 streamlit-binary-tree-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-07-09 22:14:54.000000 streamlit-binary-tree-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:15:04.236653 streamlit-binary-tree-0.1.4/streamlit_binary_tree/
+-rw-rw-rw-   0        0        0    11391 2023-07-09 21:40:13.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:15:04.227651 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-09 22:15:04.259659 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/
+-rw-rw-rw-   0        0        0      879 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     2186 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-09 22:15:04.230652 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-09 22:15:04.262660 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/css/
+-rw-rw-rw-   0        0        0     6342 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css
+-rw-rw-rw-   0        0        0    12587 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-09 22:15:04.273663 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   666670 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js
+-rw-rw-rw-   0        0        0     3049 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2405628 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.map
+-rw-rw-rw-   0        0        0     3474 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js
+-rw-rw-rw-   0        0        0    11295 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
+-rw-rw-rw-   0        0        0     8383 2023-07-09 12:09:30.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
+drwxrwxrwx   0        0        0        0 2023-07-09 22:15:04.257659 streamlit-binary-tree-0.1.4/streamlit_binary_tree.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-07-09 22:15:04.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-07-09 22:15:04.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 22:15:04.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-09 22:15:04.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-09 22:15:04.000000 streamlit-binary-tree-0.1.4/streamlit_binary_tree.egg-info/top_level.txt
```

### Comparing `streamlit-binary-tree-0.1.3/LICENSE` & `streamlit-binary-tree-0.1.4/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Yuichiro Tachibana (Tsuchiya)
+Copyright (c) 2023 Abhishek Sharma
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -16,14 +16,36 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
+The major design pattern of this package was abstracted from Streamlit's component-template, which is subject to the same license.
+Here is the original copyright notice for it:
+
+Copyright (c) 2021 Yuichiro Tachibana (Tsuchiya)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
 
 The major design pattern of this package was abstracted from Streamlit's component-template, which is subject to the same license.
 Here is the original copyright notice for it:
 
 Copyright (c) 2018 The Python Packaging Authority
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamlit-binary-tree-0.1.3/setup.py` & `streamlit-binary-tree-0.1.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-binary-tree",
-    version="0.1.3",
+    version="0.1.4",
     author="Abhishek Sharma",
     author_email="abhishek1995sharma@gmail.com",
     description="Interactive Binary Tree as a Streamlit component",
     long_description="Interactive Binary Tree as a Streamlit component",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
@@ -15,9 +15,13 @@
     python_requires=">=3.6",
     install_requires=[
         # By definition, a Custom Component depends on Streamlit.
         # If your component has other Python dependencies, list
         # them here.
         "streamlit >= 0.63",
         "scikit-learn >= 1.3.0",
+        "numpy",
+        "math",
+        "os",
+        "typing",
     ],
 )
```

### Comparing `streamlit-binary-tree-0.1.3/streamlit_binary_tree/__init__.py` & `streamlit-binary-tree-0.1.4/streamlit_binary_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/asset-manifest.json` & `streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/index.html` & `streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css` & `streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css.map` & `streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/css/main.9d901713.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js` & `streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.LICENSE.txt` & `streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.map` & `streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/2.66fc388b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js` & `streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js.map` & `streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/main.7c9f5867.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js` & `streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.3/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map` & `streamlit-binary-tree-0.1.4/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.1.3/streamlit_binary_tree.egg-info/SOURCES.txt` & `streamlit-binary-tree-0.1.4/streamlit_binary_tree.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE
 MANIFEST.in
+README.md
+setup.cfg
 setup.py
 streamlit_binary_tree/__init__.py
 streamlit_binary_tree.egg-info/PKG-INFO
 streamlit_binary_tree.egg-info/SOURCES.txt
 streamlit_binary_tree.egg-info/dependency_links.txt
 streamlit_binary_tree.egg-info/requires.txt
 streamlit_binary_tree.egg-info/top_level.txt
```

