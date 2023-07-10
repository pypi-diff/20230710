# Comparing `tmp/lesaviezvous-0.1.6.tar.gz` & `tmp/lesaviezvous-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lesaviezvous-0.1.6.tar", last modified: Mon Jul 10 17:33:01 2023, max compression
+gzip compressed data, was "lesaviezvous-0.1.9.tar", last modified: Mon Jul 10 17:44:34 2023, max compression
```

## Comparing `lesaviezvous-0.1.6.tar` & `lesaviezvous-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:33:01.459176 lesaviezvous-0.1.6/
--rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.1.6/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1339 2023-07-10 17:33:01.459176 lesaviezvous-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      501 2023-07-10 17:27:03.000000 lesaviezvous-0.1.6/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:33:01.459176 lesaviezvous-0.1.6/lesaviezvous/
--rw-r--r--   0 runner    (1000) runner    (1000)      214 2023-07-10 06:39:24.000000 lesaviezvous-0.1.6/lesaviezvous/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    79461 2023-07-10 17:32:13.000000 lesaviezvous-0.1.6/lesaviezvous/dp.py
--rw-r--r--   0 runner    (1000) runner    (1000)       96 2023-07-10 17:25:18.000000 lesaviezvous-0.1.6/lesaviezvous/lesaviezvous.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:33:01.459176 lesaviezvous-0.1.6/lesaviezvous.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1339 2023-07-10 17:33:01.000000 lesaviezvous-0.1.6/lesaviezvous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      258 2023-07-10 17:33:01.000000 lesaviezvous-0.1.6/lesaviezvous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 17:33:01.000000 lesaviezvous-0.1.6/lesaviezvous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 17:33:01.000000 lesaviezvous-0.1.6/lesaviezvous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      499 2023-07-10 16:44:12.000000 lesaviezvous-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 17:33:01.459176 lesaviezvous-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      769 2023-07-10 17:32:33.000000 lesaviezvous-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:44:34.502527 lesaviezvous-0.1.9/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1339 2023-07-10 17:44:34.502527 lesaviezvous-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      501 2023-07-10 17:27:03.000000 lesaviezvous-0.1.9/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:44:34.502527 lesaviezvous-0.1.9/lesaviezvous/
+-rw-r--r--   0 runner    (1000) runner    (1000)      214 2023-07-10 06:39:24.000000 lesaviezvous-0.1.9/lesaviezvous/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    79461 2023-07-10 17:37:05.000000 lesaviezvous-0.1.9/lesaviezvous/db.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       97 2023-07-10 17:41:41.000000 lesaviezvous-0.1.9/lesaviezvous/lesaviezvous.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:44:34.502527 lesaviezvous-0.1.9/lesaviezvous.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1339 2023-07-10 17:44:34.000000 lesaviezvous-0.1.9/lesaviezvous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      258 2023-07-10 17:44:34.000000 lesaviezvous-0.1.9/lesaviezvous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 17:44:34.000000 lesaviezvous-0.1.9/lesaviezvous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 17:44:34.000000 lesaviezvous-0.1.9/lesaviezvous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      513 2023-07-10 17:36:39.000000 lesaviezvous-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 17:44:34.502527 lesaviezvous-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      769 2023-07-10 17:44:31.000000 lesaviezvous-0.1.9/setup.py
```

### Comparing `lesaviezvous-0.1.6/LICENSE` & `lesaviezvous-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.1.6/PKG-INFO` & `lesaviezvous-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesaviezvous
-Version: 0.1.6
+Version: 0.1.9
 Summary: Un package Python pour obtenir des informations intéressantes du monde.
 Home-page: https://github.com/codingtuto/lesaviezvouspkg/
 Author: Coding Team
 Author-email: codingteam@telegmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `lesaviezvous-0.1.6/lesaviezvous/dp.py` & `lesaviezvous-0.1.9/lesaviezvous/db.py`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.1.6/lesaviezvous.egg-info/PKG-INFO` & `lesaviezvous-0.1.9/lesaviezvous.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesaviezvous
-Version: 0.1.6
+Version: 0.1.9
 Summary: Un package Python pour obtenir des informations intéressantes du monde.
 Home-page: https://github.com/codingtuto/lesaviezvouspkg/
 Author: Coding Team
 Author-email: codingteam@telegmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `lesaviezvous-0.1.6/setup.py` & `lesaviezvous-0.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = ""
 with open('README.md', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name="lesaviezvous",
-    version="0.1.6",
+    version="0.1.9",
     author="Coding Team",
     author_email="codingteam@telegmail.com",
     license='MIT',
     description='Un package Python pour obtenir des informations intéressantes du monde.',
     long_description=render(long_description),
     long_description_content_type="text/markdown",
     url="https://github.com/codingtuto/lesaviezvouspkg/",
```

