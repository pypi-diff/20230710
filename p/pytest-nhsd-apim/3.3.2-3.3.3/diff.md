# Comparing `tmp/pytest-nhsd-apim-3.3.2.tar.gz` & `tmp/pytest-nhsd-apim-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-nhsd-apim-3.3.2.tar", last modified: Wed Jun  7 12:54:22 2023, max compression
+gzip compressed data, was "pytest-nhsd-apim-3.3.3.tar", last modified: Mon Jul 10 13:09:48 2023, max compression
```

## Comparing `pytest-nhsd-apim-3.3.2.tar` & `pytest-nhsd-apim-3.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:22.479457 pytest-nhsd-apim-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-07 12:54:22.479457 pytest-nhsd-apim-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 12:54:22.479457 pytest-nhsd-apim-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:22.475458 pytest-nhsd-apim-3.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:22.479457 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57430 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/apigee_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)    18675 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/apigee_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/auth_journey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/identity_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/nhsd_apim_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/pytest_nhsd_apim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/token_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:22.479457 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-07 12:54:22.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-07 12:54:22.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:54:22.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 12:54:22.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-07 12:54:22.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 12:54:22.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:22.479457 pytest-nhsd-apim-3.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/tests/test_apigee_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/tests/test_nhsd_apim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:09:48.103177 pytest-nhsd-apim-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-10 13:09:48.103177 pytest-nhsd-apim-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 13:09:48.103177 pytest-nhsd-apim-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:09:48.099177 pytest-nhsd-apim-3.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:09:48.099177 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57430 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/apigee_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18675 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/apigee_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/auth_journey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/identity_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/nhsd_apim_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/pytest_nhsd_apim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/token_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:09:48.103177 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-10 13:09:48.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-10 13:09:48.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:09:48.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 13:09:48.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-10 13:09:48.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 13:09:48.000000 pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:09:48.103177 pytest-nhsd-apim-3.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/tests/test_apigee_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-10 13:09:15.000000 pytest-nhsd-apim-3.3.3/tests/test_nhsd_apim.py
```

### Comparing `pytest-nhsd-apim-3.3.2/PKG-INFO` & `pytest-nhsd-apim-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-nhsd-apim
-Version: 3.3.2
+Version: 3.3.3
 Summary: Pytest plugin accessing NHSDigital's APIM proxies
 Home-page: https://github.com/NHSDigital/pytest-nhsd-apim
 Author: Adrian Ciobanita
 Author-email: adrian.ciobanita1@nhs.net
 Maintainer: Alex Carrie
 Maintainer-email: alexander.carrie1@nhs.net
 License: MIT
```

### Comparing `pytest-nhsd-apim-3.3.2/README.md` & `pytest-nhsd-apim-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/pyproject.toml` & `pytest-nhsd-apim-3.3.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-nhsd-apim"
-version = "3.3.2"
+version = "3.3.3"
 description = "Pytest plugin accessing NHSDigital's APIM proxies"
 authors = ["Adrian Ciobanita <adrian.ciobanita1@nhs.net>", "Alex Carrie <alexander.carrie1@nhs.net>", "Lucas Fantini <lucas.fantini@nhs.net>"]
 maintainers = ["Alex Carrie <alexander.carrie1@nhs.net>", "Alex Hawdon <alex.hawdon1@nhs.net"]
 readme = "README.md"
 repository = "https://github.com/NHSDigital/pytest-nhsd-apim"
 classifiers = ["Framework :: Pytest"]
 license = "MIT"
@@ -18,15 +18,15 @@
 PyJWT = "^2.3.0"
 pyotp = "^2.6.0"
 pytest = "^6.2.5"
 requests = "^2.27.1"
 toml = "^0.10.2"
 typing-extensions = "^4.3.0"
 pydantic = "^1.9.1"
-wheel = "^0.37.1"
+wheel = ">=0.37.1,<0.39.0"
 
 
 [tool.poetry.dev-dependencies]
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
```

### Comparing `pytest-nhsd-apim-3.3.2/setup.py` & `pytest-nhsd-apim-3.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/apigee_apis.py` & `pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/apigee_apis.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/apigee_edge.py` & `pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/apigee_edge.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/auth_journey.py` & `pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/auth_journey.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/config.py` & `pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/config.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/identity_service.py` & `pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/identity_service.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/log.py` & `pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/log.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/nhsd_apim_authorization.py` & `pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/nhsd_apim_authorization.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/pytest_nhsd_apim.py` & `pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/pytest_nhsd_apim.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/secrets.py` & `pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/secrets.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/token_cache.py` & `pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim/token_cache.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/PKG-INFO` & `pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-nhsd-apim
-Version: 3.3.2
+Version: 3.3.3
 Summary: Pytest plugin accessing NHSDigital's APIM proxies
 Home-page: https://github.com/NHSDigital/pytest-nhsd-apim
 Author: Adrian Ciobanita
 Author-email: adrian.ciobanita1@nhs.net
 Maintainer: Alex Carrie
 Maintainer-email: alexander.carrie1@nhs.net
 License: MIT
```

### Comparing `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/SOURCES.txt` & `pytest-nhsd-apim-3.3.3/src/pytest_nhsd_apim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/tests/test_apigee_apis.py` & `pytest-nhsd-apim-3.3.3/tests/test_apigee_apis.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/tests/test_examples.py` & `pytest-nhsd-apim-3.3.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.2/tests/test_nhsd_apim.py` & `pytest-nhsd-apim-3.3.3/tests/test_nhsd_apim.py`

 * *Files identical despite different names*

