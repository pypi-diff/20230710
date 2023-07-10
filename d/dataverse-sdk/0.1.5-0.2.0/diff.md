# Comparing `tmp/dataverse-sdk-0.1.5.tar.gz` & `tmp/dataverse-sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse-sdk-0.1.5.tar", last modified: Sat Jun 17 06:47:36 2023, max compression
+gzip compressed data, was "dataverse-sdk-0.2.0.tar", last modified: Mon Jul 10 09:14:56 2023, max compression
```

## Comparing `dataverse-sdk-0.1.5.tar` & `dataverse-sdk-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.760347 dataverse-sdk-0.1.5/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     6110 2023-06-17 06:47:36.760228 dataverse-sdk-0.1.5/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5870 2023-06-17 03:34:04.000000 dataverse-sdk-0.1.5/README.md
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.757609 dataverse-sdk-0.1.5/dataverse_sdk/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/__init__.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.758539 dataverse-sdk-0.1.5/dataverse_sdk/apis/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/apis/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    10397 2023-06-17 03:34:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/apis/backend.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    21842 2023-06-17 03:34:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1550 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/connections.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      587 2023-06-09 02:47:03.000000 dataverse-sdk-0.1.5/dataverse_sdk/constants.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.758802 dataverse-sdk-0.1.5/dataverse_sdk/exceptions/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/exceptions/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       49 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/exceptions/client.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.759668 dataverse-sdk-0.1.5/dataverse_sdk/schemas/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/schemas/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     3036 2023-05-17 07:09:24.000000 dataverse-sdk-0.1.5/dataverse_sdk/schemas/api.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    10179 2023-06-17 03:34:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/schemas/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1164 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/schemas/common.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.760024 dataverse-sdk-0.1.5/dataverse_sdk/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      657 2023-06-17 03:34:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/utils/utils.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.758339 dataverse-sdk-0.1.5/dataverse_sdk.egg-info/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     6110 2023-06-17 06:47:36.000000 dataverse-sdk-0.1.5/dataverse_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2023-06-17 06:47:36.000000 dataverse-sdk-0.1.5/dataverse_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2023-06-17 06:47:36.000000 dataverse-sdk-0.1.5/dataverse_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       18 2023-06-17 06:47:36.000000 dataverse-sdk-0.1.5/dataverse_sdk.egg-info/requires.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2023-06-17 06:47:36.000000 dataverse-sdk-0.1.5/dataverse_sdk.egg-info/top_level.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2023-06-17 06:47:36.760382 dataverse-sdk-0.1.5/setup.cfg
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      613 2023-06-17 03:34:04.000000 dataverse-sdk-0.1.5/setup.py
+drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.245447 dataverse-sdk-0.2.0/
+-rw-r--r--   0 jasper     (501) staff       (20)     6112 2023-07-10 09:14:56.245239 dataverse-sdk-0.2.0/PKG-INFO
+-rw-r--r--   0 jasper     (501) staff       (20)     5872 2023-07-10 08:54:11.000000 dataverse-sdk-0.2.0/README.md
+drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.241631 dataverse-sdk-0.2.0/dataverse_sdk/
+-rw-r--r--   0 jasper     (501) staff       (20)      825 2023-05-23 03:49:12.000000 dataverse-sdk-0.2.0/dataverse_sdk/__init__.py
+drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.242953 dataverse-sdk-0.2.0/dataverse_sdk/apis/
+-rw-r--r--   0 jasper     (501) staff       (20)        0 2022-11-24 06:20:23.000000 dataverse-sdk-0.2.0/dataverse_sdk/apis/__init__.py
+-rw-r--r--   0 jasper     (501) staff       (20)    10397 2023-07-03 05:45:07.000000 dataverse-sdk-0.2.0/dataverse_sdk/apis/backend.py
+-rw-r--r--   0 jasper     (501) staff       (20)    21842 2023-07-03 05:45:07.000000 dataverse-sdk-0.2.0/dataverse_sdk/client.py
+-rw-r--r--   0 jasper     (501) staff       (20)     1550 2022-11-24 06:20:23.000000 dataverse-sdk-0.2.0/dataverse_sdk/connections.py
+-rw-r--r--   0 jasper     (501) staff       (20)      685 2023-07-10 08:53:08.000000 dataverse-sdk-0.2.0/dataverse_sdk/constants.py
+drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.243482 dataverse-sdk-0.2.0/dataverse_sdk/exceptions/
+-rw-r--r--   0 jasper     (501) staff       (20)        0 2022-11-24 06:20:23.000000 dataverse-sdk-0.2.0/dataverse_sdk/exceptions/__init__.py
+-rw-r--r--   0 jasper     (501) staff       (20)       49 2022-11-24 06:20:23.000000 dataverse-sdk-0.2.0/dataverse_sdk/exceptions/client.py
+drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.244515 dataverse-sdk-0.2.0/dataverse_sdk/schemas/
+-rw-r--r--   0 jasper     (501) staff       (20)        0 2022-11-24 06:20:23.000000 dataverse-sdk-0.2.0/dataverse_sdk/schemas/__init__.py
+-rw-r--r--   0 jasper     (501) staff       (20)     3036 2023-05-23 03:49:12.000000 dataverse-sdk-0.2.0/dataverse_sdk/schemas/api.py
+-rw-r--r--   0 jasper     (501) staff       (20)    10179 2023-07-03 05:45:07.000000 dataverse-sdk-0.2.0/dataverse_sdk/schemas/client.py
+-rw-r--r--   0 jasper     (501) staff       (20)     1164 2023-05-23 03:49:12.000000 dataverse-sdk-0.2.0/dataverse_sdk/schemas/common.py
+drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.244899 dataverse-sdk-0.2.0/dataverse_sdk/utils/
+-rw-r--r--   0 jasper     (501) staff       (20)        0 2023-05-23 03:49:12.000000 dataverse-sdk-0.2.0/dataverse_sdk/utils/__init__.py
+-rw-r--r--   0 jasper     (501) staff       (20)      657 2023-07-03 05:45:07.000000 dataverse-sdk-0.2.0/dataverse_sdk/utils/utils.py
+drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.242637 dataverse-sdk-0.2.0/dataverse_sdk.egg-info/
+-rw-r--r--   0 jasper     (501) staff       (20)     6112 2023-07-10 09:14:56.000000 dataverse-sdk-0.2.0/dataverse_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 jasper     (501) staff       (20)      629 2023-07-10 09:14:56.000000 dataverse-sdk-0.2.0/dataverse_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jasper     (501) staff       (20)        1 2023-07-10 09:14:56.000000 dataverse-sdk-0.2.0/dataverse_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jasper     (501) staff       (20)       18 2023-07-10 09:14:56.000000 dataverse-sdk-0.2.0/dataverse_sdk.egg-info/requires.txt
+-rw-r--r--   0 jasper     (501) staff       (20)       14 2023-07-10 09:14:56.000000 dataverse-sdk-0.2.0/dataverse_sdk.egg-info/top_level.txt
+-rw-r--r--   0 jasper     (501) staff       (20)       38 2023-07-10 09:14:56.245496 dataverse-sdk-0.2.0/setup.cfg
+-rw-r--r--   0 jasper     (501) staff       (20)      613 2023-07-10 08:54:32.000000 dataverse-sdk-0.2.0/setup.py
```

### Comparing `dataverse-sdk-0.1.5/PKG-INFO` & `dataverse-sdk-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 0.1.5
+Version: 0.2.0
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 
@@ -182,15 +182,15 @@
 ```Python
 model = client.get_model(model_id=30)
 model = project.get_model(model_id=30)
 ```
 From the given model, we could get the label file and the triton model file by the commands below.
 ```Python
 status, label_file_path = model.get_label_file(save_path="./labels.txt", timeout=6000)
-status, label_file_path = model.get_triton_model_file(save_path="./model.zip", timeout=6000)
+status, triton_model_path = model.get_triton_model_file(save_path="./model.zip", timeout=6000)
 
 ```
 
 
 ## Troubleshooting
```

### Comparing `dataverse-sdk-0.1.5/README.md` & `dataverse-sdk-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 ```Python
 model = client.get_model(model_id=30)
 model = project.get_model(model_id=30)
 ```
 From the given model, we could get the label file and the triton model file by the commands below.
 ```Python
 status, label_file_path = model.get_label_file(save_path="./labels.txt", timeout=6000)
-status, label_file_path = model.get_triton_model_file(save_path="./model.zip", timeout=6000)
+status, triton_model_path = model.get_triton_model_file(save_path="./model.zip", timeout=6000)
 
 ```
 
 
 ## Troubleshooting
```

### Comparing `dataverse-sdk-0.1.5/dataverse_sdk/__init__.py` & `dataverse-sdk-0.2.0/dataverse_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.5/dataverse_sdk/apis/backend.py` & `dataverse-sdk-0.2.0/dataverse_sdk/apis/backend.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.5/dataverse_sdk/client.py` & `dataverse-sdk-0.2.0/dataverse_sdk/client.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.5/dataverse_sdk/connections.py` & `dataverse-sdk-0.2.0/dataverse_sdk/connections.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.5/dataverse_sdk/constants.py` & `dataverse-sdk-0.2.0/dataverse_sdk/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,11 +9,13 @@
         if cls._value_set is None:
             cls._value_set: set[Any] = {v.value for v in cls.__members__.values()}
 
         return item in cls._value_set
 
 
 class DataverseHost(str, Enum, metaclass=BaseEnumMeta):
-    DEV = "https://dev.visionai.linkernetworks.ai"
-    STAGING = "https://staging.visionai.linkernetworks.ai"
-    DEMO = "https://demo.visionai.linkernetworks.ai"
+    DEV = "https://dev.dataverse.linkervision.ai"
+    DEV2 = "https://dev2.dataverse.linkervision.ai"
+    STAGING = "https://staging.dataverse.linkervision.ai"
+    DEMO = "https://demo.dataverse.linkervision.ai"
+    PUBLIC = "https://dataverse.linkervision.ai"
     LOCAL = "http://localhost:8000"
```

### Comparing `dataverse-sdk-0.1.5/dataverse_sdk/schemas/api.py` & `dataverse-sdk-0.2.0/dataverse_sdk/schemas/api.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.5/dataverse_sdk/schemas/client.py` & `dataverse-sdk-0.2.0/dataverse_sdk/schemas/client.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.5/dataverse_sdk/schemas/common.py` & `dataverse-sdk-0.2.0/dataverse_sdk/schemas/common.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.5/dataverse_sdk/utils/utils.py` & `dataverse-sdk-0.2.0/dataverse_sdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.5/dataverse_sdk.egg-info/PKG-INFO` & `dataverse-sdk-0.2.0/dataverse_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 0.1.5
+Version: 0.2.0
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 
@@ -182,15 +182,15 @@
 ```Python
 model = client.get_model(model_id=30)
 model = project.get_model(model_id=30)
 ```
 From the given model, we could get the label file and the triton model file by the commands below.
 ```Python
 status, label_file_path = model.get_label_file(save_path="./labels.txt", timeout=6000)
-status, label_file_path = model.get_triton_model_file(save_path="./model.zip", timeout=6000)
+status, triton_model_path = model.get_triton_model_file(save_path="./model.zip", timeout=6000)
 
 ```
 
 
 ## Troubleshooting
```

### Comparing `dataverse-sdk-0.1.5/dataverse_sdk.egg-info/SOURCES.txt` & `dataverse-sdk-0.2.0/dataverse_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.5/setup.py` & `dataverse-sdk-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "dataverse-sdk"
-PACKAGE_VERSION = "0.1.5"
+PACKAGE_VERSION = "0.2.0"
 DESC = "Dataverse SDK For Python"
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name=PACKAGE_NAME,
     version=PACKAGE_VERSION,
```

