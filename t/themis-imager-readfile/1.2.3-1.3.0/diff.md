# Comparing `tmp/themis_imager_readfile-1.2.3.tar.gz` & `tmp/themis_imager_readfile-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themis_imager_readfile-1.2.3.tar", max compression
+gzip compressed data, was "themis_imager_readfile-1.3.0.tar", max compression
```

## Comparing `themis_imager_readfile-1.2.3.tar` & `themis_imager_readfile-1.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.2.3/LICENSE
--rw-r--r--   0        0        0     3024 2023-06-01 19:32:23.797257 themis_imager_readfile-1.2.3/README.md
--rw-r--r--   0        0        0      666 2023-07-08 17:01:00.200056 themis_imager_readfile-1.2.3/pyproject.toml
--rw-r--r--   0        0        0       49 2023-07-08 17:01:00.227056 themis_imager_readfile-1.2.3/themis_imager_readfile/__init__.py
--rw-r--r--   0        0        0     9432 2023-07-08 17:01:12.764308 themis_imager_readfile-1.2.3/themis_imager_readfile/_themis.py
--rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 themis_imager_readfile-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3748 2023-07-10 02:15:56.234126 themis_imager_readfile-1.3.0/README.md
+-rw-r--r--   0        0        0      684 2023-07-10 01:25:50.386077 themis_imager_readfile-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-07-10 01:25:50.482078 themis_imager_readfile-1.3.0/themis_imager_readfile/__init__.py
+-rw-r--r--   0        0        0    10605 2023-07-10 02:00:34.699684 themis_imager_readfile-1.3.0/themis_imager_readfile/_themis.py
+-rw-r--r--   0        0        0     4455 1970-01-01 00:00:00.000000 themis_imager_readfile-1.3.0/PKG-INFO
```

### Comparing `themis_imager_readfile-1.2.3/LICENSE` & `themis_imager_readfile-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `themis_imager_readfile-1.2.3/README.md` & `themis_imager_readfile-1.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -27,16 +27,14 @@
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
 
 Import the library using `import themis_imager_readfile`
 
-**Warning**: On Windows, be sure to put any `read` calls into a `main()` method. This is because we utilize the multiprocessing library and the method of forking processes in Windows requires it. Note that if you're using Jupyter or other IPython-based interfaces, this is not required.
-
 ### Read a single file
 
 ```python
 >>> import themis_imager_readfile
 >>> filename = "path/to/data/2020/01/01/atha_themis02/ut06/20200101_0600_atha_themis02_full.pgm.gz"
 >>> img, meta, problematic_files = themis_imager_readfile.read(filename)
 ```
@@ -61,14 +59,45 @@
 
 ```python
 >>> import themis_imager_readfile, glob
 >>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")
 >>> img, meta, problematic_files = themis_imager_readfile.read(file_list, workers=4, quiet=True)
 ```
 
+### Read only the first frame of each file
+
+```python
+>>> import themis_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")
+>>> img, meta, problematic_files = themis_imager_readfile.read(file_list, first_frame=True)
+```
+
+### Exclude reading the metadata
+
+```python
+>>> import themis_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")
+>>> img, meta, problematic_files = themis_imager_readfile.read(file_list, no_metadata=True)
+```
+
+## Multiprocessing Notes
+
+If you receive error messages about multiprocessing, be sure that your code is wrapped in a `main()` method. This usually resolves the issue. One example implementation is:
+
+```python
+import themis_imager_readfile
+
+def main():
+    filename = "path/to/data/2020/01/01/atha_themis02/ut06/20200101_0600_atha_themis02_full.pgm.gz"
+    img, meta, problematic_files = themis_imager_readfile.read(filename)
+
+if (__name__ == "__main__"):
+    main()
+```
+
 ## Development
 
 Clone the repository and install dependencies using Poetry.
 
 ```console
 $ git clone https://github.com/ucalgary-aurora/themis-imager-readfile.git
 $ cd themis-imager-readfile/python
```

### Comparing `themis_imager_readfile-1.2.3/pyproject.toml` & `themis_imager_readfile-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "themis-imager-readfile"
-version = "1.2.3"
+version = "1.3.0"
 description = "Read functions for THEMIS ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
@@ -15,11 +15,12 @@
 python = "^3.8.1"
 numpy = "^1.21.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
 flake8 = "^6.0.0"
 pylint = "^2.16.0"
+psutil = "^5.9.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `themis_imager_readfile-1.2.3/themis_imager_readfile/_themis.py` & `themis_imager_readfile-1.3.0/themis_imager_readfile/_themis.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,22 +8,27 @@
 # globals
 THEMIS_IMAGE_SIZE_BYTES = 131072
 THEMIS_DT = np.dtype("uint16")
 THEMIS_DT = THEMIS_DT.newbyteorder('>')  # force big endian byte ordering
 THEMIS_EXPECTED_MINUTE_NUM_FRAMES = 20
 
 
-def read(file_list, workers=1, quiet=False):
+def read(file_list, workers=1, first_frame=False, no_metadata=False, quiet=False):
     """
     Read in a single PGM file or set of PGM files
 
     :param file_list: filename or list of filenames
     :type file_list: str
     :param workers: number of worker processes to spawn, defaults to 1
     :type workers: int, optional
+    :param first_frame: only read the first frame for each file, defaults to False
+    :type first_frame: bool, optional
+    :param no_metadata: exclude reading of metadata (performance optimization if
+                        the metadata is not needed), defaults to False
+    :type no_metadata: bool, optional
     :param quiet: reduce output while reading data
     :type quiet: bool, optional
 
     :return: images, metadata dictionaries, and problematic files
     :rtype: numpy.ndarray, list[dict], list[dict]
     """
     # if input is just a single file name in a string, convert to a list to be fed to the workers
@@ -42,26 +47,33 @@
             # of signals in this way, proceed without it
             pool = Pool(processes=workers)
 
         # call readfile function, run each iteration with a single input file from file_list
         # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
         data = []
         try:
-            data = pool.map(partial(__themis_readfile_worker, quiet=quiet), file_list)
+            data = pool.map(partial(__themis_readfile_worker,
+                                    first_frame=first_frame,
+                                    no_metadata=no_metadata,
+                                    quiet=quiet),
+                            file_list)
         except KeyboardInterrupt:
             pool.terminate()  # gracefully kill children
             return np.empty((0, 0, 0), dtype=THEMIS_DT), [], []
         else:
             pool.close()
             pool.join()
     else:
         # don't bother using multiprocessing with one worker, just call the worker function directly
         data = []
         for f in file_list:
-            data.append(__themis_readfile_worker(f, quiet=quiet))
+            data.append(__themis_readfile_worker(f,
+                                                 first_frame=first_frame,
+                                                 no_metadata=no_metadata,
+                                                 quiet=quiet))
 
     # derive number of frames to prepare for
     total_num_frames = 0
     for i in range(0, len(data)):
         if (data[i][2] is True):
             continue
         total_num_frames += data[i][0].shape[2]
@@ -103,19 +115,19 @@
     images = images.astype(np.uint16)
 
     # return
     data = None
     return images, metadata_dict_list, problematic_file_list
 
 
-def __themis_readfile_worker(file, quiet=False):
+def __themis_readfile_worker(file, first_frame=False, no_metadata=False, quiet=False):
     # init
     images = np.array([])
     metadata_dict_list = []
-    first_frame = True
+    is_first = True
     metadata_dict = {}
     site_uid = ""
     device_uid = ""
     problematic = False
     error_message = ""
 
     # check file extension to see if it's gzipped or not
@@ -137,14 +149,18 @@
             print("Failed to open file '%s' " % (file))
         problematic = True
         error_message = "failed to open file: %s" % (str(e))
         return images, metadata_dict_list, problematic, file, error_message
 
     # read the file
     while True:
+        # break out depending on first_frame param
+        if (first_frame is True and is_first is False):
+            break
+
         # read a line
         try:
             line = unzipped.readline()
         except Exception as e:
             if (quiet is False):
                 print("Error reading before image data in file '%s'" % (file))
             problematic = True
@@ -159,50 +175,54 @@
 
         # magic number; this is not a metadata or image line, exclude
         if (line.startswith(b'P5\n')):
             continue
 
         # process line
         if (line.startswith(b'#"')):
-            # metadata lines start with #"<key>"
-            try:
-                line_decoded = line.decode("ascii")
-            except Exception as e:
-                # skip metadata line if it can't be decoded, likely corrupt file but don't mark it as one yet
-                if (quiet is False):
-                    print("Warning: issue decoding metadata line: %s (line='%s', file='%s')" % (str(e), line, file))
-                continue
-
-            # split the key and value out of the metadata line
-            line_decoded_split = line_decoded.split('"')
-            if (len(line_decoded_split) != 3):
-                if (quiet is False):
-                    print("Warning: issue splitting metadata line (line='%s', file='%s')" % (line_decoded, file))
-                continue
-            key = line_decoded_split[1]
-            value = line_decoded_split[2].strip()
-
-            # add entry to dictionary
-            metadata_dict[key] = value
-
-            # set the site/device uids, or inject the site and device UIDs if they are missing
-            if ("Site unique ID" not in metadata_dict):
-                metadata_dict["Site unique ID"] = site_uid
-            else:
-                site_uid = metadata_dict["Site unique ID"]
-            if ("Imager unique ID" not in metadata_dict):
-                metadata_dict["Imager unique ID"] = device_uid
-            else:
-                device_uid = metadata_dict["Imager unique ID"]
-
-            # split dictionaries up per frame, exposure plus initial readout is
-            # always the end of metadata for frame
-            if (key.startswith("Exposure plus initial readout") or key.startswith("Exposure duration plus readout")):
-                metadata_dict_list.append(metadata_dict)
+            if (no_metadata is True):
                 metadata_dict = {}
+                metadata_dict_list.append(metadata_dict)
+            else:
+                # metadata lines start with #"<key>"
+                try:
+                    line_decoded = line.decode("ascii")
+                except Exception as e:
+                    # skip metadata line if it can't be decoded, likely corrupt file but don't mark it as one yet
+                    if (quiet is False):
+                        print("Warning: issue decoding metadata line: %s (line='%s', file='%s')" % (str(e), line, file))
+                    continue
+
+                # split the key and value out of the metadata line
+                line_decoded_split = line_decoded.split('"')
+                if (len(line_decoded_split) != 3):
+                    if (quiet is False):
+                        print("Warning: issue splitting metadata line (line='%s', file='%s')" % (line_decoded, file))
+                    continue
+                key = line_decoded_split[1]
+                value = line_decoded_split[2].strip()
+
+                # add entry to dictionary
+                metadata_dict[key] = value
+
+                # set the site/device uids, or inject the site and device UIDs if they are missing
+                if ("Site unique ID" not in metadata_dict):
+                    metadata_dict["Site unique ID"] = site_uid
+                else:
+                    site_uid = metadata_dict["Site unique ID"]
+                if ("Imager unique ID" not in metadata_dict):
+                    metadata_dict["Imager unique ID"] = device_uid
+                else:
+                    device_uid = metadata_dict["Imager unique ID"]
+
+                # split dictionaries up per frame, exposure plus initial readout is
+                # always the end of metadata for frame
+                if (key.startswith("Exposure plus initial readout") or key.startswith("Exposure duration plus readout")):
+                    metadata_dict_list.append(metadata_dict)
+                    metadata_dict = {}
         elif line == b'65535\n':
             # there are 2 lines between "exposure plus read out" and the image
             # data, the first is b'256 256\n' and the second is b'65535\n'
             #
             # read image
             try:
                 # read the image size in bytes from the file
@@ -219,17 +239,17 @@
                     print("Failed reading image data frame: %s" % (str(e)))
                 metadata_dict_list.pop()  # remove corresponding metadata entry
                 problematic = True
                 error_message = "image data read failure: %s" % (str(e))
                 continue  # skip to next frame
 
             # initialize image stack
-            if first_frame:
+            if (is_first is True):
                 images = image_matrix
-                first_frame = False
+                is_first = False
             else:
                 images = np.dstack([images, image_matrix])  # depth stack images (on 3rd axis)
 
     # close gzip file
     unzipped.close()
 
     # check to see if the image is empty
```

### Comparing `themis_imager_readfile-1.2.3/PKG-INFO` & `themis_imager_readfile-1.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themis-imager-readfile
-Version: 1.2.3
+Version: 1.3.0
 Summary: Read functions for THEMIS ASI PGM raw files
 Home-page: https://github.com/ucalgary-aurora/themis-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -45,16 +45,14 @@
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
 
 Import the library using `import themis_imager_readfile`
 
-**Warning**: On Windows, be sure to put any `read` calls into a `main()` method. This is because we utilize the multiprocessing library and the method of forking processes in Windows requires it. Note that if you're using Jupyter or other IPython-based interfaces, this is not required.
-
 ### Read a single file
 
 ```python
 >>> import themis_imager_readfile
 >>> filename = "path/to/data/2020/01/01/atha_themis02/ut06/20200101_0600_atha_themis02_full.pgm.gz"
 >>> img, meta, problematic_files = themis_imager_readfile.read(filename)
 ```
@@ -79,14 +77,45 @@
 
 ```python
 >>> import themis_imager_readfile, glob
 >>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")
 >>> img, meta, problematic_files = themis_imager_readfile.read(file_list, workers=4, quiet=True)
 ```
 
+### Read only the first frame of each file
+
+```python
+>>> import themis_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")
+>>> img, meta, problematic_files = themis_imager_readfile.read(file_list, first_frame=True)
+```
+
+### Exclude reading the metadata
+
+```python
+>>> import themis_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")
+>>> img, meta, problematic_files = themis_imager_readfile.read(file_list, no_metadata=True)
+```
+
+## Multiprocessing Notes
+
+If you receive error messages about multiprocessing, be sure that your code is wrapped in a `main()` method. This usually resolves the issue. One example implementation is:
+
+```python
+import themis_imager_readfile
+
+def main():
+    filename = "path/to/data/2020/01/01/atha_themis02/ut06/20200101_0600_atha_themis02_full.pgm.gz"
+    img, meta, problematic_files = themis_imager_readfile.read(filename)
+
+if (__name__ == "__main__"):
+    main()
+```
+
 ## Development
 
 Clone the repository and install dependencies using Poetry.
 
 ```console
 $ git clone https://github.com/ucalgary-aurora/themis-imager-readfile.git
 $ cd themis-imager-readfile/python
```

