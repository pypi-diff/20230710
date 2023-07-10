# Comparing `tmp/kadaster_kikinzage_client-0.2.0.tar.gz` & `tmp/kadaster_kikinzage_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kadaster_kikinzage_client-0.2.0.tar", max compression
+gzip compressed data, was "kadaster_kikinzage_client-0.3.0.tar", max compression
```

## Comparing `kadaster_kikinzage_client-0.2.0.tar` & `kadaster_kikinzage_client-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1071 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/LICENSE
--rw-r--r--   0        0        0     4027 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/README.md
--rw-r--r--   0        0        0     2113 2023-06-21 12:26:27.652500 kadaster_kikinzage_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       45 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/__init__.py
--rw-r--r--   0        0        0     2274 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/__main__.py
--rw-r--r--   0        0        0      302 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/client/__init__.py
--rw-r--r--   0        0        0    19206 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/client/asyncio.py
--rw-r--r--   0        0        0    22661 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/client/base.py
--rw-r--r--   0        0        0    18556 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/client/default.py
--rw-r--r--   0        0        0      610 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/client/errors.py
--rw-r--r--   0        0        0      188 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/client/utils.py
--rw-r--r--   0        0        0      401 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/__init__.py
--rw-r--r--   0        0        0     2927 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/adres.py
--rw-r--r--   0        0        0    11899 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/collectie.py
--rw-r--r--   0        0        0     5786 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/eigendomsinformatie.py
--rw-r--r--   0        0        0     1445 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/enum.py
--rw-r--r--   0        0        0     8739 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/generated.py
--rw-r--r--   0        0        0      613 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/misc.py
--rw-r--r--   0        0        0     3452 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/persoon.py
--rw-r--r--   0        0        0     4030 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/product.py
--rw-r--r--   0        0        0     2361 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/stukken.py
--rw-r--r--   0        0        0     1195 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/zekerheid.py
--rw-r--r--   0        0        0        0 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/py.typed
--rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4027 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/README.md
+-rw-r--r--   0        0        0     2113 2023-07-10 14:19:07.515283 kadaster_kikinzage_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/__init__.py
+-rw-r--r--   0        0        0     2274 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/__main__.py
+-rw-r--r--   0        0        0      302 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/client/__init__.py
+-rw-r--r--   0        0        0    19206 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/client/asyncio.py
+-rw-r--r--   0        0        0    22661 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/client/base.py
+-rw-r--r--   0        0        0    18556 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/client/default.py
+-rw-r--r--   0        0        0      610 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/client/errors.py
+-rw-r--r--   0        0        0      188 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/client/utils.py
+-rw-r--r--   0        0        0      401 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/models/__init__.py
+-rw-r--r--   0        0        0     2927 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/models/adres.py
+-rw-r--r--   0        0        0    11899 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/models/collectie.py
+-rw-r--r--   0        0        0     5786 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/models/eigendomsinformatie.py
+-rw-r--r--   0        0        0     1445 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/models/enum.py
+-rw-r--r--   0        0        0     8739 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/models/generated.py
+-rw-r--r--   0        0        0      613 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/models/misc.py
+-rw-r--r--   0        0        0     3452 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/models/persoon.py
+-rw-r--r--   0        0        0     4030 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/models/product.py
+-rw-r--r--   0        0        0     2361 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/models/stukken.py
+-rw-r--r--   0        0        0     1195 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/models/zekerheid.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:18:46.815044 kadaster_kikinzage_client-0.3.0/src/kikinzage/py.typed
+-rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.3.0/PKG-INFO
```

### Comparing `kadaster_kikinzage_client-0.2.0/LICENSE` & `kadaster_kikinzage_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/README.md` & `kadaster_kikinzage_client-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/pyproject.toml` & `kadaster_kikinzage_client-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kadaster-kikinzage-client"
-version = "0.2.0"
+version = "0.3.0"
 description = " Kadaster - KIK Inzage API Python client"
 authors = ["Jelmer Draaijer <info@jelmert.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 repository = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 documentation = "https://kadaster-kik-inzage-api-python-client.readthedocs.io"
@@ -17,15 +17,15 @@
 
 [tool.poetry.urls]
 Changelog = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
 click = ">=8.0.1"
-pydantic = ">=2.0a1"
+pydantic = ">=2.0.1"
 httpx = ">=0.24.1"
 typing-extensions = "^4.6.3"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 bandit = ">=1.7.4"
 black = ">=21.10b0"
```

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/__main__.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/__main__.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/client/asyncio.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/client/asyncio.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/client/base.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/client/base.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/client/default.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/client/default.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/client/errors.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/client/errors.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/adres.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/models/adres.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/collectie.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/models/collectie.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/eigendomsinformatie.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/models/eigendomsinformatie.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/enum.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/models/enum.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/generated.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/models/generated.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/misc.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/models/misc.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/persoon.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/models/persoon.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/product.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/models/product.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/stukken.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/models/stukken.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/zekerheid.py` & `kadaster_kikinzage_client-0.3.0/src/kikinzage/models/zekerheid.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.2.0/PKG-INFO` & `kadaster_kikinzage_client-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kadaster-kikinzage-client
-Version: 0.2.0
+Version: 0.3.0
 Summary:  Kadaster - KIK Inzage API Python client
 Home-page: https://github.com/foarsitter/kadaster-kik-inzage-api-python-client
 License: MIT
 Author: Jelmer Draaijer
 Author-email: info@jelmert.nl
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: httpx (>=0.24.1)
-Requires-Dist: pydantic (>=2.0a1)
+Requires-Dist: pydantic (>=2.0.1)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Project-URL: Changelog, https://github.com/foarsitter/kadaster-kik-inzage-api-python-client/releases
 Project-URL: Documentation, https://kadaster-kik-inzage-api-python-client.readthedocs.io
 Project-URL: Repository, https://github.com/foarsitter/kadaster-kik-inzage-api-python-client
 Description-Content-Type: text/markdown
 
 # Kadaster - KIK Inzage API Python client
```

