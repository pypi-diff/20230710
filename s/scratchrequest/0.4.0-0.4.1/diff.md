# Comparing `tmp/scratchrequest-0.4.0.tar.gz` & `tmp/scratchrequest-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchrequest-0.4.0.tar", last modified: Thu Jul  6 16:40:45 2023, max compression
+gzip compressed data, was "scratchrequest-0.4.1.tar", last modified: Mon Jul 10 19:24:26 2023, max compression
```

## Comparing `scratchrequest-0.4.0.tar` & `scratchrequest-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 16:40:45.529260 scratchrequest-0.4.0/
--rw-rw-rw-   0        0        0     1091 2023-07-06 16:37:14.000000 scratchrequest-0.4.0/LICENSE
--rw-rw-rw-   0        0        0      724 2023-07-06 16:40:45.529260 scratchrequest-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0        2 2023-07-06 16:23:32.000000 scratchrequest-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 16:40:45.482386 scratchrequest-0.4.0/scratchrequest/
--rw-rw-rw-   0        0        0      158 2023-07-03 18:02:47.000000 scratchrequest-0.4.0/scratchrequest/__init__.py
--rw-rw-rw-   0        0        0     9912 2023-07-03 16:44:51.000000 scratchrequest-0.4.0/scratchrequest/_cloud.py
--rw-rw-rw-   0        0        0      146 2023-07-03 16:24:00.000000 scratchrequest-0.4.0/scratchrequest/_exceptions.py
--rw-rw-rw-   0        0        0     2823 2023-07-03 16:46:04.000000 scratchrequest-0.4.0/scratchrequest/_session.py
--rw-rw-rw-   0        0        0     2974 2023-07-03 18:36:49.000000 scratchrequest-0.4.0/scratchrequest/_twcloud.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:40:45.513635 scratchrequest-0.4.0/scratchrequest.egg-info/
--rw-rw-rw-   0        0        0      724 2023-07-06 16:40:45.000000 scratchrequest-0.4.0/scratchrequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-07-06 16:40:45.000000 scratchrequest-0.4.0/scratchrequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 16:40:45.000000 scratchrequest-0.4.0/scratchrequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-06 16:40:45.000000 scratchrequest-0.4.0/scratchrequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-06 16:40:45.000000 scratchrequest-0.4.0/scratchrequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 16:40:45.529260 scratchrequest-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-07-06 16:29:50.000000 scratchrequest-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 19:24:26.453910 scratchrequest-0.4.1/
+-rw-rw-rw-   0        0        0     1091 2023-07-06 16:37:14.000000 scratchrequest-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0      724 2023-07-10 19:24:26.434911 scratchrequest-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2023-07-06 16:23:32.000000 scratchrequest-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 19:24:26.306909 scratchrequest-0.4.1/scratchrequest/
+-rw-rw-rw-   0        0        0      158 2023-07-03 18:02:47.000000 scratchrequest-0.4.1/scratchrequest/__init__.py
+-rw-rw-rw-   0        0        0     9912 2023-07-03 16:44:51.000000 scratchrequest-0.4.1/scratchrequest/_cloud.py
+-rw-rw-rw-   0        0        0      146 2023-07-03 16:24:00.000000 scratchrequest-0.4.1/scratchrequest/_exceptions.py
+-rw-rw-rw-   0        0        0     3146 2023-07-10 18:52:37.000000 scratchrequest-0.4.1/scratchrequest/_session.py
+-rw-rw-rw-   0        0        0     2974 2023-07-03 18:36:49.000000 scratchrequest-0.4.1/scratchrequest/_twcloud.py
+drwxrwxrwx   0        0        0        0 2023-07-10 19:24:26.428909 scratchrequest-0.4.1/scratchrequest.egg-info/
+-rw-rw-rw-   0        0        0      724 2023-07-10 19:24:25.000000 scratchrequest-0.4.1/scratchrequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-07-10 19:24:26.000000 scratchrequest-0.4.1/scratchrequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 19:24:25.000000 scratchrequest-0.4.1/scratchrequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-10 19:24:25.000000 scratchrequest-0.4.1/scratchrequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-10 19:24:25.000000 scratchrequest-0.4.1/scratchrequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 19:24:26.455912 scratchrequest-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-07-10 19:22:33.000000 scratchrequest-0.4.1/setup.py
```

### Comparing `scratchrequest-0.4.0/LICENSE` & `scratchrequest-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchrequest-0.4.0/PKG-INFO` & `scratchrequest-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchrequest
-Version: 0.4.0
+Version: 0.4.1
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/programordie2/scratchrequest
 Author: programORdie
 Author-email: 
 Keywords: scratch api,scratchrequest,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchrequest-0.4.0/scratchrequest/_cloud.py` & `scratchrequest-0.4.1/scratchrequest/_cloud.py`

 * *Files identical despite different names*

### Comparing `scratchrequest-0.4.0/scratchrequest/_session.py` & `scratchrequest-0.4.1/scratchrequest/_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,20 @@
             "scratchsessionsid": self.session_id,
             "scratchcsrftoken": "a",
             "scratchlanguage": "en",
         }).json()
         try:
             self.xtoken = account["user"]["token"]
             self.headers["X-Token"] = self.xtoken
+            self.all_login_data = account
+            self.id = account['user']['id']
+            self.username = account['user']['username']
+            self.banned = account['user']['banned']
+            self.email = account['user']['email']
+            self.new_scratcher = account['permissions']['new_scratcher']
         except KeyError:
             raise LoginError("Your login data was wrong. Check if you spelled your credits correctly, or if you are in replit, see the docs for more information.")
 
     @classmethod
     def login(cls, username : str, password : str):
         '''
         Login from your username and password.
```

### Comparing `scratchrequest-0.4.0/scratchrequest/_twcloud.py` & `scratchrequest-0.4.1/scratchrequest/_twcloud.py`

 * *Files identical despite different names*

### Comparing `scratchrequest-0.4.0/scratchrequest.egg-info/PKG-INFO` & `scratchrequest-0.4.1/scratchrequest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchrequest
-Version: 0.4.0
+Version: 0.4.1
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/programordie2/scratchrequest
 Author: programORdie
 Author-email: 
 Keywords: scratch api,scratchrequest,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchrequest-0.4.0/setup.py` & `scratchrequest-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.4.0'
+VERSION = '0.4.1'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchrequest",
     version=VERSION,
```

