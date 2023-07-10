# Comparing `tmp/animl-1.1.0.tar.gz` & `tmp/animl-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animl-1.1.0.tar", last modified: Thu Jul  6 18:17:59 2023, max compression
+gzip compressed data, was "animl-1.1.1.tar", last modified: Mon Jul 10 16:51:37 2023, max compression
```

## Comparing `animl-1.1.0.tar` & `animl-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-07-06 18:17:59.854955 animl-1.1.0/
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     1084 2023-03-07 19:37:47.000000 animl-1.1.0/LICENSE
--rw-rw-r--   0 kyra      (1000) kyra      (1000)      788 2023-07-06 18:17:59.854955 animl-1.1.0/PKG-INFO
--rw-rw-r--   0 kyra      (1000) kyra      (1000)      233 2023-03-07 19:37:47.000000 animl-1.1.0/README.md
--rw-rw-r--   0 kyra      (1000) kyra      (1000)       85 2022-08-25 18:50:16.000000 animl-1.1.0/pyproject.toml
--rw-rw-r--   0 kyra      (1000) kyra      (1000)      680 2023-07-06 18:17:59.854955 animl-1.1.0/setup.cfg
-drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-07-06 18:17:59.854955 animl-1.1.0/src/
-drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-07-06 18:17:59.854955 animl-1.1.0/src/animl/
--rwxrwxr-x   0 kyra      (1000) kyra      (1000)     6620 2023-03-07 22:19:28.000000 animl-1.1.0/src/animl/ZooniverseAPI.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)        0 2022-08-25 18:50:16.000000 animl-1.1.0/src/animl/__init__.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     4586 2023-03-08 00:33:08.000000 animl-1.1.0/src/animl/__main__.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     6305 2023-06-08 19:05:39.000000 animl-1.1.0/src/animl/detectMD.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     4046 2023-06-12 22:35:23.000000 animl-1.1.0/src/animl/fileManagement.py
--rwxrwxr-x   0 kyra      (1000) kyra      (1000)     2489 2023-06-13 21:36:40.000000 animl-1.1.0/src/animl/imageCropGenerator.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     9362 2023-06-12 18:16:13.000000 animl-1.1.0/src/animl/imageUtils.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)    15363 2023-06-06 20:15:23.000000 animl-1.1.0/src/animl/loadMD.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     2338 2023-06-13 23:24:58.000000 animl-1.1.0/src/animl/parseResults.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     1194 2023-06-13 21:35:58.000000 animl-1.1.0/src/animl/predictSpecies.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)        0 2023-05-18 17:02:37.000000 animl-1.1.0/src/animl/setupDirectory.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     1112 2023-06-13 23:48:39.000000 animl-1.1.0/src/animl/splitData.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)      693 2023-05-17 21:35:40.000000 animl-1.1.0/src/animl/symlink.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     2430 2023-05-17 22:35:04.000000 animl-1.1.0/src/animl/test.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     4880 2023-06-08 18:04:13.000000 animl-1.1.0/src/animl/videoProcessing.py
-drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-07-06 18:17:59.854955 animl-1.1.0/src/animl.egg-info/
--rw-rw-r--   0 kyra      (1000) kyra      (1000)      788 2023-07-06 18:17:59.000000 animl-1.1.0/src/animl.egg-info/PKG-INFO
--rw-rw-r--   0 kyra      (1000) kyra      (1000)      544 2023-07-06 18:17:59.000000 animl-1.1.0/src/animl.egg-info/SOURCES.txt
--rw-rw-r--   0 kyra      (1000) kyra      (1000)        1 2023-07-06 18:17:59.000000 animl-1.1.0/src/animl.egg-info/dependency_links.txt
--rw-rw-r--   0 kyra      (1000) kyra      (1000)        6 2023-07-06 18:17:59.000000 animl-1.1.0/src/animl.egg-info/top_level.txt
+drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-07-10 16:51:37.670826 animl-1.1.1/
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     1084 2023-03-07 19:37:47.000000 animl-1.1.1/LICENSE
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)      788 2023-07-10 16:51:37.670826 animl-1.1.1/PKG-INFO
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)      233 2023-03-07 19:37:47.000000 animl-1.1.1/README.md
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)       85 2022-08-25 18:50:16.000000 animl-1.1.1/pyproject.toml
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)      680 2023-07-10 16:51:37.670826 animl-1.1.1/setup.cfg
+drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-07-10 16:51:37.666825 animl-1.1.1/src/
+drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-07-10 16:51:37.670826 animl-1.1.1/src/animl/
+-rwxrwxr-x   0 kyra      (1000) kyra      (1000)     6620 2023-03-07 22:19:28.000000 animl-1.1.1/src/animl/ZooniverseAPI.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)        0 2022-08-25 18:50:16.000000 animl-1.1.1/src/animl/__init__.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     4586 2023-03-08 00:33:08.000000 animl-1.1.1/src/animl/__main__.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)        0 2023-07-07 20:34:37.000000 animl-1.1.1/src/animl/demoTools.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     6305 2023-06-08 19:05:39.000000 animl-1.1.1/src/animl/detectMD.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     4047 2023-07-07 19:40:10.000000 animl-1.1.1/src/animl/fileManagement.py
+-rwxrwxr-x   0 kyra      (1000) kyra      (1000)     2489 2023-06-13 21:36:40.000000 animl-1.1.1/src/animl/imageCropGenerator.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     9362 2023-06-12 18:16:13.000000 animl-1.1.1/src/animl/imageUtils.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)    15363 2023-06-06 20:15:23.000000 animl-1.1.1/src/animl/loadMD.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     2338 2023-06-13 23:24:58.000000 animl-1.1.1/src/animl/parseResults.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     4755 2023-07-10 16:50:49.000000 animl-1.1.1/src/animl/plotBoxes.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     1194 2023-06-13 21:35:58.000000 animl-1.1.1/src/animl/predictSpecies.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)        0 2023-05-18 17:02:37.000000 animl-1.1.1/src/animl/setupDirectory.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     1112 2023-06-13 23:48:39.000000 animl-1.1.1/src/animl/splitData.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)      693 2023-05-17 21:35:40.000000 animl-1.1.1/src/animl/symlink.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     2430 2023-05-17 22:35:04.000000 animl-1.1.1/src/animl/test.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     4956 2023-07-07 19:40:10.000000 animl-1.1.1/src/animl/videoProcessing.py
+drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-07-10 16:51:37.670826 animl-1.1.1/src/animl.egg-info/
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)      788 2023-07-10 16:51:37.000000 animl-1.1.1/src/animl.egg-info/PKG-INFO
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)      590 2023-07-10 16:51:37.000000 animl-1.1.1/src/animl.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)        1 2023-07-10 16:51:37.000000 animl-1.1.1/src/animl.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)        6 2023-07-10 16:51:37.000000 animl-1.1.1/src/animl.egg-info/top_level.txt
```

### Comparing `animl-1.1.0/LICENSE` & `animl-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `animl-1.1.0/PKG-INFO` & `animl-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animl
-Version: 1.1.0
+Version: 1.1.1
 Summary: Functions required to classify subjects within camera trap field data.
 Home-page: https://github.com/conservationtechlab/animl-py
 Author: Kyra Swanson
 Author-email: tswanson@sdzwa.org
 Project-URL: Bug Tracker, https://github.com/conservationtechlab/animl-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `animl-1.1.0/setup.cfg` & `animl-1.1.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = animl
-version = 1.1.0
+version = 1.1.1
 author = Kyra Swanson
 author_email = tswanson@sdzwa.org
 description = Functions required to classify subjects within camera trap field data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/conservationtechlab/animl-py
 project_urls =
```

### Comparing `animl-1.1.0/src/animl/ZooniverseAPI.py` & `animl-1.1.1/src/animl/ZooniverseAPI.py`

 * *Files identical despite different names*

### Comparing `animl-1.1.0/src/animl/__main__.py` & `animl-1.1.1/src/animl/__main__.py`

 * *Files identical despite different names*

### Comparing `animl-1.1.0/src/animl/detectMD.py` & `animl-1.1.1/src/animl/detectMD.py`

 * *Files identical despite different names*

### Comparing `animl-1.1.0/src/animl/fileManagement.py` & `animl-1.1.1/src/animl/fileManagement.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     files = pd.DataFrame(files, columns=["FilePath"])
     files["FileName"] = files["FilePath"].apply(
         lambda x: os.path.split(x)[1])
     files["FileModifyDate"] = files["FilePath"].apply(
         lambda x: datetime.fromtimestamp(
             os.path.getmtime(x)).strftime('%Y-%m-%d %H:%M:%S'))
 
-    if(outfile):
+    if(out_file):
         save_data(files, out_file)
 
     return files
 
 
 # Set Working Directory and Save File Global Variables
 #
```

### Comparing `animl-1.1.0/src/animl/imageCropGenerator.py` & `animl-1.1.1/src/animl/imageCropGenerator.py`

 * *Files identical despite different names*

### Comparing `animl-1.1.0/src/animl/imageUtils.py` & `animl-1.1.1/src/animl/imageUtils.py`

 * *Files identical despite different names*

### Comparing `animl-1.1.0/src/animl/loadMD.py` & `animl-1.1.1/src/animl/loadMD.py`

 * *Files identical despite different names*

### Comparing `animl-1.1.0/src/animl/parseResults.py` & `animl-1.1.1/src/animl/parseResults.py`

 * *Files identical despite different names*

### Comparing `animl-1.1.0/src/animl/predictSpecies.py` & `animl-1.1.1/src/animl/predictSpecies.py`

 * *Files identical despite different names*

### Comparing `animl-1.1.0/src/animl/splitData.py` & `animl-1.1.1/src/animl/splitData.py`

 * *Files identical despite different names*

### Comparing `animl-1.1.0/src/animl/symlink.py` & `animl-1.1.1/src/animl/symlink.py`

 * *Files identical despite different names*

### Comparing `animl-1.1.0/src/animl/test.py` & `animl-1.1.1/src/animl/test.py`

 * *Files identical despite different names*

### Comparing `animl-1.1.0/src/animl/videoProcessing.py` & `animl-1.1.1/src/animl/videoProcessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,37 +97,38 @@
     images = files[files["FileName"].apply(
         lambda x: os.path.splitext(x)[1].lower()).isin([".jpg",".jpeg",".png"])]
     images = images.assign(Frame = images["FilePath"])
     
     videos =  files[files["FileName"].apply(
         lambda x: os.path.splitext(x)[1].lower()).isin([".mp4", ".avi", ".mov", ".wmv",
                                                         ".mpg", ".mpeg", ".asf", ".m4v"])]
+    if not videos.empty:
+        if parallel:
+            pool = mp.Pool(workers)
 
-    if parallel:
-        pool = mp.Pool(workers)
+            video_frames = vstack([pool.apply(extractImages, 
+                                               args=(video, out_dir, fps, frames)) for 
+                                               video in videos["FilePath"]])
+
+            video_frames = pd.DataFrame(video_frames, columns = ["Frame","FilePath"])
+
+            pool.close()
+
+        else:
+            video_frames = []
+            for i, video in videos.iterrows():
+                video_frames += extractImages(video["FilePath"],out_dir=out_dir, 
+                                         fps=fps, frames=frames)
+
+                if (i % checkpoint == 0) and (outfile is not None):
+                    fileManagement.save_data(images,outfile)
+
+            video_frames = pd.DataFrame(video_frames, columns = ["Frame","FilePath"])
+
+        videos = videos.merge(video_frames, on="FilePath")
 
-        video_frames = vstack([pool.apply(extractImages, 
-                                   args=(video, out_dir, fps, frames)) for video in videos["FilePath"]])
-        
-        video_frames = pd.DataFrame(video_frames, columns = ["Frame","FilePath"])
-
-        pool.close()
-
-    else:
-        video_frames = []
-        for i, video in videos.iterrows():
-            video_frames += extractImages(video["FilePath"],out_dir=out_dir, 
-                                     fps=fps, frames=frames)
-            
-            if (i % checkpoint == 0) and (outfile is not None):
-                fileManagement.save_data(images,outfile)
-        
-        video_frames = pd.DataFrame(video_frames, columns = ["Frame","FilePath"])
-               
-    videos = videos.merge(video_frames, on="FilePath")
-     
     allframes = pd.concat([images,videos])
-    
+
     if (out_file is not None):
         fileManagement.save_data(allframes,out_file) 
-            
+
     return allframes
```

### Comparing `animl-1.1.0/src/animl.egg-info/PKG-INFO` & `animl-1.1.1/src/animl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animl
-Version: 1.1.0
+Version: 1.1.1
 Summary: Functions required to classify subjects within camera trap field data.
 Home-page: https://github.com/conservationtechlab/animl-py
 Author: Kyra Swanson
 Author-email: tswanson@sdzwa.org
 Project-URL: Bug Tracker, https://github.com/conservationtechlab/animl-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `animl-1.1.0/src/animl.egg-info/SOURCES.txt` & `animl-1.1.1/src/animl.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/animl/ZooniverseAPI.py
 src/animl/__init__.py
 src/animl/__main__.py
+src/animl/demoTools.py
 src/animl/detectMD.py
 src/animl/fileManagement.py
 src/animl/imageCropGenerator.py
 src/animl/imageUtils.py
 src/animl/loadMD.py
 src/animl/parseResults.py
+src/animl/plotBoxes.py
 src/animl/predictSpecies.py
 src/animl/setupDirectory.py
 src/animl/splitData.py
 src/animl/symlink.py
 src/animl/test.py
 src/animl/videoProcessing.py
 src/animl.egg-info/PKG-INFO
```

