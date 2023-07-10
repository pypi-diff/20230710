# Comparing `tmp/cornifer-0.8.tar.gz` & `tmp/cornifer-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornifer-0.8.tar", last modified: Mon Jun 19 23:32:40 2023, max compression
+gzip compressed data, was "cornifer-0.8.1.tar", last modified: Mon Jul 10 18:56:37 2023, max compression
```

## Comparing `cornifer-0.8.tar` & `cornifer-0.8.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-06-19 23:32:40.645084 cornifer-0.8/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    35823 2021-08-18 02:15:58.000000 cornifer-0.8/LICENSE
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      644 2023-06-19 23:32:40.643083 cornifer-0.8/PKG-INFO
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1376 2022-07-25 17:02:05.000000 cornifer-0.8/README.md
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-06-19 23:32:40.183039 cornifer-0.8/lib/
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-06-19 23:32:40.317010 cornifer-0.8/lib/Cornifer.egg-info/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      644 2023-06-19 23:32:40.000000 cornifer-0.8/lib/Cornifer.egg-info/PKG-INFO
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      878 2023-06-19 23:32:40.000000 cornifer-0.8/lib/Cornifer.egg-info/SOURCES.txt
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2023-06-19 23:32:40.000000 cornifer-0.8/lib/Cornifer.egg-info/dependency_links.txt
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2022-07-23 17:35:39.000000 cornifer-0.8/lib/Cornifer.egg-info/not-zip-safe
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       35 2023-06-19 23:32:40.000000 cornifer-0.8/lib/Cornifer.egg-info/requires.txt
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        9 2023-06-19 23:32:40.000000 cornifer-0.8/lib/Cornifer.egg-info/top_level.txt
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-06-19 23:32:40.483511 cornifer-0.8/lib/cornifer/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     4046 2023-06-16 20:01:49.000000 cornifer-0.8/lib/cornifer/__init__.py
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-06-19 23:32:40.571175 cornifer-0.8/lib/cornifer/_utilities/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    10788 2023-06-16 20:18:33.000000 cornifer-0.8/lib/cornifer/_utilities/__init__.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     5859 2023-05-25 21:14:31.000000 cornifer-0.8/lib/cornifer/_utilities/lmdb.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    10402 2023-06-19 23:03:27.000000 cornifer-0.8/lib/cornifer/blocks.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1142 2023-06-14 14:03:06.000000 cornifer-0.8/lib/cornifer/errors.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      943 2023-05-12 15:41:02.000000 cornifer-0.8/lib/cornifer/example.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2407 2023-05-10 16:54:32.000000 cornifer-0.8/lib/cornifer/filemetadata.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    13576 2023-05-30 15:35:39.000000 cornifer-0.8/lib/cornifer/info.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2045 2023-06-01 18:58:48.000000 cornifer-0.8/lib/cornifer/regfilestructure.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   131916 2023-06-19 23:13:06.000000 cornifer-0.8/lib/cornifer/registers.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    12329 2023-05-24 18:24:36.000000 cornifer-0.8/lib/cornifer/regloader.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      730 2023-06-19 23:15:02.000000 cornifer-0.8/lib/cornifer/version.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       38 2023-06-19 23:32:40.645084 cornifer-0.8/setup.cfg
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1897 2022-09-27 16:45:39.000000 cornifer-0.8/setup.py
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-06-19 23:32:40.624397 cornifer-0.8/tests/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     8824 2023-06-19 23:03:26.000000 cornifer-0.8/tests/test_blocks.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    11191 2023-05-12 15:41:02.000000 cornifer-0.8/tests/test_info.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2216 2023-05-26 15:26:43.000000 cornifer-0.8/tests/test_register_file_structure.py
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   146085 2023-06-19 22:47:41.000000 cornifer-0.8/tests/test_registers.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-10 18:56:36.158473 cornifer-0.8.1/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    35823 2021-08-18 02:15:58.000000 cornifer-0.8.1/LICENSE
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      646 2023-07-10 18:56:36.154333 cornifer-0.8.1/PKG-INFO
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1376 2022-07-25 17:02:05.000000 cornifer-0.8.1/README.md
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-10 18:56:35.291565 cornifer-0.8.1/lib/
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-10 18:56:35.509503 cornifer-0.8.1/lib/Cornifer.egg-info/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      646 2023-07-10 18:56:35.000000 cornifer-0.8.1/lib/Cornifer.egg-info/PKG-INFO
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      878 2023-07-10 18:56:35.000000 cornifer-0.8.1/lib/Cornifer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2023-07-10 18:56:35.000000 cornifer-0.8.1/lib/Cornifer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2022-07-23 17:35:39.000000 cornifer-0.8.1/lib/Cornifer.egg-info/not-zip-safe
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       35 2023-07-10 18:56:35.000000 cornifer-0.8.1/lib/Cornifer.egg-info/requires.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        9 2023-07-10 18:56:35.000000 cornifer-0.8.1/lib/Cornifer.egg-info/top_level.txt
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-10 18:56:35.854301 cornifer-0.8.1/lib/cornifer/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     4046 2023-06-16 20:01:49.000000 cornifer-0.8.1/lib/cornifer/__init__.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-10 18:56:36.010056 cornifer-0.8.1/lib/cornifer/_utilities/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    10788 2023-06-16 20:18:33.000000 cornifer-0.8.1/lib/cornifer/_utilities/__init__.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     5859 2023-05-25 21:14:31.000000 cornifer-0.8.1/lib/cornifer/_utilities/lmdb.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    10165 2023-06-23 15:17:52.000000 cornifer-0.8.1/lib/cornifer/blocks.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1142 2023-06-14 14:03:06.000000 cornifer-0.8.1/lib/cornifer/errors.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      943 2023-05-12 15:41:02.000000 cornifer-0.8.1/lib/cornifer/example.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2407 2023-05-10 16:54:32.000000 cornifer-0.8.1/lib/cornifer/filemetadata.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    13532 2023-06-20 03:54:35.000000 cornifer-0.8.1/lib/cornifer/info.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2043 2023-06-20 03:56:43.000000 cornifer-0.8.1/lib/cornifer/regfilestructure.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   137380 2023-07-10 18:28:43.000000 cornifer-0.8.1/lib/cornifer/registers.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    12329 2023-05-24 18:24:36.000000 cornifer-0.8.1/lib/cornifer/regloader.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      741 2023-07-10 18:36:04.000000 cornifer-0.8.1/lib/cornifer/version.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       38 2023-07-10 18:56:36.160200 cornifer-0.8.1/setup.cfg
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1897 2022-09-27 16:45:39.000000 cornifer-0.8.1/setup.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-10 18:56:36.116927 cornifer-0.8.1/tests/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     8824 2023-06-19 23:03:26.000000 cornifer-0.8.1/tests/test_blocks.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    11191 2023-05-12 15:41:02.000000 cornifer-0.8.1/tests/test_info.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2216 2023-05-26 15:26:43.000000 cornifer-0.8.1/tests/test_register_file_structure.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   146065 2023-07-10 18:34:11.000000 cornifer-0.8.1/tests/test_registers.py
```

### Comparing `cornifer-0.8/LICENSE` & `cornifer-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/PKG-INFO` & `cornifer-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornifer
-Version: 0.8
+Version: 0.8.1
 Summary: An easy-to-use data manager for experimental mathematics.
 Home-page: https://github.com/automorphis/cornifer
 Author: Michael P. Lane
 Author-email: mlanetheta@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `cornifer-0.8/README.md` & `cornifer-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/lib/Cornifer.egg-info/PKG-INFO` & `cornifer-0.8.1/lib/Cornifer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornifer
-Version: 0.8
+Version: 0.8.1
 Summary: An easy-to-use data manager for experimental mathematics.
 Home-page: https://github.com/automorphis/cornifer
 Author: Michael P. Lane
 Author-email: mlanetheta@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `cornifer-0.8/lib/Cornifer.egg-info/SOURCES.txt` & `cornifer-0.8.1/lib/Cornifer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/lib/cornifer/__init__.py` & `cornifer-0.8.1/lib/cornifer/__init__.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/lib/cornifer/_utilities/__init__.py` & `cornifer-0.8.1/lib/cornifer/_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/lib/cornifer/_utilities/lmdb.py` & `cornifer-0.8.1/lib/cornifer/_utilities/lmdb.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/lib/cornifer/blocks.py` & `cornifer-0.8.1/lib/cornifer/blocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 """
 
 import warnings
 from abc import ABC, abstractmethod
-from contextlib import contextmanager, ExitStack, AbstractContextManager
 
 import numpy as np
 
 from .errors import BlockNotOpenError
 from .info import ApriInfo
 from ._utilities import check_has_method, justify_slice, is_int, check_type, check_return_int
 
@@ -176,23 +175,23 @@
             raise NotImplementedError("Support for slices coming soon.")
 
         key = check_return_int(key, "key")
 
         if isinstance(key, tuple):
             raise IndexError("`blk[]` cannot take more than one index.")
 
-        key -= self.startn()
-
         if key not in self:
             raise IndexError(
                 f"Indices must be between {self.startn()} and {self.startn() + len(self) - 1}" +
                 ", inclusive."
             )
 
-        if not check_has_method(self._seg, "__setitem__"):
+        key -= self.startn()
+
+        if check_has_method(self._seg, "__setitem__"):
             self._seg[key, ...] = value
 
         else:
             raise NotImplementedError
 
     def __len__(self):
 
@@ -299,17 +298,15 @@
             - One or more references to the data that `_seg` point(ed) to remain after this method returns.
 
         Consider the following snippet:
 
             a = np.memmap(...)           # 1 reference  (a)
             blk1 = MemmapBlock(a, apri)  # 2 referneces (a, blk1._seg)
             with blk1:
-                with blk1[1:] as blk2:   # 3 references (a, blk1._seg, blk2._seg)
-                    ...
-                ...                      # 2 references (a, blk1._seg)
+                ...
             ...                          # 1 reference  (a)
 
         Indeed, the reference to the `a` memmap will remain until the user manually deletes the reference via
         `del a`.
         """
 
         try:
```

### Comparing `cornifer-0.8/lib/cornifer/errors.py` & `cornifer-0.8.1/lib/cornifer/errors.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/lib/cornifer/example.py` & `cornifer-0.8.1/lib/cornifer/example.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/lib/cornifer/filemetadata.py` & `cornifer-0.8.1/lib/cornifer/filemetadata.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/lib/cornifer/info.py` & `cornifer-0.8.1/lib/cornifer/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,19 +108,15 @@
             return tuple([self.object_hook(item) for item in obj])
 
         else:
             return obj
 
     def decode_root(self, obj):
 
-        try:
-            decoded_json = self.decode(obj)
-
-        except:
-            raise
+        decoded_json = self.decode(obj)
 
         if not isinstance(decoded_json, dict):
             raise ValueError(
                 "The outermost layer of the passed JSON string must be a JavaScript `object`, that is, " +
                 f"a Python `dict`. The outermost layer of the passed `json_string` is: " +
                 f"`{decoded_json.__class__.__name__}`."
             )
@@ -441,20 +437,20 @@
         self._memoize_json = True
 
         for key,val in kwargs.items():
 
             try:
                 hash_ += hash(val)
 
-            except (TypeError, AttributeError):
+            except (TypeError, AttributeError) as e:
 
                 raise ValueError(
                     f"All keyword arguments must be hashable types. The keyword argument given by \"{key}\" "+
                     f"not a hashable type. The type of that argument is `{val.__class__.__name__}`."
-                )
+                ) from e
 
             if self._memoize_json and isinstance(val, _Info):
                 self._memoize_json = False
 
         self._hash = hash_
 
     def __hash__(self):
```

### Comparing `cornifer-0.8/lib/cornifer/regfilestructure.py` & `cornifer-0.8.1/lib/cornifer/regfilestructure.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
 
     for path in [DATABASE_FILEPATH]:
         if not (local_dir / path).is_dir():
             problems.append(str(local_dir / path))
 
     if len(problems) > 0:
         raise FileNotFoundError(
-            "Could not find the following files or directories: " +
+            "Could not find the following files or directories: "
             ", ".join(problems)
         )
```

### Comparing `cornifer-0.8/lib/cornifer/registers.py` & `cornifer-0.8.1/lib/cornifer/registers.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import pickle
 import shutil
 import warnings
 import zipfile
 from contextlib import contextmanager, ExitStack
 from pathlib import Path
 from abc import ABC, abstractmethod
+from time import time
 
 import lmdb
 import numpy as np
 
 from .errors import DataNotFoundError, RegisterAlreadyOpenError, RegisterError, CompressionError, \
     DecompressionError, NOT_ABSOLUTE_ERROR_MESSAGE, RegisterRecoveryError, BlockNotOpenError
 from .info import ApriInfo, AposInfo, _InfoJsonEncoder, _InfoJsonDecoder, _Info
@@ -70,49 +71,23 @@
 _IS_NOT_COMPRESSED_VAL     = b""
 
 _SUB_VAL                   = b""
 
 #################################
 #        ERROR MESSAGES         #
 
-def _blk_not_found_err_msg(diskonly, apri, n = None, startn = None, length = None):
-
-    if (startn is not None or length is not None) and n is not None:
-        raise ValueError
-
-    if startn is None and length is not None:
-        raise ValueError
-
-    if diskonly:
-        type_ = "disk"
-
-    else:
-        type_ = "disk nor RAM"
-
-    if n is not None:
-        return f"No {type_} `Block` found with the following data: {str(apri)}, n = {n}."
-
-    elif startn is not None and length is None:
-        return f"No {type_} `Block` found with the following data: {str(apri)}, startn = {startn}."
-
-    elif startn is not None and length is not None:
-        return f"No {type_} `Block` found with the following data: {str(apri)}, startn = {startn}, length = {length}."
-
-    else:
-        return f"No {type_} `Block` found with the following data: {str(apri)}."
-
 _NOT_CREATED_ERROR_MESSAGE = (
     "The `Register` database has not been created. You must do `with reg.open() as reg:` at least once before " +
     "calling the method `{0}`."
 )
 _MEMORY_FULL_ERROR_MESSAGE = (
     "Exceeded max `Register` size of {0} Bytes. Please increase the max size using the method `increase_reg_size`."
 )
 _REG_ALREADY_ADDED_ERROR_MESSAGE = "Already added as subregister."
-_NO_APRI_ERROR_MESSAGE = "The following `ApriInfo` is not known to this `Register` : {0}"
+_NO_APRI_ERROR_MESSAGE = "The following `ApriInfo` is not known to `{0}` : {1}"
 _RAM_BLOCK_NOT_OPEN_ERROR_MESSAGE = (
     "Closed RAM `Block` with the following data (it is good practice to always keep all RAM `Block`s open) : {0}, "
     "startn = {1}."
 )
 
 #################################
 #           CONSTANTS           #
@@ -152,45 +127,49 @@
         if initial_reg_size <= 0:
             raise ValueError("`initial_reg_size` must be positive.")
 
         self.saves_dir = resolve_path(Path(saves_dir))
 
         if not self.saves_dir.is_dir():
             raise NotADirectoryError(f"The path `{str(self.saves_dir)}` exists but is not a directory.")
-
-        self._shorthand = shorthand
-        self._shorthand_filepath = None
-        self._msg = msg
+        # DATABASE #
         self._msg_filepath = None
-
+        self._shorthand_filepath = None
         self._local_dir = None
         self._local_dir_bytes = None
         self._subreg_bytes = None
-
         self._db = None
         self._db_filepath = None
         self._db_map_size = initial_reg_size
         self._db_map_size_filepath = None
+        self._cls_filepath = None
+        # ATTRIBUTES
+        self._shorthand = shorthand
         self._readonly = None
+        self._msg = msg
         self._opened = False
-
+        self._created = False
+        # VERSION #
         self._version = CURRENT_VERSION
         self._version_filepath = None
-
-        self._cls_filepath = None
-
+        # INDICES #
         self._startn_head = _START_N_HEAD_DEFAULT
         self._startn_tail_length = _START_N_TAIL_LENGTH_DEFAULT
         self._startn_tail_mod = 10 ** self._startn_tail_length
         self._length_length = _LENGTH_LENGTH_DEFAULT
         self._max_length = _MAX_LENGTH_DEFAULT
-
+        # RAM BLOCKS #
         self._ram_blks = {}
-
-        self._created = False
+        # TIMEIT #
+        self.set_elapsed = 0
+        self.get_elapsed = 0
+        self.add_elapsed = 0
+        self.load_elapsed = 0
+        self.compress_elapsed = 0
+        self.decompress_elapsed = 0
 
     def __init_subclass__(cls, **kwargs):
 
         super().__init_subclass__(**kwargs)
         Register._constructors[cls.__name__] = cls
 
     #################################
@@ -305,18 +284,18 @@
 
         else:
             return hash(str(self._local_dir)) + hash(type(self))
 
     def __str__(self):
 
         if self._created:
-            return f'{self._shorthand} ({self._local_dir}): "{self._msg}"'
+            return f'{self._shorthand} ({self._local_dir}): {self._msg}'
 
         else:
-            return f'{self._shorthand}: "{self._msg}"'
+            return f'{self._shorthand}: {self._msg}'
 
     def __repr__(self):
         return f'{self.__class__.__name__}("{str(self.saves_dir)}", "{self._shorthand}", "{self._msg}", {self._db_map_size})'
 
     def set_shorthand(self, shorthand):
 
         check_type(shorthand, "shorthand", str)
@@ -554,14 +533,23 @@
             raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("ident"))
 
         return str(self._local_dir)
 
     def shorthand(self):
         return self._shorthand
 
+    def reset_timers(self):
+
+        self.set_elapsed = 0
+        self.get_elapsed = 0
+        self.add_elapsed = 0
+        self.load_elapsed = 0
+        self.compress_elapsed = 0
+        self.decompress_elapsed = 0
+
     #################################
     #    PROTEC REGISTER METHODS    #
 
     def _open_created(self, readonly):
 
         if Register._instance_exists(self._local_dir):
             ret = Register._get_instance(self._local_dir)
@@ -621,16 +609,16 @@
                     yiel._close_created()
                     yiel._opened = False
 
     def _check_open_raise(self, method_name):
 
         if not self._opened:
             raise RegisterError(
-                f"This `Register` database has not been opened. You must open this register via `with reg.open() as " +
-                f"reg:` before calling the method `{method_name}`."
+                f"The `{self._shorthand}` database has not been opened. You must open this register via "
+                f"`with {self._shorthand}.open() as {self._shorthand}:` before calling the method `{method_name}`."
             )
 
     def _check_readwrite_raise(self, method_name):
         """Call `self._check_open_raise` before this method."""
 
         if self._readonly:
             raise RegisterError(
@@ -679,14 +667,19 @@
         self._msg_filepath = local_dir / MSG_FILEPATH
         self._cls_filepath = local_dir / CLS_FILEPATH
         self._shorthand_filepath = local_dir / SHORTHAND_FILEPATH
         self._db_map_size_filepath = local_dir / MAP_SIZE_FILEPATH
 
     def _has_compatible_version(self):
         return self._version in COMPATIBLE_VERSIONS
+
+    def _timed_final_yield(self, yield_, elapsed_name, elapsed, start_time):
+
+        self.__dict__[elapsed_name] = elapsed + time() - start_time
+        return yield_
     #
     # def _db_is_closed(self):
     #
     #     if not self._created:
     #         raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_db_is_closed"))
     #
     #     else:
@@ -861,15 +854,15 @@
             else:
                 raise e
 
     def __contains__(self, apri):
 
         self._check_open_raise("__contains__")
 
-        if any(blk.apri() == apri for blk in self._ram_blks):
+        if any(apri_ == apri for apri_ in self._ram_blks.keys()):
             return True
 
         else:
 
             with self._db.begin() as txn:
 
                 try:
@@ -934,15 +927,15 @@
 
         finally:
 
             if commit:
                 txn.commit()
 
         if apri not in self._ram_blks.keys():
-            raise DataNotFoundError(_NO_APRI_ERROR_MESSAGE.format(str(apri)))
+            raise DataNotFoundError(_NO_APRI_ERROR_MESSAGE.format(self.shorthand(), str(apri)))
 
     def _get_apri_json_by_id(self, id_, txn = None):
         """Get JSON bytestring representing an `ApriInfo` instance.
 
         :param id_: (type `bytes`)
         :param txn: (type `lmbd.Transaction`, default `None`) The transaction to query. If `None`, then use open a new
         transaction and commit it after this method resolves.
@@ -1010,15 +1003,15 @@
                 return next_id
 
             else:
 
                 if apri is None:
                     apri = relational_decode_info(self, ApriInfo, apri_json, txn)
 
-                raise DataNotFoundError(_NO_APRI_ERROR_MESSAGE.format(str(apri)))
+                raise DataNotFoundError(_NO_APRI_ERROR_MESSAGE.format(self.shorthand(), str(apri)))
 
         finally:
 
             if commit:
 
                 try:
                     txn.commit()
@@ -1358,14 +1351,16 @@
 
         except DataNotFoundError:
 
             if not missing_ok:
                 raise
 
     def subregs(self):
+
+        self._check_open_raise("subregs")
         return list(self._iter_subregs())
 
     #################################
     #  PROTEC SUB-REGISTER METHODS  #
 
     def _add_subreg_txn(self, subreg, txn):
 
@@ -1531,136 +1526,154 @@
         :param ret_metadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object, which
         contains file creation date/time and size of dumped data to the disk.
         :raises RegisterError: If a duplicate `Block` already exists in this `Register`.
         """
 
         #DEBUG : 1, 2, 3, 4, 5
 
-        self._check_open_raise("add_disk_blk")
-        self._check_readwrite_raise("add_disk_blk")
-        Register._check_blk_open_raise(blk, "add_disk_blk")
-        check_type(blk, "blk", Block)
-        check_type(exists_ok, "exists_ok", bool)
-        check_type(dups_ok, "dups_ok", bool)
-        check_type(ret_metadata, "ret_metadata", bool)
-        startn_head = blk.startn() // self._startn_tail_mod
+        start_time = time()
 
-        if startn_head != self._startn_head :
+        try:
+            # try clause followed by finally clause that increments `self.add_elapsed`
+            self._check_open_raise("add_disk_blk")
+            self._check_readwrite_raise("add_disk_blk")
+            Register._check_blk_open_raise(blk, "add_disk_blk")
+            check_type(blk, "blk", Block)
+            check_type(exists_ok, "exists_ok", bool)
+            check_type(dups_ok, "dups_ok", bool)
+            check_type(ret_metadata, "ret_metadata", bool)
+            startn_head = blk.startn() // self._startn_tail_mod
+
+            if startn_head != self._startn_head :
+
+                raise IndexError(
+                    "The `startn_` for the passed `Block` does not have the correct head:\n"
+                    f"`tail_len`      : {self._startn_tail_length}\n"
+                    f"expected `head` : {self._startn_head}\n"
+                    f"`startn`        : {blk.startn()}\n"
+                    f"`startn` head   : {startn_head}\n"
+                    "Please see the method `set_startn_info` to troubleshoot this error."
+                )
 
-            raise IndexError(
-                "The `startn_` for the passed `Block` does not have the correct head:\n"
-                f"`tail_len`      : {self._startn_tail_length}\n"
-                f"expected `head` : {self._startn_head}\n"
-                f"`startn`        : {blk.startn()}\n"
-                f"`startn` head   : {startn_head}\n"
-                "Please see the method `set_startn_info` to troubleshoot this error."
-            )
+            if len(blk) > self._max_length:
+                raise ValueError
 
-        if len(blk) > self._max_length:
-            raise ValueError
+            if _debug == 1:
+                raise KeyboardInterrupt
 
-        if _debug == 1:
-            raise KeyboardInterrupt
+            txn = None
+            filename = None
 
-        txn = None
-        filename = None
+            if not dups_ok and blk.apri() in self:
 
-        if not dups_ok and blk.apri() in self:
+                int_ = (blk.startn(), len(blk))
 
-            int_ = (blk.startn(), len(blk))
+                for t in self.intervals(blk.apri(), False, False, True, False):
 
-            for t in self.intervals(blk.apri(), False, True, False):
+                    if intervals_overlap(t, int_):
+                        raise RegisterError(
+                            "Attempted to add a `Block` with duplicate indices. Set `dups_ok` to `True` to suppress."
+                        )
 
-                if intervals_overlap(t, int_):
-                    raise RegisterError(
-                        "Attempted to add a `Block` with duplicate indices. Set `dups_ok` to `True` to suppress."
-                    )
+            if _debug == 2:
+                raise KeyboardInterrupt
 
-        if _debug == 2:
-            raise KeyboardInterrupt
+            try:
 
-        try:
+                with ReversibleTransaction(self._db).begin(write = True) as txn:
 
-            with ReversibleTransaction(self._db).begin(write = True) as txn:
+                    filename = self._add_disk_blk_txn(blk, txn)
 
-                filename = self._add_disk_blk_txn(blk, txn)
+                    if _debug == 3:
+                        raise KeyboardInterrupt
 
-                if _debug == 3:
+                if _debug == 4:
                     raise KeyboardInterrupt
 
-            if _debug == 4:
-                raise KeyboardInterrupt
+                type(self).dump_disk_data(blk.segment(), filename, **kwargs)
 
-            type(self).dump_disk_data(blk.segment(), filename, **kwargs)
+                if _debug == 5:
+                    raise KeyboardInterrupt
 
-            if _debug == 5:
-                raise KeyboardInterrupt
+            except BaseException as e:
 
-        except BaseException as e:
+                if not isinstance(e, RegisterError) or not exists_ok or not "exist" in str(e):
 
-            if not isinstance(e, RegisterError) or not exists_ok or not "exist" in str(e):
+                    try:
 
-                try:
+                        if filename is not None:
 
-                    if filename is not None:
+                            try:
+                                filename.unlink()
 
-                        try:
-                            filename.unlink()
+                            except FileNotFoundError:
+                                pass
 
-                        except FileNotFoundError:
-                            pass
+                        if txn is not None:
 
-                    if txn is not None:
+                            with self._db.begin(write = True) as txn_:
+                                txn.reverse(txn_)
 
-                        with self._db.begin(write = True) as txn_:
-                            txn.reverse(txn_)
+                    except:
+                        raise RegisterRecoveryError("Could not successfully recover from a failed disk `Block` add!") from e
 
-                except:
-                    raise RegisterRecoveryError("Could not successfully recover from a failed disk `Block` add!") from e
+                    else:
 
-                else:
+                        if isinstance(e, lmdb.MapFullError):
+                            raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
-                    if isinstance(e, lmdb.MapFullError):
-                        raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
+                        else:
+                            raise e
 
-                    else:
-                        raise e
+            if ret_metadata:
+                return self.blk_metadata(blk.apri(), blk.startn(), len(blk), False)
 
-        if ret_metadata:
-            return self.blk_metadata(blk.apri(), blk.startn(), len(blk), False)
+            else:
+                return None
 
-        else:
-            return None
+        finally:
+            self.add_elapsed += time() - start_time
 
     def append_disk_blk(self, blk, ret_metadata = False, **kwargs):
         """Add a `Block` to disk and link it with this `Register`.
 
         If no disk `Block`s with the same `ApriInfo` as `blk` have previously been added to disk, then `startn` is set
         to 0.. If not, then `startn` will be set to one more than the largest index among all disk `Block`s with the
         same `ApriInfo` as `blk`.
 
         :param blk: (type `Block`)
         :param ret_metadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object, which
         contains file creation date/time and size of dumped data to the disk.
         :raises RegisterError: If a duplicate `Block` already exists in this `Register`.
         """
 
-        self._check_open_raise("append_disk_blk")
-        self._check_readwrite_raise("append_disk_blk")
-        Register._check_blk_open_raise(blk, "append_disk_blk")
-        check_type(blk, "blk", Block)
-        check_type(ret_metadata, "ret_metadata", bool)
+        add_elapsed = self.add_elapsed
+        start_time = time()
 
-        if self.num_blks(blk.apri(), diskonly = True) == 0:
-            return self.add_disk_blk(blk, ret_metadata, **kwargs)
+        try:
+            # try clause followed by finally clause that increments `self.add_elapsed`
+            self._check_open_raise("append_disk_blk")
+            self._check_readwrite_raise("append_disk_blk")
+            Register._check_blk_open_raise(blk, "append_disk_blk")
+            check_type(blk, "blk", Block)
+            check_type(ret_metadata, "ret_metadata", bool)
 
-        else:
+            try:
+                maxn = self.maxn(blk.apri(), True, False)
+
+            except DataNotFoundError:
+                return self.add_disk_blk(blk, ret_metadata, **kwargs)
+
+            else:
+
+                blk.set_startn(maxn + 1)
+                return self.add_disk_blk(blk, ret_metadata, **kwargs)
 
-            blk.set_startn(self.maxn(blk.apri()) + 1)
-            return self.add_disk_blk(blk, ret_metadata, **kwargs)
+        finally:
+            self.add_elapsed = add_elapsed + time() - start_time
 
     def rmv_disk_blk(self, apri, startn = None, length = None, missing_ok = False, recursively = False, **kwargs):
         """Delete a disk `Block` and unlink it with this `Register`.
 
         :param apri: (type `ApriInfo`)
         :param startn: (type `int`) Non-negative.
         :param length: (type `int`) Non-negative.
@@ -1796,15 +1809,15 @@
                         subreg.rmv_disk_blk(apri, startn, length, False, True, **kwargs)
                         return
 
                     except DataNotFoundError:
                         pass
 
         if not missing_ok:
-            raise DataNotFoundError(_blk_not_found_err_msg(True, apri, None, startn, length))
+            raise DataNotFoundError(self._blk_not_found_err_msg(True, apri, None, startn, length))
 
     def blk_metadata(self, apri, startn = None, length = None, recursively = False):
 
         self._check_open_raise("blk_metadata")
         check_type(apri, "apri", ApriInfo)
         startn = check_return_int_None_default(startn, "startn", None)
         length = check_return_int_None_default(length, "length", None)
@@ -1852,15 +1865,15 @@
                     try:
                         return subreg.blk_metadata(apri, startn, length, True)
 
                     except DataNotFoundError:
                         pass
 
         raise DataNotFoundError(
-            _blk_not_found_err_msg(True, apri, None, startn, length)
+            self._blk_not_found_err_msg(True, apri, None, startn, length)
         )
 
     def compress(self, apri, startn = None, length = None, compression_level = 6, ret_metadata = False):
         """Compress a `Block`.
 
         :param apri: (type `ApriInfo`)
         :param startn: (type `int`) Non-negative.
@@ -1871,132 +1884,138 @@
         :param ret_metadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object that
         describes the compressed file.
         :raises CompressionError: If the `Block` is already compressed.
         :return: (type `File_Metadata`) If `ret_metadata is True`.
         """
 
         # DEBUG : 1, 2, 3, 4
+        start_time = time()
 
-        _FAIL_NO_RECOVER_ERROR_MESSAGE = "Could not recover successfully from a failed disk `Block` compress!"
-        self._check_open_raise("compress")
-        self._check_readwrite_raise("compress")
-        check_type(apri, "apri", ApriInfo)
-        startn = check_return_int_None_default(startn, "startn", None)
-        length = check_return_int_None_default(length, "length", None)
-        compression_level = check_return_int(compression_level, "compression_level")
-        check_type(ret_metadata, "ret_metadata", bool)
+        try:
+            # try clause followed by finally clause that increments `self.compress_elapsed`
+            _FAIL_NO_RECOVER_ERROR_MESSAGE = "Could not recover successfully from a failed disk `Block` compress!"
+            self._check_open_raise("compress")
+            self._check_readwrite_raise("compress")
+            check_type(apri, "apri", ApriInfo)
+            startn = check_return_int_None_default(startn, "startn", None)
+            length = check_return_int_None_default(length, "length", None)
+            compression_level = check_return_int(compression_level, "compression_level")
+            check_type(ret_metadata, "ret_metadata", bool)
 
-        if startn is not None and startn < 0:
-            raise ValueError("`startn` must be non-negative.")
+            if startn is not None and startn < 0:
+                raise ValueError("`startn` must be non-negative.")
 
-        if length is not None and length < 0:
-            raise ValueError("`length` must be non-negative.")
+            if length is not None and length < 0:
+                raise ValueError("`length` must be non-negative.")
 
-        if not (0 <= compression_level <= 9):
-            raise ValueError("`compression_level` must be between 0 and 9, inclusive.")
+            if not (0 <= compression_level <= 9):
+                raise ValueError("`compression_level` must be between 0 and 9, inclusive.")
 
-        startn_, length_ = self._resolve_startn_length(apri, startn, length, True)
+            startn_, length_ = self._resolve_startn_length(apri, startn, length, True)
 
-        compressed_key = self._get_disk_blk_key(
-            _COMPRESSED_KEY_PREFIX, apri, None, startn_, length_, False
-        )
+            compressed_key = self._get_disk_blk_key(
+                _COMPRESSED_KEY_PREFIX, apri, None, startn_, length_, False
+            )
 
-        blk_key, compressed_key = self._check_blk_compressed_keys_raise(
-            None, compressed_key, apri, None, startn_, length_
-        )
+            blk_key, compressed_key = self._check_blk_compressed_keys_raise(
+                None, compressed_key, apri, None, startn_, length_
+            )
 
-        with self._db.begin() as txn:
-            compressed_val = txn.get(compressed_key)
+            with self._db.begin() as txn:
+                compressed_val = txn.get(compressed_key)
 
-        if compressed_val != _IS_NOT_COMPRESSED_VAL:
+            if compressed_val != _IS_NOT_COMPRESSED_VAL:
 
-            raise CompressionError(
-                "The disk `Block` with the following data has already been compressed: " +
-                f"{str(apri)}, startn = {startn_}, length = {length_}"
-            )
+                raise CompressionError(
+                    "The disk `Block` with the following data has already been compressed: " +
+                    f"{str(apri)}, startn = {startn_}, length = {length_}"
+                )
 
-        with self._db.begin() as txn:
-            blk_filename = self._local_dir / txn.get(blk_key).decode("ASCII")
+            with self._db.begin() as txn:
+                blk_filename = self._local_dir / txn.get(blk_key).decode("ASCII")
 
-        compressed_filename = random_unique_filename(self._local_dir, COMPRESSED_FILE_SUFFIX)
-        compressed_val = compressed_filename.name.encode("ASCII")
+            compressed_filename = random_unique_filename(self._local_dir, COMPRESSED_FILE_SUFFIX)
+            compressed_val = compressed_filename.name.encode("ASCII")
 
-        cleaned = False
+            cleaned = False
 
-        if _debug == 1:
-            raise KeyboardInterrupt
+            if _debug == 1:
+                raise KeyboardInterrupt
 
-        try:
+            try:
 
-            with self._db.begin(write = True) as txn:
+                with self._db.begin(write = True) as txn:
 
-                txn.put(compressed_key, compressed_val)
+                    txn.put(compressed_key, compressed_val)
 
-                if _debug == 2:
-                    raise KeyboardInterrupt
+                    if _debug == 2:
+                        raise KeyboardInterrupt
 
-            with zipfile.ZipFile(
+                with zipfile.ZipFile(
 
-                compressed_filename,  # target filename
-                "x",  # zip mode (write, but don't overwrite)
-                zipfile.ZIP_DEFLATED,  # compression mode
-                True,  # use zip64
-                compression_level
+                    compressed_filename,  # target filename
+                    "x",  # zip mode (write, but don't overwrite)
+                    zipfile.ZIP_DEFLATED,  # compression mode
+                    True,  # use zip64
+                    compression_level
 
-            ) as compressed_fh:
+                ) as compressed_fh:
 
-                compressed_fh.write(blk_filename, blk_filename.name)
+                    compressed_fh.write(blk_filename, blk_filename.name)
 
-                if _debug == 3:
+                    if _debug == 3:
+                        raise KeyboardInterrupt
+
+                if _debug == 4:
                     raise KeyboardInterrupt
 
-            if _debug == 4:
-                raise KeyboardInterrupt
+                type(self).clean_disk_data(blk_filename)
+                cleaned = True
+                blk_filename.touch()
 
-            type(self).clean_disk_data(blk_filename)
-            cleaned = True
-            blk_filename.touch()
+            except BaseException as e:
 
-        except BaseException as e:
+                try:
 
-            try:
+                    with self._db.begin(write = True) as txn:
+                        txn.put(compressed_key, _IS_NOT_COMPRESSED_VAL)
 
-                with self._db.begin(write = True) as txn:
-                    txn.put(compressed_key, _IS_NOT_COMPRESSED_VAL)
+                    if cleaned or not blk_filename.exists():
+                        raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
 
-                if cleaned or not blk_filename.exists():
-                    raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
+                    else:
 
-                else:
+                        try:
+                            compressed_filename.unlink()
 
-                    try:
-                        compressed_filename.unlink()
+                        except FileNotFoundError:
+                            pass
 
-                    except FileNotFoundError:
-                        pass
+                except RegisterRecoveryError as ee:
+                    raise ee
 
-            except RegisterRecoveryError as ee:
-                raise ee
+                except BaseException:
+                    raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
 
-            except BaseException:
-                raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
+                else:
 
-            else:
+                    if isinstance(e, lmdb.MapFullError):
+                        raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
-                if isinstance(e, lmdb.MapFullError):
-                    raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
+                    else:
+                        raise e
 
-                else:
-                    raise e
+            if ret_metadata:
+                return FileMetadata.from_path(compressed_filename)
 
-        if ret_metadata:
-            return FileMetadata.from_path(compressed_filename)
+            else:
+                return None
 
-        else:
-            return None
+        finally:
+            self.compress_elapsed += time() - start_time
 
     def decompress(self, apri, startn = None, length = None, ret_metadata = False):
         """Decompress a `Block`.
 
         :param apri: (type `ApriInfo`)
         :param startn: (type `int`) Non-negative.
         :param length: (type `int`) Non-negative.
@@ -2004,118 +2023,125 @@
         describes the decompressed file.
         :raise DecompressionError: If the `Block` is not compressed.
         :return: (type `list`) If `ret_metadata is True`.
         """
 
         # DEBUG : 1, 2, 3, 4
 
-        _FAIL_NO_RECOVER_ERROR_MESSAGE = "Could not recover successfully from a failed disk `Block` decompress!"
-        self._check_open_raise("decompress")
-        self._check_readwrite_raise("decompress")
-        check_type(apri, "apri", ApriInfo)
-        startn = check_return_int_None_default(startn, "startn", None)
-        length = check_return_int_None_default(length, "length", None)
-        check_type(ret_metadata, "ret_metadata", bool)
-
-        if startn is not None and startn < 0:
-            raise ValueError("`startn` must be non-negative.")
+        start_time = time()
 
-        if length is not None and length < 0:
-            raise ValueError("`length` must be non-negative.")
-
-        startn_, length_ = self._resolve_startn_length(apri, startn, length, True)
-        blk_key, compressed_key = self._check_blk_compressed_keys_raise(None, None, apri, None, startn_, length_)
+        try:
+            # try clause followed by finally clause that increments `self.decompress_elapsed`
+            _FAIL_NO_RECOVER_ERROR_MESSAGE = "Could not recover successfully from a failed disk `Block` decompress!"
+            self._check_open_raise("decompress")
+            self._check_readwrite_raise("decompress")
+            check_type(apri, "apri", ApriInfo)
+            startn = check_return_int_None_default(startn, "startn", None)
+            length = check_return_int_None_default(length, "length", None)
+            check_type(ret_metadata, "ret_metadata", bool)
 
-        with self._db.begin() as txn:
-            compressed_val = txn.get(compressed_key)
+            if startn is not None and startn < 0:
+                raise ValueError("`startn` must be non-negative.")
 
-        if compressed_val == _IS_NOT_COMPRESSED_VAL:
+            if length is not None and length < 0:
+                raise ValueError("`length` must be non-negative.")
 
-            raise DecompressionError(
-                "The disk `Block` with the following data is not compressed: " +
-                f"{str(apri)}, startn = {startn_}, length = {length_}"
-            )
+            startn_, length_ = self._resolve_startn_length(apri, startn, length, True)
+            blk_key, compressed_key = self._check_blk_compressed_keys_raise(None, None, apri, None, startn_, length_)
 
-        with self._db.begin() as txn:
-            blk_filename = txn.get(blk_key).decode("ASCII")
+            with self._db.begin() as txn:
+                compressed_val = txn.get(compressed_key)
 
-        blk_filename = self._local_dir / blk_filename
-        compressed_filename = self._local_dir / compressed_val.decode("ASCII")
-        deleted = False
+            if compressed_val == _IS_NOT_COMPRESSED_VAL:
 
-        if not is_deletable(blk_filename):
-            raise OSError(f"Cannot delete ghost file `{str(blk_filename)}`.")
+                raise DecompressionError(
+                    "The disk `Block` with the following data is not compressed: " +
+                    f"{str(apri)}, startn = {startn_}, length = {length_}"
+                )
 
-        if not is_deletable(compressed_filename):
-            raise OSError(f"Cannot delete compressed file `{str(compressed_filename)}`.")
+            with self._db.begin() as txn:
+                blk_filename = txn.get(blk_key).decode("ASCII")
 
-        if _debug == 1:
-            raise KeyboardInterrupt
+            blk_filename = self._local_dir / blk_filename
+            compressed_filename = self._local_dir / compressed_val.decode("ASCII")
+            deleted = False
 
-        try:
+            if not is_deletable(blk_filename):
+                raise OSError(f"Cannot delete ghost file `{str(blk_filename)}`.")
 
-            with self._db.begin(write = True) as txn:
+            if not is_deletable(compressed_filename):
+                raise OSError(f"Cannot delete compressed file `{str(compressed_filename)}`.")
 
-                # delete ghost file
-                blk_filename.unlink()
-                deleted = True
+            if _debug == 1:
+                raise KeyboardInterrupt
 
-                if _debug == 2:
-                    raise KeyboardInterrupt
+            try:
 
-                with zipfile.ZipFile(compressed_filename, "r") as compressed_fh:
+                with self._db.begin(write = True) as txn:
 
-                    compressed_fh.extract(blk_filename.name, self._local_dir)
+                    # delete ghost file
+                    blk_filename.unlink()
+                    deleted = True
 
-                    if _debug == 3:
+                    if _debug == 2:
                         raise KeyboardInterrupt
 
-                txn.put(compressed_key, _IS_NOT_COMPRESSED_VAL)
+                    with zipfile.ZipFile(compressed_filename, "r") as compressed_fh:
 
-                if _debug == 4:
-                    raise KeyboardInterrupt
+                        compressed_fh.extract(blk_filename.name, self._local_dir)
 
-                compressed_filename.unlink()
+                        if _debug == 3:
+                            raise KeyboardInterrupt
 
-        except BaseException as e:
+                    txn.put(compressed_key, _IS_NOT_COMPRESSED_VAL)
 
-            try:
+                    if _debug == 4:
+                        raise KeyboardInterrupt
 
-                if not compressed_filename.is_file():
-                    raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
+                    compressed_filename.unlink()
 
-                elif deleted or not blk_filename.is_file():
+            except BaseException as e:
 
-                    try:
-                        blk_filename.unlink()
+                try:
 
-                    except FileNotFoundError:
-                        pass
+                    if not compressed_filename.is_file():
+                        raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
 
-                    blk_filename.touch()
+                    elif deleted or not blk_filename.is_file():
 
-            except RegisterRecoveryError as ee:
-                raise ee
+                        try:
+                            blk_filename.unlink()
 
-            except BaseException:
-                raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
+                        except FileNotFoundError:
+                            pass
 
-            else:
+                        blk_filename.touch()
 
-                if isinstance(e, lmdb.MapFullError):
-                    raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
+                except RegisterRecoveryError as ee:
+                    raise ee
+
+                except BaseException:
+                    raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
 
                 else:
-                    raise e
 
-        if ret_metadata:
-            return FileMetadata.from_path(blk_filename)
+                    if isinstance(e, lmdb.MapFullError):
+                        raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
+
+                    else:
+                        raise e
 
-        else:
-            return None
+            if ret_metadata:
+                return FileMetadata.from_path(blk_filename)
+
+            else:
+                return None
+
+        finally:
+            self.decompress_elapsed += time() - start_time
 
     def is_compressed(self, apri, startn = None, length = None):
 
         # self._check_open_raise("is_compressed")
         # check_type(apri, "apri", ApriInfo)
         # startn = check_return_int_None_default(startn, "startn", None)
         # length = check_return_int_None_default(length, "length", None)
@@ -2407,15 +2433,15 @@
                 txn.commit()
 
         if (not has_blk_key and has_compr_key) or (has_blk_key and not has_compr_key):
             raise RegisterError("Uncompressed/compressed `Block` key mismatch.")
 
         if not has_blk_key:
             raise DataNotFoundError(
-                _blk_not_found_err_msg(True, apri, None, startn, length)
+                self._blk_not_found_err_msg(True, apri, None, startn, length)
             )
 
         return blk_key, compressed_key
 
     def _check_blk_compressed_files_raise(self, blk_key, compressed_key, apri, startn, length, txn = None):
 
         commit = txn is None
@@ -2527,163 +2553,187 @@
 
     #################################
     # PUBLIC RAM & DISK BLK METHODS #
 
     @contextmanager
     def blk_by_n(self, apri, n, diskonly = False, recursively = False, ret_metadata = False, **kwargs):
 
-        self._check_open_raise("blk_by_n")
-        check_type(apri, "apri", ApriInfo)
-        n = check_return_int(n, "n")
-        check_type(diskonly, "diskonly", bool)
-        check_type(recursively, "recursively", bool)
-        check_type(ret_metadata, "ret_metadata", bool)
-
-        if n < 0:
-            raise IndexError("`n` must be non-negative.")
+        errored = False
+        load_elapsed = self.load_elapsed
+        start_time = time()
 
         try:
-            self._check_known_apri(apri)
-
-        except DataNotFoundError:
+            # try clause followed by finally clause that increments `self.load_elapsed`
+            self._check_open_raise("blk_by_n")
+            check_type(apri, "apri", ApriInfo)
+            n = check_return_int(n, "n")
+            check_type(diskonly, "diskonly", bool)
+            check_type(recursively, "recursively", bool)
+            check_type(ret_metadata, "ret_metadata", bool)
 
-            if not recursively:
-                raise
+            if n < 0:
+                raise IndexError("`n` must be non-negative.")
 
-        else:
+            try:
+                self._check_known_apri(apri)
 
-            for startn, length in self.intervals(apri, combine = False, diskonly = diskonly, recursively = False):
+            except DataNotFoundError:
 
-                if startn <= n < startn + length:
+                if not recursively:
+                    raise
 
-                    with self.blk(apri, startn, length, diskonly, False, ret_metadata, **kwargs) as blk:
+            else:
 
-                        yield blk
-                        return
+                for startn, length in self.intervals(apri, False, False, diskonly, recursively):
 
-        if recursively:
+                    if startn <= n < startn + length:
 
-            for subreg in self._iter_subregs():
+                        with self.blk(apri, startn, length, diskonly, recursively, ret_metadata, **kwargs) as blk:
 
-                with subreg._recursive_open(True) as subreg:
+                            yield self._timed_final_yield(blk, "load_elapsed", load_elapsed, start_time)
+                            return
 
-                    try:
+            raise DataNotFoundError(self._blk_not_found_err_msg(diskonly, apri, n))
 
-                        with subreg.blk_by_n(apri, n, diskonly, True, ret_metadata, **kwargs) as blk:
+        except:
 
-                            yield blk
-                            return
+            errored = True
+            raise
 
-                    except DataNotFoundError:
-                        pass
+        finally:
 
-        raise DataNotFoundError(_blk_not_found_err_msg(diskonly, apri, n))
+            if errored:
+                self.load_elapsed = load_elapsed + time() - start_time
 
     @contextmanager
     def blk(self, apri, startn = None, length = None, diskonly = False, recursively = False, ret_metadata = False, **kwargs):
 
-        self._check_open_raise("blk")
-        check_type(apri, "apri", ApriInfo)
-        startn = check_return_int_None_default(startn, "startn", None)
-        length = check_return_int_None_default(length, "length", None)
-        check_type(diskonly, "diskonly", bool)
-        check_type(recursively, "recursively", bool)
-        check_type(ret_metadata, "ret_metadata", bool)
+        load_elapsed = self.load_elapsed
+        errored = False
+        start_time = time()
+
+        try:
+            # try clause followed by finally clause that increments `self.load_elapsed`
+            self._check_open_raise("blk")
+            check_type(apri, "apri", ApriInfo)
+            startn = check_return_int_None_default(startn, "startn", None)
+            length = check_return_int_None_default(length, "length", None)
+            check_type(diskonly, "diskonly", bool)
+            check_type(recursively, "recursively", bool)
+            check_type(ret_metadata, "ret_metadata", bool)
 
-        if startn is not None and startn < 0:
-            raise ValueError("`startn` must be non-negative.")
+            if startn is not None and startn < 0:
+                raise ValueError("`startn` must be non-negative.")
 
-        if length is not None and length < 0:
-            raise ValueError("`length` must be non-negative.")
+            if length is not None and length < 0:
+                raise ValueError("`length` must be non-negative.")
 
-        try:
-            self._check_known_apri(apri)
+            try:
+                self._check_known_apri(apri)
 
-        except DataNotFoundError:
+            except DataNotFoundError:
 
-            if not recursively:
-                raise
+                if not recursively:
+                    raise
 
-        else:
+            else:
 
-            startn_, length_ = self._resolve_startn_length(apri, startn, length, diskonly)
+                startn_, length_ = self._resolve_startn_length(apri, startn, length, diskonly)
 
-            if not diskonly and apri in self._ram_blks.keys():
+                if not diskonly and apri in self._ram_blks.keys():
 
-                for blk in self._ram_blks[apri]:
+                    for blk in self._ram_blks[apri]:
 
-                    try:
-                        blk_len = len(blk)
+                        try:
+                            blk_len = len(blk)
 
-                    except BlockNotOpenError as e:
-                        raise BlockNotOpenError(_RAM_BLOCK_NOT_OPEN_ERROR_MESSAGE.format(apri, blk.startn())) from e
+                        except BlockNotOpenError as e:
+                            raise BlockNotOpenError(
+                                _RAM_BLOCK_NOT_OPEN_ERROR_MESSAGE.format(apri, blk.startn())
+                            ) from e
 
-                    if blk.startn() == startn_ and blk_len == length_:
+                        if blk.startn() == startn_ and blk_len == length_:
 
-                        if ret_metadata:
+                            self.load_elapsed += time() - start_time
 
-                            yield blk, None
-                            return
+                            if ret_metadata:
 
-                        else:
+                                yield self._timed_final_yield((blk, None), "load_elapsed", load_elapsed, start_time)
+                                return
 
-                            yield blk
-                            return
+                            else:
 
-            try:
-                blk_key, compressed_key = self._check_blk_compressed_keys_raise(None, None, apri, None, startn_, length_)
+                                yield self._timed_final_yield(blk, "load_elapsed", load_elapsed, start_time)
+                                return
 
-            except DataNotFoundError:
-                pass
+                try:
+                    blk_key, compressed_key = self._check_blk_compressed_keys_raise(None, None, apri, None, startn_, length_)
 
-            else:
+                except DataNotFoundError:
+                    pass
 
-                with self._db.begin() as txn:
+                else:
 
-                    if txn.get(compressed_key) != _IS_NOT_COMPRESSED_VAL:
-                        raise CompressionError(
-                            "Could not load disk `Block` with the following data because the `Block` is compressed. "
-                            "Please call the `Register` method `decompress` first before loading the data.\n" +
-                            f"{apri}, startn = {startn_}, length = {length_}"
-                        )
+                    with self._db.begin() as txn:
 
-                blk_filename, _ = self._check_blk_compressed_files_raise(blk_key, compressed_key, apri, startn_, length_)
-                blk_filename = self._local_dir / blk_filename
-                data = type(self).load_disk_data(blk_filename, **kwargs)
-                blk = Block(data, apri, startn_)
+                        if txn.get(compressed_key) != _IS_NOT_COMPRESSED_VAL:
+                            raise CompressionError(
+                                "Could not load disk `Block` with the following data because the `Block` is compressed. "
+                                "Please call the `Register` method `decompress` first before loading the data.\n" +
+                                f"{apri}, startn = {startn_}, length = {length_}"
+                            )
 
-                with blk:
+                    blk_filename, _ = self._check_blk_compressed_files_raise(blk_key, compressed_key, apri, startn_, length_)
+                    blk_filename = self._local_dir / blk_filename
+                    data = type(self).load_disk_data(blk_filename, **kwargs)
+                    blk = Block(data, apri, startn_)
 
-                    if ret_metadata:
-                        yield blk, FileMetadata.from_path(blk_filename)
+                    with blk:
 
-                    else:
-                        yield blk
+                        if ret_metadata:
+                            yield self._timed_final_yield(
+                                (blk, FileMetadata.from_path(blk_filename)), "load_elapsed", load_elapsed, start_time
+                            )
 
-                return
+                        else:
+                            yield self._timed_final_yield(blk, "load_elapsed", load_elapsed, start_time)
 
-        if recursively:
+                    return
 
-            for subreg in self._iter_subregs():
+            if recursively:
 
-                with subreg._recursive_open(True) as subreg:
+                for subreg in self._iter_subregs():
 
-                    try:
+                    with subreg._recursive_open(True) as subreg:
+
+                        try:
 
-                        with subreg.blk(apri, startn, length, ret_metadata, ret_metadata=True) as blk:
-                            yield blk
+                            with subreg.blk(
+                                apri, startn, length, diskonly, recursively, ret_metadata, **kwargs
+                            ) as blk:
+                                yield self._timed_final_yield(blk, "load_elapsed", load_elapsed, start_time)
 
-                        return
+                            return
 
-                    except DataNotFoundError:
-                        pass
+                        except DataNotFoundError:
+                            pass
 
-        raise DataNotFoundError(
-            _blk_not_found_err_msg(diskonly, str(apri), None, startn, length)
-        )
+            raise DataNotFoundError(
+                self._blk_not_found_err_msg(diskonly, str(apri), None, startn, length)
+            )
+
+        except:
+
+            errored = True
+            raise
+
+        finally:
+
+            if errored:
+                self.load_elapsed = load_elapsed + time() - start_time
 
     def blks(self, apri, diskonly = False, recursively = False, ret_metadata = False, **kwargs):
         """Iterate over all `Block`s with `apri`.
 
         This is a convenience method that should be used only for simple data manipulation. This method opens
         only one `Block` at a time; each is closed automatically before the next `Block` is yielded (hence it is
         not necessary to use a `with` clause).
@@ -2713,15 +2763,15 @@
         except DataNotFoundError:
 
             if not recursively:
                 raise
 
         else:
 
-            for startn, length in self.intervals(apri, combine = False, diskonly = diskonly, recursively = recursively):
+            for startn, length in self.intervals(apri, False, False, diskonly, recursively):
 
                 try:
 
                     with self.blk(apri, startn, length, diskonly, False, ret_metadata, **kwargs) as blk:
                         yield blk
 
                 except DataNotFoundError:
@@ -2730,184 +2780,220 @@
         if recursively:
 
             for subreg in self._iter_subregs():
 
                 with subreg._recursive_open(True) as subreg:
                     yield from subreg.blks(apri, diskonly, True, ret_metadata, **kwargs)
 
-    @contextmanager
     def __getitem__(self, apri_n_diskonly_recursively):
+        return self.get(*Register._resolve_apri_n_diskonly_recursively(apri_n_diskonly_recursively))
 
-        with self.get(*Register._resolve_apri_n_diskonly_recursively(apri_n_diskonly_recursively)) as yield_:
-            yield yield_
-
-    @contextmanager
     def get(self, apri, n, diskonly = False, recursively = False, **kwargs):
 
-        self._check_open_raise("get")
+        start_time = time()
 
-        n_slice = isinstance(n, slice)
+        try:
+            # try clause followed by finally clause that increments `self.get_elapsed`
+            self._check_open_raise("get")
 
-        if not isinstance(apri, ApriInfo):
-            raise TypeError("The first argument to `reg[]` must be an `ApriInfo.")
+            n_slice = isinstance(n, slice)
 
-        if not is_int(n) and n_slice:
-            raise TypeError("The second argument to `reg[]` must be an `int` or a `slice`.")
+            if not isinstance(apri, ApriInfo):
+                raise TypeError("The first argument to `reg[]` must be an `ApriInfo.")
 
-        elif not n_slice:
-            n = int(n)
+            if not is_int(n) and not n_slice:
+                raise TypeError("The second argument to `reg[]` must be an `int` or a `slice`.")
 
-        else:
+            elif not n_slice:
+                n = int(n)
 
-            _n = [None]*3
+            else:
 
-            if n.start is not None and not is_int(n.start):
-                raise TypeError("Start index of slice must be an `int`.")
+                _n = [None]*3
 
-            elif n.start is not None:
-                _n[0] = int(n.start)
+                if n.start is not None and not is_int(n.start):
+                    raise TypeError("Start index of slice must be an `int`.")
 
-            if n.stop is not None and not is_int(n.stop):
-                raise TypeError("Stop index of slice must be an `int`.")
+                elif n.start is not None:
+                    _n[0] = int(n.start)
 
-            elif n.stop is not None:
-                _n[1] = int(n.stop)
+                if n.stop is not None and not is_int(n.stop):
+                    raise TypeError("Stop index of slice must be an `int`.")
 
-            if n.step is not None and not is_int(n.step):
-                raise TypeError("Step index of slice must be an `int`.")
+                elif n.stop is not None:
+                    _n[1] = int(n.stop)
 
-            elif n.step is not None:
-                _n[2] = int(n.stop)
+                if n.step is not None and not is_int(n.step):
+                    raise TypeError("Step index of slice must be an `int`.")
 
-            n = slice(*tuple(_n))
+                elif n.step is not None:
+                    _n[2] = int(n.stop)
 
-        if not isinstance(diskonly, bool):
-            raise TypeError("The second argument of `reg[]` must be of type `bool`.")
+                n = slice(*tuple(_n))
 
-        if not isinstance(recursively, bool):
-            raise TypeError("The third argument of `reg[]` must be of type `bool`.")
+            if not isinstance(diskonly, bool):
+                raise TypeError("The third argument of `reg[]` must be of type `bool`.")
 
-        if n_slice:
+            if not isinstance(recursively, bool):
+                raise TypeError("The fourth argument of `reg[]` must be of type `bool`.")
 
-            if n.start is not None and n.start < 0:
-                raise ValueError("Start index cannot be negative.")
+            if n_slice:
 
-            if n.stop is not None and n.stop < 0:
-                raise ValueError("Stop index cannot be negative.")
+                if n.start is not None and n.start < 0:
+                    raise ValueError("Start index cannot be negative.")
 
-        try:
-            self._check_known_apri(apri)
+                if n.stop is not None and n.stop < 0:
+                    raise ValueError("Stop index cannot be negative.")
 
-        except DataNotFoundError:
+            try:
+                self._check_known_apri(apri)
 
-            if not recursively:
-                raise
+            except DataNotFoundError:
 
-        else:
+                if not recursively:
+                    raise
 
-            if n_slice:
+            else:
 
-                yield _element_iter(self, apri, n, diskonly, recursively, kwargs)
-                return
+                if n_slice:
+                    return _element_iter(self, apri, n, diskonly, recursively, kwargs)
 
-            else:
+                else:
 
-                with self.blk_by_n(apri, n, diskonly, recursively, False, **kwargs) as blk:
-                    yield blk.segment()
+                    with self.blk_by_n(apri, n, diskonly, recursively, False, **kwargs) as blk:
+                        return blk[n]
 
-        if recursively:
+            if recursively:
 
-            for subreg in self._iter_subregs():
+                for subreg in self._iter_subregs():
 
-                with subreg._recursive_open(True) as subreg:
+                    with subreg._recursive_open(True) as subreg:
 
-                    try:
-                        return subreg.get(apri, n, diskonly, recursively, **kwargs)
+                        try:
+                            return subreg.get(apri, n, diskonly, recursively, **kwargs)
 
-                    except DataNotFoundError:
-                        pass
+                        except DataNotFoundError:
+                            pass
 
-        raise DataNotFoundError(
-            _blk_not_found_err_msg(diskonly, str(apri), n)
-        )
+            raise DataNotFoundError(
+                self._blk_not_found_err_msg(diskonly, str(apri), n)
+            )
+
+        finally:
+            self.get_elapsed += time() - start_time
 
     def __setitem__(self, apri_n_diskonly_recursively, value):
 
         apri, n, diskonly, recursively = Register._resolve_apri_n_diskonly_recursively(apri_n_diskonly_recursively)
         self.set(apri, n, value, diskonly, recursively)
 
     def set(self, apri, n, value, diskonly = False, recursively = False, **kwargs):
 
-        check_type(apri, "apri", ApriInfo)
+        start_time = time()
 
-        if isinstance(n, slice):
-            raise NotImplementedError("support for slices for Register.set coming soon.")
+        try:
+            # try clause followed by finally clause that increments `self.set_elapsed`
+            check_type(apri, "apri", ApriInfo)
 
-        n = check_return_int(n, "n")
-        check_type(diskonly, "diskonly", bool)
-        check_type(recursively, "recursively", bool)
+            if isinstance(n, slice):
+                raise NotImplementedError("support for slices for Register.set coming soon.")
 
-        if n < 0:
-            raise ValueError("`n` must be non-negative.")
+            n = check_return_int(n, "n")
+            check_type(diskonly, "diskonly", bool)
+            check_type(recursively, "recursively", bool)
 
-        if not diskonly:
+            if n < 0:
+                raise ValueError("`n` must be non-negative.")
+
+            if not diskonly:
+
+                for blk in self._ram_blks[apri]:
+
+                    if n in blk:
+
+                        blk[n] = value
+                        return
 
-            for blk in self._ram_blks:
+            try:
 
-                if n in blk:
+                with self.blk_by_n(apri, n, diskonly, False, False, **kwargs) as blk:
                     blk[n] = value
-                    return
 
-        try:
-            blk = self.blk_by_n(apri, n, diskonly, False, False, **kwargs)
+            except DataNotFoundError:
+                pass
 
-        except DataNotFoundError:
-            pass
+            else:
 
-        else:
+                self.rmv_disk_blk(apri, blk.startn(), len(blk), False, False)
 
-            blk[n] = value
-            self.rmv_disk_blk(apri, blk.startn(), len(blk), False, False)
-            self.add_disk_blk(blk)
-            return
+                with blk:
+                    self.add_disk_blk(blk)
 
-        if recursively:
+                return
 
-            for subreg in self._iter_subregs():
+            if recursively:
 
-                with subreg._recursive_open(True) as subreg:
+                for subreg in self._iter_subregs():
 
-                    try:
-                        return subreg.set(apri, n, value, diskonly, recursively, **kwargs)
+                    with subreg._recursive_open(True) as subreg:
 
-                    except DataNotFoundError:
-                        pass
+                        try:
+                            return subreg.set(apri, n, value, diskonly, recursively, **kwargs)
 
-        raise DataNotFoundError(
-            _blk_not_found_err_msg(diskonly, str(apri), n)
-        )
+                        except DataNotFoundError:
+                            pass
 
-    def intervals(self, apri, combine = False, diskonly = False, recursively = False):
+            raise DataNotFoundError(
+                self._blk_not_found_err_msg(diskonly, str(apri), n)
+            )
+
+        finally:
+            self.set_elapsed += time() - start_time
+
+    def intervals(self, apri, sort = False, combine = False, diskonly = False, recursively = False):
 
         self._check_open_raise("intervals")
         check_type(apri, "apri", ApriInfo)
         check_type(diskonly, "diskonly", bool)
         check_type(recursively, "recursively", bool)
 
-        yield from self._intervals_helper(apri, combine, diskonly, recursively, True)
+        if combine:
+
+            intervals_sorted = list(self.intervals(apri, True, False, diskonly, recursively))
+            ret = []
+
+            for startn, length in intervals_sorted:
+
+                if len(ret) == 0:
+                    ret.append((startn, length))
+
+                elif startn <= ret[-1][0] + ret[-1][1]:
+                    ret[-1] = (ret[-1][0], max(startn + length - ret[-1][0], ret[-1][1]))
+
+            yield from ret
+
+        elif not sort or (diskonly and not recursively):
+            # the LMDB database returns sorted keys, so we do not need to make any slow calls to Python sort functions
+            # if it is unnecessary to do so
+            yield from self._intervals_helper(apri, diskonly, recursively)
+
+        else:
+            # if not combine and sort and (not diskonly or recursively)
+            intervals = list(self._intervals_helper(apri, diskonly, recursively))
+            yield from sorted(intervals, key = lambda t: (t[0], -t[1]))
 
     def total_len(self, apri, diskonly = False, recursively = False):
 
         self._check_open_raise("total_len")
         check_type(apri, "apri", ApriInfo)
         check_type(diskonly, "diskonly", bool)
         check_type(recursively, "recursively", bool)
 
         try:
-            return sum(t[1] for t in self.intervals(apri, combine = True, diskonly = diskonly, recursively = recursively))
+            return sum(t[1] for t in self.intervals(apri, False, False, diskonly, recursively))
 
         except DataNotFoundError:
             return 0
 
     def num_blks(self, apri, diskonly = False, recursively = False):
 
         self._check_open_raise("num_blks")
@@ -2956,46 +3042,46 @@
         except DataNotFoundError:
 
             if not recursively:
                 raise
 
         else:
 
-            for startn, length in self.intervals(apri, combine = False, diskonly = diskonly, recursively = recursively):
+            for startn, length in self.intervals(apri, False, False, diskonly, recursively):
                 ret = startn + length - 1
 
         if recursively:
 
             for subreg in self._iter_subregs():
 
                 with subreg._recursive_open(True) as subreg:
 
                     try:
-                        ret = max(ret, subreg.maxn(apri, diskonly = diskonly, recursively = True))
+                        ret = max(ret, subreg.maxn(apri, diskonly, recursively))
 
                     except DataNotFoundError:
                         pass
 
         if ret == -1:
-            raise DataNotFoundError(_blk_not_found_err_msg(diskonly, apri))
+            raise DataNotFoundError(self._blk_not_found_err_msg(diskonly, apri))
 
         else:
             return ret
 
     def contains_index(self, apri, index, diskonly = False, recursively = False):
 
         check_type(apri, "apri", ApriInfo)
         index = check_return_int(index, "index")
         check_type(diskonly, "diskonly", bool)
         check_type(recursively, "recursively", bool)
 
         if index < 0:
             raise ValueError("`index` must be non-negative.")
 
-        for startn, length in self.intervals(apri, False, diskonly, recursively):
+        for startn, length in self.intervals(apri, False, False, diskonly, recursively):
 
             if startn <= index < startn + length:
                 return True
 
         else:
             return False
 
@@ -3005,15 +3091,15 @@
         startn = check_return_int(startn, "startn")
         length = check_return_int(length, "length")
         check_type(diskonly, "diskonly", bool)
         check_type(recursively, "recursively", bool)
 
         int1 = (startn, length)
 
-        for int2 in self.intervals(apri, True, diskonly, recursively):
+        for int2 in self.intervals(apri, True, True, diskonly, recursively):
 
             if intervals_overlap(int1, int2):
                 return intervals_subset(int1, int2)
 
         else:
             return False
 
@@ -3102,96 +3188,97 @@
             with lmdb_prefix_iter(txn if txn is not None else self._db, prefix) as it:
 
                 for key, _ in it:
                     return self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key, apri, None)[1:]
 
                 else:
                     raise DataNotFoundError(
-                        _blk_not_found_err_msg(True, apri, None, startn, None)
+                        self._blk_not_found_err_msg(True, apri, None, startn, None)
                     )
 
         else:
 
             prefix = _BLK_KEY_PREFIX + self._get_id_by_apri(apri, None, False, txn, None) + _KEY_SEP
 
             with lmdb_prefix_iter(self._db, prefix) as it:
 
                 for key, _ in it:
                     return self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key, apri, None)[1:]
 
                 else:
-                    raise DataNotFoundError(_blk_not_found_err_msg(True, apri))
+                    raise DataNotFoundError(self._blk_not_found_err_msg(True, apri))
 
-    def _intervals_helper(self, apri, combine, diskonly, recursively, root_call):
+    def _intervals_helper(self, apri, diskonly, recursively):
 
-        if not combine:
+        with self._db.begin() as txn:
 
-            with self._db.begin() as txn:
+            try:
+                self._check_known_apri(apri, txn)
 
-                try:
-                    self._check_known_apri(apri, txn)
+            except DataNotFoundError:
 
-                except DataNotFoundError:
+                if not recursively:
+                    raise
 
-                    if not recursively:
-                        raise
+            else:
 
-                else:
+                if not diskonly and apri in self._ram_blks.keys():
 
-                    if not diskonly and apri in self._ram_blks.keys():
+                    for blk in self._ram_blks[apri]:
 
-                        for blk in self._ram_blks[apri]:
+                        try:
+                            blk_len = len(blk)
 
-                            try:
-                                blk_len = len(blk)
+                        except BlockNotOpenError as e:
+                            raise BlockNotOpenError(
+                                _RAM_BLOCK_NOT_OPEN_ERROR_MESSAGE.format(apri, blk.startn())
+                            ) from e
 
-                            except BlockNotOpenError as e:
-                                raise BlockNotOpenError(
-                                    _RAM_BLOCK_NOT_OPEN_ERROR_MESSAGE.format(apri, blk.startn())
-                                ) from e
+                        yield blk.startn(), blk_len
 
-                            yield blk.startn(), blk_len
+                try:
 
-                    try:
+                    for key, _ in self._iter_disk_blk_pairs(_BLK_KEY_PREFIX, apri, None, txn):
+                        yield self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key, apri, txn)[1:]
 
-                        for key, _ in self._iter_disk_blk_pairs(_BLK_KEY_PREFIX, apri, None, txn):
-                            yield self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key, apri, txn)[1:]
+                except DataNotFoundError:
+                    pass
 
-                    except DataNotFoundError:
-                        pass
+        if recursively:
 
-            if recursively:
+            for subreg in self._iter_subregs():
 
-                for subreg in self._iter_subregs():
+                with subreg._recursive_open(True) as subreg:
+                    yield from subreg._intervals_helper(apri, diskonly, recursively)
 
-                    with subreg._recursive_open(True) as subreg:
-                        yield from subreg._intervals_helper(apri, combine, diskonly, recursively, False)
+    def _blk_not_found_err_msg(self, diskonly, apri, n = None, startn = None, length = None):
 
-        if combine and root_call:
+        if (startn is not None or length is not None) and n is not None:
+            raise ValueError
 
-            if (diskonly or len(self._ram_blks) == 0) and not recursively:
-                intervals_sorted = list(self._intervals_helper(apri, False, diskonly, recursively, False))
+        if startn is None and length is not None:
+            raise ValueError
 
-            else:
-                intervals_sorted = sorted(
-                    self._intervals_helper(apri, False, diskonly, recursively, False),
-                    key = lambda t: (t[0], -t[1])
-                )
+        if diskonly:
+            type_ = "disk"
 
-            ret = []
+        else:
+            type_ = "disk nor RAM"
 
-            for startn, length in intervals_sorted:
+        if n is not None:
+            return f"No {type_} `Block` found in `{self.shorthand()}` with the following data: {str(apri)}, n = {n}."
 
-                if len(ret) == 0:
-                    ret.append((startn, length))
+        elif startn is not None and length is None:
+            return f"No {type_} `Block` found in `{self.shorthand()}` with the following data: {str(apri)}, startn = {startn}."
 
-                elif startn <= ret[-1][0] + ret[-1][1]:
-                    ret[-1] = (ret[-1][0], max(startn + length - ret[-1][0], ret[-1][1]))
+        elif startn is not None and length is not None:
+            return f"No {type_} `Block` found in `{self.shorthand()}` with the following data: {str(apri)}, startn = {startn}, length = {length}."
 
-            yield from ret
+        else:
+            return f"No {type_} `Block` found in `{self.shorthand()}` with the following data: {str(apri)}."
 
 
 class PickleRegister(Register):
 
     @classmethod
     def with_suffix(cls, filename):
         return filename.with_suffix(".pkl")
@@ -3260,72 +3347,82 @@
                 "The keyword-argument `mmap_mode` for `Numpy_Register.blk` can only have the values " +
                 "`None`, 'r+', 'r', 'w+', 'c'. Please see " +
                 "https://numpy.org/doc/stable/reference/generated/numpy.memmap.html#numpy.memmap for more information."
             )
 
     def set(self, apri, n, value, diskonly = False, recursively = False, **kwargs):
 
-        check_type(apri, "apri", ApriInfo)
-
-        if isinstance(n, slice):
-            raise NotImplementedError("support for slices for NumpyRegister.set coming soon.")
-
-        n = check_return_int(n, "n")
-        check_type(diskonly, "diskonly", bool)
-        check_type(recursively, "recursively", bool)
+        set_elapsed = self.set_elapsed
+        start_time = time()
 
         try:
-            mmap_mode = kwargs['mmap_mode']
+            # try clause followed by finally clause that increments `self.add_elapsed`
+            check_type(apri, "apri", ApriInfo)
 
-        except KeyError:
-            mmap_mode = None
+            if isinstance(n, slice):
+                raise NotImplementedError("support for slices for NumpyRegister.set coming soon.")
 
-        else:
-            del kwargs['mmap_mode']
+            n = check_return_int(n, "n")
+            check_type(diskonly, "diskonly", bool)
+            check_type(recursively, "recursively", bool)
 
-        if mmap_mode is not None and mmap_mode != "r+":
-            raise ValueError("`mmap_mode` can either be `None` or 'r+'.")
+            try:
+                mmap_mode = kwargs['mmap_mode']
 
-        if not diskonly:
+            except KeyError:
+                mmap_mode = None
 
-            for blk in self._ram_blks:
+            else:
+                del kwargs['mmap_mode']
 
-                if n in blk:
-                    blk[n] = value
-                    return
+            if mmap_mode is not None and mmap_mode != "r+":
+                raise ValueError("`mmap_mode` can either be `None` or 'r+'.")
 
-        if mmap_mode is None:
+            if not diskonly:
 
-            super().set(apri, n, value, diskonly, recursively, **kwargs)
-            return
+                for blk in self._ram_blks:
 
-        else:
+                    if n in blk:
+                        blk[n] = value
+                        return
 
-            try:
-                blk = self.blk_by_n(apri, n, diskonly, False, False, mmap_mode = "r+", **kwargs)
+            if mmap_mode is None:
 
-            except DataNotFoundError:
-                pass
+                super().set(apri, n, value, diskonly, recursively, **kwargs)
+                return
 
             else:
-                blk.segment()[n, ...] = value
 
-        if recursively:
+                try:
 
-            for subreg in self._iter_subregs():
+                    with self.blk_by_n(apri, n, diskonly, False, False, mmap_mode = "r+", **kwargs) as blk:
+                        blk[n] = value
 
-                with subreg._recursive_open(True) as subreg:
+                    return
 
-                    try:
-                        return subreg.set(apri, n, value, diskonly, recursively, mmap_mode = mmap_mode, **kwargs)
+                except DataNotFoundError:
+                    pass
 
-                    except DataNotFoundError:
-                        pass
+            if recursively:
+
+                for subreg in self._iter_subregs():
+
+                    with subreg._recursive_open(True) as subreg:
+
+                        try:
+                            return subreg.set(apri, n, value, diskonly, recursively, mmap_mode = mmap_mode, **kwargs)
+
+                        except DataNotFoundError:
+                            pass
+
+            raise DataNotFoundError(self._blk_not_found_err_msg(diskonly, str(apri), n))
+
+        finally:
+            self.set_elapsed = set_elapsed + time() - start_time
 
-        raise DataNotFoundError(_blk_not_found_err_msg(diskonly, str(apri), n))
 
     @contextmanager
     def blk(self, apri, startn = None, length = None, diskonly = False, recursively = False, ret_metadata = False, **kwargs):
         """
         :param apri: (type `ApriInfo`)
         :param startn: (type `int`)
         :param length: (type `length_`) non-negative
@@ -3413,15 +3510,15 @@
         # ones and, when ties occur, larger lengths before smaller ones.
         if length is None:
             # infer length
 
             current_segment = False
             length = 0
 
-            for startn_, length_ in self.intervals(apri, combine = False, diskonly = False):
+            for startn_, length_ in self.intervals(apri, True, False, True, False):
 
                 if length_ > 0:
 
                     if current_segment:
 
                         if startn > startn_:
                             raise RuntimeError("Could not infer a value for `length`.")
@@ -3443,15 +3540,15 @@
 
                             else:
                                 break
 
                     else:
 
                         if startn < startn_:
-                            raise DataNotFoundError(_blk_not_found_err_msg(True, apri, None, startn))
+                            raise DataNotFoundError(self._blk_not_found_err_msg(True, apri, None, startn))
 
                         elif startn == startn_:
 
                             length += length_
                             current_segment = True
 
             if length == 0:
@@ -3463,15 +3560,15 @@
 
         last_check = False
         last_startn_ = None
         startn_ = None
         length_ = None
         intervals_to_get = []
 
-        for startn_, length_ in self.intervals(apri, combine = False, diskonly = True):
+        for startn_, length_ in self.intervals(apri, True, False, True, False):
             # infer blocks to combine
 
             if last_check:
 
                 if last_startn_ == startn_ and length_ > 0:
                     raise ValueError(f"Overlapping `Block` intervals found with {str(apri)}.")
 
@@ -3533,15 +3630,15 @@
 
                         else:
                             raise ValueError(f"Overlapping `Block` intervals found with {str(apri)}.")
 
         else:
 
             if startn_ is None:
-                raise DataNotFoundError(_blk_not_found_err_msg(True, apri))
+                raise DataNotFoundError(self._blk_not_found_err_msg(True, apri))
 
             elif startn_ + length_ != startn + length:
                 raise ValueError(
                     f"The last `Block` does not have the right size. "
                     f"Try again by calling `reg.concat_disk_blks(info, {startn}, {startn_ + length_})`."
                 )
 
@@ -3629,36 +3726,47 @@
             else:
                 raise e
 
         return ret
 
 def _element_iter(reg, apri, slice_, diskonly, recursively, kwargs):
 
-    n = slice_.start if slice_.start is not None else 0
+    if slice_.start is None:
+
+        for startn, _ in reg.intervals(apri, True, False, diskonly, recursively):
+            break
+
+        else:
+            return
+
+        n = startn
+
+    else:
+        n = slice_.start
+
     stop = slice_.stop
     step = slice_.step if slice_.step is not None else 1
 
     while True:
 
         try:
-            blk_contextmanager = reg.blk_by_n(apri, n, diskonly, recursively, False, **kwargs)
-
-        except DataNotFoundError:
-            return
 
-        with blk_contextmanager as blk:
+            with reg.blk_by_n(apri, n, diskonly, recursively, False, **kwargs) as blk:
+                # raises DataNotFoundError
+                while n in blk and (stop is None or n < stop):
 
-            while n < stop and n in blk:
+                    yield blk[n]
+                    n += step
 
-                yield blk[n]
-                n += step
-
-            if n >= stop:
+            if stop is not None and n >= stop:
                 return
 
+        except DataNotFoundError:
+            return
+
 class _CopyRegister(Register):
 
     @classmethod
     def with_suffix(cls, filename):
         return filename
 
     @classmethod
```

### Comparing `cornifer-0.8/lib/cornifer/regloader.py` & `cornifer-0.8.1/lib/cornifer/regloader.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/lib/cornifer/version.py` & `cornifer-0.8.1/lib/cornifer/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 """
 
-CURRENT_VERSION          = "0.8"
-COMPATIBLE_VERSIONS      = ["0.8"]
+CURRENT_VERSION          = "0.8.1"
+COMPATIBLE_VERSIONS      = ["0.8", "0.8.1"]
```

### Comparing `cornifer-0.8/setup.py` & `cornifer-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/tests/test_blocks.py` & `cornifer-0.8.1/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/tests/test_info.py` & `cornifer-0.8.1/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/tests/test_register_file_structure.py` & `cornifer-0.8.1/tests/test_register_file_structure.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.8/tests/test_registers.py` & `cornifer-0.8.1/tests/test_registers.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,20 +269,20 @@
         #     )
 
     def test___str__(self):
 
         reg = Testy_Register(SAVES_DIR, "sh", "hello")
         self.assertEqual(
             str(reg),
-            f"sh: \"hello\""
+            f"sh: hello"
         )
         with reg.open() as reg:pass
         self.assertEqual(
             str(reg),
-            f"sh ({reg._local_dir}): \"hello\""
+            f"sh ({reg._local_dir}): hello"
         )
 
     def test___repr__(self):
 
         self.assertEqual(
             repr(Testy_Register(SAVES_DIR, "sh", "hello")),
             f"Testy_Register(\"{str(SAVES_DIR)}\", \"sh\", \"hello\", {_INITIAL_REGISTER_SIZE_DEFAULT})"
@@ -720,22 +720,22 @@
         except RegisterError as e:
             if "has not been opened" in str(e):
                 self.fail("the register doesn't need to be open for set_msg")
             else:
                 raise e
 
         self.assertEqual(
-            "sh: \"yes\"",
+            "sh: yes",
             str(reg)
         )
         with reg.open() as reg:pass
         reg.set_msg("no")
 
         self.assertEqual(
-            f"sh ({reg._local_dir}): \"no\"",
+            f"sh ({reg._local_dir}): no",
             str(reg)
         )
 
     def test_add_disk_block(self):
 
         reg = Testy_Register(SAVES_DIR, "sh", "sup")
         blk = Block([], ApriInfo(name ="hi"))
@@ -4600,20 +4600,20 @@
             self._composite_helper(reg, block_datas, apris)
 
             new_message = "\\\\new msg\"\"\\'"
             reg.set_msg(new_message)
 
             self.assertEqual(
                 str(reg),
-                f'sh ({reg._local_dir}): "\\\\new msg""\\\'"'
+                f'sh ({reg._local_dir}): \\\\new msg""\\\''
             )
 
         self.assertEqual(
             str(reg),
-            f'sh ({reg._local_dir}): "\\\\new msg""\\\'"'
+            f'sh ({reg._local_dir}): \\\\new msg""\\\''
         )
 
         reg = load(reg._local_dir)
 
         with reg.open() as reg:
 
             inner_inner_apri = ApriInfo(inner_apri = inner_apri)
```

