# Comparing `tmp/apifoncier-0.0.7.tar.gz` & `tmp/apifoncier-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apifoncier-0.0.7.tar", last modified: Mon Jul 10 13:43:57 2023, max compression
+gzip compressed data, was "apifoncier-0.0.8.tar", last modified: Mon Jul 10 15:52:29 2023, max compression
```

## Comparing `apifoncier-0.0.7.tar` & `apifoncier-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 13:43:57.390006 apifoncier-0.0.7/
--rw-rw-rw-   0        0        0     1084 2023-07-10 11:54:34.000000 apifoncier-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     9938 2023-07-10 13:43:57.389006 apifoncier-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     9344 2023-07-07 12:12:49.000000 apifoncier-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 13:43:57.374844 apifoncier-0.0.7/apifoncier/
-drwxrwxrwx   0        0        0        0 2023-07-10 13:43:57.386007 apifoncier-0.0.7/apifoncier/apifoncier.egg-info/
--rw-rw-rw-   0        0        0     9938 2023-07-10 13:43:57.000000 apifoncier-0.0.7/apifoncier/apifoncier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-10 13:43:57.000000 apifoncier-0.0.7/apifoncier/apifoncier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 13:43:57.000000 apifoncier-0.0.7/apifoncier/apifoncier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-10 13:43:57.000000 apifoncier-0.0.7/apifoncier/apifoncier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-10 13:43:57.000000 apifoncier-0.0.7/apifoncier/apifoncier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    22618 2023-07-10 13:36:11.000000 apifoncier-0.0.7/apifoncier/apifoncier.py
--rw-rw-rw-   0        0        0       42 2023-07-10 13:43:57.390006 apifoncier-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1077 2023-07-10 13:23:02.000000 apifoncier-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 15:52:29.637824 apifoncier-0.0.8/
+-rw-rw-rw-   0        0        0     1084 2023-07-10 11:54:34.000000 apifoncier-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     9938 2023-07-10 15:52:29.637824 apifoncier-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9344 2023-07-07 12:12:49.000000 apifoncier-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 15:52:29.625084 apifoncier-0.0.8/apifoncier/
+drwxrwxrwx   0        0        0        0 2023-07-10 15:52:29.635827 apifoncier-0.0.8/apifoncier/apifoncier.egg-info/
+-rw-rw-rw-   0        0        0     9938 2023-07-10 15:52:29.000000 apifoncier-0.0.8/apifoncier/apifoncier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-07-10 15:52:29.000000 apifoncier-0.0.8/apifoncier/apifoncier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 15:52:29.000000 apifoncier-0.0.8/apifoncier/apifoncier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-10 15:52:29.000000 apifoncier-0.0.8/apifoncier/apifoncier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       45 2023-07-10 15:52:29.000000 apifoncier-0.0.8/apifoncier/apifoncier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2987 2023-07-10 15:48:13.000000 apifoncier-0.0.8/apifoncier/cartofriches.py
+-rw-rw-rw-   0        0        0     5083 2023-07-10 15:45:16.000000 apifoncier-0.0.8/apifoncier/ind_conso_espace.py
+-rw-rw-rw-   0        0        0     5349 2023-07-10 15:52:23.000000 apifoncier-0.0.8/apifoncier/ind_dv3f.py
+-rw-rw-rw-   0        0        0     9809 2023-07-10 15:15:11.000000 apifoncier-0.0.8/apifoncier/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-10 15:52:29.638824 apifoncier-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1163 2023-07-10 15:39:36.000000 apifoncier-0.0.8/setup.py
```

### Comparing `apifoncier-0.0.7/LICENSE` & `apifoncier-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.7/PKG-INFO` & `apifoncier-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apifoncier
-Version: 0.0.7
+Version: 0.0.8
 Summary: Mobiliser les données foncières de l'api du Cerema directement avec python
 Home-page: https://github.com/rcadot/py.apifoncier
 Author: Romain Cadot
 Author-email: romain.cadot@cerema.fr
 License: MIT
 Keywords: api,foncier,cerema,dv3f,friches,artificialisation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apifoncier-0.0.7/README.md` & `apifoncier-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.7/apifoncier/apifoncier.egg-info/PKG-INFO` & `apifoncier-0.0.8/apifoncier/apifoncier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apifoncier
-Version: 0.0.7
+Version: 0.0.8
 Summary: Mobiliser les données foncières de l'api du Cerema directement avec python
 Home-page: https://github.com/rcadot/py.apifoncier
 Author: Romain Cadot
 Author-email: romain.cadot@cerema.fr
 License: MIT
 Keywords: api,foncier,cerema,dv3f,friches,artificialisation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apifoncier-0.0.7/setup.py` & `apifoncier-0.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from setuptools import find_packages, setup
 
 with open("README.md","r",encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name = "apifoncier",
-    version = "0.0.7",
+    version = "0.0.8",
     description = "Mobiliser les données foncières de l'api du Cerema directement avec python",
     package_dir={"":"apifoncier"},
     packages=find_packages(where="apifoncier"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rcadot/py.apifoncier",
     author="Romain Cadot",
     author_email="romain.cadot@cerema.fr",
     license="MIT",
     classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     ],
-    py_modules=["apifoncier"],
+    py_modules=[
+        "utils",
+        "cartofriches",
+        "ind_conso_espace",
+        "ind_dv3f"
+    ],
     keywords = ["api", "foncier", "cerema","dv3f","friches","artificialisation"],
     install_requires=["pandas","requests","plotly.express","geopandas"],
     extras_require={
         "dev": [
             "pytest"
         ]
     },
```

