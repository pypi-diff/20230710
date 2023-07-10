# Comparing `tmp/clappform-3.0.1.tar.gz` & `tmp/clappform-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clappform-3.0.1.tar", last modified: Fri Jun 30 13:12:36 2023, max compression
+gzip compressed data, was "clappform-3.0.2.tar", last modified: Mon Jul 10 07:50:45 2023, max compression
```

## Comparing `clappform-3.0.1.tar` & `clappform-3.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:12:36.638102 clappform-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 13:12:27.000000 clappform-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-30 13:12:36.638102 clappform-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-30 13:12:27.000000 clappform-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-30 13:12:27.000000 clappform-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:12:36.638102 clappform-3.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:12:36.638102 clappform-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:12:36.638102 clappform-3.0.1/src/clappform/
--rw-r--r--   0 runner    (1001) docker     (123)    24897 2023-06-30 13:12:27.000000 clappform-3.0.1/src/clappform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-06-30 13:12:27.000000 clappform-3.0.1/src/clappform/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-30 13:12:27.000000 clappform-3.0.1/src/clappform/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:12:36.638102 clappform-3.0.1/src/clappform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-30 13:12:36.000000 clappform-3.0.1/src/clappform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-30 13:12:36.000000 clappform-3.0.1/src/clappform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:12:36.000000 clappform-3.0.1/src/clappform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 13:12:36.000000 clappform-3.0.1/src/clappform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 13:12:36.000000 clappform-3.0.1/src/clappform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-30 13:12:27.000000 clappform-3.0.1/src/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:50:45.021735 clappform-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 07:50:32.000000 clappform-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-10 07:50:45.021735 clappform-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-10 07:50:32.000000 clappform-3.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-10 07:50:32.000000 clappform-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 07:50:45.021735 clappform-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:50:45.021735 clappform-3.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:50:45.021735 clappform-3.0.2/src/clappform/
+-rw-r--r--   0 runner    (1001) docker     (123)    24898 2023-07-10 07:50:32.000000 clappform-3.0.2/src/clappform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-07-10 07:50:32.000000 clappform-3.0.2/src/clappform/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-10 07:50:32.000000 clappform-3.0.2/src/clappform/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:50:45.021735 clappform-3.0.2/src/clappform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-10 07:50:45.000000 clappform-3.0.2/src/clappform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-10 07:50:45.000000 clappform-3.0.2/src/clappform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:50:45.000000 clappform-3.0.2/src/clappform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 07:50:45.000000 clappform-3.0.2/src/clappform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 07:50:45.000000 clappform-3.0.2/src/clappform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-10 07:50:32.000000 clappform-3.0.2/src/debug.py
```

### Comparing `clappform-3.0.1/LICENSE` & `clappform-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clappform-3.0.1/PKG-INFO` & `clappform-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 3.0.1
+Version: 3.0.2
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clappform-3.0.1/README.md` & `clappform-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `clappform-3.0.1/pyproject.toml` & `clappform-3.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clappform"
-version = "3.0.1"
+version = "3.0.2"
 authors= [
     { name="Clappform B.V.", email="info@clappform.com" },
 ]
 description = "Clappform Python API wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `clappform-3.0.1/src/clappform/__init__.py` & `clappform-3.0.2/src/clappform/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     HTTPError,
     PaginationTotalError,
     PaginationKeyError,
 )
 
 
 # Metadata
-__version__ = "3.0.1"
+__version__ = "3.0.2"
 __author__ = "Clappform B.V."
 __email__ = "info@clappform.com"
 __license__ = "MIT"
 __doc__ = "Clappform Python API wrapper"
 
 
 class Clappform:
@@ -341,15 +341,15 @@
             if isinstance(item, list):
                 # `0` element of `_seperate_id_from_item` is an item's id.
                 oids = [self._seperate_id_from_item(x)[0] for x in item]
             if isinstance(item, dict):
                 oids = [self._seperate_id_from_item(item)[0]]
             if isinstance(oids, list):
                 document = self._private_request(
-                    "DELETE", resource.reate_item_path(), json={"oids": oids}
+                    "DELETE", resource.create_item_path(), json={"oids": oids}
                 )
                 return dc.ApiResponse(**document)
             t = type(item)
             raise TypeError(
                 f"item keyword argument is not of type {list} or {dict}, got {t}"
             )
```

### Comparing `clappform-3.0.1/src/clappform/dataclasses.py` & `clappform-3.0.2/src/clappform/dataclasses.py`

 * *Files identical despite different names*

### Comparing `clappform-3.0.1/src/clappform/exceptions.py` & `clappform-3.0.2/src/clappform/exceptions.py`

 * *Files identical despite different names*

### Comparing `clappform-3.0.1/src/clappform.egg-info/PKG-INFO` & `clappform-3.0.2/src/clappform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 3.0.1
+Version: 3.0.2
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

