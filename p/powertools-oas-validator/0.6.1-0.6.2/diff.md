# Comparing `tmp/powertools_oas_validator-0.6.1.tar.gz` & `tmp/powertools_oas_validator-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powertools_oas_validator-0.6.1.tar", max compression
+gzip compressed data, was "powertools_oas_validator-0.6.2.tar", max compression
```

## Comparing `powertools_oas_validator-0.6.1.tar` & `powertools_oas_validator-0.6.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1077 2023-07-08 14:01:18.527620 powertools_oas_validator-0.6.1/LICENSE
--rw-r--r--   0        0        0     2934 2023-07-08 14:01:18.527620 powertools_oas_validator-0.6.1/README.md
--rw-r--r--   0        0        0       13 2023-07-08 14:01:18.527620 powertools_oas_validator-0.6.1/powertools_oas_validator/__init__.py
--rw-r--r--   0        0        0      252 2023-07-08 14:01:18.531620 powertools_oas_validator-0.6.1/powertools_oas_validator/exceptions.py
--rw-r--r--   0        0        0      928 2023-07-08 14:01:18.531620 powertools_oas_validator-0.6.1/powertools_oas_validator/middleware.py
--rw-r--r--   0        0        0      135 2023-07-08 14:01:18.531620 powertools_oas_validator-0.6.1/powertools_oas_validator/overrides/__init__.py
--rw-r--r--   0        0        0     1144 2023-07-08 14:01:18.531620 powertools_oas_validator-0.6.1/powertools_oas_validator/overrides/unmarshallers.py
--rw-r--r--   0        0        0     1326 2023-07-08 14:01:18.531620 powertools_oas_validator-0.6.1/powertools_oas_validator/overrides/validators.py
--rw-r--r--   0        0        0       13 2023-07-08 14:01:18.531620 powertools_oas_validator-0.6.1/powertools_oas_validator/services/__init__.py
--rw-r--r--   0        0        0     4243 2023-07-08 14:01:18.531620 powertools_oas_validator-0.6.1/powertools_oas_validator/services/error_handler.py
--rw-r--r--   0        0        0     3196 2023-07-08 14:01:18.531620 powertools_oas_validator-0.6.1/powertools_oas_validator/services/event_parser.py
--rw-r--r--   0        0        0     1120 2023-07-08 14:01:18.531620 powertools_oas_validator-0.6.1/powertools_oas_validator/services/spec_loader.py
--rw-r--r--   0        0        0      427 2023-07-08 14:01:18.531620 powertools_oas_validator-0.6.1/powertools_oas_validator/services/spec_parser.py
--rw-r--r--   0        0        0     1884 2023-07-08 14:01:18.531620 powertools_oas_validator-0.6.1/powertools_oas_validator/services/spec_validator.py
--rw-r--r--   0        0        0     1843 2023-07-08 14:01:18.531620 powertools_oas_validator-0.6.1/powertools_oas_validator/types.py
--rw-r--r--   0        0        0      975 2023-07-08 14:01:18.531620 powertools_oas_validator-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 powertools_oas_validator-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-10 12:58:13.140164 powertools_oas_validator-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2934 2023-07-10 12:58:13.140164 powertools_oas_validator-0.6.2/README.md
+-rw-r--r--   0        0        0       13 2023-07-10 12:58:13.140164 powertools_oas_validator-0.6.2/powertools_oas_validator/__init__.py
+-rw-r--r--   0        0        0      252 2023-07-10 12:58:13.140164 powertools_oas_validator-0.6.2/powertools_oas_validator/exceptions.py
+-rw-r--r--   0        0        0      928 2023-07-10 12:58:13.140164 powertools_oas_validator-0.6.2/powertools_oas_validator/middleware.py
+-rw-r--r--   0        0        0      135 2023-07-10 12:58:13.140164 powertools_oas_validator-0.6.2/powertools_oas_validator/overrides/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-10 12:58:13.140164 powertools_oas_validator-0.6.2/powertools_oas_validator/overrides/unmarshallers.py
+-rw-r--r--   0        0        0     1326 2023-07-10 12:58:13.140164 powertools_oas_validator-0.6.2/powertools_oas_validator/overrides/validators.py
+-rw-r--r--   0        0        0       13 2023-07-10 12:58:13.140164 powertools_oas_validator-0.6.2/powertools_oas_validator/services/__init__.py
+-rw-r--r--   0        0        0     4243 2023-07-10 12:58:13.140164 powertools_oas_validator-0.6.2/powertools_oas_validator/services/error_handler.py
+-rw-r--r--   0        0        0     3196 2023-07-10 12:58:13.140164 powertools_oas_validator-0.6.2/powertools_oas_validator/services/event_parser.py
+-rw-r--r--   0        0        0     1120 2023-07-10 12:58:13.140164 powertools_oas_validator-0.6.2/powertools_oas_validator/services/spec_loader.py
+-rw-r--r--   0        0        0      427 2023-07-10 12:58:13.144164 powertools_oas_validator-0.6.2/powertools_oas_validator/services/spec_parser.py
+-rw-r--r--   0        0        0     1884 2023-07-10 12:58:13.144164 powertools_oas_validator-0.6.2/powertools_oas_validator/services/spec_validator.py
+-rw-r--r--   0        0        0     1843 2023-07-10 12:58:13.144164 powertools_oas_validator-0.6.2/powertools_oas_validator/types.py
+-rw-r--r--   0        0        0      975 2023-07-10 12:58:13.144164 powertools_oas_validator-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 powertools_oas_validator-0.6.2/PKG-INFO
```

### Comparing `powertools_oas_validator-0.6.1/LICENSE` & `powertools_oas_validator-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.6.1/README.md` & `powertools_oas_validator-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.6.1/powertools_oas_validator/middleware.py` & `powertools_oas_validator-0.6.2/powertools_oas_validator/middleware.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.6.1/powertools_oas_validator/overrides/unmarshallers.py` & `powertools_oas_validator-0.6.2/powertools_oas_validator/overrides/unmarshallers.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.6.1/powertools_oas_validator/overrides/validators.py` & `powertools_oas_validator-0.6.2/powertools_oas_validator/overrides/validators.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.6.1/powertools_oas_validator/services/error_handler.py` & `powertools_oas_validator-0.6.2/powertools_oas_validator/services/error_handler.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.6.1/powertools_oas_validator/services/event_parser.py` & `powertools_oas_validator-0.6.2/powertools_oas_validator/services/event_parser.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.6.1/powertools_oas_validator/services/spec_loader.py` & `powertools_oas_validator-0.6.2/powertools_oas_validator/services/spec_loader.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.6.1/powertools_oas_validator/services/spec_validator.py` & `powertools_oas_validator-0.6.2/powertools_oas_validator/services/spec_validator.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.6.1/powertools_oas_validator/types.py` & `powertools_oas_validator-0.6.2/powertools_oas_validator/types.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.6.1/pyproject.toml` & `powertools_oas_validator-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "powertools-oas-validator"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 authors = ["Rasmus Hansen <R.FangelHansen@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 homepage = "https://github.com/RasmusFangel/powertools-oas-validator"
 repository = "https://github.com/RasmusFangel/powertools-oas-validator"
```

### Comparing `powertools_oas_validator-0.6.1/PKG-INFO` & `powertools_oas_validator-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powertools-oas-validator
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 Home-page: https://github.com/RasmusFangel/powertools-oas-validator
 License: MIT
 Author: Rasmus Hansen
 Author-email: R.FangelHansen@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powertools-oas-validator Version: 0.6.1 Summary:
+Metadata-Version: 2.1 Name: powertools-oas-validator Version: 0.6.2 Summary:
 Home-page: https://github.com/RasmusFangel/powertools-oas-validator License:
 MIT Author: Rasmus Hansen Author-email: R.FangelHansen@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aws-lambda-powertools (>=2.18.0,<3.0.0) Requires-Dist:
 fastjsonschema (>=2.17.1,<3.0.0) Requires-Dist: jmespath (>=1.0.1,<2.0.0)
```

