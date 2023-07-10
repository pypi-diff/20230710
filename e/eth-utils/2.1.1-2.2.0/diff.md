# Comparing `tmp/eth-utils-2.1.1.tar.gz` & `tmp/eth-utils-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-utils-2.1.1.tar", last modified: Wed Jun  7 17:24:29 2023, max compression
+gzip compressed data, was "eth-utils-2.2.0.tar", last modified: Mon Jul 10 20:55:01 2023, max compression
```

## Comparing `eth-utils-2.1.1.tar` & `eth-utils-2.2.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-07 17:24:29.249112 eth-utils-2.1.1/
--rw-r--r--   0 eve        (501) staff       (20)     1095 2023-06-07 17:14:58.000000 eth-utils-2.1.1/LICENSE
--rw-r--r--   0 eve        (501) staff       (20)      141 2023-06-07 17:14:58.000000 eth-utils-2.1.1/MANIFEST.in
--rw-r--r--   0 eve        (501) staff       (20)     3215 2023-06-07 17:24:29.248895 eth-utils-2.1.1/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     2312 2023-06-07 17:14:58.000000 eth-utils-2.1.1/README.md
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-07 17:24:29.246655 eth-utils-2.1.1/eth_utils/
--rw-r--r--   0 eve        (501) staff       (20)     2340 2023-06-07 17:14:58.000000 eth-utils-2.1.1/eth_utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)       77 2021-11-15 18:52:39.000000 eth-utils-2.1.1/eth_utils/__main__.py
--rw-r--r--   0 eve        (501) staff       (20)     2088 2021-11-15 18:53:08.000000 eth-utils-2.1.1/eth_utils/abi.py
--rw-r--r--   0 eve        (501) staff       (20)     4274 2023-06-07 17:14:58.000000 eth-utils-2.1.1/eth_utils/address.py
--rw-r--r--   0 eve        (501) staff       (20)     4360 2021-11-15 18:53:08.000000 eth-utils-2.1.1/eth_utils/applicators.py
--rw-r--r--   0 eve        (501) staff       (20)     5382 2023-06-07 17:14:58.000000 eth-utils-2.1.1/eth_utils/conversions.py
--rw-r--r--   0 eve        (501) staff       (20)      275 2021-11-15 18:52:39.000000 eth-utils-2.1.1/eth_utils/crypto.py
--rw-r--r--   0 eve        (501) staff       (20)     3046 2022-11-17 21:10:46.000000 eth-utils-2.1.1/eth_utils/currency.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-07 17:24:29.247974 eth-utils-2.1.1/eth_utils/curried/
--rw-r--r--   0 eve        (501) staff       (20)     6362 2023-06-07 17:14:58.000000 eth-utils-2.1.1/eth_utils/curried/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      505 2023-06-07 17:14:58.000000 eth-utils-2.1.1/eth_utils/debug.py
--rw-r--r--   0 eve        (501) staff       (20)     3895 2021-11-15 18:53:08.000000 eth-utils-2.1.1/eth_utils/decorators.py
--rw-r--r--   0 eve        (501) staff       (20)      199 2021-11-15 18:52:39.000000 eth-utils-2.1.1/eth_utils/encoding.py
--rw-r--r--   0 eve        (501) staff       (20)      120 2021-11-15 18:52:39.000000 eth-utils-2.1.1/eth_utils/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)     2091 2021-11-15 18:52:39.000000 eth-utils-2.1.1/eth_utils/functional.py
--rw-r--r--   0 eve        (501) staff       (20)     1833 2022-07-22 16:53:39.000000 eth-utils-2.1.1/eth_utils/hexadecimal.py
--rw-r--r--   0 eve        (501) staff       (20)     3847 2021-11-15 18:53:08.000000 eth-utils-2.1.1/eth_utils/humanize.py
--rw-r--r--   0 eve        (501) staff       (20)     5196 2023-06-07 17:14:58.000000 eth-utils-2.1.1/eth_utils/logging.py
--rw-r--r--   0 eve        (501) staff       (20)      867 2021-11-15 18:53:08.000000 eth-utils-2.1.1/eth_utils/module_loading.py
--rw-r--r--   0 eve        (501) staff       (20)     1162 2021-11-15 18:52:39.000000 eth-utils-2.1.1/eth_utils/numeric.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-11-15 18:52:39.000000 eth-utils-2.1.1/eth_utils/py.typed
--rw-r--r--   0 eve        (501) staff       (20)     2617 2021-11-18 22:52:05.000000 eth-utils-2.1.1/eth_utils/toolz.py
--rw-r--r--   0 eve        (501) staff       (20)     1065 2021-11-15 18:52:39.000000 eth-utils-2.1.1/eth_utils/types.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-07 17:24:29.248515 eth-utils-2.1.1/eth_utils/typing/
--rw-r--r--   0 eve        (501) staff       (20)      339 2021-11-15 18:52:39.000000 eth-utils-2.1.1/eth_utils/typing/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      181 2021-11-15 18:52:39.000000 eth-utils-2.1.1/eth_utils/typing/misc.py
--rw-r--r--   0 eve        (501) staff       (20)     1757 2021-11-15 18:52:39.000000 eth-utils-2.1.1/eth_utils/units.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-07 17:24:29.247840 eth-utils-2.1.1/eth_utils.egg-info/
--rw-r--r--   0 eve        (501) staff       (20)     3215 2023-06-07 17:24:27.000000 eth-utils-2.1.1/eth_utils.egg-info/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)      813 2023-06-07 17:24:29.000000 eth-utils-2.1.1/eth_utils.egg-info/SOURCES.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2023-06-07 17:24:27.000000 eth-utils-2.1.1/eth_utils.egg-info/dependency_links.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2021-11-15 19:07:08.000000 eth-utils-2.1.1/eth_utils.egg-info/not-zip-safe
--rw-r--r--   0 eve        (501) staff       (20)      739 2023-06-07 17:24:27.000000 eth-utils-2.1.1/eth_utils.egg-info/requires.txt
--rw-r--r--   0 eve        (501) staff       (20)       10 2023-06-07 17:24:27.000000 eth-utils-2.1.1/eth_utils.egg-info/top_level.txt
--rw-r--r--   0 eve        (501) staff       (20)     1221 2023-06-07 17:14:58.000000 eth-utils-2.1.1/pyproject.toml
--rw-r--r--   0 eve        (501) staff       (20)       38 2023-06-07 17:24:29.249161 eth-utils-2.1.1/setup.cfg
--rw-r--r--   0 eve        (501) staff       (20)     2671 2023-06-07 17:22:56.000000 eth-utils-2.1.1/setup.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-10 20:55:01.716049 eth-utils-2.2.0/
+-rw-r--r--   0 eve        (501) staff       (20)     1095 2023-06-07 17:14:58.000000 eth-utils-2.2.0/LICENSE
+-rw-r--r--   0 eve        (501) staff       (20)      141 2023-06-07 17:14:58.000000 eth-utils-2.2.0/MANIFEST.in
+-rw-r--r--   0 eve        (501) staff       (20)     3215 2023-07-10 20:55:01.715852 eth-utils-2.2.0/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     2312 2023-06-07 17:14:58.000000 eth-utils-2.2.0/README.md
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-10 20:55:01.713943 eth-utils-2.2.0/eth_utils/
+-rw-r--r--   0 eve        (501) staff       (20)     2358 2023-07-10 20:49:46.000000 eth-utils-2.2.0/eth_utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)       77 2021-11-15 18:52:39.000000 eth-utils-2.2.0/eth_utils/__main__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2088 2021-11-15 18:53:08.000000 eth-utils-2.2.0/eth_utils/abi.py
+-rw-r--r--   0 eve        (501) staff       (20)     4274 2023-06-07 17:14:58.000000 eth-utils-2.2.0/eth_utils/address.py
+-rw-r--r--   0 eve        (501) staff       (20)     4360 2021-11-15 18:53:08.000000 eth-utils-2.2.0/eth_utils/applicators.py
+-rw-r--r--   0 eve        (501) staff       (20)     5382 2023-06-07 17:14:58.000000 eth-utils-2.2.0/eth_utils/conversions.py
+-rw-r--r--   0 eve        (501) staff       (20)      275 2021-11-15 18:52:39.000000 eth-utils-2.2.0/eth_utils/crypto.py
+-rw-r--r--   0 eve        (501) staff       (20)     3046 2022-11-17 21:10:46.000000 eth-utils-2.2.0/eth_utils/currency.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-10 20:55:01.715190 eth-utils-2.2.0/eth_utils/curried/
+-rw-r--r--   0 eve        (501) staff       (20)     6380 2023-07-10 20:49:46.000000 eth-utils-2.2.0/eth_utils/curried/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      505 2023-06-07 17:14:58.000000 eth-utils-2.2.0/eth_utils/debug.py
+-rw-r--r--   0 eve        (501) staff       (20)     3895 2021-11-15 18:53:08.000000 eth-utils-2.2.0/eth_utils/decorators.py
+-rw-r--r--   0 eve        (501) staff       (20)      199 2021-11-15 18:52:39.000000 eth-utils-2.2.0/eth_utils/encoding.py
+-rw-r--r--   0 eve        (501) staff       (20)      120 2021-11-15 18:52:39.000000 eth-utils-2.2.0/eth_utils/exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)     2091 2021-11-15 18:52:39.000000 eth-utils-2.2.0/eth_utils/functional.py
+-rw-r--r--   0 eve        (501) staff       (20)     1833 2022-07-22 16:53:39.000000 eth-utils-2.2.0/eth_utils/hexadecimal.py
+-rw-r--r--   0 eve        (501) staff       (20)     4157 2023-07-10 20:49:46.000000 eth-utils-2.2.0/eth_utils/humanize.py
+-rw-r--r--   0 eve        (501) staff       (20)     5196 2023-06-07 17:14:58.000000 eth-utils-2.2.0/eth_utils/logging.py
+-rw-r--r--   0 eve        (501) staff       (20)      867 2021-11-15 18:53:08.000000 eth-utils-2.2.0/eth_utils/module_loading.py
+-rw-r--r--   0 eve        (501) staff       (20)     1162 2021-11-15 18:52:39.000000 eth-utils-2.2.0/eth_utils/numeric.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-11-15 18:52:39.000000 eth-utils-2.2.0/eth_utils/py.typed
+-rw-r--r--   0 eve        (501) staff       (20)     2617 2021-11-18 22:52:05.000000 eth-utils-2.2.0/eth_utils/toolz.py
+-rw-r--r--   0 eve        (501) staff       (20)     1065 2021-11-15 18:52:39.000000 eth-utils-2.2.0/eth_utils/types.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-10 20:55:01.715621 eth-utils-2.2.0/eth_utils/typing/
+-rw-r--r--   0 eve        (501) staff       (20)      339 2021-11-15 18:52:39.000000 eth-utils-2.2.0/eth_utils/typing/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      181 2021-11-15 18:52:39.000000 eth-utils-2.2.0/eth_utils/typing/misc.py
+-rw-r--r--   0 eve        (501) staff       (20)     1757 2021-11-15 18:52:39.000000 eth-utils-2.2.0/eth_utils/units.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-10 20:55:01.715041 eth-utils-2.2.0/eth_utils.egg-info/
+-rw-r--r--   0 eve        (501) staff       (20)     3215 2023-07-10 20:54:59.000000 eth-utils-2.2.0/eth_utils.egg-info/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)      813 2023-07-10 20:55:01.000000 eth-utils-2.2.0/eth_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-07-10 20:54:59.000000 eth-utils-2.2.0/eth_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2021-11-15 19:07:08.000000 eth-utils-2.2.0/eth_utils.egg-info/not-zip-safe
+-rw-r--r--   0 eve        (501) staff       (20)      739 2023-07-10 20:54:59.000000 eth-utils-2.2.0/eth_utils.egg-info/requires.txt
+-rw-r--r--   0 eve        (501) staff       (20)       10 2023-07-10 20:54:59.000000 eth-utils-2.2.0/eth_utils.egg-info/top_level.txt
+-rw-r--r--   0 eve        (501) staff       (20)     1221 2023-06-07 17:14:58.000000 eth-utils-2.2.0/pyproject.toml
+-rw-r--r--   0 eve        (501) staff       (20)       38 2023-07-10 20:55:01.716096 eth-utils-2.2.0/setup.cfg
+-rw-r--r--   0 eve        (501) staff       (20)     2671 2023-07-10 20:54:04.000000 eth-utils-2.2.0/setup.py
```

### Comparing `eth-utils-2.1.1/LICENSE` & `eth-utils-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/PKG-INFO` & `eth-utils-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-utils
-Version: 2.1.1
+Version: 2.2.0
 Summary: eth-utils: Common utility functions for python code that interacts with Ethereum
 Home-page: https://github.com/ethereum/eth-utils
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Intended Audience :: Developers
```

### Comparing `eth-utils-2.1.1/README.md` & `eth-utils-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/__init__.py` & `eth-utils-2.2.0/eth_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 )
 from .humanize import (  # noqa: F401
     humanize_bytes,
     humanize_hash,
     humanize_integer_sequence,
     humanize_ipfs_uri,
     humanize_seconds,
+    humanize_wei,
 )
 from .logging import (  # noqa: F401
     DEBUG2_LEVEL_NUM,
     ExtendedDebugLogger,
     HasExtendedDebugLogger,
     HasExtendedDebugLoggerMeta,
     HasLogger,
```

### Comparing `eth-utils-2.1.1/eth_utils/abi.py` & `eth-utils-2.2.0/eth_utils/abi.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/address.py` & `eth-utils-2.2.0/eth_utils/address.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/applicators.py` & `eth-utils-2.2.0/eth_utils/applicators.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/conversions.py` & `eth-utils-2.2.0/eth_utils/conversions.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/currency.py` & `eth-utils-2.2.0/eth_utils/currency.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/curried/__init__.py` & `eth-utils-2.2.0/eth_utils/curried/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 )
 from eth_utils import (
     humanize_bytes,
     humanize_hash,
     humanize_integer_sequence,
     humanize_ipfs_uri,
     humanize_seconds,
+    humanize_wei,
     import_string,
     int_to_big_endian,
     is_0x_prefixed,
     is_address,
     is_binary_address,
     is_boolean,
     is_bytes,
```

### Comparing `eth-utils-2.1.1/eth_utils/decorators.py` & `eth-utils-2.2.0/eth_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/functional.py` & `eth-utils-2.2.0/eth_utils/functional.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/hexadecimal.py` & `eth-utils-2.2.0/eth_utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/humanize.py` & `eth-utils-2.2.0/eth_utils/humanize.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Any, Iterable, Iterator, Tuple, Union
 from urllib import parse
 
 from eth_typing import URI, Hash32
 
+from eth_utils.currency import denoms, from_wei
+
 from .toolz import sliding_window, take
 
 
 def humanize_seconds(seconds: Union[float, int]) -> str:
     if int(seconds) == 0:
         return "0s"
 
@@ -153,7 +155,19 @@
     - fn((1, 7, 8, 9)) -> '1|7-9'
     """
     values = tuple(values_iter)
     if not values:
         return "(empty)"
     else:
         return "|".join(map(_humanize_range, _extract_integer_ranges(*values)))
+
+
+def humanize_wei(number: int) -> str:
+    if number >= denoms.finney:
+        unit = "ether"
+    elif number >= denoms.mwei:
+        unit = "gwei"
+    else:
+        unit = "wei"
+    amount = from_wei(number, unit)
+    x = f"{str(amount)} {unit}"
+    return x
```

### Comparing `eth-utils-2.1.1/eth_utils/logging.py` & `eth-utils-2.2.0/eth_utils/logging.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/module_loading.py` & `eth-utils-2.2.0/eth_utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/numeric.py` & `eth-utils-2.2.0/eth_utils/numeric.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/toolz.py` & `eth-utils-2.2.0/eth_utils/toolz.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/types.py` & `eth-utils-2.2.0/eth_utils/types.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils/units.py` & `eth-utils-2.2.0/eth_utils/units.py`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils.egg-info/PKG-INFO` & `eth-utils-2.2.0/eth_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-utils
-Version: 2.1.1
+Version: 2.2.0
 Summary: eth-utils: Common utility functions for python code that interacts with Ethereum
 Home-page: https://github.com/ethereum/eth-utils
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Intended Audience :: Developers
```

### Comparing `eth-utils-2.1.1/eth_utils.egg-info/SOURCES.txt` & `eth-utils-2.2.0/eth_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/eth_utils.egg-info/requires.txt` & `eth-utils-2.2.0/eth_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/pyproject.toml` & `eth-utils-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth-utils-2.1.1/setup.py` & `eth-utils-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="eth-utils",
     # *IMPORTANT*: Don't manually change the version here. Use `make bump`, as described in readme
-    version="2.1.1",
+    version="2.2.0",
     description=(
         """eth-utils: Common utility functions for python code that interacts with Ethereum"""
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
```

