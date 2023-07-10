# Comparing `tmp/wizata-dsapi-0.2.2.tar.gz` & `tmp/wizata-dsapi-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.2.2.tar", last modified: Thu Jul  6 08:02:48 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.2.3.tar", last modified: Mon Jul 10 09:48:43 2023, max compression
```

## Comparing `wizata-dsapi-0.2.2.tar` & `wizata-dsapi-0.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 08:02:48.793025 wizata-dsapi-0.2.2/
--rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0      176 2023-07-06 08:02:48.791023 wizata-dsapi-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-23 08:41:25.000000 wizata-dsapi-0.2.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-06 08:02:48.793025 wizata-dsapi-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-07-06 08:02:29.000000 wizata-dsapi-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:02:48.765787 wizata-dsapi-0.2.2/wizata_dsapi/
--rw-rw-rw-   0        0        0      996 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.2/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.2.2/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     5763 2023-06-18 19:31:22.000000 wizata-dsapi-0.2.2/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     5714 2023-06-12 08:44:45.000000 wizata-dsapi-0.2.2/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-07 10:55:37.000000 wizata-dsapi-0.2.2/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.2.2/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    14903 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.2/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-01 19:11:05.000000 wizata-dsapi-0.2.2/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     9999 2023-06-20 18:59:20.000000 wizata-dsapi-0.2.2/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-06-20 16:08:31.000000 wizata-dsapi-0.2.2/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0    17900 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.2/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.2/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    18221 2023-07-06 08:02:29.000000 wizata-dsapi-0.2.2/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8716 2023-06-14 12:20:26.000000 wizata-dsapi-0.2.2/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     4961 2023-06-14 14:10:02.000000 wizata-dsapi-0.2.2/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2599 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.2/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2701 2023-04-27 15:26:26.000000 wizata-dsapi-0.2.2/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.2/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    56198 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.2/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:02:48.789026 wizata-dsapi-0.2.2/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      176 2023-07-06 08:02:48.000000 wizata-dsapi-0.2.2/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-07-06 08:02:48.000000 wizata-dsapi-0.2.2/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 08:02:48.000000 wizata-dsapi-0.2.2/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-07-06 08:02:48.000000 wizata-dsapi-0.2.2/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-06 08:02:48.000000 wizata-dsapi-0.2.2/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 09:48:43.514644 wizata-dsapi-0.2.3/
+-rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      176 2023-07-10 09:48:43.513645 wizata-dsapi-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-23 08:41:25.000000 wizata-dsapi-0.2.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-10 09:48:43.514644 wizata-dsapi-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2023-07-10 09:47:53.000000 wizata-dsapi-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:48:43.487842 wizata-dsapi-0.2.3/wizata_dsapi/
+-rw-rw-rw-   0        0        0     1014 2023-07-10 09:47:53.000000 wizata-dsapi-0.2.3/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.2.3/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     5763 2023-06-18 19:31:22.000000 wizata-dsapi-0.2.3/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     5714 2023-06-12 08:44:45.000000 wizata-dsapi-0.2.3/wizata_dsapi/datapoint.py
+-rw-rw-rw-   0        0        0     1877 2023-05-07 10:55:37.000000 wizata-dsapi-0.2.3/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.2.3/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    14903 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.3/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3810 2023-06-01 19:11:05.000000 wizata-dsapi-0.2.3/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     9999 2023-06-20 18:59:20.000000 wizata-dsapi-0.2.3/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-06-20 16:08:31.000000 wizata-dsapi-0.2.3/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0    17900 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.3/wizata_dsapi/pipeline.py
+-rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.3/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0    18221 2023-07-10 09:09:24.000000 wizata-dsapi-0.2.3/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     8716 2023-06-14 12:20:26.000000 wizata-dsapi-0.2.3/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     6889 2023-07-10 09:47:53.000000 wizata-dsapi-0.2.3/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2599 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.3/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2701 2023-04-27 15:26:26.000000 wizata-dsapi-0.2.3/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.3/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    56198 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.3/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:48:43.512645 wizata-dsapi-0.2.3/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-07-10 09:48:43.000000 wizata-dsapi-0.2.3/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-07-10 09:48:43.000000 wizata-dsapi-0.2.3/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 09:48:43.000000 wizata-dsapi-0.2.3/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-07-10 09:48:43.000000 wizata-dsapi-0.2.3/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-10 09:48:43.000000 wizata-dsapi-0.2.3/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.2.2/LICENSE.txt` & `wizata-dsapi-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/setup.py` & `wizata-dsapi-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.2.2',
+    version='0.2.3',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/__init__.py` & `wizata-dsapi-0.2.3/wizata_dsapi/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .plot import Plot
 from .mlmodel import MLModel, MLModelConfig
 from .request import Request
 from .execution import Execution, ExecutionStatus
 from .experiment import Experiment
 from .ds_dataframe import DSDataFrame
 from .script import Script, ScriptConfig
-from .template import Template
+from .template import Template, TemplateProperty
 from .twinregistration import TwinRegistration
 
 # Sql Entities (Dto)
 from .twin import Twin, TwinBlockType
 from .datapoint import DataPoint, BusinessType, Label, Unit, Category
 
 # Api
```

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.2.3/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.2.3/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.2.3/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.2.3/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.2.3/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/execution.py` & `wizata-dsapi-0.2.3/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/experiment.py` & `wizata-dsapi-0.2.3/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.2.3/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.2.3/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.2.3/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/plot.py` & `wizata-dsapi-0.2.3/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/request.py` & `wizata-dsapi-0.2.3/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/script.py` & `wizata-dsapi-0.2.3/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/template.py` & `wizata-dsapi-0.2.3/wizata_dsapi/template.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,48 @@
 import uuid
 import json
 from .api_dto import ApiDto
+from .pipeline import VarType
+
+
+class TemplateProperty(ApiDto):
+
+    def __init__(self, name: str = None, p_type: VarType = None, required: bool = True):
+        self.name = name
+        self.p_type = p_type
+        self.required = required
+
+    def from_json(self, obj):
+        if "name" in obj.keys():
+            self.name = obj["name"]
+        if "type" in obj.keys() and obj["type"] is not None:
+            self.p_type = VarType(obj["type"])
+        if "required" in obj.keys() and obj["required"] is not None:
+            if not isinstance(bool, obj["required"]):
+                raise TypeError(f'template property field "required" should be a valid boolean')
+            self.required = obj["required"]
+        else:
+            self.required = True
+
+    def to_json(self):
+        """
+        Convert the template to a dictionary compatible to JSON format.
+
+        :return: dictionary representation of the Template object.
+        """
+        obj = {}
+        if self.name is not None:
+            obj["name"] = str(self.name)
+        if self.p_type is not None:
+            obj["type"] = str(self.p_type.value)
+        if self.required is not None:
+            if not isinstance(self.required, bool):
+                raise TypeError(f'template property field "required" should be a valid boolean')
+            obj["required"] = self.required
+        return obj
 
 
 class Template(ApiDto):
     """
     Template of a solution and/or asset.
 
     :ivar template_id: UUID of the Template.
@@ -82,49 +120,71 @@
             "id": str(self.template_id)
         }
         if self.key is not None:
             obj["key"] = str(self.key)
         if self.name is not None:
             obj["name"] = str(self.name)
         if self.properties is not None:
-            obj["properties"] = json.dumps(self.properties)
+            obj_properties = []
+            template_property: TemplateProperty
+            for template_property in self.properties:
+                obj_properties.append(template_property.to_json())
+            obj["steps"] = json.dumps(obj_properties)
         if self.createdById is not None:
             obj["createdById"] = str(self.createdById)
         if self.createdDate is not None:
             obj["createdDate"] = str(self.createdDate)
         if self.updatedById is not None:
             obj["updatedById"] = str(self.updatedById)
         if self.updatedDate is not None:
             obj["updatedDate"] = str(self.updatedDate)
         return obj
 
     def add_property(self, property_value):
         """
         add a property in list of properties
-        :param property_value: property { type , name }
+        by default - a property is required
+        :param property_value: property { "type" : "xxx" , "name" : "xxx" , "required" : false/true }
         """
         if self.properties is None:
             self.properties = []
+
         if "type" not in property_value:
             raise KeyError("property must have a type.")
+        p_type = VarType(property_value['type'])
+
         if "name" not in property_value:
             raise KeyError("property must have a name")
-        if property_value["type"] not in ['datapoint', 'float', 'integer', 'string']:
-            raise ValueError('property type must be datapoint, float, integer or string')
+        name = property_value["name"]
+
+        required = True
+        if "required" in property_value:
+            required = property_value["required"]
+
+        existing_property: TemplateProperty
         for existing_property in self.properties:
-            if existing_property["name"] == property_value["name"]:
-                raise ValueError(f'property {property_value["name"]} already exists in template.')
-        self.properties.append(property_value)
+            if existing_property.name == name:
+                raise ValueError(f'property {name} already exists in template.')
+
+        new_property = TemplateProperty(
+            p_type=p_type,
+            required=required,
+            name=name
+        )
+        self.properties.append(new_property)
 
     def remove_property(self, name):
         """
         remove a property from the list based on its name
         :param name: property to remove
         """
         found_property = None
+
+        existing_property: TemplateProperty
         for existing_property in self.properties:
-            if existing_property["name"] == name:
+            if existing_property.name == name:
                 found_property = existing_property
+
         if self.properties is not None and found_property is not None:
             self.properties.remove(found_property)
```

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/twin.py` & `wizata-dsapi-0.2.3/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.2.3/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.2.3/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.2.3/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.2/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.2.3/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

