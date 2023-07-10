# Comparing `tmp/rainbow_imager_readfile-1.2.1.tar.gz` & `tmp/rainbow_imager_readfile-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rainbow_imager_readfile-1.2.1.tar", max compression
+gzip compressed data, was "rainbow_imager_readfile-1.2.2.tar", max compression
```

## Comparing `rainbow_imager_readfile-1.2.1.tar` & `rainbow_imager_readfile-1.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2021-06-16 15:28:11.000000 rainbow_imager_readfile-1.2.1/LICENSE
--rw-r--r--   0        0        0     2672 2023-05-31 17:20:46.890601 rainbow_imager_readfile-1.2.1/README.md
--rw-r--r--   0        0        0      671 2023-06-01 19:22:22.656891 rainbow_imager_readfile-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-01 19:22:22.692892 rainbow_imager_readfile-1.2.1/rainbow_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8719 2023-06-01 19:23:49.079671 rainbow_imager_readfile-1.2.1/rainbow_imager_readfile/_rainbow.py
--rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 rainbow_imager_readfile-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2021-06-16 15:28:11.000000 rainbow_imager_readfile-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2937 2023-06-01 19:33:18.624382 rainbow_imager_readfile-1.2.2/README.md
+-rw-r--r--   0        0        0      671 2023-07-10 00:17:26.757686 rainbow_imager_readfile-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-07-10 00:17:26.802686 rainbow_imager_readfile-1.2.2/rainbow_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8743 2023-07-10 00:17:45.211053 rainbow_imager_readfile-1.2.2/rainbow_imager_readfile/_rainbow.py
+-rw-r--r--   0        0        0     3648 1970-01-01 00:00:00.000000 rainbow_imager_readfile-1.2.2/PKG-INFO
```

### Comparing `rainbow_imager_readfile-1.2.1/LICENSE` & `rainbow_imager_readfile-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rainbow_imager_readfile-1.2.1/README.md` & `rainbow_imager_readfile-1.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -49,14 +49,22 @@
 
 ```python
 >>> import rainbow_imager_readfile, glob
 >>> file_list = glob.glob("path/to/files/2015/01/01/fsmi_rainbow-11/ut06/*full.pgm*")
 >>> img, meta, problematic_files = rainbow_imager_readfile.read(file_list, workers=4)
 ```
 
+### Read with no output
+
+```python
+>>> import rainbow_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2015/01/01/fsmi_rainbow-11/ut06/*full.pgm*")
+>>> img, meta, problematic_files = rainbow_imager_readfile.read(file_list, workers=4, quiet=True)
+```
+
 ## Development
 
 Clone the repository and install dependencies using Poetry.
 
 ```console
 $ git clone https://github.com/ucalgary-aurora/rainbow-imager-readfile.git
 $ cd rainbow-imager-readfile/python
```

### Comparing `rainbow_imager_readfile-1.2.1/pyproject.toml` & `rainbow_imager_readfile-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rainbow-imager-readfile"
-version = "1.2.1"
+version = "1.2.2"
 description = "Read functions for Rainbow ASI PNM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/rainbow-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/rainbow-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `rainbow_imager_readfile-1.2.1/rainbow_imager_readfile/_rainbow.py` & `rainbow_imager_readfile-1.2.2/rainbow_imager_readfile/_rainbow.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         try:
             data = pool.map(partial(__rainbow_readfile_worker, quiet=quiet), file_list)
         except KeyboardInterrupt:
             pool.terminate()  # gracefully kill children
             return np.empty((0, 0, 0), dtype=RAINBOW_DT), [], []
         else:
             pool.close()
+            pool.join()
     else:
         # don't bother using multiprocessing with one worker, just call the worker function directly
         data = []
         for f in file_list:
             data.append(__rainbow_readfile_worker(f, quiet=quiet))
 
     # reorganize data
```

### Comparing `rainbow_imager_readfile-1.2.1/PKG-INFO` & `rainbow_imager_readfile-1.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rainbow-imager-readfile
-Version: 1.2.1
+Version: 1.2.2
 Summary: Read functions for Rainbow ASI PNM raw files
 Home-page: https://github.com/ucalgary-aurora/rainbow-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -67,14 +67,22 @@
 
 ```python
 >>> import rainbow_imager_readfile, glob
 >>> file_list = glob.glob("path/to/files/2015/01/01/fsmi_rainbow-11/ut06/*full.pgm*")
 >>> img, meta, problematic_files = rainbow_imager_readfile.read(file_list, workers=4)
 ```
 
+### Read with no output
+
+```python
+>>> import rainbow_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2015/01/01/fsmi_rainbow-11/ut06/*full.pgm*")
+>>> img, meta, problematic_files = rainbow_imager_readfile.read(file_list, workers=4, quiet=True)
+```
+
 ## Development
 
 Clone the repository and install dependencies using Poetry.
 
 ```console
 $ git clone https://github.com/ucalgary-aurora/rainbow-imager-readfile.git
 $ cd rainbow-imager-readfile/python
```

