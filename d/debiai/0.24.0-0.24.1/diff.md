# Comparing `tmp/debiai-0.24.0.tar.gz` & `tmp/debiai-0.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debiai-0.24.0.tar", last modified: Thu Jul  6 15:19:47 2023, max compression
+gzip compressed data, was "debiai-0.24.1.tar", last modified: Mon Jul 10 16:11:02 2023, max compression
```

## Comparing `debiai-0.24.0.tar` & `debiai-0.24.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:47.874458 debiai-0.24.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-06 15:19:42.000000 debiai-0.24.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-07-06 15:19:47.870458 debiai-0.24.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-07-06 15:19:42.000000 debiai-0.24.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:47.870458 debiai-0.24.0/debiai/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai.py
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21746 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:47.870458 debiai-0.24.0/debiai/debiai_services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_services/df_to_dict_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_services/np_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:47.870458 debiai-0.24.0/debiai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-07-06 15:19:47.000000 debiai-0.24.0/debiai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-06 15:19:47.000000 debiai-0.24.0/debiai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 15:19:47.000000 debiai-0.24.0/debiai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 15:19:47.000000 debiai-0.24.0/debiai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 15:19:47.000000 debiai-0.24.0/debiai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 15:19:47.874458 debiai-0.24.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-06 15:19:42.000000 debiai-0.24.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:47.870458 debiai-0.24.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:42.000000 debiai-0.24.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-06 15:19:42.000000 debiai-0.24.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-06 15:19:42.000000 debiai-0.24.0/tests/test_project_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-06 15:19:42.000000 debiai-0.24.0/tests/test_projects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:02.747187 debiai-0.24.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-10 16:10:57.000000 debiai-0.24.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-07-10 16:11:02.747187 debiai-0.24.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-07-10 16:10:57.000000 debiai-0.24.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:02.747187 debiai-0.24.1/debiai/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 16:10:57.000000 debiai-0.24.1/debiai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-10 16:10:57.000000 debiai-0.24.1/debiai/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-10 16:10:57.000000 debiai-0.24.1/debiai/debiai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-10 16:10:57.000000 debiai-0.24.1/debiai/debiai_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22443 2023-07-10 16:10:57.000000 debiai-0.24.1/debiai/debiai_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-10 16:10:57.000000 debiai-0.24.1/debiai/debiai_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:02.747187 debiai-0.24.1/debiai/debiai_services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:57.000000 debiai-0.24.1/debiai/debiai_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-10 16:10:57.000000 debiai-0.24.1/debiai/debiai_services/df_to_dict_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-10 16:10:57.000000 debiai-0.24.1/debiai/debiai_services/np_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-10 16:10:57.000000 debiai-0.24.1/debiai/debiai_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-10 16:10:57.000000 debiai-0.24.1/debiai/debiai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-10 16:10:57.000000 debiai-0.24.1/debiai/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:02.747187 debiai-0.24.1/debiai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-07-10 16:11:02.000000 debiai-0.24.1/debiai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-10 16:11:02.000000 debiai-0.24.1/debiai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:11:02.000000 debiai-0.24.1/debiai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 16:11:02.000000 debiai-0.24.1/debiai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 16:11:02.000000 debiai-0.24.1/debiai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:11:02.747187 debiai-0.24.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-10 16:10:57.000000 debiai-0.24.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:02.747187 debiai-0.24.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:57.000000 debiai-0.24.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-10 16:10:57.000000 debiai-0.24.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-10 16:10:57.000000 debiai-0.24.1/tests/test_project_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-10 16:10:57.000000 debiai-0.24.1/tests/test_projects.py
```

### Comparing `debiai-0.24.0/LICENSE` & `debiai-0.24.1/LICENSE`

 * *Files identical despite different names*

### Comparing `debiai-0.24.0/PKG-INFO` & `debiai-0.24.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debiai
-Version: 0.24.0
+Version: 0.24.1
 Summary: DebiAI python module
 Home-page: https://github.com/debiai/py-debiai
 Author: IRT-SystemX
 Author-email: debiai@irt-systemx.fr
 License: Apache 2.0
 Keywords: DebiAI,Data vis,AI,Bias
 Classifier: Programming Language :: Python :: 3
```

### Comparing `debiai-0.24.0/README.md` & `debiai-0.24.1/README.md`

 * *Files identical despite different names*

### Comparing `debiai-0.24.0/debiai/config.py` & `debiai-0.24.1/debiai/config.py`

 * *Files identical despite different names*

### Comparing `debiai-0.24.0/debiai/debiai.py` & `debiai-0.24.1/debiai/debiai.py`

 * *Files identical despite different names*

### Comparing `debiai-0.24.0/debiai/debiai_model.py` & `debiai-0.24.1/debiai/debiai_model.py`

 * *Files identical despite different names*

### Comparing `debiai-0.24.0/debiai/debiai_project.py` & `debiai-0.24.1/debiai/debiai_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,24 @@
                                 "Unknown type of the column '"
                                 + column["name"]
                                 + "' in the block '"
                                 + block["name"]
                                 + "'. Use : ['text', 'number', 'boolean']"
                             )
 
+                        if "group" in column:
+                            if not isinstance(column["group"], str):
+                                raise ValueError(
+                                    "The group of the column '"
+                                    + column["name"]
+                                    + "' in the block '"
+                                    + block["name"]
+                                    + "' must be a string"
+                                )
+
         # Set the block_structure
         utils.add_blocklevel(self.debiai_url, self.id, block_structure)
         self.block_structure = block_structure
 
     # Results structure
     def expected_results_defined(self):
         self.project_infos()
@@ -232,14 +242,20 @@
 
             newRes = {"name": column["name"], "type": column["type"]}
 
             if "default" in column:
                 newRes["default"] = column["default"]
                 # TODO check default type same as col type
 
+            if "group" in column:
+                if type(column["group"]) != str:
+                    raise ValueError("The group attribute must be a string")
+
+                newRes["group"] = column["group"]
+
             expResults.append(newRes)
 
         utils.post_expected_results(self.debiai_url, self.id, expResults)
         self.expected_results = expResults
 
     def add_expected_result(self, column: dict) -> List[dict]:
         if self.expected_results is None:
```

### Comparing `debiai-0.24.0/debiai/debiai_selection.py` & `debiai-0.24.1/debiai/debiai_selection.py`

 * *Files identical despite different names*

### Comparing `debiai-0.24.0/debiai/debiai_services/df_to_dict_tree.py` & `debiai-0.24.1/debiai/debiai_services/df_to_dict_tree.py`

 * *Files identical despite different names*

### Comparing `debiai-0.24.0/debiai/debiai_services/np_to_dict.py` & `debiai-0.24.1/debiai/debiai_services/np_to_dict.py`

 * *Files identical despite different names*

### Comparing `debiai-0.24.0/debiai/debiai_tag.py` & `debiai-0.24.1/debiai/debiai_tag.py`

 * *Files identical despite different names*

### Comparing `debiai-0.24.0/debiai/debiai_utils.py` & `debiai-0.24.1/debiai/debiai_utils.py`

 * *Files identical despite different names*

### Comparing `debiai-0.24.0/debiai/utils.py` & `debiai-0.24.1/debiai/utils.py`

 * *Files identical despite different names*

### Comparing `debiai-0.24.0/debiai.egg-info/PKG-INFO` & `debiai-0.24.1/debiai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debiai
-Version: 0.24.0
+Version: 0.24.1
 Summary: DebiAI python module
 Home-page: https://github.com/debiai/py-debiai
 Author: IRT-SystemX
 Author-email: debiai@irt-systemx.fr
 License: Apache 2.0
 Keywords: DebiAI,Data vis,AI,Bias
 Classifier: Programming Language :: Python :: 3
```

### Comparing `debiai-0.24.0/debiai.egg-info/SOURCES.txt` & `debiai-0.24.1/debiai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `debiai-0.24.0/setup.py` & `debiai-0.24.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="debiai",
-    version="0.24.0",
+    version="0.24.1",
     author="IRT-SystemX",
     author_email="debiai@irt-systemx.fr",
     description="DebiAI python module",
     license="Apache 2.0",
     keywords="DebiAI, Data vis, AI, Bias",
     url="https://github.com/debiai/py-debiai",
     long_description=open("README.md").read(),
```

### Comparing `debiai-0.24.0/tests/test_project_samples.py` & `debiai-0.24.1/tests/test_project_samples.py`

 * *Files identical despite different names*

### Comparing `debiai-0.24.0/tests/test_projects.py` & `debiai-0.24.1/tests/test_projects.py`

 * *Files identical despite different names*

