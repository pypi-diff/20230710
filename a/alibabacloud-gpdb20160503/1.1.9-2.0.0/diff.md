# Comparing `tmp/alibabacloud_gpdb20160503-1.1.9.tar.gz` & `tmp/alibabacloud_gpdb20160503-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gpdb20160503-1.1.9.tar", last modified: Mon Jun 27 06:57:58 2022, max compression
+gzip compressed data, was "dist/alibabacloud_gpdb20160503-2.0.0.tar", last modified: Mon Jul 10 03:44:50 2023, max compression
```

## Comparing `alibabacloud_gpdb20160503-1.1.9.tar` & `alibabacloud_gpdb20160503-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/
--rw-r--r--   0 root         (0) root         (0)      307 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2355 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/alibabacloud_gpdb20160503/
--rw-r--r--   0 root         (0) root         (0)       21 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/alibabacloud_gpdb20160503/__init__.py
--rw-r--r--   0 root         (0) root         (0)   287454 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/alibabacloud_gpdb20160503/client.py
--rw-r--r--   0 root         (0) root         (0)   533081 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/alibabacloud_gpdb20160503/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/alibabacloud_gpdb20160503.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2355 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/alibabacloud_gpdb20160503.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/alibabacloud_gpdb20160503.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/alibabacloud_gpdb20160503.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/alibabacloud_gpdb20160503.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/alibabacloud_gpdb20160503.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2022-06-27 06:57:58.000000 alibabacloud_gpdb20160503-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   505840 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503/client.py
+-rw-r--r--   0 root         (0) root         (0)   737881 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/setup.py
```

### Comparing `alibabacloud_gpdb20160503-1.1.9/LICENSE` & `alibabacloud_gpdb20160503-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503-1.1.9/PKG-INFO` & `alibabacloud_gpdb20160503-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gpdb20160503
-Version: 1.1.9
+Version: 2.0.0
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503-1.1.9/README-CN.md` & `alibabacloud_gpdb20160503-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503-1.1.9/README.md` & `alibabacloud_gpdb20160503-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503-1.1.9/alibabacloud_gpdb20160503.egg-info/PKG-INFO` & `alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gpdb20160503
-Version: 1.1.9
+Version: 2.0.0
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503-1.1.9/setup.py` & `alibabacloud_gpdb20160503-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gpdb20160503.
 
-Created on 27/06/2022
+Created on 10/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gpdb20160503"
 NAME = "alibabacloud_gpdb20160503" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

