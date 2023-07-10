# Comparing `tmp/elytra_ms-0.0.2.tar.gz` & `tmp/elytra_ms-0.0.2.1.tar.gz`

## Comparing `elytra_ms-0.0.2.tar` & `elytra_ms-0.0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/const.py
--rw-r--r--   0        0        0    14263 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/core.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/protocols.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/bedrock_realms/__init__.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/bedrock_realms/models.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/scripts/authenticate.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/xbox/__init__.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/xbox/core.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/xbox/club/__init__.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/xbox/club/models.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/xbox/peoplehub/__init__.py
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/xbox/peoplehub/models.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/xbox/profile/__init__.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/elytra/xbox/profile/models.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/LICENSE
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/README.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 elytra_ms-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/const.py
+-rw-r--r--   0        0        0    14292 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/core.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/protocols.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/bedrock_realms/__init__.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/bedrock_realms/models.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/scripts/authenticate.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/__init__.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/core.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/club/__init__.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/club/models.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/peoplehub/__init__.py
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/peoplehub/models.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/profile/__init__.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/profile/models.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/LICENSE
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/README.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/PKG-INFO
```

### Comparing `elytra_ms-0.0.2/elytra/core.py` & `elytra_ms-0.0.2.1/elytra/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "CamelBaseModel",
     "PascalBaseModel",
     "ParsableModel",
     "ParsableCamelModel",
     "ParsablePascalModel",
     "add_decoder",
     "AuthenticationManager",
+    "MicrosoftAPIException",
     "BaseMicrosoftAPI",
 )
 
 
 class BetterResponse(aiohttp.ClientResponse):
     def raise_for_status(self) -> None:
         # i just dont want the resp to close lol
```

### Comparing `elytra_ms-0.0.2/elytra/protocols.py` & `elytra_ms-0.0.2.1/elytra/protocols.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2/elytra/bedrock_realms/__init__.py` & `elytra_ms-0.0.2.1/elytra/bedrock_realms/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2/elytra/bedrock_realms/models.py` & `elytra_ms-0.0.2.1/elytra/bedrock_realms/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2/elytra/scripts/authenticate.py` & `elytra_ms-0.0.2.1/elytra/scripts/authenticate.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2/elytra/xbox/club/__init__.py` & `elytra_ms-0.0.2.1/elytra/xbox/club/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2/elytra/xbox/club/models.py` & `elytra_ms-0.0.2.1/elytra/xbox/club/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2/elytra/xbox/peoplehub/__init__.py` & `elytra_ms-0.0.2.1/elytra/xbox/peoplehub/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2/elytra/xbox/peoplehub/models.py` & `elytra_ms-0.0.2.1/elytra/xbox/peoplehub/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2/elytra/xbox/profile/__init__.py` & `elytra_ms-0.0.2.1/elytra/xbox/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2/.gitignore` & `elytra_ms-0.0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2/LICENSE` & `elytra_ms-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2/README.md` & `elytra_ms-0.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2/pyproject.toml` & `elytra_ms-0.0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2/PKG-INFO` & `elytra_ms-0.0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elytra-ms
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: A Python Library for various Microsoft APIs, including the Xbox and Bedrock Realms APIs.
 Project-URL: Homepage, https://github.com/AstreaTSS/elytra-ms
 Author: AstreaTSS
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

