# Comparing `tmp/wizata-dsapi-0.2.5.tar.gz` & `tmp/wizata-dsapi-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.2.5.tar", last modified: Mon Jul 10 12:09:50 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.2.6.tar", last modified: Mon Jul 10 12:18:01 2023, max compression
```

## Comparing `wizata-dsapi-0.2.5.tar` & `wizata-dsapi-0.2.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 12:09:50.359044 wizata-dsapi-0.2.5/
--rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0      176 2023-07-10 12:09:50.358038 wizata-dsapi-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-23 08:41:25.000000 wizata-dsapi-0.2.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-10 12:09:50.360037 wizata-dsapi-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-07-10 12:09:46.000000 wizata-dsapi-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 12:09:50.338205 wizata-dsapi-0.2.5/wizata_dsapi/
--rw-rw-rw-   0        0        0     1014 2023-07-10 09:47:53.000000 wizata-dsapi-0.2.5/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.2.5/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     5763 2023-06-18 19:31:22.000000 wizata-dsapi-0.2.5/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     5714 2023-06-12 08:44:45.000000 wizata-dsapi-0.2.5/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-07 10:55:37.000000 wizata-dsapi-0.2.5/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.2.5/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    14903 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.5/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-01 19:11:05.000000 wizata-dsapi-0.2.5/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     9999 2023-06-20 18:59:20.000000 wizata-dsapi-0.2.5/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-06-20 16:08:31.000000 wizata-dsapi-0.2.5/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0    17900 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.5/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.5/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    18221 2023-07-10 09:09:24.000000 wizata-dsapi-0.2.5/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8716 2023-06-14 12:20:26.000000 wizata-dsapi-0.2.5/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     7221 2023-07-10 12:09:46.000000 wizata-dsapi-0.2.5/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2599 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.5/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2701 2023-04-27 15:26:26.000000 wizata-dsapi-0.2.5/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.5/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    56198 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.5/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-07-10 12:09:50.355038 wizata-dsapi-0.2.5/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      176 2023-07-10 12:09:50.000000 wizata-dsapi-0.2.5/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-07-10 12:09:50.000000 wizata-dsapi-0.2.5/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 12:09:50.000000 wizata-dsapi-0.2.5/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-07-10 12:09:50.000000 wizata-dsapi-0.2.5/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-10 12:09:50.000000 wizata-dsapi-0.2.5/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:01.180370 wizata-dsapi-0.2.6/
+-rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      176 2023-07-10 12:18:01.179357 wizata-dsapi-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-23 08:41:25.000000 wizata-dsapi-0.2.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-10 12:18:01.180370 wizata-dsapi-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2023-07-10 12:17:56.000000 wizata-dsapi-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:01.155194 wizata-dsapi-0.2.6/wizata_dsapi/
+-rw-rw-rw-   0        0        0     1014 2023-07-10 09:47:53.000000 wizata-dsapi-0.2.6/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.2.6/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     5763 2023-06-18 19:31:22.000000 wizata-dsapi-0.2.6/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     5714 2023-06-12 08:44:45.000000 wizata-dsapi-0.2.6/wizata_dsapi/datapoint.py
+-rw-rw-rw-   0        0        0     1877 2023-05-07 10:55:37.000000 wizata-dsapi-0.2.6/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.2.6/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    14903 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.6/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3810 2023-06-01 19:11:05.000000 wizata-dsapi-0.2.6/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     9999 2023-06-20 18:59:20.000000 wizata-dsapi-0.2.6/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-06-20 16:08:31.000000 wizata-dsapi-0.2.6/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0    17900 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.6/wizata_dsapi/pipeline.py
+-rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.6/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0    18221 2023-07-10 09:09:24.000000 wizata-dsapi-0.2.6/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     8716 2023-06-14 12:20:26.000000 wizata-dsapi-0.2.6/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     7221 2023-07-10 12:09:46.000000 wizata-dsapi-0.2.6/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2599 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.6/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2762 2023-07-10 12:17:56.000000 wizata-dsapi-0.2.6/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.6/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    56198 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.6/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:01.178388 wizata-dsapi-0.2.6/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-07-10 12:18:01.000000 wizata-dsapi-0.2.6/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-07-10 12:18:01.000000 wizata-dsapi-0.2.6/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 12:18:01.000000 wizata-dsapi-0.2.6/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-07-10 12:18:01.000000 wizata-dsapi-0.2.6/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-10 12:18:01.000000 wizata-dsapi-0.2.6/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.2.5/LICENSE.txt` & `wizata-dsapi-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/setup.py` & `wizata-dsapi-0.2.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.2.5',
+    version='0.2.6',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/__init__.py` & `wizata-dsapi-0.2.6/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.2.6/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.2.6/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.2.6/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.2.6/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.2.6/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/execution.py` & `wizata-dsapi-0.2.6/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/experiment.py` & `wizata-dsapi-0.2.6/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.2.6/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.2.6/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.2.6/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/plot.py` & `wizata-dsapi-0.2.6/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/request.py` & `wizata-dsapi-0.2.6/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/script.py` & `wizata-dsapi-0.2.6/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/template.py` & `wizata-dsapi-0.2.6/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/twin.py` & `wizata-dsapi-0.2.6/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.2.6/wizata_dsapi/twinregistration.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     def __init__(self, twin_registration_id=None, twin_id=None, template_id=None, properties=None):
         if twin_registration_id is None:
             self.twin_registration_id = uuid.uuid4()
         else:
             self.twin_registration_id = twin_registration_id
         self.twin_id = twin_id
         self.template_id = template_id
+        if properties is None:
+            properties = []
         self.properties = properties
 
     def api_id(self) -> str:
         """
         Id of the TwinRegistrations (twin_registration_id)
 
         :return: string formatted UUID of the template.
```

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.2.6/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.2.6/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.5/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.2.6/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

