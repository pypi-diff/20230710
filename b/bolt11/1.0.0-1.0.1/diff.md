# Comparing `tmp/bolt11-1.0.0.tar.gz` & `tmp/bolt11-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bolt11-1.0.0.tar", max compression
+gzip compressed data, was "bolt11-1.0.1.tar", max compression
```

## Comparing `bolt11-1.0.0.tar` & `bolt11-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1112 2023-07-10 18:02:06.217296 bolt11-1.0.0/LICENSE
--rwxr-xr-x   0        0        0     3119 2023-07-10 18:02:06.217296 bolt11-1.0.0/README.md
--rw-r--r--   0        0        0      353 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/__init__.py
--rw-r--r--   0        0        0     1127 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/bit_utils.py
--rw-r--r--   0        0        0      599 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/cli.py
--rw-r--r--   0        0        0      243 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/compat.py
--rw-r--r--   0        0        0     3932 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/decode.py
--rw-r--r--   0        0        0     2926 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/encode.py
--rw-r--r--   0        0        0     2850 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/models/fallback.py
--rw-r--r--   0        0        0     3486 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/models/features.py
--rw-r--r--   0        0        0     1768 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/models/routehint.py
--rw-r--r--   0        0        0     2322 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/models/signature.py
--rw-r--r--   0        0        0       26 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/py.typed
--rw-r--r--   0        0        0     3940 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/types.py
--rw-r--r--   0        0        0     1947 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/utils.py
--rw-r--r--   0        0        0     1549 2023-07-10 18:02:06.217296 bolt11-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 bolt11-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1112 2023-07-10 21:30:03.466005 bolt11-1.0.1/LICENSE
+-rwxr-xr-x   0        0        0     3119 2023-07-10 21:30:03.466005 bolt11-1.0.1/README.md
+-rw-r--r--   0        0        0      353 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/__init__.py
+-rw-r--r--   0        0        0     1127 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/bit_utils.py
+-rw-r--r--   0        0        0      599 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/cli.py
+-rw-r--r--   0        0        0      243 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/compat.py
+-rw-r--r--   0        0        0     3932 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/decode.py
+-rw-r--r--   0        0        0     2926 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/encode.py
+-rw-r--r--   0        0        0     2850 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/models/fallback.py
+-rw-r--r--   0        0        0     3486 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/models/features.py
+-rw-r--r--   0        0        0     1768 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/models/routehint.py
+-rw-r--r--   0        0        0     2322 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/models/signature.py
+-rw-r--r--   0        0        0       26 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/py.typed
+-rw-r--r--   0        0        0     3940 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/types.py
+-rw-r--r--   0        0        0     1947 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/utils.py
+-rw-r--r--   0        0        0     1545 2023-07-10 21:30:03.466005 bolt11-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3924 1970-01-01 00:00:00.000000 bolt11-1.0.1/PKG-INFO
```

### Comparing `bolt11-1.0.0/LICENSE` & `bolt11-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.0/README.md` & `bolt11-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.0/bolt11/bit_utils.py` & `bolt11-1.0.1/bolt11/bit_utils.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.0/bolt11/cli.py` & `bolt11-1.0.1/bolt11/cli.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.0/bolt11/decode.py` & `bolt11-1.0.1/bolt11/decode.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.0/bolt11/encode.py` & `bolt11-1.0.1/bolt11/encode.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.0/bolt11/models/fallback.py` & `bolt11-1.0.1/bolt11/models/fallback.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.0/bolt11/models/features.py` & `bolt11-1.0.1/bolt11/models/features.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.0/bolt11/models/routehint.py` & `bolt11-1.0.1/bolt11/models/routehint.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.0/bolt11/models/signature.py` & `bolt11-1.0.1/bolt11/models/signature.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.0/bolt11/types.py` & `bolt11-1.0.1/bolt11/types.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.0/bolt11/utils.py` & `bolt11-1.0.1/bolt11/utils.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.0/pyproject.toml` & `bolt11-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bolt11"
-version = "1.0.0"
+version = "1.0.1"
 description = "A library for encoding and decoding BOLT11 payment requests."
 repository = "https://github.com/lnbits/bolt11"
 authors = [
     "eillarra <eneko@illarra.com>",
     "Alan Bits <alan@lnbits.com>"
 ]
 license = "MIT"
@@ -15,15 +15,15 @@
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 base58 = "^2.1.1"
 bech32 = "^1.2.0"
-bitstring = "^4.0.2"
+bitstring = "^3"
 ecdsa = "^0.18.0"
 secp256k1 = "^0.14.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 flake8 = "^6.0.0"
```

### Comparing `bolt11-1.0.0/PKG-INFO` & `bolt11-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: bolt11
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for encoding and decoding BOLT11 payment requests.
 Home-page: https://github.com/lnbits/bolt11
 License: MIT
 Author: eillarra
 Author-email: eneko@illarra.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: base58 (>=2.1.1,<3.0.0)
 Requires-Dist: bech32 (>=1.2.0,<2.0.0)
-Requires-Dist: bitstring (>=4.0.2,<5.0.0)
+Requires-Dist: bitstring (>=3,<4)
 Requires-Dist: ecdsa (>=0.18.0,<0.19.0)
 Requires-Dist: secp256k1 (>=0.14.0,<0.15.0)
 Project-URL: Repository, https://github.com/lnbits/bolt11
 Description-Content-Type: text/markdown
 
 Lightning BOLT11 utils
 ======================
```

