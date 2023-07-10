# Comparing `tmp/lytics-smm-demo-0.1.0.tar.gz` & `tmp/lytics-smm-demo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytics-smm-demo-0.1.0.tar", last modified: Mon Jul 10 18:31:27 2023, max compression
+gzip compressed data, was "lytics-smm-demo-0.1.1.tar", last modified: Mon Jul 10 18:45:58 2023, max compression
```

## Comparing `lytics-smm-demo-0.1.0.tar` & `lytics-smm-demo-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 18:31:27.276701 lytics-smm-demo-0.1.0/
--rw-rw-rw-   0        0        0     3202 2023-07-10 18:31:27.225048 lytics-smm-demo-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2924 2023-07-10 18:25:46.000000 lytics-smm-demo-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 18:31:26.615598 lytics-smm-demo-0.1.0/lytics/
--rw-rw-rw-   0        0        0     2680 2023-07-10 18:19:59.000000 lytics-smm-demo-0.1.0/lytics/__init__.py
--rw-rw-rw-   0        0        0     3525 2023-07-10 18:22:01.000000 lytics-smm-demo-0.1.0/lytics/main.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:31:27.223062 lytics-smm-demo-0.1.0/lytics_smm_demo.egg-info/
--rw-rw-rw-   0        0        0     3202 2023-07-10 18:31:25.000000 lytics-smm-demo-0.1.0/lytics_smm_demo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-07-10 18:31:26.000000 lytics-smm-demo-0.1.0/lytics_smm_demo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 18:31:25.000000 lytics-smm-demo-0.1.0/lytics_smm_demo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-10 18:31:25.000000 lytics-smm-demo-0.1.0/lytics_smm_demo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 18:31:27.277695 lytics-smm-demo-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      515 2023-07-10 18:26:06.000000 lytics-smm-demo-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:45:58.789395 lytics-smm-demo-0.1.1/
+-rw-rw-rw-   0        0        0     3202 2023-07-10 18:45:58.759259 lytics-smm-demo-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2924 2023-07-10 18:25:46.000000 lytics-smm-demo-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 18:45:58.274697 lytics-smm-demo-0.1.1/lytics/
+-rw-rw-rw-   0        0        0     2680 2023-07-10 18:19:59.000000 lytics-smm-demo-0.1.1/lytics/__init__.py
+-rw-rw-rw-   0        0        0     3525 2023-07-10 18:22:01.000000 lytics-smm-demo-0.1.1/lytics/main.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:45:58.759259 lytics-smm-demo-0.1.1/lytics_smm_demo.egg-info/
+-rw-rw-rw-   0        0        0     3202 2023-07-10 18:45:56.000000 lytics-smm-demo-0.1.1/lytics_smm_demo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-07-10 18:45:57.000000 lytics-smm-demo-0.1.1/lytics_smm_demo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 18:45:56.000000 lytics-smm-demo-0.1.1/lytics_smm_demo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 18:45:56.000000 lytics-smm-demo-0.1.1/lytics_smm_demo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 18:45:56.000000 lytics-smm-demo-0.1.1/lytics_smm_demo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 18:45:58.790388 lytics-smm-demo-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      568 2023-07-10 18:45:51.000000 lytics-smm-demo-0.1.1/setup.py
```

### Comparing `lytics-smm-demo-0.1.0/PKG-INFO` & `lytics-smm-demo-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytics-smm-demo
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for interacting with the Lytics SMM API
 Home-page: https://github.com/accesstokens/lytics-smm-demo
 Author: Lytics SMM
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # lytics-smm-demo
```

### Comparing `lytics-smm-demo-0.1.0/README.md` & `lytics-smm-demo-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lytics-smm-demo-0.1.0/lytics/__init__.py` & `lytics-smm-demo-0.1.1/lytics/__init__.py`

 * *Files identical despite different names*

### Comparing `lytics-smm-demo-0.1.0/lytics/main.py` & `lytics-smm-demo-0.1.1/lytics/main.py`

 * *Files identical despite different names*

### Comparing `lytics-smm-demo-0.1.0/lytics_smm_demo.egg-info/PKG-INFO` & `lytics-smm-demo-0.1.1/lytics_smm_demo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytics-smm-demo
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for interacting with the Lytics SMM API
 Home-page: https://github.com/accesstokens/lytics-smm-demo
 Author: Lytics SMM
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # lytics-smm-demo
```

### Comparing `lytics-smm-demo-0.1.0/setup.py` & `lytics-smm-demo-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="lytics-smm-demo",
-    version="0.1.0",
+    version="0.1.1",
     author="Lytics SMM",
     description="A Python package for interacting with the Lytics SMM API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/accesstokens/lytics-smm-demo",
     packages=find_packages(),
+    install_requires=[
+        'requests',
+    ],
     python_requires=">=3.6",
 )
```

