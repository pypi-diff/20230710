# Comparing `tmp/helicone-1.0.1.tar.gz` & `tmp/helicone-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helicone-1.0.1.tar", max compression
+gzip compressed data, was "helicone-1.0.2.tar", max compression
```

## Comparing `helicone-1.0.1.tar` & `helicone-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11341 2023-07-03 21:17:48.000658 helicone-1.0.1/LICENSE
--rw-r--r--   0        0        0        1 2023-07-10 04:44:07.860264 helicone-1.0.1/helicone/async_logger/__init__.py
--rw-r--r--   0        0        0     3165 2023-07-10 04:44:07.860522 helicone-1.0.1/helicone/async_logger/async_logger.py
--rw-r--r--   0        0        0       52 2023-07-10 04:44:07.860863 helicone-1.0.1/helicone/globals/__init__.py
--rw-r--r--   0        0        0     1350 2023-07-10 04:44:07.861152 helicone-1.0.1/helicone/globals/helicone.py
--rw-r--r--   0        0        0      102 2023-07-10 04:44:07.861504 helicone-1.0.1/helicone/openai_async/__init__.py
--rw-r--r--   0        0        0     8835 2023-07-10 04:44:07.861726 helicone-1.0.1/helicone/openai_async/openai_injector.py
--rw-r--r--   0        0        0     9942 2023-07-10 04:44:07.861894 helicone-1.0.1/helicone/openai_proxy/__init__.py
--rw-r--r--   0        0        0       20 2023-07-03 21:17:48.000891 helicone-1.0.1/helicone/requirements.txt
--rw-r--r--   0        0        0    11545 2023-07-10 04:44:07.862095 helicone-1.0.1/helicone/test.py
--rw-r--r--   0        0        0      380 2023-07-10 04:44:07.862921 helicone-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 helicone-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-03 21:17:48.000658 helicone-1.0.2/LICENSE
+-rw-r--r--   0        0        0        1 2023-07-10 04:44:07.860264 helicone-1.0.2/helicone/async_logger/__init__.py
+-rw-r--r--   0        0        0     3165 2023-07-10 04:44:07.860522 helicone-1.0.2/helicone/async_logger/async_logger.py
+-rw-r--r--   0        0        0       52 2023-07-10 04:44:07.860863 helicone-1.0.2/helicone/globals/__init__.py
+-rw-r--r--   0        0        0     1347 2023-07-10 17:47:57.079414 helicone-1.0.2/helicone/globals/helicone.py
+-rw-r--r--   0        0        0      102 2023-07-10 04:44:07.861504 helicone-1.0.2/helicone/openai_async/__init__.py
+-rw-r--r--   0        0        0     8835 2023-07-10 04:44:07.861726 helicone-1.0.2/helicone/openai_async/openai_injector.py
+-rw-r--r--   0        0        0     9942 2023-07-10 04:44:07.861894 helicone-1.0.2/helicone/openai_proxy/__init__.py
+-rw-r--r--   0        0        0       20 2023-07-03 21:17:48.000891 helicone-1.0.2/helicone/requirements.txt
+-rw-r--r--   0        0        0    11545 2023-07-10 04:44:07.862095 helicone-1.0.2/helicone/test.py
+-rw-r--r--   0        0        0      380 2023-07-10 17:47:57.079878 helicone-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 helicone-1.0.2/PKG-INFO
```

### Comparing `helicone-1.0.1/LICENSE` & `helicone-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `helicone-1.0.1/helicone/async_logger/async_logger.py` & `helicone-1.0.2/helicone/async_logger/async_logger.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.1/helicone/globals/helicone.py` & `helicone-1.0.2/helicone/globals/helicone.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     @api_key.setter
     def api_key(self, value: Optional[str]):
         self._api_key = value
 
     @property
     def base_url(self) -> Optional[str]:
         if (self._base_url is None):
-            return "https://api.hconeai.com/v1"
+            return "https://api.hconeai.com"
         return self._base_url
 
     @base_url.setter
     def base_url(self, value: Optional[str]):
         self._base_url = value
 
     @property
```

### Comparing `helicone-1.0.1/helicone/openai_async/openai_injector.py` & `helicone-1.0.2/helicone/openai_async/openai_injector.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.1/helicone/openai_proxy/__init__.py` & `helicone-1.0.2/helicone/openai_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.1/helicone/test.py` & `helicone-1.0.2/helicone/test.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.1/PKG-INFO` & `helicone-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helicone
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python wrapper for the OpenAI API that logs all requests to Helicone.
 Home-page: https://www.helicone.ai
 License: Apache-2.0
 Author: Helicone, Inc.
 Author-email: help@helicone.ai
 Requires-Python: >=3.8.1
 Classifier: License :: OSI Approved :: Apache Software License
```

