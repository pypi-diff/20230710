# Comparing `tmp/tos-2.6.0.tar.gz` & `tmp/tos-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tos-2.6.0.tar", last modified: Tue Jul  4 03:28:22 2023, max compression
+gzip compressed data, was "dist/tos-2.6.1.tar", last modified: Mon Jul 10 02:21:05 2023, max compression
```

## Comparing `tos-2.6.0.tar` & `tos-2.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-04 03:28:22.000000 tos-2.6.0/
--rw-r--r--   0 bytedance   (502) staff       (20)     3373 2023-07-04 03:28:22.000000 tos-2.6.0/PKG-INFO
--rw-r--r--   0 bytedance   (502) staff       (20)     2149 2023-07-04 03:26:55.000000 tos-2.6.0/README.md
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-04 03:28:22.000000 tos-2.6.0/tos.egg-info/
--rw-r--r--   0 bytedance   (502) staff       (20)     3373 2023-07-04 03:28:22.000000 tos-2.6.0/tos.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (502) staff       (20)      426 2023-07-04 03:28:22.000000 tos-2.6.0/tos.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (502) staff       (20)       70 2023-07-04 03:28:22.000000 tos-2.6.0/tos.egg-info/requires.txt
--rw-r--r--   0 bytedance   (502) staff       (20)        4 2023-07-04 03:28:22.000000 tos-2.6.0/tos.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (502) staff       (20)        1 2023-07-04 03:28:22.000000 tos-2.6.0/tos.egg-info/dependency_links.txt
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-04 03:28:22.000000 tos-2.6.0/tos/
--rw-r--r--   0 bytedance   (502) staff       (20)    11053 2023-07-04 03:26:55.000000 tos-2.6.0/tos/auth.py
--rw-r--r--   0 bytedance   (502) staff       (20)    71060 2023-07-04 03:26:55.000000 tos-2.6.0/tos/models2.py
--rw-r--r--   0 bytedance   (502) staff       (20)    20455 2022-04-26 02:50:40.000000 tos-2.6.0/tos/mine_type.py
--rw-r--r--   0 bytedance   (502) staff       (20)    25991 2023-07-04 03:26:55.000000 tos-2.6.0/tos/checkpoint.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10701 2023-07-04 03:26:55.000000 tos-2.6.0/tos/models.py
--rw-r--r--   0 bytedance   (502) staff       (20)      111 2023-07-04 03:26:55.000000 tos-2.6.0/tos/log.py
--rw-r--r--   0 bytedance   (502) staff       (20)    47212 2023-07-04 03:26:55.000000 tos-2.6.0/tos/client.py
--rw-r--r--   0 bytedance   (502) staff       (20)      759 2023-07-04 03:26:55.000000 tos-2.6.0/tos/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)       23 2023-07-04 03:26:55.000000 tos-2.6.0/tos/__version__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     1780 2023-07-04 03:26:55.000000 tos-2.6.0/tos/consts.py
--rw-r--r--   0 bytedance   (502) staff       (20)    37822 2023-07-04 03:26:55.000000 tos-2.6.0/tos/utils.py
--rw-r--r--   0 bytedance   (502) staff       (20)     2327 2023-07-04 03:26:55.000000 tos-2.6.0/tos/http.py
--rw-r--r--   0 bytedance   (502) staff       (20)    11459 2023-07-04 03:26:55.000000 tos-2.6.0/tos/convertor.py
--rw-r--r--   0 bytedance   (502) staff       (20)     3348 2023-07-04 03:26:55.000000 tos-2.6.0/tos/exceptions.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6381 2023-07-04 03:26:55.000000 tos-2.6.0/tos/enum.py
--rw-r--r--   0 bytedance   (502) staff       (20)   170603 2023-07-04 03:26:55.000000 tos-2.6.0/tos/clientv2.py
--rw-r--r--   0 bytedance   (502) staff       (20)    18069 2023-07-04 03:26:55.000000 tos-2.6.0/tos/json_utils.py
--rw-r--r--   0 bytedance   (502) staff       (20)     3098 2023-07-04 03:26:55.000000 tos-2.6.0/tos/credential.py
--rw-r--r--   0 bytedance   (502) staff       (20)     1754 2023-07-04 03:26:55.000000 tos-2.6.0/setup.py
--rw-r--r--   0 bytedance   (502) staff       (20)       38 2023-07-04 03:28:22.000000 tos-2.6.0/setup.cfg
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-10 02:21:05.000000 tos-2.6.1/
+-rw-r--r--   0 bytedance   (502) staff       (20)     3373 2023-07-10 02:21:05.000000 tos-2.6.1/PKG-INFO
+-rw-r--r--   0 bytedance   (502) staff       (20)     2149 2023-05-19 09:50:01.000000 tos-2.6.1/README.md
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-10 02:21:05.000000 tos-2.6.1/tos.egg-info/
+-rw-r--r--   0 bytedance   (502) staff       (20)     3373 2023-07-10 02:21:05.000000 tos-2.6.1/tos.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (502) staff       (20)      426 2023-07-10 02:21:05.000000 tos-2.6.1/tos.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)       70 2023-07-10 02:21:05.000000 tos-2.6.1/tos.egg-info/requires.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)        4 2023-07-10 02:21:05.000000 tos-2.6.1/tos.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)        1 2023-07-10 02:21:05.000000 tos-2.6.1/tos.egg-info/dependency_links.txt
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-10 02:21:05.000000 tos-2.6.1/tos/
+-rw-r--r--   0 bytedance   (502) staff       (20)    11053 2023-06-01 07:43:04.000000 tos-2.6.1/tos/auth.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    71070 2023-07-10 02:20:37.000000 tos-2.6.1/tos/models2.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    20455 2022-04-19 06:26:12.000000 tos-2.6.1/tos/mine_type.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    25991 2023-06-01 07:43:04.000000 tos-2.6.1/tos/checkpoint.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    10701 2023-05-19 09:50:01.000000 tos-2.6.1/tos/models.py
+-rw-r--r--   0 bytedance   (502) staff       (20)      111 2023-05-19 09:50:01.000000 tos-2.6.1/tos/log.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    47212 2023-06-01 07:43:04.000000 tos-2.6.1/tos/client.py
+-rw-r--r--   0 bytedance   (502) staff       (20)      759 2023-05-19 09:50:01.000000 tos-2.6.1/tos/__init__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)       23 2023-07-10 02:20:37.000000 tos-2.6.1/tos/__version__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     1780 2023-07-10 02:20:37.000000 tos-2.6.1/tos/consts.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    37822 2023-07-10 02:20:37.000000 tos-2.6.1/tos/utils.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     2327 2023-05-19 09:50:01.000000 tos-2.6.1/tos/http.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    11459 2023-05-19 09:50:01.000000 tos-2.6.1/tos/convertor.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     3348 2023-05-19 09:50:01.000000 tos-2.6.1/tos/exceptions.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     6381 2023-05-22 13:13:00.000000 tos-2.6.1/tos/enum.py
+-rw-r--r--   0 bytedance   (502) staff       (20)   170603 2023-07-10 02:20:37.000000 tos-2.6.1/tos/clientv2.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    18069 2023-07-10 02:20:37.000000 tos-2.6.1/tos/json_utils.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     3098 2023-05-19 09:50:01.000000 tos-2.6.1/tos/credential.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     1754 2023-06-01 07:43:04.000000 tos-2.6.1/setup.py
+-rw-r--r--   0 bytedance   (502) staff       (20)       38 2023-07-10 02:21:05.000000 tos-2.6.1/setup.cfg
```

### Comparing `tos-2.6.0/PKG-INFO` & `tos-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tos
-Version: 2.6.0
+Version: 2.6.1
 Summary: Volc TOS (Tinder Object Storage) SDK
 Home-page: https://www.volcengine.com/
 Author: sunyushan
 Author-email: sunyushan.jason@bytedance.com
 License: UNKNOWN
 Description: 
         # Volcengine TOS SDK for Python
```

### Comparing `tos-2.6.0/README.md` & `tos-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos.egg-info/PKG-INFO` & `tos-2.6.1/tos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tos
-Version: 2.6.0
+Version: 2.6.1
 Summary: Volc TOS (Tinder Object Storage) SDK
 Home-page: https://www.volcengine.com/
 Author: sunyushan
 Author-email: sunyushan.jason@bytedance.com
 License: UNKNOWN
 Description: 
         # Volcengine TOS SDK for Python
```

### Comparing `tos-2.6.0/tos/auth.py` & `tos-2.6.1/tos/auth.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/models2.py` & `tos-2.6.1/tos/models2.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
         self.etag = etag
         self.size = size
         self.owner = owner
         self.storage_class = storage_class
         self.hash_crc64_ecma = hash_crc64_ecma
 
     def __str__(self):
-        info = {"key": self.key, "last_modified": self.key, "etag": self.etag, "size": self.size, "owner": self.owner,
+        info = {"key": self.key, "last_modified": self.last_modified, "etag": self.etag, "size": self.size, "owner": self.owner,
                 "storage_class": self.storage_class, 'hash_crc64_ecma': self.hash_crc64_ecma}
 
         return str(info)
 
 
 class ListedCommonPrefix(object):
     def __init__(self, prefix: str):
```

### Comparing `tos-2.6.0/tos/mine_type.py` & `tos-2.6.1/tos/mine_type.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/checkpoint.py` & `tos-2.6.1/tos/checkpoint.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/models.py` & `tos-2.6.1/tos/models.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/client.py` & `tos-2.6.1/tos/client.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/__init__.py` & `tos-2.6.1/tos/__init__.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/consts.py` & `tos-2.6.1/tos/consts.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/utils.py` & `tos-2.6.1/tos/utils.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/http.py` & `tos-2.6.1/tos/http.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/convertor.py` & `tos-2.6.1/tos/convertor.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/exceptions.py` & `tos-2.6.1/tos/exceptions.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/enum.py` & `tos-2.6.1/tos/enum.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/clientv2.py` & `tos-2.6.1/tos/clientv2.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/json_utils.py` & `tos-2.6.1/tos/json_utils.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/tos/credential.py` & `tos-2.6.1/tos/credential.py`

 * *Files identical despite different names*

### Comparing `tos-2.6.0/setup.py` & `tos-2.6.1/setup.py`

 * *Files identical despite different names*

