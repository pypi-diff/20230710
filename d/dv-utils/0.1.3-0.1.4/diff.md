# Comparing `tmp/dv_utils-0.1.3.tar.gz` & `tmp/dv_utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dv_utils-0.1.3.tar", max compression
+gzip compressed data, was "dv_utils-0.1.4.tar", max compression
```

## Comparing `dv_utils-0.1.3.tar` & `dv_utils-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      622 2022-09-23 12:38:21.911471 dv_utils-0.1.3/README.md
--rw-r--r--   0        0        0      378 2023-04-26 12:10:23.887056 dv_utils-0.1.3/dv_utils/__init__.py
--rw-r--r--   0        0        0      452 2023-04-26 10:45:42.041117 dv_utils-0.1.3/dv_utils/__main__.py
--rw-r--r--   0        0        0     3239 2023-02-20 08:24:19.300581 dv_utils-0.1.3/dv_utils/client.py
--rw-r--r--   0        0        0     1663 2023-06-22 10:12:01.387002 dv_utils-0.1.3/dv_utils/listener.py
--rw-r--r--   0        0        0     1932 2023-04-26 12:04:07.208975 dv_utils-0.1.3/dv_utils/log_utils.py
--rw-r--r--   0        0        0     1521 2022-08-05 13:05:56.151683 dv_utils-0.1.3/dv_utils/process.py
--rw-r--r--   0        0        0     2813 2023-06-20 13:29:43.364033 dv_utils-0.1.3/dv_utils/redis.py
--rw-r--r--   0        0        0     1413 2022-08-05 13:04:09.726787 dv_utils-0.1.3/dv_utils/settings.py
--rw-r--r--   0        0        0     1186 2023-06-22 10:12:11.275091 dv_utils-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1514 1970-01-01 00:00:00.000000 dv_utils-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      622 2022-09-23 12:38:21.911471 dv_utils-0.1.4/README.md
+-rw-r--r--   0        0        0      378 2023-04-26 12:10:23.887056 dv_utils-0.1.4/dv_utils/__init__.py
+-rw-r--r--   0        0        0      452 2023-04-26 10:45:42.041117 dv_utils-0.1.4/dv_utils/__main__.py
+-rw-r--r--   0        0        0     3239 2023-02-20 08:24:19.300581 dv_utils-0.1.4/dv_utils/client.py
+-rw-r--r--   0        0        0     1663 2023-06-22 10:12:01.387002 dv_utils-0.1.4/dv_utils/listener.py
+-rw-r--r--   0        0        0     1932 2023-04-26 12:04:07.208975 dv_utils-0.1.4/dv_utils/log_utils.py
+-rw-r--r--   0        0        0     1521 2022-08-05 13:05:56.151683 dv_utils-0.1.4/dv_utils/process.py
+-rw-r--r--   0        0        0     2813 2023-06-20 13:29:43.364033 dv_utils-0.1.4/dv_utils/redis.py
+-rw-r--r--   0        0        0     1412 2023-07-10 13:54:39.792306 dv_utils-0.1.4/dv_utils/settings.py
+-rw-r--r--   0        0        0     1186 2023-07-10 13:55:27.464519 dv_utils-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1514 1970-01-01 00:00:00.000000 dv_utils-0.1.4/PKG-INFO
```

### Comparing `dv_utils-0.1.3/README.md` & `dv_utils-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dv_utils-0.1.3/dv_utils/client.py` & `dv_utils-0.1.4/dv_utils/client.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.1.3/dv_utils/listener.py` & `dv_utils-0.1.4/dv_utils/listener.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.1.3/dv_utils/log_utils.py` & `dv_utils-0.1.4/dv_utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.1.3/dv_utils/process.py` & `dv_utils-0.1.4/dv_utils/process.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.1.3/dv_utils/redis.py` & `dv_utils-0.1.4/dv_utils/redis.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.1.3/dv_utils/settings.py` & `dv_utils-0.1.4/dv_utils/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.config = config
 
         self.base_url: str = config("DV_URL", default="", cast=str)
         self.token: str = config("DV_TOKEN", default="", cast=str)
         self.app_id: str = config("DV_APP_ID", default="", cast=str)
         self.client_id: str = config("DV_CLIENT_ID", default="", cast=str)
 
-        self.log_level = config("LOGLEVEL", default="DEBUG", cast=str)
+        self.log_level = config("LOGLEVEL", default="INFO", cast=str)
         self.daemon = config("DAEMON", default=False, cast=bool)
 
         self.redis_host = config("REDIS_SERVICE_HOST", default="localhost", cast=str)
         self.redis_port = config("REDIS_SERVICE_PORT", default="6379", cast=str)
 
 
 settings = Settings()
```

### Comparing `dv_utils-0.1.3/pyproject.toml` & `dv_utils-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry>=0.12", "setuptools>=40.8.0"]
 build-backend = "poetry.masonry.api"
 
 [tool]
 [tool.poetry]
 name = "dv-utils"
-version = "0.1.3"
+version = "0.1.4"
 description = "DataVillage Python utils for interaction with the middleware and building algo processing code"
 authors = ["Loic Quertenmont <loic@deeperanalytics.be>"]
 readme = "README.md"
 repository = "https://github.com/datavillage-me/dv-utils"
 
 [tool.poetry.dependencies]
 python = ">=3.10.4,<4"
```

### Comparing `dv_utils-0.1.3/PKG-INFO` & `dv_utils-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dv-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: DataVillage Python utils for interaction with the middleware and building algo processing code
 Home-page: https://github.com/datavillage-me/dv-utils
 Author: Loic Quertenmont
 Author-email: loic@deeperanalytics.be
 Requires-Python: >=3.10.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

