# Comparing `tmp/trex_imager_readfile-1.4.3.tar.gz` & `tmp/trex_imager_readfile-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex_imager_readfile-1.4.3.tar", max compression
+gzip compressed data, was "trex_imager_readfile-1.4.4.tar", max compression
```

## Comparing `trex_imager_readfile-1.4.3.tar` & `trex_imager_readfile-1.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      186 2023-04-25 13:48:57.783144 trex_imager_readfile-1.4.3/README.md
--rw-r--r--   0        0        0      699 2023-06-29 20:11:26.057359 trex_imager_readfile-1.4.3/pyproject.toml
--rw-r--r--   0        0        0      397 2023-06-29 20:11:26.104359 trex_imager_readfile-1.4.3/trex_imager_readfile/__init__.py
--rw-r--r--   0        0        0     9073 2023-06-01 18:59:35.187783 trex_imager_readfile-1.4.3/trex_imager_readfile/blueline.py
--rw-r--r--   0        0        0     9018 2023-06-01 19:04:02.929246 trex_imager_readfile-1.4.3/trex_imager_readfile/nir.py
--rw-r--r--   0        0        0    20553 2023-06-29 20:10:53.755392 trex_imager_readfile-1.4.3/trex_imager_readfile/rgb.py
--rw-r--r--   0        0        0     9121 2023-06-01 18:59:34.177762 trex_imager_readfile-1.4.3/trex_imager_readfile/spectrograph.py
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 trex_imager_readfile-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-04-25 13:48:57.783144 trex_imager_readfile-1.4.4/README.md
+-rw-r--r--   0        0        0      699 2023-07-10 00:22:44.601009 trex_imager_readfile-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0      397 2023-07-10 00:22:44.642010 trex_imager_readfile-1.4.4/trex_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     9097 2023-07-10 00:20:55.065830 trex_imager_readfile-1.4.4/trex_imager_readfile/blueline.py
+-rw-r--r--   0        0        0     9042 2023-07-10 00:20:42.442579 trex_imager_readfile-1.4.4/trex_imager_readfile/nir.py
+-rw-r--r--   0        0        0    20577 2023-07-10 00:22:26.795655 trex_imager_readfile-1.4.4/trex_imager_readfile/rgb.py
+-rw-r--r--   0        0        0     9145 2023-07-10 00:20:26.845268 trex_imager_readfile-1.4.4/trex_imager_readfile/spectrograph.py
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 trex_imager_readfile-1.4.4/PKG-INFO
```

### Comparing `trex_imager_readfile-1.4.3/pyproject.toml` & `trex_imager_readfile-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trex-imager-readfile"
-version = "1.4.3"
+version = "1.4.4"
 description = "Read functions for TREx ASI raw image files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/trex-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/trex-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `trex_imager_readfile-1.4.3/trex_imager_readfile/blueline.py` & `trex_imager_readfile-1.4.4/trex_imager_readfile/blueline.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,15 @@
         try:
             data = pool.map(partial(__blueline_readfile_worker, quiet=quiet), file_list)
         except KeyboardInterrupt:
             pool.terminate()  # gracefully kill children
             return np.empty((0, 0, 0), dtype=__BLUELINE_DT), [], []
         else:
             pool.close()
+            pool.join()
     else:
         # don't bother using multiprocessing with one worker, just call the worker function directly
         data = []
         for f in file_list:
             data.append(__blueline_readfile_worker(f, quiet=quiet))
 
     # reorganize data
```

### Comparing `trex_imager_readfile-1.4.3/trex_imager_readfile/nir.py` & `trex_imager_readfile-1.4.4/trex_imager_readfile/nir.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,15 @@
         try:
             data = pool.map(partial(__nir_readfile_worker, quiet=quiet), file_list)
         except KeyboardInterrupt:
             pool.terminate()  # gracefully kill children
             return np.empty((0, 0, 0), dtype=__NIR_DT), [], []
         else:
             pool.close()
+            pool.join()
     else:
         # don't bother using multiprocessing with one worker, just call the worker function directly
         data = []
         for f in file_list:
             data.append(__nir_readfile_worker(f, quiet=quiet))
 
     # reorganize data
```

### Comparing `trex_imager_readfile-1.4.3/trex_imager_readfile/rgb.py` & `trex_imager_readfile-1.4.4/trex_imager_readfile/rgb.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,14 +468,15 @@
         try:
             pool_data = pool.map(__trex_readfile_worker, processing_list)
         except KeyboardInterrupt:
             pool.terminate()  # gracefully kill children
             return np.empty((0, 0, 0)), [], []
         else:
             pool.close()
+            pool.join()
     else:
         # don't bother using multiprocessing with one worker, just call the worker function directly
         pool_data = []
         for p in processing_list:
             pool_data.append(__trex_readfile_worker(p))
 
     # set sizes
```

### Comparing `trex_imager_readfile-1.4.3/trex_imager_readfile/spectrograph.py` & `trex_imager_readfile-1.4.4/trex_imager_readfile/spectrograph.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,15 @@
         try:
             data = pool.map(partial(__spectrograph_readfile_worker, quiet=quiet), file_list)
         except KeyboardInterrupt:
             pool.terminate()  # gracefully kill children
             return np.empty((0, 0, 0), dtype=__SPECTROGRAPH_DT), [], []
         else:
             pool.close()
+            pool.join()
     else:
         # don't bother using multiprocessing with one worker, just call the worker function directly
         data = []
         for f in file_list:
             data.append(__spectrograph_readfile_worker(f, quiet=quiet))
 
     # reorganize data
```

### Comparing `trex_imager_readfile-1.4.3/PKG-INFO` & `trex_imager_readfile-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trex-imager-readfile
-Version: 1.4.3
+Version: 1.4.4
 Summary: Read functions for TREx ASI raw image files
 Home-page: https://github.com/ucalgary-aurora/trex-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

