# Comparing `tmp/cru-dse-utils-0.1.1.tar.gz` & `tmp/cru-dse-utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cru-dse-utils-0.1.1.tar", last modified: Fri Jun 30 20:10:45 2023, max compression
+gzip compressed data, was "cru-dse-utils-0.1.3.tar", last modified: Mon Jul 10 12:01:27 2023, max compression
```

## Comparing `cru-dse-utils-0.1.1.tar` & `cru-dse-utils-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 20:10:45.753614 cru-dse-utils-0.1.1/
--rw-rw-rw-   0        0        0     1085 2023-06-30 12:20:25.000000 cru-dse-utils-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2854 2023-06-30 20:10:45.752093 cru-dse-utils-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1099 2023-06-30 20:02:14.000000 cru-dse-utils-0.1.1/README.md
--rw-rw-rw-   0        0        0      685 2023-06-30 20:08:58.000000 cru-dse-utils-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 20:10:45.755619 cru-dse-utils-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 20:10:45.696146 cru-dse-utils-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 20:10:45.722808 cru-dse-utils-0.1.1/src/cru_dse_utils/
--rw-rw-rw-   0        0        0       34 2023-06-30 12:20:25.000000 cru-dse-utils-0.1.1/src/cru_dse_utils/__init__.py
--rw-rw-rw-   0        0        0     4382 2023-06-30 12:20:25.000000 cru-dse-utils-0.1.1/src/cru_dse_utils/general.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:10:45.748092 cru-dse-utils-0.1.1/src/cru_dse_utils.egg-info/
--rw-rw-rw-   0        0        0     2854 2023-06-30 20:10:45.000000 cru-dse-utils-0.1.1/src/cru_dse_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-30 20:10:45.000000 cru-dse-utils-0.1.1/src/cru_dse_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 20:10:45.000000 cru-dse-utils-0.1.1/src/cru_dse_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-30 20:10:45.000000 cru-dse-utils-0.1.1/src/cru_dse_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 20:10:45.000000 cru-dse-utils-0.1.1/src/cru_dse_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 12:01:27.107308 cru-dse-utils-0.1.3/
+-rw-rw-rw-   0        0        0     1085 2023-06-30 12:20:25.000000 cru-dse-utils-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3049 2023-07-10 12:01:27.106337 cru-dse-utils-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2023-07-08 19:47:45.000000 cru-dse-utils-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1040 2023-07-08 19:52:42.000000 cru-dse-utils-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 12:01:27.108307 cru-dse-utils-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 12:01:26.942391 cru-dse-utils-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 12:01:27.035192 cru-dse-utils-0.1.3/src/cru_dse_utils/
+-rw-rw-rw-   0        0        0      493 2023-07-08 19:06:36.000000 cru-dse-utils-0.1.3/src/cru_dse_utils/__init__.py
+-rw-rw-rw-   0        0        0     4099 2023-07-07 14:40:08.000000 cru-dse-utils-0.1.3/src/cru_dse_utils/auth.py
+-rw-rw-rw-   0        0        0     9866 2023-07-08 20:13:30.000000 cru-dse-utils-0.1.3/src/cru_dse_utils/bigquery.py
+-rw-rw-rw-   0        0        0     5836 2023-07-07 16:33:53.000000 cru-dse-utils-0.1.3/src/cru_dse_utils/dbt.py
+-rw-rw-rw-   0        0        0     4540 2023-07-08 16:29:06.000000 cru-dse-utils-0.1.3/src/cru_dse_utils/gcs.py
+-rw-rw-rw-   0        0        0     4814 2023-07-07 14:39:34.000000 cru-dse-utils-0.1.3/src/cru_dse_utils/general.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:01:27.057512 cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/
+-rw-rw-rw-   0        0        0     3049 2023-07-10 12:01:26.000000 cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-07-10 12:01:26.000000 cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 12:01:26.000000 cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-07-10 12:01:26.000000 cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-10 12:01:26.000000 cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 12:01:27.099914 cru-dse-utils-0.1.3/tests/
+-rw-rw-rw-   0        0        0     4026 2023-07-07 15:29:57.000000 cru-dse-utils-0.1.3/tests/test_auth.py
+-rw-rw-rw-   0        0        0    11645 2023-07-08 20:14:13.000000 cru-dse-utils-0.1.3/tests/test_bigquery.py
+-rw-rw-rw-   0        0        0     6164 2023-07-07 19:10:39.000000 cru-dse-utils-0.1.3/tests/test_dbt.py
+-rw-rw-rw-   0        0        0    10458 2023-07-08 17:00:42.000000 cru-dse-utils-0.1.3/tests/test_gcs.py
+-rw-rw-rw-   0        0        0     1718 2023-07-07 15:11:00.000000 cru-dse-utils-0.1.3/tests/test_general.py
```

### Comparing `cru-dse-utils-0.1.1/LICENSE` & `cru-dse-utils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cru-dse-utils-0.1.1/PKG-INFO` & `cru-dse-utils-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cru-dse-utils
-Version: 0.1.1
+Version: 0.1.3
 Summary: Cru DSE Python Utils
-Author-email: Cru/Tony Guan <tony.guan@cru.org>
+Author-email: Cru DSE Team <tony.guan@cru.org>
 License: MIT License
         
         Copyright (c) [2023] [Cru]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -22,29 +22,32 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repository, https://github.com/CruGlobal/dse-python-utils
+Project-URL: homepage, https://github.com/CruGlobal/dse-python-utils
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
 
-# dse-python-utils
+# cru-dse-utils
 This is a package of useful functions developed by the Cru Data Sciences & Engineering team. The package includes the following files:
 
 - `general.py`: Contains general data extraction related functions.
+- `auth.py`: Contains functions for fetching credentials. 
 - `bigquery.py`: Contains functions for bigquery operations.
+- `gcs.py`: Contains functions for Google Cloud Storage operations.
 - `dbt.py`: Contains functions for dbt operations.
 
 ## Installation
 To install the package, run the following command:
 `pip install cru-dse-utils`
 
 ## Usage
```

### Comparing `cru-dse-utils-0.1.1/README.md` & `cru-dse-utils-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
-# dse-python-utils
+# cru-dse-utils
 This is a package of useful functions developed by the Cru Data Sciences & Engineering team. The package includes the following files:
 
 - `general.py`: Contains general data extraction related functions.
+- `auth.py`: Contains functions for fetching credentials. 
 - `bigquery.py`: Contains functions for bigquery operations.
+- `gcs.py`: Contains functions for Google Cloud Storage operations.
 - `dbt.py`: Contains functions for dbt operations.
 
 ## Installation
 To install the package, run the following command:
 `pip install cru-dse-utils`
 
 ## Usage
```

### Comparing `cru-dse-utils-0.1.1/pyproject.toml` & `cru-dse-utils-0.1.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cru-dse-utils"
-version = "0.1.1"
+version = "0.1.3"
 description = "Cru DSE Python Utils"
 readme = "README.md"
-authors = [{ name = "Cru/Tony Guan", email = "tony.guan@cru.org" }]
+authors = [{ name = "Cru DSE Team", email = "tony.guan@cru.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-dependencies = ["requests"]
+dependencies = [
+    "requests",
+    "google-auth",
+    "google-cloud-bigquery",
+    "google-cloud-storage",
+    "pandas",
+]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 build = ["build", "twine"]
 dev = ["pytest"]
 
 [project.urls]
 repository = "https://github.com/CruGlobal/dse-python-utils"
+homepage = "https://github.com/CruGlobal/dse-python-utils"
+
+[tool.pytest.ini_options]
+pythonpath = "src"
+filterwarnings = [
+    "ignore:::.*pkg_resources",
+    "ignore:Deprecated call to `pkg_resources.declare_namespace.*:DeprecationWarning",
+]
```

### Comparing `cru-dse-utils-0.1.1/src/cru_dse_utils/general.py` & `cru-dse-utils-0.1.3/src/cru_dse_utils/general.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,68 @@
 import requests
 from typing import List, Dict, Any, Optional, Union
 import time
 import logging
 
 
 def get_request(
-    url: str, headers: Dict[str, str], params: Dict[Any, Any], logger: logging.Logger
+    url: str,
+    headers: Dict[str, str],
+    params: Dict[Any, Any],
+    logger: logging.Logger,
+    max_retries: int = 5,
 ) -> Union[requests.Response, None]:
     """
     Sends an HTTP GET request to the specified URL with the specified headers.
 
-    This function sends an HTTP GET request to the specified URL with the specified headers. If the response is not a
-    valid JSON object, the function will retry the request up to `max_retries` times. If the response is a 429 error,
-    the function will retry the request with an increasing delay between retries.
+    This function sends an HTTP GET request to the specified URL with the
+    specified headers. If the response is not a valid JSON object, the
+    function will retry the request up to `max_retries` times. If the response
+    is a 429 error, the function will retry the request with an increasing
+    delay between retries.
 
     Args:
         url (str): The URL to send the request to.
-        headers (Dict[str, str]): A dictionary of headers to include in the GET request.
-        params (Dict[Any, Any]): A dictionary of parameters to include in the GET request.
+        headers (Dict[str, str]): A dictionary of headers to include in the
+        GET request.
+        params (Dict[Any, Any]): A dictionary of parameters to include in the
+        GET request.
+        logger (logging.Logger): The logger object to use for logging.
+        max_retries (int): The maximum number of times to retry the request
+        if the response is not a valid JSON object. Defaults to 5.
 
     Returns:
-        requests.Response or None: The response object if the request is successful and returns valid JSON,
-        or None if the request fails after the maximum number of retries.
+        requests.Response or None: The response object if the request is
+        successful and returns valid JSON, or None if the request fails after
+        the maximum number of retries.
 
     Raises:
-        requests.exceptions.HTTPError: If the GET request encounters an HTTP error (other than 429).
+        requests.exceptions.HTTPError: If the GET request encounters an HTTP
+        error (other than 429).
         requests.exceptions.Timeout: If the GET request times out.
-        requests.exceptions.ConnectionError: If there is a connection error during the GET request.
-        requests.exceptions.RequestException: If there is a general request error.
+        requests.exceptions.ConnectionError: If there is a connection error
+        during the GET request.
+        requests.exceptions.RequestException: If there is a general request
+        error.
     """
     logger = logging.getLogger("primary_logger")
-    max_retries = 5
     retries = 0
     while retries <= max_retries:
         try:
             r = requests.get(url, headers=headers, params=params, timeout=60)
             r.raise_for_status()
             try:
                 _ = r.json()
                 return r
             except ValueError as e:
                 # In case of invalid JSON response, retry the request
                 retries += 1
-                logger.warning(f"Invalid JSON response: {e}. Retry in 5 minutes...")
+                logger.warning(
+                    f"Invalid JSON response: {str(e)}. Retry in 5 minutes..."
+                )
                 time.sleep(300)
         except requests.exceptions.HTTPError as err:
             if err.response.status_code == 429:  # Handle 429 error
                 logger.warning("API rate limit exceeded. Retry in 1 second...")
                 delay = 1  # Initial delay is 1 second
                 while True:
                     time.sleep(delay)  # Wait for the delay period
@@ -57,15 +73,15 @@
                         r.raise_for_status()
                         try:
                             _ = r.json()
                             return r
                         except ValueError as e:
                             retries += 1
                             logger.warning(
-                                f"Invalid JSON response: {e}. Retry in 5 minutes..."
+                                f"Invalid JSON response: {str(e)}. Retry in 5 minutes..."
                             )
                             time.sleep(300)
                     except requests.exceptions.HTTPError as err:
                         if err.response.status_code == 429:  # Handle 429 error
                             logger.warning(
                                 f"API rate limit exceeded. Retry in {delay*2} seconds..."
                             )
@@ -73,20 +89,24 @@
                             continue  # Retry the same URL
                         else:
                             raise
                     break  # Break out of the retry loop if the request is successful
             else:
                 raise
         except requests.exceptions.Timeout as e:
-            logger.warning(f"Request timed out: {e}. Retry in 1 minutes...")
+            logger.warning(f"Request timed out: {str(e)}. Retry in 1 minutes...")
             retries += 1
             time.sleep(60)
         except requests.exceptions.ConnectionError as e:
-            logger.warning(f"Get request connection error: {e}. Retry in 1 minutes...")
+            logger.warning(
+                f"Get request connection error: {str(e)}. Retry in 1 minutes..."
+            )
             retries += 1
             time.sleep(60)
         except requests.exceptions.RequestException as e:
-            logger.warning(f"Get general request error: {e}. Retry in 5 minutes...")
+            logger.warning(
+                f"Get general request error: {str(e)}. Retry in 5 minutes..."
+            )
             retries += 1
             time.sleep(300)
     logger.error(f"Get request failed after {max_retries + 1} attempts.")
     return None
```

### Comparing `cru-dse-utils-0.1.1/src/cru_dse_utils.egg-info/PKG-INFO` & `cru-dse-utils-0.1.3/src/cru_dse_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cru-dse-utils
-Version: 0.1.1
+Version: 0.1.3
 Summary: Cru DSE Python Utils
-Author-email: Cru/Tony Guan <tony.guan@cru.org>
+Author-email: Cru DSE Team <tony.guan@cru.org>
 License: MIT License
         
         Copyright (c) [2023] [Cru]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -22,29 +22,32 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repository, https://github.com/CruGlobal/dse-python-utils
+Project-URL: homepage, https://github.com/CruGlobal/dse-python-utils
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
 
-# dse-python-utils
+# cru-dse-utils
 This is a package of useful functions developed by the Cru Data Sciences & Engineering team. The package includes the following files:
 
 - `general.py`: Contains general data extraction related functions.
+- `auth.py`: Contains functions for fetching credentials. 
 - `bigquery.py`: Contains functions for bigquery operations.
+- `gcs.py`: Contains functions for Google Cloud Storage operations.
 - `dbt.py`: Contains functions for dbt operations.
 
 ## Installation
 To install the package, run the following command:
 `pip install cru-dse-utils`
 
 ## Usage
```

