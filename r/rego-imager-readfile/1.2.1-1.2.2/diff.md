# Comparing `tmp/rego_imager_readfile-1.2.1.tar.gz` & `tmp/rego_imager_readfile-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rego_imager_readfile-1.2.1.tar", max compression
+gzip compressed data, was "rego_imager_readfile-1.2.2.tar", max compression
```

## Comparing `rego_imager_readfile-1.2.1.tar` & `rego_imager_readfile-1.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2021-02-25 19:14:26.000000 rego_imager_readfile-1.2.1/LICENSE
--rw-r--r--   0        0        0     2688 2023-05-30 20:01:33.986595 rego_imager_readfile-1.2.1/README.md
--rw-r--r--   0        0        0      656 2023-06-01 19:14:18.280872 rego_imager_readfile-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       47 2023-06-01 19:14:18.317873 rego_imager_readfile-1.2.1/rego_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8579 2023-06-01 19:15:57.945935 rego_imager_readfile-1.2.1/rego_imager_readfile/_rego.py
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 rego_imager_readfile-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2021-02-25 19:14:26.000000 rego_imager_readfile-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2945 2023-06-01 19:32:39.647582 rego_imager_readfile-1.2.2/README.md
+-rw-r--r--   0        0        0      656 2023-07-10 00:18:50.441351 rego_imager_readfile-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-07-10 00:18:50.477351 rego_imager_readfile-1.2.2/rego_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8603 2023-07-10 00:19:10.401748 rego_imager_readfile-1.2.2/rego_imager_readfile/_rego.py
+-rw-r--r--   0        0        0     3644 1970-01-01 00:00:00.000000 rego_imager_readfile-1.2.2/PKG-INFO
```

### Comparing `rego_imager_readfile-1.2.1/LICENSE` & `rego_imager_readfile-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rego_imager_readfile-1.2.1/README.md` & `rego_imager_readfile-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,22 @@
 
 ```python
 >>> import rego_imager_readfile, glob
 >>> file_list = glob.glob("path/to/files/2020/01/01/fsmi_rego-654/ut06/*6300.pgm*")
 >>> img, meta, problematic_files = rego_imager_readfile.read(file_list, workers=4)
 ```
 
+### Read with no output
+
+```python
+>>> import rego_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2020/01/01/fsmi_rego-654/ut06/*6300.pgm*")
+>>> img, meta, problematic_files = rego_imager_readfile.read(file_list, workers=4, quiet=True)
+```
+
 ## Development
 
 Clone the repository and install dependencies using Poetry.
 
 ```console
 $ git clone https://github.com/ucalgary-aurora/rego-imager-readfile.git
 $ cd rego-imager-readfile/python
```

### Comparing `rego_imager_readfile-1.2.1/pyproject.toml` & `rego_imager_readfile-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rego-imager-readfile"
-version = "1.2.1"
+version = "1.2.2"
 description = "Read functions for REGO ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/rego-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/rego-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `rego_imager_readfile-1.2.1/rego_imager_readfile/_rego.py` & `rego_imager_readfile-1.2.2/rego_imager_readfile/_rego.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         try:
             data = pool.map(partial(__rego_readfile_worker, quiet=quiet), file_list)
         except KeyboardInterrupt:
             pool.terminate()  # gracefully kill children
             return np.empty((0, 0, 0), dtype=REGO_DT), [], []
         else:
             pool.close()
+            pool.join()
     else:
         # don't bother using multiprocessing with one worker, just call the worker function directly
         data = []
         for f in file_list:
             data.append(__rego_readfile_worker(f, quiet=quiet))
 
     # reorganize data
```

### Comparing `rego_imager_readfile-1.2.1/PKG-INFO` & `rego_imager_readfile-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rego-imager-readfile
-Version: 1.2.1
+Version: 1.2.2
 Summary: Read functions for REGO ASI PGM raw files
 Home-page: https://github.com/ucalgary-aurora/rego-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -71,14 +71,22 @@
 
 ```python
 >>> import rego_imager_readfile, glob
 >>> file_list = glob.glob("path/to/files/2020/01/01/fsmi_rego-654/ut06/*6300.pgm*")
 >>> img, meta, problematic_files = rego_imager_readfile.read(file_list, workers=4)
 ```
 
+### Read with no output
+
+```python
+>>> import rego_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2020/01/01/fsmi_rego-654/ut06/*6300.pgm*")
+>>> img, meta, problematic_files = rego_imager_readfile.read(file_list, workers=4, quiet=True)
+```
+
 ## Development
 
 Clone the repository and install dependencies using Poetry.
 
 ```console
 $ git clone https://github.com/ucalgary-aurora/rego-imager-readfile.git
 $ cd rego-imager-readfile/python
```

