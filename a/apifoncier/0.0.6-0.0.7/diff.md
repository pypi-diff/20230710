# Comparing `tmp/apifoncier-0.0.6.tar.gz` & `tmp/apifoncier-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apifoncier-0.0.6.tar", last modified: Mon Jul 10 12:41:40 2023, max compression
+gzip compressed data, was "apifoncier-0.0.7.tar", last modified: Mon Jul 10 13:43:57 2023, max compression
```

## Comparing `apifoncier-0.0.6.tar` & `apifoncier-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 12:41:40.706169 apifoncier-0.0.6/
--rw-rw-rw-   0        0        0     1084 2023-07-10 11:54:34.000000 apifoncier-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     9917 2023-07-10 12:41:40.704174 apifoncier-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     9344 2023-07-07 12:12:49.000000 apifoncier-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 12:41:40.684168 apifoncier-0.0.6/apifoncier/
-drwxrwxrwx   0        0        0        0 2023-07-10 12:41:40.701171 apifoncier-0.0.6/apifoncier/apifoncier.egg-info/
--rw-rw-rw-   0        0        0     9917 2023-07-10 12:41:40.000000 apifoncier-0.0.6/apifoncier/apifoncier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-07-10 12:41:40.000000 apifoncier-0.0.6/apifoncier/apifoncier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 12:41:40.000000 apifoncier-0.0.6/apifoncier/apifoncier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-10 12:41:40.000000 apifoncier-0.0.6/apifoncier/apifoncier.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 12:41:40.000000 apifoncier-0.0.6/apifoncier/apifoncier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 12:41:40.707176 apifoncier-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      964 2023-07-10 12:41:34.000000 apifoncier-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:43:57.390006 apifoncier-0.0.7/
+-rw-rw-rw-   0        0        0     1084 2023-07-10 11:54:34.000000 apifoncier-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     9938 2023-07-10 13:43:57.389006 apifoncier-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9344 2023-07-07 12:12:49.000000 apifoncier-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 13:43:57.374844 apifoncier-0.0.7/apifoncier/
+drwxrwxrwx   0        0        0        0 2023-07-10 13:43:57.386007 apifoncier-0.0.7/apifoncier/apifoncier.egg-info/
+-rw-rw-rw-   0        0        0     9938 2023-07-10 13:43:57.000000 apifoncier-0.0.7/apifoncier/apifoncier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-10 13:43:57.000000 apifoncier-0.0.7/apifoncier/apifoncier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 13:43:57.000000 apifoncier-0.0.7/apifoncier/apifoncier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-10 13:43:57.000000 apifoncier-0.0.7/apifoncier/apifoncier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-10 13:43:57.000000 apifoncier-0.0.7/apifoncier/apifoncier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    22618 2023-07-10 13:36:11.000000 apifoncier-0.0.7/apifoncier/apifoncier.py
+-rw-rw-rw-   0        0        0       42 2023-07-10 13:43:57.390006 apifoncier-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1077 2023-07-10 13:23:02.000000 apifoncier-0.0.7/setup.py
```

### Comparing `apifoncier-0.0.6/LICENSE` & `apifoncier-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.6/PKG-INFO` & `apifoncier-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: apifoncier
-Version: 0.0.6
+Version: 0.0.7
 Summary: Mobiliser les données foncières de l'api du Cerema directement avec python
 Home-page: https://github.com/rcadot/py.apifoncier
 Author: Romain Cadot
 Author-email: romain.cadot@cerema.fr
 License: MIT
 Keywords: api,foncier,cerema,dv3f,friches,artificialisation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
  
 
 > 🚧 Avertissement
 >
 > Il s’agit d’une version de développement. Des modifications sur les
```

### Comparing `apifoncier-0.0.6/README.md` & `apifoncier-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.6/apifoncier/apifoncier.egg-info/PKG-INFO` & `apifoncier-0.0.7/apifoncier/apifoncier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: apifoncier
-Version: 0.0.6
+Version: 0.0.7
 Summary: Mobiliser les données foncières de l'api du Cerema directement avec python
 Home-page: https://github.com/rcadot/py.apifoncier
 Author: Romain Cadot
 Author-email: romain.cadot@cerema.fr
 License: MIT
 Keywords: api,foncier,cerema,dv3f,friches,artificialisation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
  
 
 > 🚧 Avertissement
 >
 > Il s’agit d’une version de développement. Des modifications sur les
```

### Comparing `apifoncier-0.0.6/setup.py` & `apifoncier-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from setuptools import find_packages, setup
 
 with open("README.md","r",encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name = "apifoncier",
-    version = "0.0.6",
+    version = "0.0.7",
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
+    py_modules=["apifoncier"],
     keywords = ["api", "foncier", "cerema","dv3f","friches","artificialisation"],
     install_requires=["pandas","requests","plotly.express","geopandas"],
+    extras_require={
+        "dev": [
+            "pytest"
+        ]
+    },
     python_requires=">=3.10.9"
 )
```

