# Comparing `tmp/streamlit_baseweb-0.1.1.tar.gz` & `tmp/streamlit_baseweb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_baseweb-0.1.1.tar", last modified: Thu Jul  6 00:17:08 2023, max compression
+gzip compressed data, was "streamlit_baseweb-0.1.2.tar", last modified: Mon Jul 10 09:27:05 2023, max compression
```

## Comparing `streamlit_baseweb-0.1.1.tar` & `streamlit_baseweb-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.983423 streamlit_baseweb-0.1.1/
--rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_baseweb-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      101 2023-07-06 00:06:11.000000 streamlit_baseweb-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4755 2023-07-06 00:17:08.982449 streamlit_baseweb-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2832 2023-07-06 00:14:27.000000 streamlit_baseweb-0.1.1/README.md
--rw-rw-rw-   0        0        0      911 2023-07-06 00:16:01.000000 streamlit_baseweb-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 00:17:08.983423 streamlit_baseweb-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-07-06 00:16:01.000000 streamlit_baseweb-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.913210 streamlit_baseweb-0.1.1/streamlit_baseweb/
--rw-rw-rw-   0        0        0     4453 2023-07-06 00:04:10.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.890997 streamlit_baseweb-0.1.1/streamlit_baseweb/button/
-drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.930452 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/
--rw-rw-rw-   0        0        0      859 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/asset-manifest.json
--rw-rw-rw-   0        0        0     1870 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/index.html
--rw-rw-rw-   0        0        0      564 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/precache-manifest.b5d74bd96e379274fd2ea14bfa52007c.js
--rw-rw-rw-   0        0        0     1183 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/service-worker.js
-drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.891995 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.951924 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/
--rw-rw-rw-   0        0        0   655678 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js
--rw-rw-rw-   0        0        0     1803 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1790536 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.map
--rw-rw-rw-   0        0        0     1191 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js
--rw-rw-rw-   0        0        0     3410 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js.map
--rw-rw-rw-   0        0        0     1590 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js
--rw-rw-rw-   0        0        0     8309 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js.map
-drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.893017 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/
-drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.958908 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/
--rw-rw-rw-   0        0        0      859 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/asset-manifest.json
--rw-rw-rw-   0        0        0     1870 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/index.html
--rw-rw-rw-   0        0        0      564 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/precache-manifest.335beef11633fc996a1434855591b164.js
--rw-rw-rw-   0        0        0     1183 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/service-worker.js
-drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.893998 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.981071 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/
--rw-rw-rw-   0        0        0   700106 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js
--rw-rw-rw-   0        0        0     1803 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1996642 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.map
--rw-rw-rw-   0        0        0     1488 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js
--rw-rw-rw-   0        0        0     4819 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js.map
--rw-rw-rw-   0        0        0     1590 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js
--rw-rw-rw-   0        0        0     8309 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js.map
-drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.924095 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/
--rw-rw-rw-   0        0        0     4755 2023-07-06 00:17:08.000000 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1708 2023-07-06 00:17:08.000000 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 00:17:08.000000 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-06 00:17:08.000000 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2023-07-06 00:17:08.000000 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-06 00:17:08.000000 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 09:27:05.291543 streamlit_baseweb-0.1.2/
+-rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_baseweb-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-07-06 00:06:11.000000 streamlit_baseweb-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4755 2023-07-10 09:27:05.290547 streamlit_baseweb-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2832 2023-07-06 00:14:27.000000 streamlit_baseweb-0.1.2/README.md
+-rw-rw-rw-   0        0        0      911 2023-07-10 09:21:36.000000 streamlit_baseweb-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 09:27:05.292548 streamlit_baseweb-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-07-10 09:21:44.000000 streamlit_baseweb-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:27:05.205245 streamlit_baseweb-0.1.2/streamlit_baseweb/
+-rw-rw-rw-   0        0        0     4077 2023-07-10 09:20:53.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:27:05.175501 streamlit_baseweb-0.1.2/streamlit_baseweb/button/
+drwxrwxrwx   0        0        0        0 2023-07-10 09:27:05.226060 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/
+-rw-rw-rw-   0        0        0      859 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     1870 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/index.html
+-rw-rw-rw-   0        0        0      564 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/precache-manifest.b5d74bd96e379274fd2ea14bfa52007c.js
+-rw-rw-rw-   0        0        0     1183 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/service-worker.js
+drwxrwxrwx   0        0        0        0 2023-07-10 09:27:05.178785 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-10 09:27:05.251608 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/
+-rw-rw-rw-   0        0        0   655678 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js
+-rw-rw-rw-   0        0        0     1803 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1790536 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.map
+-rw-rw-rw-   0        0        0     1191 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js
+-rw-rw-rw-   0        0        0     3410 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js.map
+-rw-rw-rw-   0        0        0     1590 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js
+-rw-rw-rw-   0        0        0     8309 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js.map
+drwxrwxrwx   0        0        0        0 2023-07-10 09:27:05.182057 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/
+drwxrwxrwx   0        0        0        0 2023-07-10 09:27:05.262746 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/
+-rw-rw-rw-   0        0        0      859 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     1870 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/index.html
+-rw-rw-rw-   0        0        0      564 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/precache-manifest.335beef11633fc996a1434855591b164.js
+-rw-rw-rw-   0        0        0     1183 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/service-worker.js
+drwxrwxrwx   0        0        0        0 2023-07-10 09:27:05.184058 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-10 09:27:05.288319 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/
+-rw-rw-rw-   0        0        0   700106 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js
+-rw-rw-rw-   0        0        0     1803 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1996642 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.map
+-rw-rw-rw-   0        0        0     1488 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js
+-rw-rw-rw-   0        0        0     4819 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js.map
+-rw-rw-rw-   0        0        0     1590 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js
+-rw-rw-rw-   0        0        0     8309 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js.map
+drwxrwxrwx   0        0        0        0 2023-07-10 09:27:05.218052 streamlit_baseweb-0.1.2/streamlit_baseweb.egg-info/
+-rw-rw-rw-   0        0        0     4755 2023-07-10 09:27:05.000000 streamlit_baseweb-0.1.2/streamlit_baseweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1708 2023-07-10 09:27:05.000000 streamlit_baseweb-0.1.2/streamlit_baseweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 09:27:05.000000 streamlit_baseweb-0.1.2/streamlit_baseweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-10 09:27:05.000000 streamlit_baseweb-0.1.2/streamlit_baseweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2023-07-10 09:27:05.000000 streamlit_baseweb-0.1.2/streamlit_baseweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-10 09:27:05.000000 streamlit_baseweb-0.1.2/streamlit_baseweb.egg-info/top_level.txt
```

### Comparing `streamlit_baseweb-0.1.1/LICENSE` & `streamlit_baseweb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/PKG-INFO` & `streamlit_baseweb-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_baseweb
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Streamlit implementation of the Base Web library.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/baseweb_components
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamlit_baseweb-0.1.1/README.md` & `streamlit_baseweb-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/pyproject.toml` & `streamlit_baseweb-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit_baseweb"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Streamlit implementation of the Base Web library."
 readme = "README.md"
 authors = [{ name = "Thomas Bouamoud", email = "thomas.bouamoud@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `streamlit_baseweb-0.1.1/setup.py` & `streamlit_baseweb-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_baseweb",
-    version="0.1.1",
+    version="0.1.2",
     author="Thomas Bouamoud",
     author_email="thomas.bouamoud@gmail.com",
     description="A Streamlit implementation of the Base Web library.",
     long_description="https://baseweb.design/",
     long_description_content_type="text/plain",
     url="https://github.com/thomasbs17/streamlit-contributions/baseweb_components",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/__init__.py` & `streamlit_baseweb-0.1.2/streamlit_baseweb/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,36 +62,21 @@
     )
     modal_css = """
     div[data-stale="false"]>iframe[title="streamlit_baseweb.base_web_modal"] {
         position: fixed;
         top: 50%;
         left: 50%;
         transform: translate(-50%, -50%);
-        background-color: rgba(0, 0, 0, 1);
+        background-color: rgba(0, 0, 0, 0);
+        border-radius: 25px;
         z-index: 9999;
     }
-    [data-baseweb="modal"] {
-        background-color: rgba(0, 0, 0, 1);
-    }
     [data-testid="stSidebar"] {
         display: none
     }
-    [data-testid="stHeader"] {
-        background-color: rgba(0, 0, 0, 1);
-        color: rgba(255, 255, 255, 1);
-    }
-    .stApp {
-        position: fixed;
-        top: 0;
-        left: 0;
-        width: 100%;
-        height: 100%;
-        background-color: rgba(0, 0, 0, 1);
-        z-index: 9998;
-    }    
         """
     st.sidebar.markdown(f"<style>{modal_css}</style>", unsafe_allow_html=True)
 
 
 def base_web_button(
     label: str = "Submit",
     disabled: bool = False,
```

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/asset-manifest.json` & `streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/index.html` & `streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/precache-manifest.b5d74bd96e379274fd2ea14bfa52007c.js` & `streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/precache-manifest.b5d74bd96e379274fd2ea14bfa52007c.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/service-worker.js` & `streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js` & `streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.LICENSE.txt` & `streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.map` & `streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js` & `streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js.map` & `streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js` & `streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js.map` & `streamlit_baseweb-0.1.2/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/asset-manifest.json` & `streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/index.html` & `streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/precache-manifest.335beef11633fc996a1434855591b164.js` & `streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/precache-manifest.335beef11633fc996a1434855591b164.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/service-worker.js` & `streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js` & `streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.LICENSE.txt` & `streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.map` & `streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js` & `streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js.map` & `streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js` & `streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js.map` & `streamlit_baseweb-0.1.2/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/PKG-INFO` & `streamlit_baseweb-0.1.2/streamlit_baseweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-baseweb
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Streamlit implementation of the Base Web library.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/baseweb_components
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/SOURCES.txt` & `streamlit_baseweb-0.1.2/streamlit_baseweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

