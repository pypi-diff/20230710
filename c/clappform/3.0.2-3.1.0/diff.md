# Comparing `tmp/clappform-3.0.2.tar.gz` & `tmp/clappform-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clappform-3.0.2.tar", last modified: Mon Jul 10 07:50:45 2023, max compression
+gzip compressed data, was "clappform-3.1.0.tar", last modified: Mon Jul 10 08:04:41 2023, max compression
```

## Comparing `clappform-3.0.2.tar` & `clappform-3.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:50:45.021735 clappform-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 07:50:32.000000 clappform-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-10 07:50:45.021735 clappform-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-10 07:50:32.000000 clappform-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-10 07:50:32.000000 clappform-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 07:50:45.021735 clappform-3.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:50:45.021735 clappform-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:50:45.021735 clappform-3.0.2/src/clappform/
--rw-r--r--   0 runner    (1001) docker     (123)    24898 2023-07-10 07:50:32.000000 clappform-3.0.2/src/clappform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-07-10 07:50:32.000000 clappform-3.0.2/src/clappform/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-10 07:50:32.000000 clappform-3.0.2/src/clappform/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:50:45.021735 clappform-3.0.2/src/clappform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-10 07:50:45.000000 clappform-3.0.2/src/clappform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-10 07:50:45.000000 clappform-3.0.2/src/clappform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:50:45.000000 clappform-3.0.2/src/clappform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 07:50:45.000000 clappform-3.0.2/src/clappform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 07:50:45.000000 clappform-3.0.2/src/clappform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-10 07:50:32.000000 clappform-3.0.2/src/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:04:41.903506 clappform-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 08:04:31.000000 clappform-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-10 08:04:41.903506 clappform-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-10 08:04:31.000000 clappform-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-10 08:04:31.000000 clappform-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 08:04:41.903506 clappform-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:04:41.903506 clappform-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:04:41.903506 clappform-3.1.0/src/clappform/
+-rw-r--r--   0 runner    (1001) docker     (123)    26080 2023-07-10 08:04:31.000000 clappform-3.1.0/src/clappform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-07-10 08:04:31.000000 clappform-3.1.0/src/clappform/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-10 08:04:31.000000 clappform-3.1.0/src/clappform/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:04:41.903506 clappform-3.1.0/src/clappform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-10 08:04:41.000000 clappform-3.1.0/src/clappform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-10 08:04:41.000000 clappform-3.1.0/src/clappform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:04:41.000000 clappform-3.1.0/src/clappform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 08:04:41.000000 clappform-3.1.0/src/clappform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 08:04:41.000000 clappform-3.1.0/src/clappform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-10 08:04:31.000000 clappform-3.1.0/src/debug.py
```

### Comparing `clappform-3.0.2/LICENSE` & `clappform-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clappform-3.0.2/PKG-INFO` & `clappform-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 3.0.2
+Version: 3.1.0
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clappform-3.0.2/README.md` & `clappform-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `clappform-3.0.2/pyproject.toml` & `clappform-3.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clappform"
-version = "3.0.2"
+version = "3.1.0"
 authors= [
     { name="Clappform B.V.", email="info@clappform.com" },
 ]
 description = "Clappform Python API wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -52,8 +52,9 @@
 '''
 
 [tool.pylint]
 max-line-length = 88
 disable = [
     "C0103", # (invalid-name)
     "R0902", # (too-many-instance-attributes)
+    "W0613", # (unused-argument)
 ]
```

### Comparing `clappform-3.0.2/src/clappform/__init__.py` & `clappform-3.1.0/src/clappform/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 :copyright: (c) 2022 Clappform B.V..
 :license: MIT, see LICENSE for more details.
 """
 __requires__ = ["requests==2.28.1", "Cerberus==1.3.4", "pandas==1.5.2"]
 # Python Standard Library modules
 from urllib.parse import urlparse
 from dataclasses import asdict
+from concurrent import futures
 import tempfile
 import math
 import time
+import os
 
 # PyPi modules
 from requests.adapters import HTTPAdapter
 import requests as r
 
 from cerberus import Validator
 from pandas import DataFrame
@@ -27,15 +29,15 @@
     HTTPError,
     PaginationTotalError,
     PaginationKeyError,
 )
 
 
 # Metadata
-__version__ = "3.0.2"
+__version__ = "3.1.0"
 __author__ = "Clappform B.V."
 __email__ = "info@clappform.com"
 __license__ = "MIT"
 __doc__ = "Clappform Python API wrapper"
 
 
 class Clappform:
@@ -89,15 +91,18 @@
         password: str,
     ):
         self._base_url: str = f"{base_url}/api"
 
         #: Session for all HTTP requests.
         self.session: r.sessions.Session = r.Session()
         self.session.headers.update({"User-Agent": self._default_user_agent()})
-        self.session.mount(self._base_url, HTTPAdapter(max_retries=3))
+        self.session.mount(
+            self._base_url,
+            HTTPAdapter(max_retries=3, pool_maxsize=min(32, os.cpu_count() + 4)),
+        )
 
         #: Username to use in the :meth:`auth <auth>`
         self.username: str = username
 
         #: Password to use in the :meth:`auth <auth>`
         self.password: str = password
 
@@ -352,18 +357,24 @@
             raise TypeError(
                 f"item keyword argument is not of type {list} or {dict}, got {t}"
             )
 
         document = self._private_request("DELETE", resource.one_path())
         return dc.ApiResponse(**document)
 
-    def aggregate_dataframe(self, options: dict, interval_timeout: int = 0):
+    def aggregate_dataframe(
+        self, options: dict, interval_timeout: int = 0, max_workers=None
+    ):
         """Aggregate a dataframe
 
         :param dict options: Options for dataframe aggregation.
+        :param interval_timeout: Optional time to sleep per request, defaults to:
+            ``0.0``.
+        :type interval_timeout: int
+        :param int max_workers: Optional number of workers to use in thread pool.
 
         :returns: Generator to read dataframe
         :rtype: :class:`generator`
         """
         v = Validator(
             {
                 "app": {"type": "string"},
@@ -393,52 +404,60 @@
                 "deep_dive": {"type": "dict"},
             },
             require_all=True,
         )
         v.validate(options)
 
         path = "/dataframe/read_data?extended=true"
-        params = {
-            "method": "POST",
-            "path": path,
-            "json": v.document,
-        }
+        payload = v.document
 
-        document = self._private_request(**params)
+        document = self._private_request("POST", path, json=payload)
         if "total" not in document:
             raise PaginationKeyError(missing_key="total", data=document)
         if document["total"] == 0:
             raise PaginationTotalError(total=document["total"], data=document)
 
         pages_to_get = math.ceil(document["total"] / options["limit"])
         if pages_to_get == 1:
             yield DataFrame(document["data"])
+        elif isinstance(document["next_page"], int):
+            _, *pages = [x * options["limit"] for x in range(pages_to_get)]
+            with futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
+                for result in executor.map(
+                    lambda x: self._private_request(
+                        "POST", f"{path}&next_page={x}", json=payload
+                    ),
+                    pages,
+                ):
+                    yield DataFrame(result["data"])
         else:
             for i in range(pages_to_get):
                 yield DataFrame(document["data"])
                 if i >= pages_to_get - 1:
                     break
-                params["path"] = f"{path}&next_page={document['next_page']}"
-                time.sleep(
-                    interval_timeout
-                )  # Prevent Denial Of Service (dos) flagging.
-                document = self._private_request(**params)
+                time.sleep(interval_timeout)
+                document = self._private_request(
+                    "POST", f"{path}&next_page={document['next_page']}", json=payload
+                )
 
-    def read_dataframe(self, query, limit: int = 100, interval_timeout: int = 0):
+    def read_dataframe(
+        self, query, limit: int = 100, interval_timeout: int = 0, max_workers=None
+    ):
         """Read a dataframe.
 
         :param query: Query to for retreiving data. When Query is of type
             :class:`clappform.dataclasses.Collection` everything inside the collection
             is retreived.
         :type query: :class:`clappform.dataclasses.Query` |
             :class:`clappform.dataclasses.Collection`
         :param int limit: Amount of records to retreive per request.
         :param interval_timeout: Optional time to sleep per request, defaults to:
             ``0.0``.
         :type interval_timeout: int
+        :param int max_workers: Optional number of workers to use in thread pool.
 
         Usage::
 
             >>> from clappform import Clappform
             >>> import clappform.dataclasses as r
             >>> import pandas as pd
             >>> c = Clappform(
@@ -452,49 +471,55 @@
             ...     list_df.append(df)
             >>> master_df = pd.concat(list_df)
 
         :returns: Generator to read dataframe
         :rtype: :class:`generator`
         """
         path = "/dataframe/read_data?extended=true"
-        params = {
-            "method": "POST",
-            "path": path,
-            "json": {"limit": limit},
-        }
+        payload = {"limit": limit}
+
         if isinstance(query, dc.Query):
-            params["json"]["query"] = query.slug
+            payload["query"] = query.slug
         elif isinstance(query, dc.Collection):
-            params["json"]["app"] = query.app
-            params["json"]["collection"] = query.slug
+            payload["app"] = query.app
+            payload["collection"] = query.slug
         else:
             t = type(query)
             raise TypeError(
                 f"query arg must be of type {dc.Query} or {dc.Collection}, got {t}"
             )
 
-        document = self._private_request(**params)
+        document = self._private_request("POST", path, json=payload)
         if "total" not in document:
             raise PaginationKeyError(missing_key="total", data=document)
         if document["total"] == 0:
             raise PaginationTotalError(total=document["total"], data=document)
 
         pages_to_get = math.ceil(document["total"] / limit)
         if pages_to_get == 1:
             yield DataFrame(document["data"])
+        elif isinstance(document["next_page"], int):
+            _, *pages = [x * limit for x in range(pages_to_get)]
+            with futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
+                for result in executor.map(
+                    lambda x: self._private_request(
+                        "POST", f"{path}&next_page={x}", json=payload
+                    ),
+                    pages,
+                ):
+                    yield DataFrame(result["data"])
         else:
             for i in range(pages_to_get):
                 yield DataFrame(document["data"])
-                params["path"] = f"{path}&next_page={document['next_page']}"
                 if i >= pages_to_get - 1:
                     break
-                time.sleep(
-                    interval_timeout
-                )  # Prevent Denial Of Service (dos) flagging.
-                document = self._private_request(**params)
+                time.sleep(interval_timeout)
+                document = self._private_request(
+                    "POST", f"{path}&next_page={document['next_page']}", json=payload
+                )
 
     def write_dataframe(
         self,
         df: DataFrame,
         collection: dc.Collection,
         size: int = 100,
         interval_timeout: int = 0,
```

### Comparing `clappform-3.0.2/src/clappform/dataclasses.py` & `clappform-3.1.0/src/clappform/dataclasses.py`

 * *Files identical despite different names*

### Comparing `clappform-3.0.2/src/clappform/exceptions.py` & `clappform-3.1.0/src/clappform/exceptions.py`

 * *Files identical despite different names*

### Comparing `clappform-3.0.2/src/clappform.egg-info/PKG-INFO` & `clappform-3.1.0/src/clappform.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 3.0.2
+Version: 3.1.0
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

