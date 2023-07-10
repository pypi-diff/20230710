# Comparing `tmp/mekab-2.0.5.tar.gz` & `tmp/mekab-8.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mekab-2.0.5.tar", last modified: Sun Jul  9 11:33:52 2023, max compression
+gzip compressed data, was "mekab-8.9.5.tar", last modified: Mon Jul 10 12:04:26 2023, max compression
```

## Comparing `mekab-2.0.5.tar` & `mekab-8.9.5.tar`

### file list

```diff
@@ -1,40 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 11:33:52.271050 mekab-2.0.5/
--rw-r--r--   0 root         (0) root         (0)     2510 2023-07-09 11:33:52.271050 mekab-2.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1584 2023-07-09 09:20:41.000000 mekab-2.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 11:33:52.263049 mekab-2.0.5/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)     1051 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 11:33:52.263049 mekab-2.0.5/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)     1737 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/load.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 11:33:52.267049 mekab-2.0.5/kynaylibs/nan/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 11:33:52.267049 mekab-2.0.5/kynaylibs/nan/utils/db/
--rw-r--r--   0 root         (0) root         (0)    14229 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/function.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/get_id.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     2061 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/pilter.py
--rw-r--r--   0 root         (0) root         (0)    17772 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/nan/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-09 09:20:41.000000 mekab-2.0.5/kynaylibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 11:33:52.271050 mekab-2.0.5/mekab.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2510 2023-07-09 11:33:52.000000 mekab-2.0.5/mekab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      901 2023-07-09 11:33:52.000000 mekab-2.0.5/mekab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 11:33:52.000000 mekab-2.0.5/mekab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-09 11:33:52.000000 mekab-2.0.5/mekab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-09 11:33:52.000000 mekab-2.0.5/mekab.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 11:33:52.271050 mekab-2.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-09 11:31:58.000000 mekab-2.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 12:04:26.402769 mekab-8.9.5/
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-07-10 12:04:26.402769 mekab-8.9.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-07-09 09:20:41.000000 mekab-8.9.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 12:04:26.402769 mekab-8.9.5/mekab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-07-10 12:04:26.000000 mekab-8.9.5/mekab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-10 12:04:26.000000 mekab-8.9.5/mekab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 12:04:26.000000 mekab-8.9.5/mekab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-10 12:04:26.000000 mekab-8.9.5/mekab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 12:04:26.000000 mekab-8.9.5/mekab.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 12:04:26.402769 mekab-8.9.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 12:03:58.000000 mekab-8.9.5/setup.py
```

### Comparing `mekab-2.0.5/PKG-INFO` & `mekab-8.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mekab
-Version: 2.0.5
+Version: 8.9.5
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
-Author: bakem
+Author: cariin
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
 Project-URL: Source Code, https://github.com/naya1503/kynaylibs
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `mekab-2.0.5/README.md` & `mekab-8.9.5/README.md`

 * *Files identical despite different names*

### Comparing `mekab-2.0.5/mekab.egg-info/PKG-INFO` & `mekab-8.9.5/mekab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mekab
-Version: 2.0.5
+Version: 8.9.5
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
-Author: bakem
+Author: cariin
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
 Project-URL: Source Code, https://github.com/naya1503/kynaylibs
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `mekab-2.0.5/setup.py` & `mekab-8.9.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import re 
 import setuptools
- 
-with open("requirements.txt", encoding="utf-8") as r:
-    requirements = [i.strip() for i in r] 
- 
+  
 with open("kynaylibs/version.py", "rt", encoding="utf8") as x:
     version = re.search(r'version = "(.*?)"', x.read()).group(1) 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read() 
 name = "mekab" 
-author = "bakem" 
+author = "cariin" 
 author_email = "cosmospanas70@gmail.com" 
 description = "A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro." 
 license_ = "GNU AFFERO GENERAL PUBLIC LICENSE (v3)" 
 url = "https://github.com/naya1503/kynaylibs" 
 project_urls = {
     "Bug Tracker": "https://github.com/naya1503/kynaylibs/issues", 
     "Documentation": "https://t.me/kynansupport", "Source Code": 
@@ -39,11 +36,11 @@
     description=description, 
     long_description=long_description, 
     long_description_content_type="text/markdown", 
     url=url, 
     project_urls=project_urls, 
     license=license_, 
     packages=setuptools.find_packages(), 
-    install_requires=requirements, 
+    install_requires=["aiosqlite<0.18.0,>=0.16.0", "pyaes==1.6.1", "pysocks==1.7.1", "pytgcalls==3.0.0.dev24", "pytz", "tgcrypto"], 
     classifiers=classifiers, 
     python_requires=">3.7, <3.12",
 )
```

