# Comparing `tmp/wizata-dsapi-0.2.6.tar.gz` & `tmp/wizata-dsapi-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.2.6.tar", last modified: Mon Jul 10 12:18:01 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.2.7.tar", last modified: Mon Jul 10 14:02:28 2023, max compression
```

## Comparing `wizata-dsapi-0.2.6.tar` & `wizata-dsapi-0.2.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 12:18:01.180370 wizata-dsapi-0.2.6/
--rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.2.6/LICENSE.txt
--rw-rw-rw-   0        0        0      176 2023-07-10 12:18:01.179357 wizata-dsapi-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-23 08:41:25.000000 wizata-dsapi-0.2.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-10 12:18:01.180370 wizata-dsapi-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-07-10 12:17:56.000000 wizata-dsapi-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 12:18:01.155194 wizata-dsapi-0.2.6/wizata_dsapi/
--rw-rw-rw-   0        0        0     1014 2023-07-10 09:47:53.000000 wizata-dsapi-0.2.6/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.2.6/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     5763 2023-06-18 19:31:22.000000 wizata-dsapi-0.2.6/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     5714 2023-06-12 08:44:45.000000 wizata-dsapi-0.2.6/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-07 10:55:37.000000 wizata-dsapi-0.2.6/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.2.6/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    14903 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.6/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-01 19:11:05.000000 wizata-dsapi-0.2.6/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     9999 2023-06-20 18:59:20.000000 wizata-dsapi-0.2.6/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-06-20 16:08:31.000000 wizata-dsapi-0.2.6/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0    17900 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.6/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.6/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    18221 2023-07-10 09:09:24.000000 wizata-dsapi-0.2.6/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8716 2023-06-14 12:20:26.000000 wizata-dsapi-0.2.6/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     7221 2023-07-10 12:09:46.000000 wizata-dsapi-0.2.6/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2599 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.6/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2762 2023-07-10 12:17:56.000000 wizata-dsapi-0.2.6/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.6/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    56198 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.6/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-07-10 12:18:01.178388 wizata-dsapi-0.2.6/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      176 2023-07-10 12:18:01.000000 wizata-dsapi-0.2.6/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-07-10 12:18:01.000000 wizata-dsapi-0.2.6/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 12:18:01.000000 wizata-dsapi-0.2.6/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-07-10 12:18:01.000000 wizata-dsapi-0.2.6/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-10 12:18:01.000000 wizata-dsapi-0.2.6/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 14:02:28.900266 wizata-dsapi-0.2.7/
+-rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.2.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      176 2023-07-10 14:02:28.899267 wizata-dsapi-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-23 08:41:25.000000 wizata-dsapi-0.2.7/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-10 14:02:28.900266 wizata-dsapi-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2023-07-10 13:55:20.000000 wizata-dsapi-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:02:28.873571 wizata-dsapi-0.2.7/wizata_dsapi/
+-rw-rw-rw-   0        0        0     1014 2023-07-10 13:54:24.000000 wizata-dsapi-0.2.7/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.2.7/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     5763 2023-06-18 19:31:22.000000 wizata-dsapi-0.2.7/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     5714 2023-06-12 08:44:45.000000 wizata-dsapi-0.2.7/wizata_dsapi/datapoint.py
+-rw-rw-rw-   0        0        0     1877 2023-05-07 10:55:37.000000 wizata-dsapi-0.2.7/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.2.7/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    14903 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.7/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3810 2023-06-01 19:11:05.000000 wizata-dsapi-0.2.7/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     9999 2023-06-20 18:59:20.000000 wizata-dsapi-0.2.7/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-06-20 16:08:31.000000 wizata-dsapi-0.2.7/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0    17900 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.7/wizata_dsapi/pipeline.py
+-rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.7/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0    18221 2023-07-10 09:09:24.000000 wizata-dsapi-0.2.7/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     8716 2023-06-14 12:20:26.000000 wizata-dsapi-0.2.7/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     7221 2023-07-10 13:54:24.000000 wizata-dsapi-0.2.7/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2599 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.7/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2762 2023-07-10 13:54:24.000000 wizata-dsapi-0.2.7/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.7/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    56463 2023-07-10 14:00:26.000000 wizata-dsapi-0.2.7/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:02:28.898266 wizata-dsapi-0.2.7/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-07-10 14:02:28.000000 wizata-dsapi-0.2.7/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-07-10 14:02:28.000000 wizata-dsapi-0.2.7/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 14:02:28.000000 wizata-dsapi-0.2.7/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-07-10 14:02:28.000000 wizata-dsapi-0.2.7/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-10 14:02:28.000000 wizata-dsapi-0.2.7/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.2.6/LICENSE.txt` & `wizata-dsapi-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/setup.py` & `wizata-dsapi-0.2.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.2.6',
+    version='0.2.7',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/__init__.py` & `wizata-dsapi-0.2.7/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.2.7/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.2.7/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.2.7/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.2.7/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.2.7/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/execution.py` & `wizata-dsapi-0.2.7/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/experiment.py` & `wizata-dsapi-0.2.7/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.2.7/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.2.7/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.2.7/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/plot.py` & `wizata-dsapi-0.2.7/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/request.py` & `wizata-dsapi-0.2.7/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/script.py` & `wizata-dsapi-0.2.7/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/template.py` & `wizata-dsapi-0.2.7/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/twin.py` & `wizata-dsapi-0.2.7/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.2.7/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.2.7/wizata_dsapi/wizata_dsapi_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 from .mlmodel import MLModel
 from .experiment import Experiment
 from .script import Script
 from .execution import Execution
 from .dsapi_json_encoder import DSAPIEncoder
 from .ds_dataframe import DSDataFrame
 from .model_toolkit import predict
-from .template import Template
+from .template import Template, TemplateProperty
 from .twinregistration import TwinRegistration
 from .twin import Twin
 from .datapoint import DataPoint, BusinessType, Label, Category
-from .pipeline import Pipeline, PipelineStep
+from .pipeline import Pipeline, PipelineStep, VarType
 
 
 class WizataDSAPIClient:
 
     def __init__(self,
                  client_id=None,
                  scope=None,
@@ -1067,30 +1067,34 @@
         get = self.get(pipeline_key=pipeline.key)
         if get is not None:
             pipeline.pipeline_id = get.pipeline_id
             return self.update(pipeline)
         else:
             return self.create(pipeline)
 
-    def add_template_property(self, template, property_name: str, property_type: str = "datapoint"):
+    def add_template_property(self,
+                              template,
+                              property_name: str, property_type: str = "datapoint",
+                              is_required: bool = True):
 
         if property_type not in ['datapoint', 'float', 'integer', 'string']:
             raise ValueError('property type must be datapoint, float, integer or string')
 
         if isinstance(template, str):
             template = self.get(template_key=template)
         elif not isinstance(template, Template):
             raise TypeError('template must be a key str referring template or a proper wizata_dsapi Template')
 
         if property_name is None:
             raise ValueError('please provide a valid name for the property')
 
         property_dict = {
             "type": property_type,
-            "name": property_name
+            "name": property_name,
+            "required": is_required
         }
 
         response = requests.post(self.__url() + "templates/" + str(template.template_id) + '/properties/',
                                  headers=self.__header(),
                                  data=json.dumps(property_dict))
         if response.status_code == 200:
             return
@@ -1151,15 +1155,15 @@
             raise self.__raise_error(response)
 
     def register_twin(self, template, twin, properties: dict, override=True):
         """
         register a twin on a specific template using a map.
         :param template: template object, UUID or str key.
         :param twin: twin object, UUID or str key.
-        :param properties: dict where key = template property and value = datapoint name or const value (str, int or float).
+        :param properties: dict where key = template property and value = datapoint name or const value (str, int, float, relative or epoch datetime).
         :param override: by default at True - allow overriding any existing subscription
         """
 
         if template is None:
             raise ValueError('template must be specified.')
         elif isinstance(template, uuid.UUID):
             template = self.get(wizata_dsapi.Template(template_id=template))
@@ -1190,21 +1194,22 @@
 
         twin_properties = {
             "properties": []
         }
         for key in properties.keys():
             property_type = None
             for template_property in template.properties:
-                if key == template_property['name']:
-                    property_type = template_property['type']
+                template_property: TemplateProperty
+                if key == template_property.name:
+                    property_type = template_property.p_type
             if property_type is None:
                 raise ValueError(f'cannot find property {key} in template or cannot determine its type')
             twin_properties["properties"].append({
                 'name': key,
-                property_type: properties[key]
+                property_type.value: properties[key]
             })
 
         # Check if already exist
         exists = False
         response_exists = requests.get(self.__url() + "templates/" + str(template.template_id)
                                        + '/registrations/' + str(twin_id) + '/',
                                        headers=self.__header())
```

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.2.7/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.6/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.2.7/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

