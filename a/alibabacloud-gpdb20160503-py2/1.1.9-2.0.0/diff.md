# Comparing `tmp/alibabacloud_gpdb20160503_py2-1.1.9.tar.gz` & `tmp/alibabacloud_gpdb20160503_py2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gpdb20160503_py2-1.1.9.tar", last modified: Mon May 30 12:27:25 2022, max compression
+gzip compressed data, was "dist/alibabacloud_gpdb20160503_py2-2.0.0.tar", last modified: Mon Jul 10 03:44:51 2023, max compression
```

## Comparing `alibabacloud_gpdb20160503_py2-1.1.9.tar` & `alibabacloud_gpdb20160503_py2-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-30 12:27:25.000000 alibabacloud_gpdb20160503_py2-1.1.9/
--rw-r--r--   0 root         (0) root         (0)      159 2022-05-30 12:27:24.000000 alibabacloud_gpdb20160503_py2-1.1.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-05-30 12:27:24.000000 alibabacloud_gpdb20160503_py2-1.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-05-30 12:27:24.000000 alibabacloud_gpdb20160503_py2-1.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2499 2022-05-30 12:27:25.000000 alibabacloud_gpdb20160503_py2-1.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2022-05-30 12:27:24.000000 alibabacloud_gpdb20160503_py2-1.1.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2022-05-30 12:27:24.000000 alibabacloud_gpdb20160503_py2-1.1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-30 12:27:25.000000 alibabacloud_gpdb20160503_py2-1.1.9/alibabacloud_gpdb20160503/
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-30 12:27:24.000000 alibabacloud_gpdb20160503_py2-1.1.9/alibabacloud_gpdb20160503/__init__.py
--rw-r--r--   0 root         (0) root         (0)   103740 2022-05-30 12:27:24.000000 alibabacloud_gpdb20160503_py2-1.1.9/alibabacloud_gpdb20160503/client.py
--rw-r--r--   0 root         (0) root         (0)   455741 2022-05-30 12:27:24.000000 alibabacloud_gpdb20160503_py2-1.1.9/alibabacloud_gpdb20160503/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-30 12:27:25.000000 alibabacloud_gpdb20160503_py2-1.1.9/alibabacloud_gpdb20160503_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2499 2022-05-30 12:27:25.000000 alibabacloud_gpdb20160503_py2-1.1.9/alibabacloud_gpdb20160503_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2022-05-30 12:27:25.000000 alibabacloud_gpdb20160503_py2-1.1.9/alibabacloud_gpdb20160503_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-30 12:27:25.000000 alibabacloud_gpdb20160503_py2-1.1.9/alibabacloud_gpdb20160503_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-05-30 12:27:25.000000 alibabacloud_gpdb20160503_py2-1.1.9/alibabacloud_gpdb20160503_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2022-05-30 12:27:25.000000 alibabacloud_gpdb20160503_py2-1.1.9/alibabacloud_gpdb20160503_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-05-30 12:27:25.000000 alibabacloud_gpdb20160503_py2-1.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2929 2022-05-30 12:27:24.000000 alibabacloud_gpdb20160503_py2-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      924 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   224085 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503/client.py
+-rw-r--r--   0 root         (0) root         (0)   743628 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2929 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/setup.py
```

### Comparing `alibabacloud_gpdb20160503_py2-1.1.9/LICENSE` & `alibabacloud_gpdb20160503_py2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503_py2-1.1.9/PKG-INFO` & `alibabacloud_gpdb20160503_py2-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gpdb20160503_py2
-Version: 1.1.9
+Version: 2.0.0
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503_py2-1.1.9/README-CN.md` & `alibabacloud_gpdb20160503_py2-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503_py2-1.1.9/README.md` & `alibabacloud_gpdb20160503_py2-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503_py2-1.1.9/alibabacloud_gpdb20160503_py2.egg-info/PKG-INFO` & `alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gpdb20160503-py2
-Version: 1.1.9
+Version: 2.0.0
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503_py2-1.1.9/setup.py` & `alibabacloud_gpdb20160503_py2-2.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gpdb20160503_py2.
 
-Created on 30/05/2022
+Created on 10/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gpdb20160503"
 NAME = "alibabacloud_gpdb20160503_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.5, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

