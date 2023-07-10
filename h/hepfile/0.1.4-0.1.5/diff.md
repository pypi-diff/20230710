# Comparing `tmp/hepfile-0.1.4.tar.gz` & `tmp/hepfile-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hepfile-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hepfile-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hepfile-0.1.4.tar` & `hepfile-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     2975 2023-07-07 14:08:15.978160 hepfile-0.1.4/README.md
--rw-r--r--   0        0        0     1782 2023-07-07 14:08:15.986160 hepfile-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      506 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/__init__.py
--rw-r--r--   0        0        0       76 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/_version.py
--rw-r--r--   0        0        0     7823 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/awkward_tools.py
--rw-r--r--   0        0        0      402 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/constants.py
--rw-r--r--   0        0        0     1757 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/csv_tools.py
--rw-r--r--   0        0        0     8405 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/df_tools.py
--rw-r--r--   0        0        0     6843 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/dict_tools.py
--rw-r--r--   0        0        0     1452 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/errors.py
--rw-r--r--   0        0        0        0 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/py.typed
--rw-r--r--   0        0        0    21124 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/read.py
--rw-r--r--   0        0        0    28546 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/write.py
--rw-r--r--   0        0        0     4590 1970-01-01 00:00:00.000000 hepfile-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11389 2023-07-10 16:29:56.189257 hepfile-0.1.5/LICENSE
+-rw-r--r--   0        0        0     8357 2023-07-10 16:29:56.189257 hepfile-0.1.5/README.md
+-rw-r--r--   0        0        0     1912 2023-07-10 16:29:56.209257 hepfile-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1346 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/__init__.py
+-rw-r--r--   0        0        0       76 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/_version.py
+-rw-r--r--   0        0        0     8051 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/awkward_tools.py
+-rw-r--r--   0        0        0      402 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/constants.py
+-rw-r--r--   0        0        0     1764 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/csv_tools.py
+-rw-r--r--   0        0        0     8548 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/df_tools.py
+-rw-r--r--   0        0        0     7291 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/dict_tools.py
+-rw-r--r--   0        0        0     1935 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/errors.py
+-rw-r--r--   0        0        0        0 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/py.typed
+-rw-r--r--   0        0        0    21588 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/read.py
+-rw-r--r--   0        0        0    28372 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/write.py
+-rw-r--r--   0        0        0    10227 1970-01-01 00:00:00.000000 hepfile-0.1.5/PKG-INFO
```

### Comparing `hepfile-0.1.4/src/hepfile/awkward_tools.py` & `hepfile-0.1.5/src/hepfile/awkward_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 and hepfile data objects easier.
 """
 from __future__ import annotations
 
 import warnings
 import awkward as ak
 import numpy as np
-from .write import (
+from hepfile.write import (
     initialize,
     create_group,
     create_dataset,
     write_to_file,
     create_single_bucket,
     pack,
 )
-from .errors import AwkwardStructureError, InputError
+from hepfile.errors import AwkwardStructureError, InputError
 
 
 ################################################################################
 def hepfile_to_awkward(
     data: dict, groups: list = None, datasets: list = None
 ) -> ak.Record:
     """
@@ -168,14 +168,22 @@
                 name = f"{group}/{dataset}"
                 bucket[name] = data_dict[group][dataset].to_list()
         pack(data, bucket)
 
     # then write it out to a file
     if write_hepfile:
         print("Writing the hdf5 file from the awkward array...")
+
+        for key, item in data.items():
+            if isinstance(item, (ak.Record, ak.Array)):
+                try:
+                    data[key] = ak.to_numpy(item)
+                except:
+                    data[key] = ak.to_list(item)
+
         write_to_file(outfile, data)
 
     return data
 
 
 def _awkward_depth(ak_array: ak.Record) -> int:
     max_depth = 0
@@ -197,15 +205,15 @@
     Checks if the input awkward array is valid and raises an exception if not
 
     Args:
         ak_array (ak.Array): awkward array to check
     """
 
     # validate input array
-    if not isinstance(ak_array, ak.Array) and not isinstance(ak_array, ak.Record):
+    if not isinstance(ak_array, (ak.Array, ak.Record)):
         raise AwkwardStructureError("Please input an Awkward Array or Awkward Record")
 
     if ak_array.fields == 0:
         raise AwkwardStructureError(
             "Your input Awkward Array must be a Record. \
             This means it needs to have fields in it."
         )
```

### Comparing `hepfile-0.1.4/src/hepfile/csv_tools.py` & `hepfile-0.1.5/src/hepfile/csv_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from __future__ import annotations
 
 import os
 from typing import Optional
 
 import pandas as pd
-from .df_tools import df_to_hepfile
+from hepfile.df_tools import df_to_hepfile
 
 
 def csv_to_hepfile(
     csvpaths: list[str],
     common_key: str,
     outfile: Optional[str] = None,
     group_names: Optional[list] = None,
```

### Comparing `hepfile-0.1.4/src/hepfile/df_tools.py` & `hepfile-0.1.5/src/hepfile/df_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Tools to work with Pandas DataFrames and Hepfile data
 """
 from __future__ import annotations
 
 import pandas as pd
-import awkward as ak
-from .errors import InputError
-from .dict_tools import dictlike_to_hepfile
+import hepfile as hf
+from hepfile.errors import InputError, MissingOptionalDependency
+from hepfile.dict_tools import dictlike_to_hepfile
 
 
 def hepfile_to_df(
     data: dict,
     groups: list[str] = None,
     events: list[int] = None,
 ) -> dict[pd.DataFrame]:
@@ -106,14 +106,19 @@
         events [list]: list of event indexes to include
 
     Returns:
         Dictionary of requested groups as dataframes where the keys are the group names.
         If only one group is requested then it just returns a dataframe of that group.
     """
 
+    if not hf._AWKWARD:
+        raise MissingOptionalDependency("awkward")
+
+    import awkward as ak
+
     dfs = {}  # list to of dataframes to return
 
     # check inputs
     if not groups is None and not isinstance(groups, (list, str)):
         raise InputError("groups must be either a list or a string")
 
     if not events is None and not isinstance(events, (list, int)):
```

### Comparing `hepfile-0.1.4/src/hepfile/dict_tools.py` & `hepfile-0.1.5/src/hepfile/dict_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 """
 Functions to help convert dictionaries into hepfiles
 """
 from __future__ import annotations
 
 import warnings
-import awkward as ak
 import numpy as np
 
-from .awkward_tools import awkward_to_hepfile, _is_valid_awkward
-from .errors import AwkwardStructureError, DictStructureError, InputError
-from .write import (
+import hepfile as hf
+from hepfile.errors import (
+    AwkwardStructureError,
+    DictStructureError,
+    InputError,
+    MissingOptionalDependency,
+)
+from hepfile.write import (
     initialize,
     write_to_file,
     create_dataset,
     create_group,
     pack,
     create_single_bucket,
 )
 
 
 def dictlike_to_hepfile(
-    dict_list: list[dict], outfile: str = None, how_to_pack="awkward", **kwargs
-) -> ak.Record:
+    dict_list: list[dict], outfile: str = None, how_to_pack="classic", **kwargs
+) -> dict:
     """
     This wraps on `hepfile.awkward_tools.awkward_to_hepfile`
     and writes a list of dictionaries to a hepfile.
 
     Writes a list of dictlike object to a hepfile. Must have a specific format:
     - each dictlike object is a "event"
     - first level of dict keys are the groups
@@ -52,14 +56,17 @@
             dict_list = [dict_list[key].to_dict() for key in dict_list.to_dict()]
         except Exception as exc:
             raise InputError(
                 "Please input either a dataframe or list \
             of dictionaries"
             ) from exc
 
+    if how_to_pack == "awkward" and not hf._AWKWARD:
+        raise MissingOptionalDependency("awkward")
+
     # validate input dictionary
     keys = dict_list[0].keys()
     for item in dict_list:
         if item.keys() != keys:
             raise InputError(
                 "Keys must match across the entire input dictionary list!!!"
             )
@@ -87,15 +94,15 @@
         return _classic(dict_list, outfile, **kwargs)
 
     raise InputError("how_to_pack should either be 'awkward' or 'classic'")
 
 
 def _classic(
     dict_list: dict, outfile: str = None, write_hepfile=True, ignore_protected=False
-) -> ak.Record:
+) -> dict:
     """Private method to convert a list of events to a hepfile using the traditional method"""
 
     if outfile is None and write_hepfile:
         raise InputError("if write_hepfile is True, and outfile name must be provided")
 
     # first create the group names and dataset names
     data = initialize()
@@ -146,14 +153,21 @@
     if write_hepfile:
         write_to_file(outfile, data)
     return data
 
 
 def _awkward(dict_list: list[dict], outfile: str = None, **kwargs):
     """Private method to convert a list of events to a hepfile using awkward arrays"""
+
+    if not hf._AWKWARD:
+        raise MissingOptionalDependency("awkward")
+
+    import awkward as ak
+    from hepfile.awkward_tools import awkward_to_hepfile, _is_valid_awkward
+
     # convert dictionary list to  an awkward array and write to hepfile
     out_ak = ak.Array(dict_list)
 
     # catch an awkward structure error and instead return a dictionary structure error
     try:
         awkward_to_hepfile(out_ak, outfile, **kwargs)
     except AwkwardStructureError as err:
@@ -168,14 +182,19 @@
 
     Args:
         ak_dict (ak.Record): awkward Record of data
         new_dict (dict): Dictionary of value to append to ak_dict. All keys must match ak_dict!
     Return:
         Awkward Record of awkward arrays with the new_dict appended
     """
+    if not hf._AWKWARD:
+        raise MissingOptionalDependency("awkward")
+
+    import awkward as ak
+    from hepfile.awkward_tools import awkward_to_hepfile, _is_valid_awkward
 
     _is_valid_awkward(ak_dict)
 
     if sorted(list(new_dict.keys())) != sorted(ak_dict.fields):
         raise InputError(
             f"Keys of new array do not match keys of existing array!\nExisting \
             Array Keys: {ak_dict.fields}\nNew Dictionary Keys: {new_dict.keys()}"
```

### Comparing `hepfile-0.1.4/src/hepfile/read.py` & `hepfile-0.1.5/src/hepfile/read.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,24 @@
 """
 
 from __future__ import annotations
 
 import warnings
 import h5py as h5
 import numpy as np
-import pandas as pd
-from . import constants
-from .errors import RangeSubsetError, InputError, MetadataNotFound, HeaderNotFound
-from .awkward_tools import hepfile_to_awkward
-from .df_tools import hepfile_to_df
+
+import hepfile as hf
+from hepfile import constants
+from hepfile.errors import (
+    RangeSubsetError,
+    InputError,
+    MetadataNotFound,
+    HeaderNotFound,
+    MissingOptionalDependency,
+)
 
 
 ################################################################################
 def load(
     filename: str,
     verbose: bool = False,
     desired_groups: list[str] = None,
@@ -44,14 +49,20 @@
         bucket (dict): An empty bucket dictionary to be filled by data from select buckets
 
     """
 
     if return_type not in {"dictionary", "awkward", "pandas"}:
         raise InputError("return_type must be dictionary, awkward, or pandas")
 
+    if return_type == "awkward" and not hf._AWKWARD:
+        raise MissingOptionalDependency(return_type)
+
+    if return_type == "pandas" and not hf._PANDAS:
+        raise MissingOptionalDependency(return_type)
+
     with h5.File(filename, "r+") as infile:
         # Create the initial data and bucket dictionary to hold the data
         data = {}
         bucket = {}
 
         # We'll fill the data dictionary with some extra fields, though we won't
         # need them all for the bucket
@@ -344,17 +355,21 @@
 
     data["_MAP_DATASETS_TO_DATA_TYPES_"] = dtypes
 
     # 3) add _PROTECTED_NAMES_
     data["_PROTECTED_NAMES_"] = constants.protected_names
 
     if return_type == "awkward":
+        from hepfile.awkward_tools import hepfile_to_awkward
+
         return hepfile_to_awkward(data), bucket
 
     if return_type == "pandas":
+        from hepfile.df_tools import hepfile_to_df
+
         return hepfile_to_df(data), bucket
 
     return data, bucket
 
 
 ################################################################################
 
@@ -479,14 +494,19 @@
 
     return_type(string): If 'dict' return the header information as a dictionary.
                          If 'df' or 'dataframe', return the information as a
                          pandas dataframe.
 
     """
 
+    if return_type in {"df", "dataframe"}:
+        if not hf._PANDAS:
+            raise MissingOptionalDependency("pandas")
+        import pandas as pd
+
     if return_type is not None and return_type not in ["dict", "df", "dataframe"]:
         print("'return_type' must be 'dict', 'df', or 'dataframe'")
         print("Not returning any header information")
         return None
 
     with h5.File(filename, "r+") as infile:
         if "_HEADER_" not in infile:
```

### Comparing `hepfile-0.1.4/src/hepfile/write.py` & `hepfile-0.1.5/src/hepfile/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 from __future__ import annotations
 
 import datetime
 import sys
 import warnings
 
 import numpy as np
-import awkward as ak
 import h5py as h5
 
 import hepfile
-from . import constants
-from .errors import InputError, DatasetSizeDiscrepancy, MissingSingletonValue
+from hepfile import constants
+from hepfile.errors import InputError, DatasetSizeDiscrepancy, MissingSingletonValue
 
 
 ################################################################################
 def initialize() -> dict:
     """Creates an empty data dictionary
 
     Returns:
@@ -559,15 +558,14 @@
                     del hdoutfile.attrs[key]
 
         if write_default_values:
             hdoutfile.attrs["date"] = datetime.datetime.now().isoformat(sep=" ")
             hdoutfile.attrs["hepfile_version"] = hepfile.__version__
             hdoutfile.attrs["numpy_version"] = np.__version__
             hdoutfile.attrs["h5py_version"] = h5.__version__
-            hdoutfile.attrs["awkward_version"] = ak.__version__
             hdoutfile.attrs["python_version"] = sys.version
 
         if mydict is not None:
             for key in mydict:
                 hdoutfile.attrs[key] = mydict[key]
 
     print("Metadata added")
@@ -732,16 +730,14 @@
                     x = np.array(x)
 
                 # Do single precision only, unless specified
                 if force_single_precision:
                     # different type calls depending on input datastructure
                     if isinstance(x, np.ndarray):
                         dtype = x.dtype
-                    elif isinstance(x, (ak.Array, ak.Record)):
-                        dtype = x.type
                     else:
                         dtype = None
                         warnings.warn(
                             "Not a proper data type to convert to single precision, skipping!"
                         )
 
                     if dtype == np.float64:
```

