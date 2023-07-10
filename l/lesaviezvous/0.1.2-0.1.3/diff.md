# Comparing `tmp/lesaviezvous-0.1.2.tar.gz` & `tmp/lesaviezvous-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lesaviezvous-0.1.2.tar", last modified: Mon Jul 10 07:20:26 2023, max compression
+gzip compressed data, was "lesaviezvous-0.1.3.tar", last modified: Mon Jul 10 16:50:23 2023, max compression
```

## Comparing `lesaviezvous-0.1.2.tar` & `lesaviezvous-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 07:20:26.967120 lesaviezvous-0.1.2/
--rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.1.2/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1947 2023-07-10 07:20:26.967120 lesaviezvous-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      865 2023-07-10 07:15:22.000000 lesaviezvous-0.1.2/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 07:20:26.963120 lesaviezvous-0.1.2/lesaviezvous/
--rw-r--r--   0 runner    (1000) runner    (1000)      214 2023-07-10 06:39:24.000000 lesaviezvous-0.1.2/lesaviezvous/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      228 2023-07-10 07:18:13.000000 lesaviezvous-0.1.2/lesaviezvous/lesaviezvous.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 07:20:26.967120 lesaviezvous-0.1.2/lesaviezvous.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1947 2023-07-10 07:20:26.000000 lesaviezvous-0.1.2/lesaviezvous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      274 2023-07-10 07:20:26.000000 lesaviezvous-0.1.2/lesaviezvous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 07:20:26.000000 lesaviezvous-0.1.2/lesaviezvous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-10 07:20:26.000000 lesaviezvous-0.1.2/lesaviezvous.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 07:20:26.000000 lesaviezvous-0.1.2/lesaviezvous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 lesaviezvous-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 07:20:26.967120 lesaviezvous-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      815 2023-07-10 07:19:29.000000 lesaviezvous-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 16:50:23.912023 lesaviezvous-0.1.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1947 2023-07-10 16:50:23.912023 lesaviezvous-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      865 2023-07-10 07:15:22.000000 lesaviezvous-0.1.3/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 16:50:23.912023 lesaviezvous-0.1.3/lesaviezvous/
+-rw-r--r--   0 runner    (1000) runner    (1000)      214 2023-07-10 06:39:24.000000 lesaviezvous-0.1.3/lesaviezvous/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      243 2023-07-10 16:45:22.000000 lesaviezvous-0.1.3/lesaviezvous/lesaviezvous.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 16:50:23.912023 lesaviezvous-0.1.3/lesaviezvous.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1947 2023-07-10 16:50:23.000000 lesaviezvous-0.1.3/lesaviezvous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      274 2023-07-10 16:50:23.000000 lesaviezvous-0.1.3/lesaviezvous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 16:50:23.000000 lesaviezvous-0.1.3/lesaviezvous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-10 16:50:23.000000 lesaviezvous-0.1.3/lesaviezvous.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 16:50:23.000000 lesaviezvous-0.1.3/lesaviezvous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      499 2023-07-10 16:44:12.000000 lesaviezvous-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 16:50:23.912023 lesaviezvous-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      815 2023-07-10 16:46:27.000000 lesaviezvous-0.1.3/setup.py
```

### Comparing `lesaviezvous-0.1.2/LICENSE` & `lesaviezvous-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.1.2/PKG-INFO` & `lesaviezvous-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesaviezvous
-Version: 0.1.2
+Version: 0.1.3
 Summary: Un package Python pour obtenir des informations intéressantes du monde.
 Home-page: https://github.com/codingtuto/lesaviezvouspkg/
 Author: Coding Team
 Author-email: codingteam@telegmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lesaviezvous-0.1.2/README.md` & `lesaviezvous-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.1.2/lesaviezvous.egg-info/PKG-INFO` & `lesaviezvous-0.1.3/lesaviezvous.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesaviezvous
-Version: 0.1.2
+Version: 0.1.3
 Summary: Un package Python pour obtenir des informations intéressantes du monde.
 Home-page: https://github.com/codingtuto/lesaviezvouspkg/
 Author: Coding Team
 Author-email: codingteam@telegmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lesaviezvous-0.1.2/setup.py` & `lesaviezvous-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = ""
 with open('README.md', encoding='utf-8') as file:
   long_description = file.read()
 
 setup(
   name = "lesaviezvous",
-  version = "0.1.2",
+  version = "0.1.3",
   author="Coding Team",
   author_email="codingteam@telegmail.com",
   license='MIT',
   description='Un package Python pour obtenir des informations intéressantes du monde.',
   long_description=render(long_description),
   long_description_content_type="text/markdown",
   url="https://github.com/codingtuto/lesaviezvouspkg/",
```

