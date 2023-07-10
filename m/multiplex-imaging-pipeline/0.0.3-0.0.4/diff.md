# Comparing `tmp/multiplex-imaging-pipeline-0.0.3.tar.gz` & `tmp/multiplex-imaging-pipeline-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/multiplex-imaging-pipeline-0.0.3.tar", last modified: Mon Jul 10 21:15:59 2023, max compression
+gzip compressed data, was "dist/multiplex-imaging-pipeline-0.0.4.tar", last modified: Mon Jul 10 21:39:27 2023, max compression
```

## Comparing `multiplex-imaging-pipeline-0.0.3.tar` & `multiplex-imaging-pipeline-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:15:59.441954 multiplex-imaging-pipeline-0.0.3/
--rw-r--r--   0 estorrs   (1048) users      (100)     1068 2022-05-03 13:51:26.000000 multiplex-imaging-pipeline-0.0.3/LICENSE
--rw-r--r--   0 estorrs   (1048) users      (100)    11200 2023-07-10 21:15:59.440954 multiplex-imaging-pipeline-0.0.3/PKG-INFO
--rw-r--r--   0 estorrs   (1048) users      (100)    10542 2023-07-10 20:30:49.000000 multiplex-imaging-pipeline-0.0.3/README.md
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:15:59.424954 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/
--rw-r--r--   0 estorrs   (1048) users      (100)        0 2022-05-03 13:56:19.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/__init__.py
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:15:59.438954 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/compute1/
--rw-r--r--   0 estorrs   (1048) users      (100)        0 2023-07-10 19:12:30.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/compute1/__init__.py
--rw-r--r--   0 estorrs   (1048) users      (100)     4886 2023-07-10 19:24:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/compute1/generate_run_commands.py
--rw-r--r--   0 estorrs   (1048) users      (100)    10432 2023-07-07 15:00:12.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py
--rw-r--r--   0 estorrs   (1048) users      (100)    12125 2023-07-10 18:24:27.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/ome.py
--rw-r--r--   0 estorrs   (1048) users      (100)    10283 2023-07-10 18:57:35.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/region_features.py
--rw-r--r--   0 estorrs   (1048) users      (100)     5319 2023-06-29 15:42:55.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/segmentation.py
--rw-r--r--   0 estorrs   (1048) users      (100)     8976 2023-07-10 18:14:03.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/spatial_features.py
--rw-r--r--   0 estorrs   (1048) users      (100)    10291 2023-07-07 14:20:21.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/utils.py
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:15:59.435954 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/
--rw-r--r--   0 estorrs   (1048) users      (100)    11200 2023-07-10 21:15:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 estorrs   (1048) users      (100)      739 2023-07-10 21:15:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 estorrs   (1048) users      (100)        1 2023-07-10 21:15:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       83 2023-07-10 21:15:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/entry_points.txt
--rw-r--r--   0 estorrs   (1048) users      (100)      148 2023-07-10 21:15:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/requires.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       27 2023-07-10 21:15:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/top_level.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       38 2023-07-10 21:15:59.442954 multiplex-imaging-pipeline-0.0.3/setup.cfg
--rw-r--r--   0 estorrs   (1048) users      (100)     1637 2023-07-10 21:15:53.000000 multiplex-imaging-pipeline-0.0.3/setup.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:39:27.009103 multiplex-imaging-pipeline-0.0.4/
+-rw-r--r--   0 estorrs   (1048) users      (100)     1068 2022-05-03 13:51:26.000000 multiplex-imaging-pipeline-0.0.4/LICENSE
+-rw-r--r--   0 estorrs   (1048) users      (100)    11200 2023-07-10 21:39:27.008103 multiplex-imaging-pipeline-0.0.4/PKG-INFO
+-rw-r--r--   0 estorrs   (1048) users      (100)    10542 2023-07-10 20:30:49.000000 multiplex-imaging-pipeline-0.0.4/README.md
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:39:26.998103 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/
+-rw-r--r--   0 estorrs   (1048) users      (100)        0 2022-05-03 13:56:19.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/__init__.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:39:27.007103 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/compute1/
+-rw-r--r--   0 estorrs   (1048) users      (100)        0 2023-07-10 19:12:30.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/compute1/__init__.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     4886 2023-07-10 19:24:58.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/compute1/generate_run_commands.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10432 2023-07-07 15:00:12.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    12125 2023-07-10 18:24:27.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/ome.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10283 2023-07-10 18:57:35.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/region_features.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     5319 2023-06-29 15:42:55.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/segmentation.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     8976 2023-07-10 18:14:03.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/spatial_features.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10291 2023-07-07 14:20:21.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/utils.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:39:27.005103 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/
+-rw-r--r--   0 estorrs   (1048) users      (100)    11200 2023-07-10 21:39:26.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 estorrs   (1048) users      (100)      739 2023-07-10 21:39:26.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)        1 2023-07-10 21:39:26.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       83 2023-07-10 21:39:26.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/entry_points.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)      148 2023-07-10 21:39:26.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/requires.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       27 2023-07-10 21:39:26.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       38 2023-07-10 21:39:27.009103 multiplex-imaging-pipeline-0.0.4/setup.cfg
+-rw-r--r--   0 estorrs   (1048) users      (100)     1637 2023-07-10 21:39:15.000000 multiplex-imaging-pipeline-0.0.4/setup.py
```

### Comparing `multiplex-imaging-pipeline-0.0.3/LICENSE` & `multiplex-imaging-pipeline-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.3/PKG-INFO` & `multiplex-imaging-pipeline-0.0.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiplex-imaging-pipeline
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python library for multiplex imaging analysis
 Home-page: https://github.com/estorrs/multiplex-imaging-analysis
 Author: Erik Storrs
 Author-email: estorrs@wustl.edu
 Keywords: multiplex imaging codex neighborhood analysis image segmentation visualization mibi codex phenocycler mihc hyperion
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `multiplex-imaging-pipeline-0.0.3/README.md` & `multiplex-imaging-pipeline-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/compute1/generate_run_commands.py` & `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/compute1/generate_run_commands.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py` & `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/ome.py` & `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/ome.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/region_features.py` & `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/region_features.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/segmentation.py` & `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/segmentation.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/spatial_features.py` & `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/spatial_features.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/utils.py` & `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/PKG-INFO` & `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiplex-imaging-pipeline
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python library for multiplex imaging analysis
 Home-page: https://github.com/estorrs/multiplex-imaging-analysis
 Author: Erik Storrs
 Author-email: estorrs@wustl.edu
 Keywords: multiplex imaging codex neighborhood analysis image segmentation visualization mibi codex phenocycler mihc hyperion
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/SOURCES.txt` & `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.3/setup.py` & `multiplex-imaging-pipeline-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     # $ pip install multiplex-imaging-pipeline
     name='multiplex-imaging-pipeline',
-    version='0.0.3',
+    version='0.0.4',
     description='A Python library for multiplex imaging analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/estorrs/multiplex-imaging-analysis',
     author='Erik Storrs',
     author_email='estorrs@wustl.edu',
     classifiers=[
```

