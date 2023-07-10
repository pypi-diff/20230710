# Comparing `tmp/napari-stpt-0.1.0.4.tar.gz` & `tmp/napari-stpt-0.1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-stpt-0.1.0.4.tar", last modified: Mon Jul 10 03:39:33 2023, max compression
+gzip compressed data, was "napari-stpt-0.1.0.5.tar", last modified: Mon Jul 10 11:51:53 2023, max compression
```

## Comparing `napari-stpt-0.1.0.4.tar` & `napari-stpt-0.1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-10 03:39:33.946569 napari-stpt-0.1.0.4/
--rw-r--r--   0 tristan   (1000) tristan   (1000)    35149 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.4/LICENSE
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-07-10 03:39:33.945569 napari-stpt-0.1.0.4/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3170 2021-07-01 22:42:19.000000 napari-stpt-0.1.0.4/README.md
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-10 03:39:33.870568 napari-stpt-0.1.0.4/napari_stpt/
--rw-r--r--   0 tristan   (1000) tristan   (1000)       46 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.4/napari_stpt/__init__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)      267 2022-01-28 14:11:11.000000 napari-stpt-0.1.0.4/napari_stpt/__main__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)   147416 2023-07-08 14:57:22.000000 napari-stpt-0.1.0.4/napari_stpt/napari_stpt.py
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-10 03:39:33.942569 napari-stpt-0.1.0.4/napari_stpt.egg-info/
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-07-10 03:39:33.000000 napari-stpt-0.1.0.4/napari_stpt.egg-info/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)      313 2023-07-10 03:39:33.000000 napari-stpt-0.1.0.4/napari_stpt.egg-info/SOURCES.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2023-07-10 03:39:33.000000 napari-stpt-0.1.0.4/napari_stpt.egg-info/dependency_links.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       58 2023-07-10 03:39:33.000000 napari-stpt-0.1.0.4/napari_stpt.egg-info/entry_points.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)      116 2023-07-10 03:39:33.000000 napari-stpt-0.1.0.4/napari_stpt.egg-info/requires.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       12 2023-07-10 03:39:33.000000 napari-stpt-0.1.0.4/napari_stpt.egg-info/top_level.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       38 2023-07-10 03:39:33.946569 napari-stpt-0.1.0.4/setup.cfg
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1343 2023-07-10 03:38:36.000000 napari-stpt-0.1.0.4/setup.py
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-10 11:51:53.629359 napari-stpt-0.1.0.5/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)    35149 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.5/LICENSE
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-07-10 11:51:53.627359 napari-stpt-0.1.0.5/PKG-INFO
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3170 2021-07-01 22:42:19.000000 napari-stpt-0.1.0.5/README.md
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-10 11:51:53.566359 napari-stpt-0.1.0.5/napari_stpt/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       46 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.5/napari_stpt/__init__.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      267 2022-01-28 14:11:11.000000 napari-stpt-0.1.0.5/napari_stpt/__main__.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)   147412 2023-07-10 11:01:58.000000 napari-stpt-0.1.0.5/napari_stpt/napari_stpt.py
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-10 11:51:53.625359 napari-stpt-0.1.0.5/napari_stpt.egg-info/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-07-10 11:51:53.000000 napari-stpt-0.1.0.5/napari_stpt.egg-info/PKG-INFO
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      313 2023-07-10 11:51:53.000000 napari-stpt-0.1.0.5/napari_stpt.egg-info/SOURCES.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2023-07-10 11:51:53.000000 napari-stpt-0.1.0.5/napari_stpt.egg-info/dependency_links.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       58 2023-07-10 11:51:53.000000 napari-stpt-0.1.0.5/napari_stpt.egg-info/entry_points.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      116 2023-07-10 11:51:53.000000 napari-stpt-0.1.0.5/napari_stpt.egg-info/requires.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       12 2023-07-10 11:51:53.000000 napari-stpt-0.1.0.5/napari_stpt.egg-info/top_level.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       38 2023-07-10 11:51:53.629359 napari-stpt-0.1.0.5/setup.cfg
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     1343 2023-07-10 11:51:44.000000 napari-stpt-0.1.0.5/setup.py
```

### Comparing `napari-stpt-0.1.0.4/LICENSE` & `napari-stpt-0.1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.0.4/PKG-INFO` & `napari-stpt-0.1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stpt
-Version: 0.1.0.4
+Version: 0.1.0.5
 Summary: napari viewer which can read stpt images as zarr files
 Home-page: https://github.com/TristanWhitmarsh/napari-stpt
 Author: Tristan Whitmarsh
 Author-email: tw401@cam.ac.uk
 License: GNU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-stpt-0.1.0.4/README.md` & `napari-stpt-0.1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.0.4/napari_stpt/napari_stpt.py` & `napari-stpt-0.1.0.5/napari_stpt/napari_stpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -2698,15 +2698,15 @@
             self.old_method = False
             self.axio = False
             self.image_folders = {
                 '/storage/processed.2022/stpt/',
                 '/storage/processed/stpt/',
                 '/storage/imaxt.processed.2022/stpt/',
                 '/data/meds1_c/storage/processed0/stpt/',
-                '/storage/tristan/imaxt_zarr/'
+                '/storage/imaxt/imaxt_zarr/'
             }
             print("setting STPT method")
 
         file_list = []
         for folder in self.image_folders:
             print(sys.platform)
             if sys.platform == 'linux':
@@ -2826,15 +2826,15 @@
         self.comboBoxPath = ExtendedComboBox()
 
         self.image_folders = {
             '/storage/processed.2022/stpt/',
             '/storage/processed/stpt/',
             '/storage/imaxt.processed.2022/stpt/',
             '/data/meds1_c/storage/processed0/stpt/',
-            '/storage/tristan/imaxt_zarr/'
+            '/storage/imaxt/imaxt_zarr/'
         }
         file_list = []
         for folder in self.image_folders:
             self.search_folder = QtWidgets.QLineEdit(folder)
             if os.path.exists(self.search_folder.text()):
                 for f in os.scandir(self.search_folder.text()):
                     if f.is_dir():
```

### Comparing `napari-stpt-0.1.0.4/napari_stpt.egg-info/PKG-INFO` & `napari-stpt-0.1.0.5/napari_stpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stpt
-Version: 0.1.0.4
+Version: 0.1.0.5
 Summary: napari viewer which can read stpt images as zarr files
 Home-page: https://github.com/TristanWhitmarsh/napari-stpt
 Author: Tristan Whitmarsh
 Author-email: tw401@cam.ac.uk
 License: GNU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-stpt-0.1.0.4/setup.py` & `napari-stpt-0.1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # this grabs the requirements from requirements.txt
 #REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 # This call to setup() does all the work
 setup(
     name="napari-stpt",
-    version="0.1.0.4",
+    version="0.1.0.5",
     description="napari viewer which can read stpt images as zarr files",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/TristanWhitmarsh/napari-stpt",
     author="Tristan Whitmarsh",
     author_email="tw401@cam.ac.uk",
     license="GNU",
```

