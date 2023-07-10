# Comparing `tmp/labelbase-0.1.0.tar.gz` & `tmp/labelbase-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelbase-0.1.0.tar", last modified: Mon Apr  3 19:22:41 2023, max compression
+gzip compressed data, was "labelbase-0.1.1.tar", last modified: Mon Jul 10 18:47:49 2023, max compression
```

## Comparing `labelbase-0.1.0.tar` & `labelbase-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:22:41.582594 labelbase-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 19:22:29.000000 labelbase-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-03 19:22:41.582594 labelbase-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-03 19:22:29.000000 labelbase-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:22:41.582594 labelbase-0.1.0/labelbase/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-03 19:22:29.000000 labelbase-0.1.0/labelbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21673 2023-04-03 19:22:29.000000 labelbase-0.1.0/labelbase/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-04-03 19:22:29.000000 labelbase-0.1.0/labelbase/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:22:41.582594 labelbase-0.1.0/labelbase/converters/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-03 19:22:29.000000 labelbase-0.1.0/labelbase/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-04-03 19:22:29.000000 labelbase-0.1.0/labelbase/converters/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-03 19:22:29.000000 labelbase-0.1.0/labelbase/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-03 19:22:29.000000 labelbase-0.1.0/labelbase/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-03 19:22:29.000000 labelbase-0.1.0/labelbase/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-04-03 19:22:29.000000 labelbase-0.1.0/labelbase/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-04-03 19:22:29.000000 labelbase-0.1.0/labelbase/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-04-03 19:22:29.000000 labelbase-0.1.0/labelbase/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:22:41.582594 labelbase-0.1.0/labelbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-03 19:22:41.000000 labelbase-0.1.0/labelbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-03 19:22:41.000000 labelbase-0.1.0/labelbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 19:22:41.000000 labelbase-0.1.0/labelbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-03 19:22:41.000000 labelbase-0.1.0/labelbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-03 19:22:41.000000 labelbase-0.1.0/labelbase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 19:22:41.582594 labelbase-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-03 19:22:29.000000 labelbase-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:47:49.533362 labelbase-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 18:47:40.000000 labelbase-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-10 18:47:49.533362 labelbase-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-10 18:47:40.000000 labelbase-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:47:49.533362 labelbase-0.1.1/labelbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26686 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14027 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:47:49.533362 labelbase-0.1.1/labelbase/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/converters/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26427 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:47:49.533362 labelbase-0.1.1/labelbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-10 18:47:49.000000 labelbase-0.1.1/labelbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-10 18:47:49.000000 labelbase-0.1.1/labelbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:47:49.000000 labelbase-0.1.1/labelbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 18:47:49.000000 labelbase-0.1.1/labelbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 18:47:49.000000 labelbase-0.1.1/labelbase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:47:49.533362 labelbase-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-10 18:47:40.000000 labelbase-0.1.1/setup.py
```

### Comparing `labelbase-0.1.0/LICENSE` & `labelbase-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.0/PKG-INFO` & `labelbase-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelbase
-Version: 0.1.0
+Version: 0.1.1
 Summary: Labelbox Helper Library
 Home-page: https://labelbox.com
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Keywords: labelbox,labelbase
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `labelbase-0.1.0/labelbase/annotate.py` & `labelbase-0.1.1/labelbase/annotate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,176 +1,57 @@
 import uuid
 import json
 from labelbase.masks import mask_to_bytes
 
-def get_leaf_paths(export_classifications:list, schema_to_name_path:dict, divider:str="///"):
-    """ Given a flat list of labelox export classifications, constructs leaf name paths given a divider
-    Args:
-        export_classifications  :   Required (list) - List of classifications from label["Label"]["objects"][0]["classifications"] or label["Label"]["classificaitons"]
-        schema_to_name_path     :   Required (dict) - Dictionary where {key=schema_id : value=feature_name_path} created from running:
-                                            labelbase.get_ontology_schema_to_name_path(ontology, divider=divider, invert=False, detailed=False)
-        divider                 :   Optional (str): String delimiter for name paths
-    Returns:
-        List of all leaf name paths 
-    """
-    def build_leaf_paths(root:dict, acc="", name_paths=[], divider="///"):
-        for parent in root.keys():
-            name_path = f"{acc}{divider}{parent}" if acc else f"{parent}"
-            child = root[parent]
-            if child:
-                name_paths = build_leaf_paths(root=root[parent], acc=name_path, name_paths=name_paths)
-            else:
-                name_paths.append(name_path)
-        return name_paths    
-    name_paths = []
-    for cla in export_classifications:
-        if type(cla) == dict:
-            if "answers" in cla.keys():
-                for answer in cla["answers"]:
-                    name_paths.append(schema_to_name_path[answer["schemaId"]])
-            if "answer" in cla.keys():
-                if type(cla["answer"]) == str:
-                    name_paths.append(schema_to_name_path[cla["schemaId"]]+divider+cla["answer"])
-                else:
-                    name_paths.append(schema_to_name_path[cla["answer"]["schemaId"]]) 
-        else:
-            for c in cla:
-                if "answers" in c.keys():
-                    for answer in c["answers"]:
-                        name_paths.append(schema_to_name_path[answer["schemaId"]])
-                if "answer" in c.keys():
-                    if type(c["answer"]) == str:
-                        name_paths.append(schema_to_name_path[c["schemaId"]]+divider+c["answer"])
-                    else:
-                        name_paths.append(schema_to_name_path[c["answer"]["schemaId"]])                 
-    root = {}
-    for input_path in name_paths:
-        parts = input_path.split(divider)
-        current_node = root
-        for part in parts:
-            if part not in current_node:
-                current_node[part] = {}
-            current_node = current_node[part]    
-    return build_leaf_paths(root)  
+from labelbox import Client as labelboxClient
+import labelbox as lb
 
-def flatten_label(label_dict:dict, ontology_index:dict, schema_to_name_path:dict, mask_method:str="url", divider:str="///"):
-    """ For a label from project.export_labels(download=True), creates a flat dictionary where:
-            { key = annotation_type + divider + annotation_name  :  value = [annotation_value, list_of_nested_name_paths]}
-        Each accepted annotation type and the expected output annotation value is listed below:
+def create_ndjsons(top_level_name:str, annotation_inputs:list, ontology_index:dict, confidence:bool=False, mask_method:str="url", divider:str="///"):
+    """ From an annotation in the expected format, creates a Labelbox NDJSON of that annotation -- note the data row ID is not added here
+        Each accepted annotation type and the expected input annotation value is listed below:
+        ** IF confidence == False **
             For tools:
-                bbox            :   [[top, left, height, width], [nested_classification_name_paths], [top, left, height, width], [nested_classification_name_paths]]
-                polygon         :   [[(x, y), (x, y),...(x, y)], [nested_classification_name_paths], [(x, y), (x, y),...(x, y)], [nested_classification_name_paths]]
-                line            :   [[(x, y), (x, y),...(x, y)], [nested_classification_name_paths], [(x, y), (x, y),...(x, y)], [nested_classification_name_paths]]
-                point           :   [[x, y], [nested_classification_name_paths], [x, y], [nested_classification_name_paths]]
-                mask            :   [[URL, colorRGB], [nested_classification_name_paths], [URL, colorRGB], [nested_classification_name_paths]]
+                bbox            :   [[top, left, height, width], [nested_classification_name_paths]], [[top, left, height, width], [nested_classification_name_paths]]
+                polygon         :   [[(x, y), (x, y),...(x, y)], [nested_classification_name_paths]], [[(x, y), (x, y),...(x, y)], [nested_classification_name_paths]]
+                line            :   [[(x, y), (x, y),...(x, y)], [nested_classification_name_paths]], [(x, y), (x, y),...(x, y)], [nested_classification_name_paths]]
+                point           :   [(x, y), [nested_classification_name_paths]], [(x, y), [nested_classification_name_paths]]
+                mask            :   [[URL, colorRGB], [nested_classification_name_paths]], [[URL, colorRGB], [nested_classification_name_paths]]
                                             OR
-                                    [[array, colorRGB], [nested_classification_name_paths], [array, colorRGB], [nested_classification_name_paths]]
+                                    [[array, colorRGB], [nested_classification_name_paths]], [[array, colorRGB], [nested_classification_name_paths]]
                                             OR
-                                    [[png_bytes, "null"], [nested_classification_name_paths], [png_bytes, "null"], [nested_classification_name_paths]]                                    
-                named-entity    :   [[start, end], [nested_classification_name_paths], [start, end], [nested_classification_name_paths]]
+                                    [[png_bytes, None], [nested_classification_name_paths]], [[png_bytes, None], [nested_classification_name_paths]]                                    
+                named-entity    :   [[(start, end), [nested_classification_name_paths]], [(start, end)], [nested_classification_name_paths]]
             For classifications:
                 radio           :   [[answer_name_paths]]
                 check           :   [[answer_name_paths]]
                 text            :   [[answer_name_paths]] -- the last string in a text name path is the text value itself
-    Args:    
-        label_dict              :   Required (dict) - Dictionary representation of a label from project.export_labels(download=True)
-        ontology_index          :   Required (dict) - Dictionary created from running:
-                                            labelbase.ontology.get_ontology_schema_to_name_path(ontology, divider=divider, invert=True, detailed=True)
-        schema_to_name_path     :   Required (dict) - Dictionary where {key=schema_id : value=feature_name_path} created from running:
-                                            labelbase.ontology.get_ontology_schema_to_name_path(ontology, divider=divider, invert=False, detailed=False)
-        mask_method             :   Optional (str) - Specifies your desired mask data format
-                                        - "url" leaves masks as-is
-                                        - "array" converts URLs to numpy arrays
-                                        - "png" converts URLs to png byte strings                                               
-        divider                 :   Optional (str) - String delimiter for name paths        
-    Returns:        
-        Dictionary with one key per annotation class in a given label in the specified format written above
-    """
-    flat_label = {}
-    annotations = label_dict["Label"]
-    objects = annotations["objects"]
-    classifications = annotations["classifications"]
-    if objects:
-        for obj in objects:
-            annotation_type = ontology_index[obj["title"]]["type"]
-            annotation_type = "mask" if annotation_type == "raster-segmentation" else annotation_type
-            annotation_type = "bbox" if annotation_type == "rectangle" else annotation_type
-            column_name = f'{annotation_type}{divider}{obj["title"]}'           
-            if column_name not in flat_label.keys():
-                flat_label[column_name] = []
-            if "bbox" in obj.keys():
-                annotation_value = [obj["bbox"]["top"], obj["bbox"]["left"], obj["bbox"]["height"], obj["bbox"]["width"]]
-            elif "polygon" in obj.keys():
-                annotation_value = [[coord["x"], coord["y"]] for coord in obj["polygon"]]
-            elif "line" in obj.keys():
-                annotation_value = [[coord["x"], coord["y"]] for coord in obj["line"]]
-            elif "point" in obj.keys():
-                annotation_value = [obj["point"]["x"], obj["point"]["y"]]
-            elif "location" in obj.keys():
-                annotation_value = [obj["location"]["start"], obj["location"]["end"]]
-            else:
-                if mask_method == "url":
-                    annotation_value = [obj["instanceURI"], [255,255,255]]
-                elif mask_method == "array": 
-                    array = mask_to_bytes(input=obj["instanceURI"], method="url", color=[255,255,255], output="array")
-                    annotation_value = [array, [255,255,255]]
-                else:
-                    png = mask_to_bytes(input=obj["instanceURI"], method="url", color=[255,255,255], output="png")
-                    annotation_value = [png, "null"]
-            if "classifications" in obj.keys():
-                nested_classification_name_paths = get_leaf_paths(
-                    export_classifications=obj["classifications"], 
-                    schema_to_name_path=schema_to_name_path,
-                    divider=divider
-                )
-                return_paths = get_child_paths(first=obj["title"], name_paths=nested_classification_name_paths, divider=divider)
-            else:
-                return_paths = []
-            flat_label[column_name].append([annotation_value, return_paths])
-    if classifications:
-        leaf_paths = get_leaf_paths(
-            export_classifications=classifications, 
-            schema_to_name_path=schema_to_name_path,
-            divider=divider
-        )
-        classification_names = pull_first_name_from_paths(
-            name_paths=leaf_paths, 
-            divider=divider
-        )
-        for classification_name in classification_names:
-            annotation_type = ontology_index[classification_name]["type"]
-            child_paths = get_child_paths(first=classification_name, name_paths=leaf_paths, divider=divider)
-            flat_label[f'{annotation_type}{divider}{classification_name}'] = [[name_path for name_path in child_paths]]
-    return flat_label
-
-def create_ndjsons(top_level_name:str, annotation_inputs:list, ontology_index:dict, mask_method:str="url", divider:str="///"):
-    """ From an annotation in the expected format, creates a Labelbox NDJSON of that annotation -- note the data row ID is not added here
-        Each accepted annotation type and the expected input annotation value is listed below:
+        ** IF confidence == True **                
             For tools:
-                bbox            :   [[top, left, height, width], [nested_classification_name_paths], [top, left, height, width], [nested_classification_name_paths]]
-                polygon         :   [[(x, y), (x, y),...(x, y)], [nested_classification_name_paths], [(x, y), (x, y),...(x, y)], [nested_classification_name_paths]]
-                line            :   [[(x, y), (x, y),...(x, y)], [nested_classification_name_paths], [(x, y), (x, y),...(x, y)], [nested_classification_name_paths]]
-                point           :   [[x, y], [nested_classification_name_paths], [x, y], [nested_classification_name_paths]]
-                mask            :   [[URL, colorRGB], [nested_classification_name_paths], [URL, colorRGB], [nested_classification_name_paths]]
+                bbox            :   [[top, left, height, width], [nested_classification_name_paths], confidence_score], [[top, left, height, width], [nested_classification_name_paths], confidence_score]
+                polygon         :   [[(x, y), (x, y),...(x, y)], [nested_classification_name_paths], confidence_score], [[(x, y), (x, y),...(x, y)], [nested_classification_name_paths], confidence_score]
+                line            :   [[(x, y), (x, y),...(x, y)], [nested_classification_name_paths], confidence_score], [(x, y), (x, y),...(x, y)], [nested_classification_name_paths], confidence_score]
+                point           :   [(x, y), [nested_classification_name_paths], confidence_score], [(x, y), [nested_classification_name_paths], confidence_score]
+                mask            :   [[URL, colorRGB], [nested_classification_name_paths], confidence_score], [[URL, colorRGB], [nested_classification_name_paths], confidence_score]
                                             OR
-                                    [[array, colorRGB], [nested_classification_name_paths], [array, colorRGB], [nested_classification_name_paths]]
+                                    [[array, colorRGB], [nested_classification_name_paths], confidence_score], [[array, colorRGB], [nested_classification_name_paths], confidence_score]
                                             OR
-                                    [[png_bytes, None], [nested_classification_name_paths], [png_bytes, None], [nested_classification_name_paths]]                                    
-                named-entity    :   [[start, end], [nested_classification_name_paths], [start, end], [nested_classification_name_paths]]
+                                    [[png_bytes, None], [nested_classification_name_paths], confidence_score], [[png_bytes, None], [nested_classification_name_paths], confidence_score]                                    
+                named-entity    :   [[(start, end), [nested_classification_name_paths], confidence_score], [(start, end)], [nested_classification_name_paths], confidence_score]
             For classifications:
-                radio           :   [[answer_name_paths]]
-                check           :   [[answer_name_paths]]
-                text            :   [[answer_name_paths]] -- the last string in a text name path is the text value itself
+                radio           :   [[answer_name_paths], confidence_score]
+                check           :   [[answer_name_paths], confidence_score]
+                text            :   [[answer_name_paths], confidence_score] -- the last string in a text name path is the text value itself                
     Args:
         data_row_id             :   Required (str) - Labelbox Data Row ID
         top_level_name          :   Required (str) - Name of the top-level tool or classification        
-        annotation_inputs       :   Required (list) - List of annotation value lists where 1 list element must correspond to the following format:        
+        annotation_inputs       :   Required (list) - List of annotation value lists where the list of lists corresponds to the above format:        
         annotation_type         :   Required (str) - Type of annotation in question - must be a string of one of the above options
         ontology_index          :   Required (dict) - Dictionary created from running:
                                             labelbase.ontology.get_ontology_schema_to_name_path(ontology, divider=divider, invert=True, detailed=True)
+        confidence              :   Optional (bool) - If True, will expect a different format and add confidence scores to each ndjson created
         mask_method             :   Optional (str) - Specifies your input mask data format
                                         - "url" means your mask is an accessible URL (must provide color)
                                         - "array" means your mask is a numpy array (must provide color)
                                         - "png" means your mask value is a png-string                                       
         divider                 :   Optional (str) - String delimiter for name paths        
     """
     if mask_method not in ["url", "png", "array"]:
@@ -180,57 +61,83 @@
         annotation_inputs = json.loads(annotation_inputs.replace("'",'"').replace("None","null"))
     if type(annotation_inputs) == list:
         for annotation_input in annotation_inputs:
             ndjsons.append(ndjson_builder(
                 top_level_name=top_level_name,
                 annotation_input=annotation_input, 
                 ontology_index=ontology_index, 
+                confidence=confidence,
                 mask_method=mask_method,
                 divider=divider
             ))
     return ndjsons
 
-def ndjson_builder(top_level_name:str, annotation_input:list, ontology_index:dict, mask_method:str="url", divider:str="///"):
+def ndjson_builder(top_level_name:str, annotation_input:list, ontology_index:dict, confidence:bool=False, mask_method:str="url", divider:str="///"):
     """ Returns an ndjson of an annotation given a list of values - the values needed differ depending on the annotation type
     Args:
         top_level_name          :   Required (str) - Name of the top-level tool or classification        
         annotation_input        :   Required (list) - List that corresponds to a single annotation for a label in the specified format
         ontology_index          :   Required (dict) - Dictionary created from running:
                                             labelbase.ontology.get_ontology_schema_to_name_path(ontology, divider=divider, invert=True, detailed=True)
+        confidence              :   Optional (bool) - If True, will expect a different format and add confidence scores to each ndjson created                                            
         mask_method             :   Optional (str) - Specifies your input mask data format
                                         - "url" treats annotation input values as URLs uploads them directly
                                         - "array" converts the annotation input values into png bytes
                                         - "png" uploads png bytes directly
         divider                 :   Optional (str) - String delimiter for name paths        
     Returns
         NDJSON representation of an annotation
     """
     annotation_type = ontology_index[top_level_name]["type"]
+    if ontology_index['project_type'] == str(lb.MediaType.Geospatial_Tile):
+        annotation_type = 'geo_' + annotation_type
+
     ndjson = {
         "uuid" : str(uuid.uuid4())
     }  
     # Catches tools
-    if annotation_type in ["bbox", "polygon", "line", "point", "mask", "named-entity"]:
+    if annotation_type in ["bbox", "polygon", "line", "point", "mask", "named-entity", "geo_bbox", "geo_polygon", "geo_line", "geo_point"]:
+        if confidence:
+            ndjson["confidence"] = annotation_input[2] if len(annotation_input) == 3 else 0.0
         ndjson["name"] = top_level_name
-        if annotation_type == "bbox":
+        if annotation_type == "geo_bbox":
+                ndjson['bbox'] = {
+                    'top': annotation_input[0][0][1][1],
+                    'left': annotation_input[0][0][1][0],
+                    'height': annotation_input[0][0][3][1] - annotation_input[0][0][1][1],        
+                    'width': annotation_input[0][0][3][0] - annotation_input[0][0][1][0]
+                }
+        elif annotation_type == "geo_polygon":
+            polygon_points_ndjson = []
+            for sub in annotation_input[0][0]:
+                polygon_points_ndjson.append({"x":sub[0], "y":sub[1]})
+            ndjson["polygon"] = polygon_points_ndjson
+        elif annotation_type == "geo_line":
+            line_points_ndjson = []
+            for sub in annotation_input[0]:
+                line_points_ndjson.append({"x":sub[0], "y":sub[1]})
+            ndjson["line"] = line_points_ndjson
+        elif annotation_type == "geo_point":
+            ndjson["point"] = {'x':annotation_input[0][0], 'y':annotation_input[0][1]}
+        elif annotation_type == "bbox":
             ndjson[annotation_type] = {"top":annotation_input[0][0],"left":annotation_input[0][1],"height":annotation_input[0][2],"width":annotation_input[0][3]}
         elif annotation_type in ["polygon", "line"]:
             ndjson[annotation_type] = [{"x":xy_pair[0],"y":xy_pair[1]} for xy_pair in annotation_input[0]]     
         elif annotation_type == "point":
             ndjson[annotation_type] = {"x":annotation_input[0][0],"y":annotation_input[0][1]}
         elif annotation_type == "mask":
             if mask_method == "url": 
                 ndjson[annotation_type] = {"instanceURI":annotation_input[0][0],"colorRGB":annotation_input[0][1]}
             elif mask_method == "array": # input masks as numpy arrays
                 png = mask_to_bytes(input=annotation_input[0][0], method=mask_method, color=annotation_input[0][1], output="png")
                 ndjson[annotation_type] = {"png":png}
             else: # Only one left is png
                 ndjson[annotation_type] = {"png":annotation_input[0][0]}
         else: # Only one left is named-entity 
-            ndjson["location"] = {"start" : annotation_input[0][0],"end":annotation_input[0][1]}
+            ndjson['data']["location"] = {"start" : annotation_input[0][0],"end":annotation_input[0][1]}
         if annotation_input[1]:
             ndjson["classifications"] = []
             classification_names = pull_first_name_from_paths(name_paths=annotation_input[1], divider=divider)
             for classification_name in classification_names:
                 ndjson["classifications"].append(
                     classification_builder(
                         classification_path=classification_name,
@@ -241,61 +148,110 @@
                     )
                 )
     # Otherwise, the top level feature is a classification
     else:
         ndjson.update(
             classification_builder(
                 classification_path=top_level_name, 
-                answer_paths=annotation_input,
+                answer_paths=[annotation_input[0]],
                 ontology_index=ontology_index,
                 divider=divider
             )
         )
-    return ndjson    
+        if confidence:
+            ndjson["confidence"] = annotation_input[1] if len(annotation_input) == 2 else 0.0        
+    return ndjson   
+
+def pull_first_name_from_paths(name_paths:list, divider:str="///"):
+    """ Pulls the first name from every name path in a list a divider-delimited name paths
+    Args:    
+        name_paths              :   Required (list) - List of name paths
+        divider                 :   Optional (str) - String delimiter for all name keys generated for parent/child schemas     
+    Returns:
+        List of unique first names from a given name path
+    """    
+    firsts = []
+    for name_path in name_paths:
+        firsts.append(str(name_path.split(divider)[0]))
+    return list(set(firsts))
+
+def get_child_paths(first, name_paths, divider:str="///"):
+    """ From a list of name paths, grabs paths starting with the `first` string and removes the `first` name from the name path
+    Args
+        first                   :   Required (str) - The parent feature name you want to find paths for
+        name_paths              :   Required (list) - List of name paths
+        divider                 :   Optional (str) - String delimiter for all name keys generated for parent/child schemas             
+    Returns
+        List of children name paths
+    """
+    child_paths = []
+    for path in name_paths:
+        if path.startswith(first):
+            child_path = ""
+            for name in path.split(divider)[1:]:
+                child_path += str(name)+str(divider)
+            child_path = child_path[:-len(divider)] 
+            child_paths.append(child_path)
+    return child_paths  
 
 def classification_builder(classification_path:str, answer_paths:list, ontology_index:dict, tool_name:str="", divider:str="///"):
     """ Given a classification path and all its child paths, constructs an ndjson.
         If the classification answer's paths have nested classifications, will recursuively call this function.
     """
+    # Determine full classification path, including tool name
     index_input = f"{tool_name}{divider}{classification_path}" if tool_name else classification_path
-    c_type = ontology_index[index_input]["type"]
-    c_name = classification_path.split(divider)[-1] if divider in classification_path else classification_path
+    # Determine the classification type from full classification path
+    c_type = ontology_index[index_input]["type"] 
+    # Get the current classification name at the end of full classification path
+    c_name = classification_path.split(divider)[-1] if divider in classification_path else classification_path 
+    # Initiate your classification ndjson
     classification_ndjson = {
         "name" : c_name
     }
+    # If this is a radio, there's only one answer
     if c_type == "radio":
+        # For the current classification, get the first answer path where the current classification is the parent feature
         answer_name = pull_first_name_from_paths(name_paths=answer_paths, divider=divider)[0]
         classification_ndjson["answer"] = {
             "name" : answer_name
         }
+        # For the current answer, get all nested classification paths where the current answer is the parent feature 
         n_c_paths = get_child_paths(first=answer_name, name_paths=answer_paths, divider=divider)
+        # Get the current nested classification names
         n_c_names = pull_first_name_from_paths(name_paths=n_c_paths, divider=divider)
+        # For each nested classification path, loop this process, finding answers and nested classifications
         for n_c_name in n_c_names:
             if n_c_name:
                 if "classifications" not in classification_ndjson["answer"].keys():
                     classification_ndjson["answer"]["classifications"] = []
                 n_a_paths = get_child_paths(first=n_c_name, name_paths=n_c_paths, divider=divider)  
                 classification_ndjson["answer"]["classifications"].append(
                     classification_builder(
                         classification_path=f"{classification_path}{divider}{answer_name}{divider}{n_c_name}",
                         answer_paths=n_a_paths,
                         ontology_index=ontology_index,
                         tool_name=tool_name,
                         divider=divider
                     )
                 )
+    # If this is a checklist, there are potentially multiple answers
     elif c_type == "checklist":
         classification_ndjson["answers"] = []
+        # For the current classification, get all answer paths where the current classification is the parent feature        
         answer_names = pull_first_name_from_paths(name_paths=answer_paths, divider=divider)
+        # For each current answer....
         for answer_name in answer_names:
             answer_ndjson = {
                 "name" : answer_name
             }
+            # For the current answer, get all nested classification paths where the current answer is the parent feature                
             n_c_paths = get_child_paths(first=answer_name, name_paths=answer_paths, divider=divider)
+            # Get the current nested classification names            
             n_c_names = pull_first_name_from_paths(name_paths=n_c_paths, divider=divider)
+            # For each nested classification path, loop this process, finding answers and nested classifications                             
             for n_c_name in n_c_names:
                 if n_c_name:
                     if "classifications" not in answer_ndjson.keys():
                         answer_ndjson["classifications"] = []
                     n_a_paths = get_child_paths(first=n_c_name, name_paths=n_c_paths, divider=divider) 
                     answer_ndjson["classifications"].append(
                         classification_builder(
@@ -303,42 +259,147 @@
                             answer_paths=n_a_paths,
                             ontology_index=ontology_index,
                             tool_name=tool_name,
                             divider=divider                            
                         )
                     )
             classification_ndjson["answers"].append(answer_ndjson)
+    # If this is text, there the answer is whatever is at the end of the current answer path
     else:
         classification_ndjson["answer"] = answer_paths[0]
-    return classification_ndjson
+    return classification_ndjson  
 
-def pull_first_name_from_paths(name_paths:list, divider:str="///"):
-    """ Pulls the first name from every name path in a list a divider-delimited name paths
-    Args:    
-        name_paths              :   Required (list) - List of name paths
-        divider                 :   Optional (str) - String delimiter for all name keys generated for parent/child schemas     
+def get_leaf_paths(classifications, current_path="", divider="///"):
+    """ Given a flat list of labelox export classifications, constructs leaf name paths given a divider
+    Args:
+        classifications         :   Required (list) - List of classifications from exported label
+        current_path            :   Optional (str) - Used to recursively build name paths for nested classifications
+        divider                 :   Optional (str) - String delimiter for name paths
     Returns:
-        List of unique first names from a given name path
-    """    
-    firsts = []
-    for name_path in name_paths:
-        firsts.append(str(name_path.split(divider)[0]))
-    return list(set(firsts))
+        List of all leaf name paths 
+    """
+    name_paths = []
+    for classification in classifications:
+        if current_path == "":
+            name_path = classification['name']
+        else:
+            name_path = f"{current_path}{divider}{classification['name']}"
+        if "text_answer" in classification.keys():
+            name_path = f"{name_path}{divider}{classification['text_answer']['content']}"
+            name_paths.append(name_path)
+        if "checklist_answers" in classification.keys():
+            for answer in classification['checklist_answers']:
+                new_path = f"{name_path}{divider}{answer['name']}"
+                if "classifications" in answer.keys():
+                    if len(answer['classifications']) > 0:
+                        name_paths += get_leaf_paths(answer['classifications'], current_path=new_path, divider=divider)
+                    else:
+                        name_paths.append(new_path)
+                else:
+                    name_paths.append(new_path)
+        if "radio_answer" in classification.keys():
+            answer = classification['radio_answer']
+            new_path = f"{name_path}{divider}{answer['name']}"
+            if "classifications" in answer.keys():
+                if len(answer['classifications']) > 0:
+                    name_paths += get_leaf_paths(answer['classifications'], current_path=new_path, divider=divider)
+                else:
+                    name_paths.append(new_path)
+            else:
+                name_paths.append(new_path)
+    return name_paths
+                    
 
-def get_child_paths(first, name_paths, divider:str="///"):
-    """ From a list of name paths, grabs paths starting with the `first` string and removes the `first` name from the name path
-    Args
-        first                   :   Required (str) - The parent feature name you want to find paths for
-        name_paths              :   Required (list) - List of name paths
-        divider                 :   Optional (str) - String delimiter for all name keys generated for parent/child schemas             
-    Returns
-        List of children name paths
+def flatten_label(client:labelboxClient, label_dict:dict, ontology_index:dict, datarow_id:str="", mask_method:str="url", divider:str="///"):
+    """ For a label from project.export_v2(), creates a flat dictionary where:
+            { key = annotation_type + divider + annotation_name  :  value = [annotation_value, list_of_nested_name_paths]}
+        Each accepted annotation type and the expected output annotation value is listed below:
+            For tools:
+                bbox            :   [[top, left, height, width], [nested_classification_name_paths], [top, left, height, width], [nested_classification_name_paths]]
+                polygon         :   [[(x, y), (x, y),...(x, y)], [nested_classification_name_paths], [(x, y), (x, y),...(x, y)], [nested_classification_name_paths]]
+                line            :   [[(x, y), (x, y),...(x, y)], [nested_classification_name_paths], [(x, y), (x, y),...(x, y)], [nested_classification_name_paths]]
+                point           :   [[x, y], [nested_classification_name_paths], [x, y], [nested_classification_name_paths]]
+                mask            :   [[URL, colorRGB], [nested_classification_name_paths], [URL, colorRGB], [nested_classification_name_paths]]
+                                            OR
+                                    [[array, colorRGB], [nested_classification_name_paths], [array, colorRGB], [nested_classification_name_paths]]
+                                            OR
+                                    [[png_bytes, "null"], [nested_classification_name_paths], [png_bytes, "null"], [nested_classification_name_paths]]                                    
+                named-entity    :   [[start, end], [nested_classification_name_paths], [start, end], [nested_classification_name_paths]]
+            For classifications:
+                radio           :   [[answer_name_paths]]
+                check           :   [[answer_name_paths]]
+                text            :   [[answer_name_paths]] -- the last string in a text name path is the text value itself
+    Args:    
+        client                  :   Required        - Labelbox client
+        label_dict              :   Required (dict) - Dictionary representation of a label from project.export_labels(download=True)
+        ontology_index          :   Required (dict) - Dictionary created from running:
+                                            labelbase.ontology.get_ontology_schema_to_name_path(ontology, divider=divider, invert=True, detailed=True)
+        datarow_id              :   Required (str) - Datarow id, only required for datarows with mask annotations
+        mask_method             :   Optional (str) - Specifies your desired mask data format
+                                        - "url" leaves masks as-is
+                                        - "array" converts URLs to numpy arrays
+                                        - "png" converts URLs to png byte strings                                               
+        divider                 :   Optional (str) - String delimiter for name paths        
+    Returns:        
+        Dictionary with one key per annotation class in a given label in the specified format written above
     """
-    child_paths = []
-    for path in name_paths:
-        if path.startswith(first):
-            child_path = ""
-            for name in path.split(divider)[1:]:
-                child_path += str(name)+str(divider)
-            child_path = child_path[:-len(divider)] 
-            child_paths.append(child_path)
-    return child_paths      
+    flat_label = {}
+    annotations = label_dict['annotations']
+    objects = annotations["objects"]
+    classifications = annotations["classifications"]
+    if objects:
+        for obj in objects:
+            annotation_type = ontology_index[obj["name"]]["type"]
+            annotation_type = "mask" if annotation_type == "raster-segmentation" else annotation_type
+            annotation_type = "bbox" if annotation_type == "rectangle" else annotation_type
+            if 'geojson' in obj.keys():
+                annotation_type = 'geo_' + annotation_type
+            column_name = f'{annotation_type}{divider}{obj["name"]}'           
+            if column_name not in flat_label.keys():
+                flat_label[column_name] = []
+            if "bounding_box" in obj.keys():
+                annotation_value = [obj["bounding_box"]["top"], obj["bounding_box"]["left"], obj["bounding_box"]["height"], obj["bounding_box"]["width"]]
+            elif "polygon" in obj.keys():
+                annotation_value = [[coord["x"], coord["y"]] for coord in obj["polygon"]]
+            elif "line" in obj.keys():
+                annotation_value = [[coord["x"], coord["y"]] for coord in obj["line"]]
+            elif "point" in obj.keys():
+                annotation_value = [obj["point"]["x"], obj["point"]["y"]]
+            elif "data" in obj.keys():
+                annotation_value = [obj['data']["location"]["start"], obj['data']["location"]["end"]]
+            elif "geojson" in obj.keys():
+                annotation_value = obj['geojson']['coordinates']
+            else:
+                if mask_method == "url":
+                    annotation_value = [obj['mask']["url"], [255,255,255]]
+                elif mask_method == "array": 
+                    array = mask_to_bytes(client=client, input=obj['mask']["url"], datarow_id=datarow_id, method="url", color=[255,255,255], output="array")
+                    annotation_value = [array, [255,255,255]]
+                else:
+                    png = mask_to_bytes(client=client, input=obj['mask']["url"], datarow_id=datarow_id, method="url", color=[255,255,255], output="png")
+                    annotation_value = [png, "null"]
+            if "classifications" in obj.keys():
+                if len(obj['classifications']) > 0:
+                    return_paths = get_leaf_paths(
+                        classifications=obj["classifications"], 
+                        divider=divider
+                    )
+                    print(return_paths)
+                else:
+                    return_paths = []
+            else:
+                return_paths = []
+            flat_label[column_name].append([annotation_value, return_paths])
+    if classifications:
+        leaf_paths = get_leaf_paths(
+            classifications=classifications, 
+            divider=divider
+        )
+        classification_names = pull_first_name_from_paths(
+            name_paths=leaf_paths, 
+            divider=divider
+        )
+        for classification_name in classification_names:
+            annotation_type = ontology_index[classification_name]["type"]
+            child_paths = get_child_paths(first=classification_name, name_paths=leaf_paths, divider=divider)
+            flat_label[f'{annotation_type}{divider}{classification_name}'] = [[name_path for name_path in child_paths]]
+    return flat_label
```

### Comparing `labelbase-0.1.0/labelbase/connector.py` & `labelbase-0.1.1/labelbase/metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,162 +1,148 @@
 from labelbox import Client as labelboxClient
 from labelbox.schema.data_row_metadata import DataRowMetadataKind
-from labelbase.metadata import _refresh_metadata_ontology
+from datetime import datetime
+from dateutil import parser
+import pytz
 
-def determine_actions(dataset_id:str, dataset_id_col:str, project_id:str, project_id_col:str, upload_method:str, annotation_index:dict):
-    """ Determines if this upload action can batch data rows to projects - does so by checking if a project ID string or column has been provided
+def get_metadata_schema_to_type(client:labelboxClient, lb_mdo=False, invert:bool=False):
+    """ Creates a dictionary where {key=metadata_schema_id: value=metadata_type} 
+    - metadata_type either "string" "enum" "datetime" or "number"
     Args:
-        dataset_id                  :   Required (str) - Labelbox Dataset ID
-        dataset_id_col              :   Required (str) - Column name pertaining to dataset_id        
-        project_id                  :   Required (str) - Labelbox Project ID
-        project_id_col              :   Required (str) - Column name pertaining to project_id
-        upload_method               :   Required (bool) - Either "mal", "import", or ""
-        annotation_index            :   Required (dict) - Dictonary where {key=column_name : value=top_level_feature_name}        
+        client              :   Required (labelbox.client.Client) - Labelbox Client object    
+        lb_mdo              :   Optional (labelbox.schema.data_row_metadata.DataRowMetadataOntology) - Labelbox metadata ontology
+        divider             :   Optional (str) - String separating parent and enum option metadata values
+        invert              :   Optional (bool) - If True, inverts the dictionary to be where {key=metadata_name_key: value=metadata_schema_id}
     Returns:
-        batch_action                :   Required (bool) - True if batching to projects, False if not
-        annotate_action             :   Required (bool) - True if uploading annotations to projects, False if not
+        Dictionary where {key=metadata_schema_id: value=metadata_type} - or the inverse
+    """    
+    metadata_schema_to_type = {}
+    lb_mdo = client.get_data_row_metadata_ontology() if not lb_mdo else lb_mdo
+    for field in lb_mdo._get_ontology():
+        metadata_type = ""
+        if "enum" in field["kind"].lower():
+            metadata_type = "enum"
+        if "string" in field["kind"].lower():
+            metadata_type = "string"
+        if "datetime" in field["kind"].lower():
+            metadata_type = "datetime"
+        if "number" in field["kind"].lower():
+            metadata_type = "number"
+        if metadata_type:
+            metadata_schema_to_type[field["id"]] = metadata_type
+    return_value = metadata_schema_to_type if not invert else {v:k for k,v in metadata_schema_to_type.items()}
+    return return_value
+
+def get_metadata_schema_to_name_key(client:labelboxClient, lb_mdo=False, divider="///", invert:bool=False):
+    """ Creates a dictionary where {key=metadata_schema_id: value=metadata_name_key} 
+    - name_key is name for all metadata fields, and for enum options, it is "parent_name{divider}child_name"
+    Args:
+        client              :   Required (labelbox.client.Client) - Labelbox Client object    
+        lb_mdo              :   Optional (labelbox.schema.data_row_metadata.DataRowMetadataOntology) - Labelbox metadata ontology
+        divider             :   Optional (str) - String separating parent and enum option metadata values
+        invert              :   Optional (bool) - If True, inverts the dictionary to be where {key=metadata_name_key: value=metadata_schema_id}
+    Returns:
+        Dictionary where {key=metadata_schema_id: value=metadata_name_key} - or the inverse
     """
-    if (dataset_id_col=="") and (dataset_id==""):
-        raise ValueError(f"To create data rows, please provide either a `dataset_id` column or a Labelbox dataset ID to argument `dataset_id`")    
-    if (project_id == "") and (project_id_col == ""):
-        batch_action = False
-    else:
-        batch_action = True
-    if upload_method: # If there's an upload method, the user at least wants to upload annotations
-        if upload_method in ["mal", "import"]:
-            if not batch_action:
-                raise ValueError(f"Upload method was provided, but data rows have not been configured to-be-batched to projects")
-            elif annotation_index == {}:
-                raise ValueError(f"Upload method was provided, but no columns have been identified as columns containing annotation values")
-            else: # There's a batch_action and there's an annotation_index
-                annotate_action = True
+    lb_mdo = client.get_data_row_metadata_ontology() if not lb_mdo else lb_mdo
+    lb_metadata_dict = lb_mdo.reserved_by_name
+    lb_metadata_dict.update(lb_mdo.custom_by_name)
+    metadata_schema_to_name_key = {}
+    for metadata_field_name_key in lb_metadata_dict:
+        if type(lb_metadata_dict[metadata_field_name_key]) == dict:
+            metadata_schema_to_name_key[lb_metadata_dict[metadata_field_name_key][next(iter(lb_metadata_dict[metadata_field_name_key]))].parent] = str(metadata_field_name_key)
+            for enum_option in lb_metadata_dict[metadata_field_name_key]:
+                metadata_schema_to_name_key[lb_metadata_dict[metadata_field_name_key][enum_option].uid] = f"{str(metadata_field_name_key)}{str(divider)}{str(enum_option)}"
         else:
-            raise ValueError(f"Upload method was provided, but must be one of `mal` or `import` - received `{upload_method}`")
-    else:
-        annotate_action = False
-    return batch_action, annotate_action  
+            metadata_schema_to_name_key[lb_metadata_dict[metadata_field_name_key].uid] = str(metadata_field_name_key)
+    return_value = metadata_schema_to_name_key if not invert else {v:k for k,v in metadata_schema_to_name_key.items()}
+    return return_value  
+
+def _refresh_metadata_ontology(client:labelboxClient):
+    """ Refreshes a Labelbox Metadata Ontology
+    Args:
+        client              :   Required (labelbox.client.Client) - Labelbox Client object    
+    Returns:
+        lb_mdo              :   labelbox.schema.data_row_metadata.DataRowMetadataOntology
+        lb_metadata_names   :   List of metadata field names from a Labelbox metadata ontology
+    """
+    lb_mdo = client.get_data_row_metadata_ontology()
+    lb_metadata_names = [field['name'] for field in lb_mdo._get_ontology()]
+    return lb_mdo, lb_metadata_names
 
-def validate_columns(client:labelboxClient, table, get_columns_function, get_unique_values_function, 
-                     divider:str="///", verbose:bool=False, extra_client=None):
-    """ Given a table of columns with the right naming formats, does the following:
-    
-    1. Identifies a `row_data_col` name, `global_key_col` name, and an `external_id_col` name
-    
-    - `row_data_col` must be identified as the column with the name `row_data`
-    - `global_key_col` defaults to `row_data_col` if not identified
-    - `external_id_col` defaults to `global_key_col` if not identified
-    
-    2. Creates a metadata_index, attachment_index, and annotation_index - validates that the column names are in the right format:
-    
-    - Metadata columns must be `metadata{divider}metadata_type{divider}metadata_field_name`
-        - metadata_type must be one of |"enum", "string", "datetime", "number"| (not case sensitive)
-        
-    - Attachment columns must be `attachment{divider}attachment_type{divider}column_name` (column_name is not relevant for attachment columns
-        - metadata_type must be one of |"IMAGE", "VIDEO", "RAW_TEXT", "HTML", "TEXT_URL"| (not case sensitive)
-        
-    - Metadata columns must be `annotation{divider}annotation_type{divider}top_level_name`
-        - annotation_type must be one of |"bbox", "polygon", "point", "mask", "line", "named-entity", "radio", "checklist", "text"| (not case sensitive)
-        
+def sync_metadata_fields(client:labelboxClient, table, get_columns_function, add_column_function, get_unique_values_function, metadata_index:dict={}, verbose:bool=False, extra_client=None):
+    """ Ensures Labelbox's Metadata Ontology and your input have all necessary metadata fields / columns given a metadata_index
     Args:
         client                      :   Required (labelbox.client.Client) - Labelbox Client object    
-        table                       :   Required - Input user table    
+        table                       :   Required - Input user table
         get_columns_function        :   Required (function) - Function that can get the column names from the table provided, returns list of strings
+        add_column_function         :   Required (function) - Function that can add an empty column to the table provided, returns table
         get_unique_values_function  :   Required (function) - Function that grabs all unique values from a column, returns list of strings
+        metadata_index              :   Optional (dict) - Dictionary where {key=column_name : value=metadata_type} - metadata_type must be one of "enum", "string", "datetime" or "number"
         verbose                     :   Optional (bool) - If True, prints information about code execution
-        extra_client                :   Optional - If relevant, the input get_columns_function / get_unique_values_function required other client object
+        extra_client                :   Optional - If relevant, the input functions' required other client object
     Returns:
-        row_data_col                :   Raises an error if no `row_data` column is provided
-        global_key_col              :   Defaults to row_data_col
-        external_id_col             :   Defaults to global_key_col
-        project_id_col              :   Returns "" if no `project_id` column is provided
-        dataset_id_col              :   Returns "" if no `dataset_id` column is provided
-        metadata_index              :   Dictonary where {key=metadata_field_name : value=metadata_type}
-        attachment_index            :   Dictonary where {key=column_name : value=attachment_type}
-        annotation_index            :   Dictonary where {key=column_name : value=annotation_type}
+        Updated table if successful, False if not
     """
-    metadata_index = {}
-    attachment_index = {}
-    annotation_index = {}
-    row_data_col = ""
-    global_key_col = ""
-    external_id_col = ""
-    project_id_col = ""
-    dataset_id_col = ""
-    accepted_metadata_types = ["enum", "string", "datetime", "number"]
-    accepted_attachment_types = ["IMAGE", "VIDEO", "RAW_TEXT", "HTML", "TEXT_URL"]
-    accepted_annotation_types = ["bbox", "polygon", "point", "mask", "line", "named-entity", "radio", "checklist", "text"]
-    column_names = get_columns_function(table=table, extra_client=extra_client)
-    for column_name in column_names:
-        if divider in column_name:
-            input_type, column_type, header = column_name.split(divider)
-            if input_type.lower() == "metadata":
-                if column_type.lower() not in accepted_metadata_types:
-                    raise ValueError(f"Invalid value in metadata column name {column_name} - must be `metadata{divider}` followed by one of the following: |{accepted_metadata_types}| followed by `{divider}metadata_field_name`")
-                metadata_index[header] = column_type.lower()
-            elif input_type.lower() == "attachment":
-                if column_type.upper() not in accepted_attachment_types:
-                    raise ValueError(f"Invalid value in attachment column name {column_name} - must be `attachment{divider}` followed by one of the following: |{accepted_attachment_types}| followed by `{divider}column_name`")
-                attachment_index[column_name] = column_type.upper()
-            elif input_type.lower() == "annotation":
-                if column_type.lower() not in accepted_annotation_types:
-                    raise ValueError(f"Invalid value in annotation column name {column_name} - must be `annotation{divider}` followed by one of the following: |{accepted_annotation_types}| followed by `{divider}top_level_feature_name`")
-                annotation_index[column_name] = header
-        else:
-            if column_name == "row_data":
-                row_data_col = "row_data"
-            if column_name == "global_key":
-                global_key_col = "global_key"
-            if column_name == "external_id":
-                external_id_col = "external_id"   
-            if column_name == "project_id":
-                project_id_col = "project_id"   
-            if column_name == "dataset_id":
-                dataset_id_col = "dataset_id" 
-    if not row_data_col:
-        raise ValueError(f"No `row_data` column found - please provide a column of row data URls with the colunn name `row_data`")
-    global_key_col = global_key_col if global_key_col else row_data_col
-    external_id_col = external_id_col if external_id_col else global_key_col
+    # Get your metadata ontology, grab all the metadata field names
     lb_mdo, lb_metadata_names = _refresh_metadata_ontology(client)
-    metadata_types = {
-      "enum" : DataRowMetadataKind.enum, 
-      "string" : DataRowMetadataKind.string, 
-      "datetime" : DataRowMetadataKind.datetime, 
-      "number" : DataRowMetadataKind.number
-    }
-    # If a metadata field name was passed in that doesn't exist, create it in Labelbox
-    if metadata_index:
-        for metadata_field_name in metadata_index.keys():
-            metadata_string_type = metadata_index[metadata_field_name]
-            if metadata_field_name not in lb_metadata_names:
-                enum_options = get_unique_values_function(table=table, col=f"metadata{divider}{metadata_string_type}{divider}{metadata_field_name}", extra_client=extra_client) if metadata_string_type == "enum" else []
-                if verbose:
-                    print(f"Creating Labelbox metadata field with name {metadata_field_name} of type {metadata_string_type}")
-                lb_mdo.create_schema(name=metadata_field_name, kind=metadata_types[metadata_string_type], options=enum_options)
-    if "lb_integration_source" not in lb_metadata_names:
-        lb_mdo.create_schema(name="lb_integration_source", kind=metadata_types["string"])
-    return row_data_col, global_key_col, external_id_col, project_id_col, dataset_id_col, metadata_index, attachment_index, annotation_index
-  
-def validate_column_name_change(old_col_name:str, new_col_name:str, existing_col_names:list):
-    """ Validates that the rename aligns with LabelPandas column name specifications
+    # Convert your meatdata_index values from strings into labelbox.schema.data_row_metadata.DataRowMetadataKind types
+    conversion = {"enum" : DataRowMetadataKind.enum, "string" : DataRowMetadataKind.string, "datetime" : DataRowMetadataKind.datetime, "number" : DataRowMetadataKind.number}
+    # Check to make sure the value in your metadata index is one of the accepted values        
+    _enforce_metadata_index(metadata_index, verbose)
+    # If your table doesn't have columns for all your metadata_field_names, make columns for them
+    if type(table) != bool:
+        if metadata_index:
+            column_names = get_columns_function(table, extra_client=extra_client)
+            for metadata_field_name in metadata_index.keys():
+                if metadata_field_name not in column_names:
+                    table = add_column_function(table=table, col=metadata_field_name, default_value=None, extra_client=extra_client)
+    # If Labelbox doesn't have metadata for all your metadata_field_names, make Labelbox metadata fields
+    for metadata_field_name in metadata_index.keys():
+        metadata_type = metadata_index[metadata_field_name]
+        # Check to see if a metadata index input is a metadata field in Labelbox. If not, create the metadata field in Labelbox. 
+        if metadata_field_name not in lb_metadata_names:
+            enum_options = get_unique_values_function(table=table, col=metadata_field_name, extra_client=extra_client) if metadata_type == "enum" else []
+            lb_mdo.create_schema(name=metadata_field_name, kind=conversion[metadata_type], options=enum_options)
+            lb_mdo, lb_metadata_names = _refresh_metadata_ontology(client)
+    if 'lb_integration_source' not in lb_metadata_names:
+        lb_mdo.create_schema(name='lb_integration_source', kind=conversion["string"])
+    return table  
+
+def process_metadata_value(metadata_value, metadata_type:str, parent_name:str, metadata_name_key_to_schema:dict, divider:str="///"):
+    """ Processes inbound values to ensure only valid values are added as metadata to Labelbox given the metadata type. Returns None if invalid or None
     Args:
-        old_col_name                :   Required (str) - Original column name
-        new_col_name                :   Required (str) - Desired new name
-        existing_col_names          :   Required (list) - List of existing column names
+        metadata_value              :   Required (any) - Value to-be-screeened and inserted as a proper metadata value to-be-uploaded to Labelbox
+        metadata_type               :   Required (str) - Either "string", "datetime", "enum", or "number"
+        parent_name                 :   Required (str) - Parent metadata field name
+        metadata_name_key_to_schema :   Required (dict) - Dictionary where {key=metadata_field_name_key : value=metadata_schema_id}
+        divider                     :   Required (str) - String delimiter for all name keys generated
     Returns:
-        Nothing - 
-        - Will raise an error if the old column name isn't in the passed in DataFrame
-        - Will also raise an error if the new column name isn't what LabelPandas is expecting
-    """ 
-    if old_col_name not in existing_col_names:
-        raise ValueError(f"Argument `rename_dict` requires a dictionary where:\n            \n        `old_column_name` : `new_column_name`,\n        `old_column_name` : `new_column_name`\n    \nReceived key `{old_col_name}` which is not an existing column name")    
-    if new_col_name in ["row_data", "external_id", "global_key", "file_path"]:
-        valid_column = True
-    elif new_col_name.startswith("metadata"):
-        valid_column = True
-    elif new_col_name.startswith("attachment"):
-        valid_column = True
-    elif new_col_name.startswith("annotation"):
-        valid_column = True   
-    else:
-        valid_column = False
-    if not valid_column:
-        raise ValueError(f"New name assignment invalid for LabelPandas - colmn name must be one of `row_data`, `external_id` or `global_key` or start with `metadata`, `attachment` or `annotation` -- received new column name `{new_col_name}`")  
+        The proper data type given the metadata type for the input value. None if the value is invalud - should be skipped
+    """
+    if not metadata_value: # Catch empty values
+        return_value = None
+    if str(metadata_value) == "nan": # Catch NaN values
+        return_value = None
+    # By metadata type
+    if metadata_type == "enum": # For enums, it must be a schema ID - if we can't match it, we have to skip it
+        name_key = f"{parent_name}{divider}{str(metadata_value)}"
+        if name_key in metadata_name_key_to_schema.keys():
+            return_value = str(metadata_name_key_to_schema[name_key])
+        else:
+            return_value = None                  
+    elif metadata_type == "number": # For numbers, it's ints as strings
+        try:
+            return_value = str(int(metadata_value))
+        except:
+            return_value = None                  
+    elif metadata_type == "string": 
+        return_value = str(metadata_value)
+    else: # For datetime, it's an isoformat string
+        if type(metadata_value) == str:
+            metadata_value = parser.parse(metadata_value)
+        if type(metadata_value) == datetime:
+            metadata_value = metadata_value.astimezone(pytz.utc).replace(tzinfo=None)
+            return_value = metadata_value.isoformat(sep='Z',timespec='auto')                
+        else:
+            return_value = None     
+    return return_value
```

### Comparing `labelbase-0.1.0/labelbase/converters/coco.py` & `labelbase-0.1.1/labelbase/converters/coco.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.0/labelbase/dataset.py` & `labelbase-0.1.1/labelbase/dataset.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.0/labelbase/masks.py` & `labelbase-0.1.1/labelbase/masks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 import numpy as np
 from PIL import Image
 from io import BytesIO
 import requests
 from labelbox.data import annotation_types as lb_types
 from labelbox.data.serialization import NDJsonConverter
+from labelbox import Client as labelboxClient
 
-def mask_to_bytes(input:str, method:str="url", color=[255,255,255], output:str="png"):
+def get_mask_from_url(url, headers, max_retries=5, n=0):
+    try:
+        if n >= max_retries:
+            return
+        r = requests.get(url, headers=headers).content
+        return np.array(Image.open(BytesIO(r)))[:,:,:3]
+    except:
+        return get_mask_from_url(url, headers, max_retries, n=n+1)
+
+def mask_to_bytes(client:labelboxClient, input:str, datarow_id:str, method:str="url", color=[255,255,255], output:str="png"):
     """ Given a mask input, returns a png bytearray of said mask
     Args:
-        input     :   Required (str) - URL of a mask
-        method    :   Required (str) - Either "url" or "array" - determines how you want the input treated
-        color     :   Required (arr or int) - The color of your mask in your input value
-        output    :   Required (str) - Either "array" or "png" - determines how you want the data returned
+        client      :   Required       - Labelbox client
+        input       :   Required (str) - URL of a mask
+        datarow_id  :   Required (str) - Datarow id that has the mask annotation
+        method      :   Required (str) - Either "url" or "array" - determines how you want the input treated
+        color       :   Required (arr or int) - The color of your mask in your input value
+        output      :   Required (str) - Either "array" or "png" - determines how you want the data returned
     Returns:
         Mask as a numpy array or as string png bytes
     """
     # Convert URL or array mask into a binary array
     if method not in ["url", "array"]:
         raise ValueError(f'Downloading bytes requires input method to be either a "url" or a "array" - received method {method}')
     if output not in ["array", "png"]:
         raise ValueError(f'Downloading bytes requires output method to be either a "png" or a "array" - received method {method}')     
     # Either download a mask URL or ensure the shape of your numpy array
     if method == "url":
-        r = requests.get(input).content
-        np_mask = np.array(Image.open(BytesIO(r)))[:,:,:3]
+        headers = {
+            "Authorization": f"Bearer {client.api_key}"
+        }
+        np_mask = get_mask_from_url(input, headers)
     else:
         if len(input.shape) == 3:
             np_mask = input
         elif len(input.shape) == 2:
             np_mask = [input, input, input]
         else:
             raise ValueError(f"Input segmentation mask arrays must either be 2D or 3D - shape of input mask: {input.shape}")
@@ -38,15 +52,15 @@
     else:
         raise ValueError(f"The specified color of your segmentation mask must either be a number (for 2D masks) or an RGB code (for 3D masks) - {color}")
     # Return either a numpy array or a png byte string
     if output == "array":
         return np_mask
     else:
         mask_label = lb_types.Label(
-            data=lb_types.ImageData(uid=""),
+            data=lb_types.ImageData(uid=datarow_id),
             annotations=[
                 lb_types.ObjectAnnotation(
                     name="", 
                     value=lb_types.Mask(
                         mask=lb_types.MaskData(arr=np_mask), 
                         color=np_color
                     )
```

### Comparing `labelbase-0.1.0/labelbase/ontology.py` & `labelbase-0.1.1/labelbase/ontology.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.0/labelbase.egg-info/PKG-INFO` & `labelbase-0.1.1/labelbase.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelbase
-Version: 0.1.0
+Version: 0.1.1
 Summary: Labelbox Helper Library
 Home-page: https://labelbox.com
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Keywords: labelbox,labelbase
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `labelbase-0.1.0/setup.py` & `labelbase-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
       name='labelbase',
-      version='0.1.00',
+      version='0.1.01',
       author='Labelbox',
       author_email='raphael@labelbox.com',
       description='Labelbox Helper Library',      
       packages=setuptools.find_packages(),
       url="https://labelbox.com",
       long_description=long_description,
       long_description_content_type="text/markdown",
```

