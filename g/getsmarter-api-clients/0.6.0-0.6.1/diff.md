# Comparing `tmp/getsmarter-api-clients-0.6.0.tar.gz` & `tmp/getsmarter-api-clients-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getsmarter-api-clients-0.6.0.tar", last modified: Fri Jun  9 14:52:35 2023, max compression
+gzip compressed data, was "getsmarter-api-clients-0.6.1.tar", last modified: Mon Jul 10 17:17:25 2023, max compression
```

## Comparing `getsmarter-api-clients-0.6.0.tar` & `getsmarter-api-clients-0.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:52:35.072590 getsmarter-api-clients-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6585 2023-06-09 14:52:35.072590 getsmarter-api-clients-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:52:35.068590 getsmarter-api-clients-0.6.0/getsmarter_api_clients/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9923 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients/geag.py
--rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:52:35.072590 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6585 2023-06-09 14:52:35.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-09 14:52:35.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 14:52:35.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 14:52:35.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-09 14:52:35.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-09 14:52:35.000000 getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:52:35.072590 getsmarter-api-clients-0.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-09 14:52:35.072590 getsmarter-api-clients-0.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     4952 2023-06-09 14:52:30.000000 getsmarter-api-clients-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 17:17:25.068928 getsmarter-api-clients-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-07-10 17:17:19.000000 getsmarter-api-clients-0.6.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-10 17:17:19.000000 getsmarter-api-clients-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-07-10 17:17:19.000000 getsmarter-api-clients-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6654 2023-07-10 17:17:25.068928 getsmarter-api-clients-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-07-10 17:17:19.000000 getsmarter-api-clients-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 17:17:25.064928 getsmarter-api-clients-0.6.1/getsmarter_api_clients/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-10 17:17:19.000000 getsmarter-api-clients-0.6.1/getsmarter_api_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10842 2023-07-10 17:17:19.000000 getsmarter-api-clients-0.6.1/getsmarter_api_clients/geag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-07-10 17:17:19.000000 getsmarter-api-clients-0.6.1/getsmarter_api_clients/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 17:17:25.068928 getsmarter-api-clients-0.6.1/getsmarter_api_clients.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6654 2023-07-10 17:17:25.000000 getsmarter-api-clients-0.6.1/getsmarter_api_clients.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-07-10 17:17:25.000000 getsmarter-api-clients-0.6.1/getsmarter_api_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 17:17:25.000000 getsmarter-api-clients-0.6.1/getsmarter_api_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 17:17:25.000000 getsmarter-api-clients-0.6.1/getsmarter_api_clients.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-10 17:17:25.000000 getsmarter-api-clients-0.6.1/getsmarter_api_clients.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-10 17:17:25.000000 getsmarter-api-clients-0.6.1/getsmarter_api_clients.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 17:17:25.068928 getsmarter-api-clients-0.6.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-07-10 17:17:19.000000 getsmarter-api-clients-0.6.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-10 17:17:19.000000 getsmarter-api-clients-0.6.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-07-10 17:17:25.068928 getsmarter-api-clients-0.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4952 2023-07-10 17:17:19.000000 getsmarter-api-clients-0.6.1/setup.py
```

### Comparing `getsmarter-api-clients-0.6.0/CHANGELOG.rst` & `getsmarter-api-clients-0.6.1/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 * Nothing unreleased
 
+[0.6.1]
+~~~~~~~
+* Adds an enterprise allocation cancellation method
+
 [0.6.0]
 ~~~~~~~
 * Adds optional arg to create_enterprise_allocation() to either raise (current/default behavior),
   or not raise and fall through to returning the response. This will allow callers
   to do things with the response payload in error conditions.
 
 [0.5.4]
```

### Comparing `getsmarter-api-clients-0.6.0/LICENSE.txt` & `getsmarter-api-clients-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.6.0/PKG-INFO` & `getsmarter-api-clients-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getsmarter-api-clients
-Version: 0.6.0
+Version: 0.6.1
 Summary: Clients to interact with GetSmarter APIs.
 Home-page: https://github.com/edx/getsmarter-api-clients
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -168,14 +168,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 * Nothing unreleased
 
+[0.6.1]
+~~~~~~~
+* Adds an enterprise allocation cancellation method
+
 [0.6.0]
 ~~~~~~~
 * Adds optional arg to create_enterprise_allocation() to either raise (current/default behavior),
   or not raise and fall through to returning the response. This will allow callers
   to do things with the response payload in error conditions.
 
 [0.5.4]
```

### Comparing `getsmarter-api-clients-0.6.0/README.rst` & `getsmarter-api-clients-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.6.0/getsmarter_api_clients/geag.py` & `getsmarter-api-clients-0.6.1/getsmarter_api_clients/geag.py`

 * *Files 6% similar despite different names*

```diff
@@ -269,7 +269,39 @@
               f'with reasons: {response.text}, '
               f'with payload: {payload}'
             )
             logger.error(message)
             if should_raise:
                 raise
         return response
+
+    def cancel_enterprise_allocation(
+        self,
+        order_uuid,
+        should_raise=True,
+    ):
+        """
+        Cancel an enterprise_allocation (enrollment) through GEAG.
+
+        :Parameters:
+          - `order_uuid` (str): The order UUID of the allocation
+          - `should_raise` (boolean): Should exceptions be re-raised
+        """
+        url = f'{self.api_url}/enterprise_allocations/cancel'
+
+        payload = {
+            'orderUuid': str(order_uuid),
+        }
+
+        response = self.post(url, json=payload)
+        try:
+            response.raise_for_status()
+        except HTTPError:
+            message = (
+              f'Allocation cancelation failed for {order_uuid} '
+              f'with reasons: {response.text}, '
+              f'with payload: {payload}'
+            )
+            logger.error(message)
+            if should_raise:
+                raise
+        return response
```

### Comparing `getsmarter-api-clients-0.6.0/getsmarter_api_clients/oauth.py` & `getsmarter-api-clients-0.6.1/getsmarter_api_clients/oauth.py`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.6.0/getsmarter_api_clients.egg-info/PKG-INFO` & `getsmarter-api-clients-0.6.1/getsmarter_api_clients.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getsmarter-api-clients
-Version: 0.6.0
+Version: 0.6.1
 Summary: Clients to interact with GetSmarter APIs.
 Home-page: https://github.com/edx/getsmarter-api-clients
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -168,14 +168,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 * Nothing unreleased
 
+[0.6.1]
+~~~~~~~
+* Adds an enterprise allocation cancellation method
+
 [0.6.0]
 ~~~~~~~
 * Adds optional arg to create_enterprise_allocation() to either raise (current/default behavior),
   or not raise and fall through to returning the response. This will allow callers
   to do things with the response payload in error conditions.
 
 [0.5.4]
```

### Comparing `getsmarter-api-clients-0.6.0/requirements/constraints.txt` & `getsmarter-api-clients-0.6.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.6.0/setup.py` & `getsmarter-api-clients-0.6.1/setup.py`

 * *Files identical despite different names*

