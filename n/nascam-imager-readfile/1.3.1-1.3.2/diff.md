# Comparing `tmp/nascam_imager_readfile-1.3.1.tar.gz` & `tmp/nascam_imager_readfile-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nascam_imager_readfile-1.3.1.tar", max compression
+gzip compressed data, was "nascam_imager_readfile-1.3.2.tar", max compression
```

## Comparing `nascam_imager_readfile-1.3.1.tar` & `nascam_imager_readfile-1.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2022-05-07 17:20:12.000000 nascam_imager_readfile-1.3.1/LICENSE
--rw-r--r--   0        0        0     2801 2023-05-31 17:29:41.564429 nascam_imager_readfile-1.3.1/README.md
--rw-r--r--   0        0        0       49 2023-06-01 19:18:41.798327 nascam_imager_readfile-1.3.1/nascam_imager_readfile/__init__.py
--rw-r--r--   0        0        0     9399 2023-06-01 19:21:15.106500 nascam_imager_readfile-1.3.1/nascam_imager_readfile/_nascam.py
--rw-r--r--   0        0        0      687 2023-06-01 19:18:41.752326 nascam_imager_readfile-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 nascam_imager_readfile-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-05-07 17:20:12.000000 nascam_imager_readfile-1.3.2/LICENSE
+-rw-r--r--   0        0        0     3062 2023-06-01 19:32:49.117776 nascam_imager_readfile-1.3.2/README.md
+-rw-r--r--   0        0        0       49 2023-07-10 00:16:02.327006 nascam_imager_readfile-1.3.2/nascam_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     9423 2023-07-10 00:15:35.943481 nascam_imager_readfile-1.3.2/nascam_imager_readfile/_nascam.py
+-rw-r--r--   0        0        0      687 2023-07-10 00:16:02.288005 nascam_imager_readfile-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3811 1970-01-01 00:00:00.000000 nascam_imager_readfile-1.3.2/PKG-INFO
```

### Comparing `nascam_imager_readfile-1.3.1/LICENSE` & `nascam_imager_readfile-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nascam_imager_readfile-1.3.1/README.md` & `nascam_imager_readfile-1.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,22 @@
 
 ```python
 >>> import nascam_imager_readfile, glob
 >>> file_list = glob.glob("path/to/files/2010/01/01/atha_nascam-iccd04/ut06/*.tar")
 >>> img, meta, problematic_files = nascam_imager_readfile.read(file_list, workers=4)
 ```
 
+### Read with no output
+
+```python
+>>> import nascam_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2010/01/01/atha_nascam-iccd04/ut06/*.tar")
+>>> img, meta, problematic_files = nascam_imager_readfile.read(file_list, workers=4, quiet=True)
+```
+
 ## Development
 
 Clone the repository and install dependencies using Poetry.
 
 ```console
 $ git clone https://github.com/ucalgary-aurora/nascam-imager-readfile.git
 $ cd nascam-imager-readfile/python
```

### Comparing `nascam_imager_readfile-1.3.1/nascam_imager_readfile/_nascam.py` & `nascam_imager_readfile-1.3.2/nascam_imager_readfile/_nascam.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
         try:
             pool_data = pool.map(__nascam_readfile_worker, processing_list)
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
             pool_data.append(__nascam_readfile_worker(p))
 
     # set sizes
```

### Comparing `nascam_imager_readfile-1.3.1/pyproject.toml` & `nascam_imager_readfile-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nascam-imager-readfile"
-version = "1.3.1"
+version = "1.3.2"
 description = "Read functions for NASCAM ASI raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/nascam-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/nascam-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `nascam_imager_readfile-1.3.1/PKG-INFO` & `nascam_imager_readfile-1.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nascam-imager-readfile
-Version: 1.3.1
+Version: 1.3.2
 Summary: Read functions for NASCAM ASI raw files
 Home-page: https://github.com/ucalgary-aurora/nascam-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -72,14 +72,22 @@
 
 ```python
 >>> import nascam_imager_readfile, glob
 >>> file_list = glob.glob("path/to/files/2010/01/01/atha_nascam-iccd04/ut06/*.tar")
 >>> img, meta, problematic_files = nascam_imager_readfile.read(file_list, workers=4)
 ```
 
+### Read with no output
+
+```python
+>>> import nascam_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2010/01/01/atha_nascam-iccd04/ut06/*.tar")
+>>> img, meta, problematic_files = nascam_imager_readfile.read(file_list, workers=4, quiet=True)
+```
+
 ## Development
 
 Clone the repository and install dependencies using Poetry.
 
 ```console
 $ git clone https://github.com/ucalgary-aurora/nascam-imager-readfile.git
 $ cd nascam-imager-readfile/python
```

