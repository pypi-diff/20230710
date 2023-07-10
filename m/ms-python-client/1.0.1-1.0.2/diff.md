# Comparing `tmp/ms_python_client-1.0.1.tar.gz` & `tmp/ms_python_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_python_client-1.0.1.tar", max compression
+gzip compressed data, was "ms_python_client-1.0.2.tar", max compression
```

## Comparing `ms_python_client-1.0.1.tar` & `ms_python_client-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1100 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/LICENSE
--rw-r--r--   0        0        0     5657 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/__init__.py
--rw-r--r--   0        0        0     5551 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/api_client.py
--rw-r--r--   0        0        0     1380 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/cern_ms_api_client.py
--rw-r--r--   0        0        0        0 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/components/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/components/events/__init__.py
--rw-r--r--   0        0        0     3856 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/components/events/cern_events_component.py
--rw-r--r--   0        0        0     3100 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/components/events/events_component.py
--rw-r--r--   0        0        0      874 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/components/events/users_component.py
--rw-r--r--   0        0        0     5696 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/ms_api_client.py
--rw-r--r--   0        0        0     1312 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/ms_client_interface.py
--rw-r--r--   0        0        0        0 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/utils/__init__.py
--rw-r--r--   0        0        0      383 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/utils/error.py
--rw-r--r--   0        0        0     5047 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/utils/event_generator.py
--rw-r--r--   0        0        0       97 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/utils/file_system.py
--rw-r--r--   0        0        0     1276 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/utils/init_from_env.py
--rw-r--r--   0        0        0      729 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/utils/logger.py
--rw-r--r--   0        0        0     1033 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6461 1970-01-01 00:00:00.000000 ms_python_client-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5657 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/__init__.py
+-rw-r--r--   0        0        0     5551 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/api_client.py
+-rw-r--r--   0        0        0     1380 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/cern_ms_api_client.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/components/events/__init__.py
+-rw-r--r--   0        0        0     3856 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/components/events/cern_events_component.py
+-rw-r--r--   0        0        0     3100 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/components/events/events_component.py
+-rw-r--r--   0        0        0      874 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/components/events/users_component.py
+-rw-r--r--   0        0        0     5696 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/ms_api_client.py
+-rw-r--r--   0        0        0     1312 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/ms_client_interface.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/utils/__init__.py
+-rw-r--r--   0        0        0      383 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/utils/error.py
+-rw-r--r--   0        0        0     5047 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/utils/event_generator.py
+-rw-r--r--   0        0        0       97 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/utils/file_system.py
+-rw-r--r--   0        0        0     1276 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/utils/init_from_env.py
+-rw-r--r--   0        0        0      729 2023-07-10 15:21:45.844628 ms_python_client-1.0.2/ms_python_client/utils/logger.py
+-rw-r--r--   0        0        0     1003 2023-07-10 15:21:45.848628 ms_python_client-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6409 1970-01-01 00:00:00.000000 ms_python_client-1.0.2/PKG-INFO
```

### Comparing `ms_python_client-1.0.1/LICENSE` & `ms_python_client-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.1/README.md` & `ms_python_client-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.1/ms_python_client/api_client.py` & `ms_python_client-1.0.2/ms_python_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.1/ms_python_client/cern_ms_api_client.py` & `ms_python_client-1.0.2/ms_python_client/cern_ms_api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.1/ms_python_client/components/events/cern_events_component.py` & `ms_python_client-1.0.2/ms_python_client/components/events/cern_events_component.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.1/ms_python_client/components/events/events_component.py` & `ms_python_client-1.0.2/ms_python_client/components/events/events_component.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.1/ms_python_client/components/events/users_component.py` & `ms_python_client-1.0.2/ms_python_client/components/events/users_component.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.1/ms_python_client/ms_api_client.py` & `ms_python_client-1.0.2/ms_python_client/ms_api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.1/ms_python_client/ms_client_interface.py` & `ms_python_client-1.0.2/ms_python_client/ms_client_interface.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.1/ms_python_client/utils/event_generator.py` & `ms_python_client-1.0.2/ms_python_client/utils/event_generator.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.1/ms_python_client/utils/init_from_env.py` & `ms_python_client-1.0.2/ms_python_client/utils/init_from_env.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.1/ms_python_client/utils/logger.py` & `ms_python_client-1.0.2/ms_python_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.1/pyproject.toml` & `ms_python_client-1.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [tool.poetry]
 name = "ms-python-client"
-version = "1.0.1"
+version = "1.0.2"
 exclude = ["tests*", "example*", ".github*", ".git*", ".vscode*"]
 description = "This package is used to interact with the microsoft graph API"
 authors = ["Samuel Guillemet <samuel.guillemet@telecom-sudparis.eu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ms_python_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-python-dotenv = "^0.21.0"
-typing_extensions = "^4.3.0"
+python-dotenv = "^1.0.0"
 msal = "^1.22.0"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 black = "23.3.0"
 flake8 = "6.0.0"
-isort = "5.10.1"
+isort = "5.12.0"
 pre-commit = "2.15.0"
-mypy = "1.2.0"
+mypy = "1.4.1"
 mypy-extensions = "1.0.0"
 pylint = "2.17.4"
-pytest = "7.1.3"
-pytest-cov = "3.0.0"
-responses = "0.17.0"
+pytest = "7.4.0"
+pytest-cov = "4.1.0"
+responses = "0.23.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/SamuelGuillemet/ms-python-client/issues"
```

### Comparing `ms_python_client-1.0.1/PKG-INFO` & `ms_python_client-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ms-python-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: This package is used to interact with the microsoft graph API
 License: MIT
 Author: Samuel Guillemet
 Author-email: samuel.guillemet@telecom-sudparis.eu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: msal (>=1.22.0,<2.0.0)
-Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/SamuelGuillemet/ms-python-client/issues
 Description-Content-Type: text/markdown
 
 # Microsoft Python client
 
 [![Python tests](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/python-tests.yml/badge.svg)](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/python-tests.yml)
 [![pre-commit](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/SamuelGuillemet/ms-python-client/actions/workflows/pre-commit.yaml)
```

