# Comparing `tmp/coscine-0.9.3.tar.gz` & `tmp/coscine-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coscine-0.9.3.tar", last modified: Thu Jun 22 14:08:05 2023, max compression
+gzip compressed data, was "dist/coscine-0.9.4.tar", last modified: Mon Jul 10 19:03:18 2023, max compression
```

## Comparing `coscine-0.9.3.tar` & `coscine-0.9.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:08:05.000000 coscine-0.9.3/
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-04-11 13:11:08.000000 coscine-0.9.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     7630 2023-06-22 14:08:05.000000 coscine-0.9.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6100 2023-06-22 14:06:09.000000 coscine-0.9.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 14:08:05.000000 coscine-0.9.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3905 2023-04-11 13:11:08.000000 coscine-0.9.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:08:05.000000 coscine-0.9.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine/
--rw-rw-rw-   0 root         (0) root         (0)     2954 2023-06-22 14:06:09.000000 coscine-0.9.3/src/coscine/__about__.py
--rw-rw-rw-   0 root         (0) root         (0)     2231 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6267 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    24288 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine/data/
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/data/project.json
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/data/resource.json
--rw-rw-rw-   0 root         (0) root         (0)     2276 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)    28275 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/form.py
--rw-rw-rw-   0 root         (0) root         (0)     6907 2023-06-22 14:06:09.000000 coscine-0.9.3/src/coscine/graph.py
--rw-rw-rw-   0 root         (0) root         (0)    19265 2023-06-22 14:06:09.000000 coscine-0.9.3/src/coscine/object.py
--rw-rw-rw-   0 root         (0) root         (0)    21761 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/project.py
--rw-rw-rw-   0 root         (0) root         (0)    26362 2023-04-11 13:46:13.000000 coscine-0.9.3/src/coscine/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     7402 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/s3.py
--rw-rw-rw-   0 root         (0) root         (0)    11884 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14870 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/vocabulary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7630 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:03:18.000000 coscine-0.9.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2023-04-11 13:11:08.000000 coscine-0.9.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     7001 2023-07-10 19:03:18.000000 coscine-0.9.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5471 2023-07-10 19:00:16.000000 coscine-0.9.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 19:03:18.000000 coscine-0.9.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2023-04-11 13:11:08.000000 coscine-0.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:03:18.000000 coscine-0.9.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine/
+-rw-rw-rw-   0 root         (0) root         (0)     2954 2023-07-10 19:00:16.000000 coscine-0.9.4/src/coscine/__about__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2231 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6267 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    24288 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/data/project.json
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/data/resource.json
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)    28689 2023-07-10 19:00:16.000000 coscine-0.9.4/src/coscine/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     6907 2023-06-22 14:06:09.000000 coscine-0.9.4/src/coscine/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    19265 2023-06-22 14:06:09.000000 coscine-0.9.4/src/coscine/object.py
+-rw-rw-rw-   0 root         (0) root         (0)    21761 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/project.py
+-rw-rw-rw-   0 root         (0) root         (0)    26362 2023-04-11 13:46:13.000000 coscine-0.9.4/src/coscine/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     7402 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)    11884 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14870 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/vocabulary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7001 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine.egg-info/top_level.txt
```

### Comparing `coscine-0.9.3/LICENSE.txt` & `coscine-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/PKG-INFO` & `coscine-0.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coscine
-Version: 0.9.3
+Version: 0.9.4
 Summary: The Coscine Python SDK provides a pythonic interface to the Coscine REST API.
 Home-page: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/
 Author: RWTH Aachen University
 Author-email: coscine@itc.rwth-aachen.de
 License: MIT License
 Project-URL: Issues, https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/issues
 Project-URL: Documentation, https://coscine.pages.rwth-aachen.de/community-features/coscine-python-sdk/
@@ -24,23 +24,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-## DISCLAIMER
-> Issues have been permanently disabled due to increasing amounts of spam.
-> If you have any questions or would like to report a bug, request a feature or
-> have any other business similar to that, you can send a good old-fashioned E-Mail
-> to the [Coscine Technical Adaption Mailing List](mailto:coscine-technical-adaptation@itc.rwth-aachen.de)
-> or contact me personally via my personal Mail (Click on my GitLab profile and copy the full name
-> in the browsers address bar including the dot between first and last name.
-> Then append (at) rwth-aachen.de). In either cases I'll get a Mail and am able to respond.
-
 # Coscine Python SDK
 ![Coscine] ![Python]  
 [Coscine](https://coscine.de/), short for **Co**llaborative **Sc**ientific
 **In**tegration **E**nvironment, is a platform for Research Data Management.  
 
 [Coscine]: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/raw/master/data/coscine_logo_rgb.png
 [Python]: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/raw/master/data/python-powered-w-200x80.png
```

### Comparing `coscine-0.9.3/README.md` & `coscine-0.9.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-## DISCLAIMER
-> Issues have been permanently disabled due to increasing amounts of spam.
-> If you have any questions or would like to report a bug, request a feature or
-> have any other business similar to that, you can send a good old-fashioned E-Mail
-> to the [Coscine Technical Adaption Mailing List](mailto:coscine-technical-adaptation@itc.rwth-aachen.de)
-> or contact me personally via my personal Mail (Click on my GitLab profile and copy the full name
-> in the browsers address bar including the dot between first and last name.
-> Then append (at) rwth-aachen.de). In either cases I'll get a Mail and am able to respond.
-
 # Coscine Python SDK
 ![Coscine] ![Python]  
 [Coscine](https://coscine.de/), short for **Co**llaborative **Sc**ientific
 **In**tegration **E**nvironment, is a platform for Research Data Management.  
 
 [Coscine]: ./data/coscine_logo_rgb.png
 [Python]: ./data/python-powered-w-200x80.png
```

### Comparing `coscine-0.9.3/setup.py` & `coscine-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine/__about__.py` & `coscine-0.9.4/src/coscine/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ###############################################################################
 
 # Package title/name as it would appear in PyPi
 __title__ = "coscine"
 
 # Current package version
 # Do not set version to 1.0.0 before update to Coscine API version 2
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 # Short package description
 __summary__ = (
     "The Coscine Python SDK provides a pythonic interface to "
     "the Coscine REST API."
 )
```

### Comparing `coscine-0.9.3/src/coscine/__init__.py` & `coscine-0.9.4/src/coscine/__init__.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine/cache.py` & `coscine-0.9.4/src/coscine/cache.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine/client.py` & `coscine-0.9.4/src/coscine/client.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine/data/project.json` & `coscine-0.9.4/src/coscine/data/project.json`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine/data/resource.json` & `coscine-0.9.4/src/coscine/data/resource.json`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine/defaults.py` & `coscine-0.9.4/src/coscine/defaults.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine/form.py` & `coscine-0.9.4/src/coscine/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -576,43 +576,54 @@
         for item in XSD_TYPES.values():
             if xsd_type in item["values"]:
                 return item["type"]
         return str
 
 ###############################################################################
 
+    def xsd_type(self, key: str) -> str:
+        """
+        Returns the xsd type identifier for a given field.
+        """
+        datatype = self.properties(key).datatype
+        if datatype and datatype.startswith("http:"):
+            datatype = f"xsd:{urllib.parse.urlparse(datatype)[-1]}"
+        return datatype
+
 ###############################################################################
 
     def datatype(self, key: str) -> type:
         """
         Returns the datatype for a given field (which may be None).
         """
-        datatype = self.properties(key).datatype
-        if datatype and datatype.startswith("http:"):
-            datatype = f"xsd:{urllib.parse.urlparse(datatype)[-1]}"
         if self.is_controlled(key):
             return str
-        return self._xsd_typeof(datatype)
+        else:
+            datatype: str = self.xsd_type(key)
+            return self._xsd_typeof(datatype)
 
 ###############################################################################
-
+# FIXME: Lots of xsd types still unhandled, especially datetime formats
     def type_format(self, key: str) -> str:
         """
         Returns the format for a datatype of a field.
         This is especially useful for instances of type datetype.
         """
         datatype = self.datatype(key)
         if datatype == str:
             return "%s"
         if datatype in (bool, int):
             return "%d"
         if datatype == float:
             return "%f"
         if datatype == datetime:
-            return "%Y-%m-%d"
+            if self.xsd_type(key) == "xsd:dateTime":
+                return "%Y-%m-%dT%H:%M:%S"
+            else:
+                return "%Y-%m-%d"
         return "Invalid Format"
 
 ###############################################################################
 
     def is_typed(self, key: str) -> bool:
         """
         Returns whether a value is expecting a certain datatype.
```

### Comparing `coscine-0.9.3/src/coscine/graph.py` & `coscine-0.9.4/src/coscine/graph.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine/object.py` & `coscine-0.9.4/src/coscine/object.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine/project.py` & `coscine-0.9.4/src/coscine/project.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine/resource.py` & `coscine-0.9.4/src/coscine/resource.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine/s3.py` & `coscine-0.9.4/src/coscine/s3.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine/utils.py` & `coscine-0.9.4/src/coscine/utils.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine/vocabulary.py` & `coscine-0.9.4/src/coscine/vocabulary.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.3/src/coscine.egg-info/PKG-INFO` & `coscine-0.9.4/src/coscine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coscine
-Version: 0.9.3
+Version: 0.9.4
 Summary: The Coscine Python SDK provides a pythonic interface to the Coscine REST API.
 Home-page: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/
 Author: RWTH Aachen University
 Author-email: coscine@itc.rwth-aachen.de
 License: MIT License
 Project-URL: Issues, https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/issues
 Project-URL: Documentation, https://coscine.pages.rwth-aachen.de/community-features/coscine-python-sdk/
@@ -24,23 +24,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-## DISCLAIMER
-> Issues have been permanently disabled due to increasing amounts of spam.
-> If you have any questions or would like to report a bug, request a feature or
-> have any other business similar to that, you can send a good old-fashioned E-Mail
-> to the [Coscine Technical Adaption Mailing List](mailto:coscine-technical-adaptation@itc.rwth-aachen.de)
-> or contact me personally via my personal Mail (Click on my GitLab profile and copy the full name
-> in the browsers address bar including the dot between first and last name.
-> Then append (at) rwth-aachen.de). In either cases I'll get a Mail and am able to respond.
-
 # Coscine Python SDK
 ![Coscine] ![Python]  
 [Coscine](https://coscine.de/), short for **Co**llaborative **Sc**ientific
 **In**tegration **E**nvironment, is a platform for Research Data Management.  
 
 [Coscine]: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/raw/master/data/coscine_logo_rgb.png
 [Python]: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/raw/master/data/python-powered-w-200x80.png
```

### Comparing `coscine-0.9.3/src/coscine.egg-info/SOURCES.txt` & `coscine-0.9.4/src/coscine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

