# Comparing `tmp/multiplex-imaging-pipeline-0.0.2.tar.gz` & `tmp/multiplex-imaging-pipeline-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiplex-imaging-pipeline-0.0.2.tar", last modified: Tue Jan 17 14:45:02 2023, max compression
+gzip compressed data, was "dist/multiplex-imaging-pipeline-0.0.3.tar", last modified: Mon Jul 10 21:15:59 2023, max compression
```

## Comparing `multiplex-imaging-pipeline-0.0.2.tar` & `multiplex-imaging-pipeline-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-01-17 14:45:02.125426 multiplex-imaging-pipeline-0.0.2/
--rw-r--r--   0 estorrs   (1048) users      (100)     1068 2022-05-03 13:51:26.000000 multiplex-imaging-pipeline-0.0.2/LICENSE
--rw-r--r--   0 estorrs   (1048) users      (100)     7035 2023-01-17 14:45:02.124426 multiplex-imaging-pipeline-0.0.2/PKG-INFO
--rw-r--r--   0 estorrs   (1048) users      (100)     6277 2023-01-13 15:09:54.000000 multiplex-imaging-pipeline-0.0.2/README.md
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-01-17 14:45:02.113426 multiplex-imaging-pipeline-0.0.2/mip/
--rw-r--r--   0 estorrs   (1048) users      (100)        0 2022-05-03 13:56:19.000000 multiplex-imaging-pipeline-0.0.2/mip/__init__.py
--rw-r--r--   0 estorrs   (1048) users      (100)     4217 2022-07-15 15:16:11.000000 multiplex-imaging-pipeline-0.0.2/mip/gating.py
--rw-r--r--   0 estorrs   (1048) users      (100)     7666 2023-01-12 15:15:09.000000 multiplex-imaging-pipeline-0.0.2/mip/mip.py
--rw-r--r--   0 estorrs   (1048) users      (100)     5548 2023-01-11 19:55:33.000000 multiplex-imaging-pipeline-0.0.2/mip/ome.py
--rw-r--r--   0 estorrs   (1048) users      (100)    26795 2023-01-11 14:14:38.000000 multiplex-imaging-pipeline-0.0.2/mip/region_analysis.py
--rw-r--r--   0 estorrs   (1048) users      (100)     2058 2022-05-09 13:43:22.000000 multiplex-imaging-pipeline-0.0.2/mip/spatial_features.py
--rw-r--r--   0 estorrs   (1048) users      (100)     5106 2023-01-13 15:50:42.000000 multiplex-imaging-pipeline-0.0.2/mip/utils.py
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-01-17 14:45:02.122426 multiplex-imaging-pipeline-0.0.2/multiplex_imaging_pipeline.egg-info/
--rw-r--r--   0 estorrs   (1048) users      (100)     7035 2023-01-17 14:45:00.000000 multiplex-imaging-pipeline-0.0.2/multiplex_imaging_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 estorrs   (1048) users      (100)      440 2023-01-17 14:45:00.000000 multiplex-imaging-pipeline-0.0.2/multiplex_imaging_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 estorrs   (1048) users      (100)        1 2023-01-17 14:45:00.000000 multiplex-imaging-pipeline-0.0.2/multiplex_imaging_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       37 2023-01-17 14:45:00.000000 multiplex-imaging-pipeline-0.0.2/multiplex_imaging_pipeline.egg-info/entry_points.txt
--rw-r--r--   0 estorrs   (1048) users      (100)      128 2023-01-17 14:45:00.000000 multiplex-imaging-pipeline-0.0.2/multiplex_imaging_pipeline.egg-info/requires.txt
--rw-r--r--   0 estorrs   (1048) users      (100)        4 2023-01-17 14:45:00.000000 multiplex-imaging-pipeline-0.0.2/multiplex_imaging_pipeline.egg-info/top_level.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       38 2023-01-17 14:45:02.126426 multiplex-imaging-pipeline-0.0.2/setup.cfg
--rw-r--r--   0 estorrs   (1048) users      (100)     1658 2023-01-17 14:44:47.000000 multiplex-imaging-pipeline-0.0.2/setup.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:15:59.441954 multiplex-imaging-pipeline-0.0.3/
+-rw-r--r--   0 estorrs   (1048) users      (100)     1068 2022-05-03 13:51:26.000000 multiplex-imaging-pipeline-0.0.3/LICENSE
+-rw-r--r--   0 estorrs   (1048) users      (100)    11200 2023-07-10 21:15:59.440954 multiplex-imaging-pipeline-0.0.3/PKG-INFO
+-rw-r--r--   0 estorrs   (1048) users      (100)    10542 2023-07-10 20:30:49.000000 multiplex-imaging-pipeline-0.0.3/README.md
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:15:59.424954 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/
+-rw-r--r--   0 estorrs   (1048) users      (100)        0 2022-05-03 13:56:19.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/__init__.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:15:59.438954 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/compute1/
+-rw-r--r--   0 estorrs   (1048) users      (100)        0 2023-07-10 19:12:30.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/compute1/__init__.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     4886 2023-07-10 19:24:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/compute1/generate_run_commands.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10432 2023-07-07 15:00:12.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    12125 2023-07-10 18:24:27.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/ome.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10283 2023-07-10 18:57:35.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/region_features.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     5319 2023-06-29 15:42:55.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/segmentation.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     8976 2023-07-10 18:14:03.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/spatial_features.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10291 2023-07-07 14:20:21.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline/utils.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:15:59.435954 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/
+-rw-r--r--   0 estorrs   (1048) users      (100)    11200 2023-07-10 21:15:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 estorrs   (1048) users      (100)      739 2023-07-10 21:15:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)        1 2023-07-10 21:15:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       83 2023-07-10 21:15:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/entry_points.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)      148 2023-07-10 21:15:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/requires.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       27 2023-07-10 21:15:58.000000 multiplex-imaging-pipeline-0.0.3/multiplex_imaging_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       38 2023-07-10 21:15:59.442954 multiplex-imaging-pipeline-0.0.3/setup.cfg
+-rw-r--r--   0 estorrs   (1048) users      (100)     1637 2023-07-10 21:15:53.000000 multiplex-imaging-pipeline-0.0.3/setup.py
```

### Comparing `multiplex-imaging-pipeline-0.0.2/LICENSE` & `multiplex-imaging-pipeline-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.2/setup.py` & `multiplex-imaging-pipeline-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,49 +8,48 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     # $ pip install multiplex-imaging-pipeline
     name='multiplex-imaging-pipeline',
-    version='0.0.2',
+    version='0.0.3',
     description='A Python library for multiplex imaging analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/estorrs/multiplex-imaging-analysis',
     author='Erik Storrs',
     author_email='estorrs@wustl.edu',
     classifiers=[
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     keywords='multiplex imaging codex neighborhood analysis image segmentation visualization mibi codex phenocycler mihc hyperion',
     packages=find_packages(),
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     install_requires=[
+        'pyyaml',
         'numpy',
         'pandas',
+        'einops',
         'matplotlib',
         'scanpy',
         'seaborn',
         'tifffile',
         'ome-types',
         'scikit-image',
         'scikit-learn',
-        'shapely',
-        'rasterio',
-        'gensim',
-        'squidpy',
-        'imagecodecs',
+        'imagecodecs>=2022.7.27',
+        'torch',
+        'torchvision',
+        'deepcell',
     ],
     include_package_data=True,
 
     entry_points={
         'console_scripts': [
-            'mip=mip.mip:main',
+            'mip=multiplex_imaging_pipeline.multiplex_imaging_pipeline:main',
         ],
     },
 )
```

