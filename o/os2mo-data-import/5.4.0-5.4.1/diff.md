# Comparing `tmp/os2mo_data_import-5.4.0.tar.gz` & `tmp/os2mo_data_import-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2mo_data_import-5.4.0.tar", max compression
+gzip compressed data, was "os2mo_data_import-5.4.1.tar", max compression
```

## Comparing `os2mo_data_import-5.4.0.tar` & `os2mo_data_import-5.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0        0        0        0 2023-06-14 12:01:32.702858 os2mo_data_import-5.4.0/LICENSES/
--rw-r--r--   0        0        0    11696 2023-06-14 12:01:32.702858 os2mo_data_import-5.4.0/README.rst
--rw-r--r--   0        0        0      332 2023-06-14 12:01:32.703858 os2mo_data_import-5.4.0/mox_helpers/__init__.py
--rw-r--r--   0        0        0     7243 2023-06-14 12:01:32.703858 os2mo_data_import-5.4.0/mox_helpers/mox_helper.py
--rw-r--r--   0        0        0    20756 2023-06-14 12:01:32.704858 os2mo_data_import-5.4.0/mox_helpers/mox_util.py
--rw-r--r--   0        0        0     2736 2023-06-14 12:01:32.704858 os2mo_data_import-5.4.0/mox_helpers/payloads.py
--rw-r--r--   0        0        0       40 2023-06-14 12:01:32.704858 os2mo_data_import-5.4.0/mox_helpers/requirements.txt
--rw-r--r--   0        0        0      899 2023-06-14 12:01:32.704858 os2mo_data_import-5.4.0/mox_helpers/utils.py
--rw-r--r--   0        0        0      397 2023-06-14 12:01:32.704858 os2mo_data_import-5.4.0/os2mo_data_import/__init__.py
--rw-r--r--   0        0        0     3799 2023-06-14 12:01:32.704858 os2mo_data_import-5.4.0/os2mo_data_import/caching_import.py
--rw-r--r--   0        0        0     1300 2023-06-14 12:01:32.705859 os2mo_data_import-5.4.0/os2mo_data_import/defaults.py
--rw-r--r--   0        0        0    19484 2023-06-14 12:01:32.705859 os2mo_data_import-5.4.0/os2mo_data_import/helpers.py
--rw-r--r--   0        0        0    22987 2023-06-14 12:01:32.705859 os2mo_data_import-5.4.0/os2mo_data_import/mora_data_types.py
--rw-r--r--   0        0        0    13436 2023-06-14 12:01:32.706858 os2mo_data_import-5.4.0/os2mo_data_import/mox_data_types.py
--rw-r--r--   0        0        0       99 2023-06-14 12:01:32.706858 os2mo_data_import-5.4.0/os2mo_data_import/tests/__init__.py
--rw-r--r--   0        0        0     1650 2023-06-14 12:01:32.706858 os2mo_data_import-5.4.0/os2mo_data_import/tests/test_utilities.py
--rw-r--r--   0        0        0    27431 2023-06-14 12:01:32.706858 os2mo_data_import-5.4.0/os2mo_data_import/utilities.py
--rw-r--r--   0        0        0      332 2023-06-14 12:01:32.707859 os2mo_data_import-5.4.0/os2mo_helpers/__init__.py
--rw-r--r--   0        0        0    30502 2023-06-14 12:01:32.707859 os2mo_data_import-5.4.0/os2mo_helpers/mora_helpers.py
--rw-r--r--   0        0        0       41 2023-06-14 12:01:32.707859 os2mo_data_import-5.4.0/os2mo_helpers/requirements.txt
--rw-r--r--   0        0        0     1169 2023-06-14 12:01:32.707859 os2mo_data_import-5.4.0/os2mo_helpers/settings.py
--rw-r--r--   0        0        0       99 2023-06-14 12:01:32.708859 os2mo_data_import-5.4.0/os2mo_helpers/tests/__init__.py
--rw-r--r--   0        0        0     3412 2023-06-14 12:01:32.708859 os2mo_data_import-5.4.0/os2mo_helpers/tests/test_morahelpers.py
--rw-r--r--   0        0        0     1054 2023-06-14 12:01:33.402911 os2mo_data_import-5.4.0/pyproject.toml
--rw-r--r--   0        0        0    13094 1970-01-01 00:00:00.000000 os2mo_data_import-5.4.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-07-10 12:46:39.778113 os2mo_data_import-5.4.1/LICENSES/
+-rw-r--r--   0        0        0    11696 2023-07-10 12:46:39.779114 os2mo_data_import-5.4.1/README.rst
+-rw-r--r--   0        0        0      332 2023-07-10 12:46:39.779114 os2mo_data_import-5.4.1/mox_helpers/__init__.py
+-rw-r--r--   0        0        0     7243 2023-07-10 12:46:39.779114 os2mo_data_import-5.4.1/mox_helpers/mox_helper.py
+-rw-r--r--   0        0        0    20756 2023-07-10 12:46:39.779114 os2mo_data_import-5.4.1/mox_helpers/mox_util.py
+-rw-r--r--   0        0        0     2736 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/mox_helpers/payloads.py
+-rw-r--r--   0        0        0       40 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/mox_helpers/requirements.txt
+-rw-r--r--   0        0        0      899 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/mox_helpers/utils.py
+-rw-r--r--   0        0        0      397 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/os2mo_data_import/__init__.py
+-rw-r--r--   0        0        0     3799 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/os2mo_data_import/caching_import.py
+-rw-r--r--   0        0        0     1300 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/os2mo_data_import/defaults.py
+-rw-r--r--   0        0        0    19484 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/os2mo_data_import/helpers.py
+-rw-r--r--   0        0        0    22987 2023-07-10 12:46:39.781114 os2mo_data_import-5.4.1/os2mo_data_import/mora_data_types.py
+-rw-r--r--   0        0        0    13436 2023-07-10 12:46:39.781114 os2mo_data_import-5.4.1/os2mo_data_import/mox_data_types.py
+-rw-r--r--   0        0        0       99 2023-07-10 12:46:39.781114 os2mo_data_import-5.4.1/os2mo_data_import/tests/__init__.py
+-rw-r--r--   0        0        0     1650 2023-07-10 12:46:39.781114 os2mo_data_import-5.4.1/os2mo_data_import/tests/test_utilities.py
+-rw-r--r--   0        0        0    27431 2023-07-10 12:46:39.782114 os2mo_data_import-5.4.1/os2mo_data_import/utilities.py
+-rw-r--r--   0        0        0      332 2023-07-10 12:46:39.782114 os2mo_data_import-5.4.1/os2mo_helpers/__init__.py
+-rw-r--r--   0        0        0    30591 2023-07-10 12:46:39.782114 os2mo_data_import-5.4.1/os2mo_helpers/mora_helpers.py
+-rw-r--r--   0        0        0       41 2023-07-10 12:46:39.782114 os2mo_data_import-5.4.1/os2mo_helpers/requirements.txt
+-rw-r--r--   0        0        0     1169 2023-07-10 12:46:39.783114 os2mo_data_import-5.4.1/os2mo_helpers/settings.py
+-rw-r--r--   0        0        0       99 2023-07-10 12:46:39.783114 os2mo_data_import-5.4.1/os2mo_helpers/tests/__init__.py
+-rw-r--r--   0        0        0     3412 2023-07-10 12:46:39.783114 os2mo_data_import-5.4.1/os2mo_helpers/tests/test_morahelpers.py
+-rw-r--r--   0        0        0     1054 2023-07-10 12:46:41.055231 os2mo_data_import-5.4.1/pyproject.toml
+-rw-r--r--   0        0        0    13094 1970-01-01 00:00:00.000000 os2mo_data_import-5.4.1/PKG-INFO
```

### Comparing `os2mo_data_import-5.4.0/README.rst` & `os2mo_data_import-5.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/mox_helpers/mox_helper.py` & `os2mo_data_import-5.4.1/mox_helpers/mox_helper.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/mox_helpers/mox_util.py` & `os2mo_data_import-5.4.1/mox_helpers/mox_util.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/mox_helpers/payloads.py` & `os2mo_data_import-5.4.1/mox_helpers/payloads.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/mox_helpers/utils.py` & `os2mo_data_import-5.4.1/mox_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/os2mo_data_import/caching_import.py` & `os2mo_data_import-5.4.1/os2mo_data_import/caching_import.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/os2mo_data_import/defaults.py` & `os2mo_data_import-5.4.1/os2mo_data_import/defaults.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/os2mo_data_import/helpers.py` & `os2mo_data_import-5.4.1/os2mo_data_import/helpers.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/os2mo_data_import/mora_data_types.py` & `os2mo_data_import-5.4.1/os2mo_data_import/mora_data_types.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/os2mo_data_import/mox_data_types.py` & `os2mo_data_import-5.4.1/os2mo_data_import/mox_data_types.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/os2mo_data_import/tests/test_utilities.py` & `os2mo_data_import-5.4.1/os2mo_data_import/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/os2mo_data_import/utilities.py` & `os2mo_data_import-5.4.1/os2mo_data_import/utilities.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/os2mo_helpers/mora_helpers.py` & `os2mo_data_import-5.4.1/os2mo_helpers/mora_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -652,14 +652,17 @@
             for validity in validity_times:
                 persons = self._mo_lookup(
                     org_uuid, "ou/{}/details/" + person_type, validity=validity
                 )
                 all_persons = all_persons + persons
 
         for person in all_persons:
+            if not person:
+                # Vacant association
+                continue
             uuid = person["person"]["uuid"]
             data = {
                 "Ansættelse gyldig fra": person["validity"]["from"],
                 "Ansættelse gyldig til": person["validity"]["to"],
                 "Person UUID": uuid,
                 "Org-enhed": person["org_unit"]["name"],
                 "Org-enhed UUID": person["org_unit"]["uuid"],
```

### Comparing `os2mo_data_import-5.4.0/os2mo_helpers/settings.py` & `os2mo_data_import-5.4.1/os2mo_helpers/settings.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/os2mo_helpers/tests/test_morahelpers.py` & `os2mo_data_import-5.4.1/os2mo_helpers/tests/test_morahelpers.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.0/pyproject.toml` & `os2mo_data_import-5.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "os2mo_data_import"
-version = "5.4.0"
+version = "5.4.1"
 description = "A set of tools for OS2MO data import and export"
 authors = ["Magenta <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.rst"
 repository = "https://git.magenta.dk/rammearkitektur/os2mo_data_import"
 keywords = ["os2mo", "dipex"]
 packages = [
```

### Comparing `os2mo_data_import-5.4.0/PKG-INFO` & `os2mo_data_import-5.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2mo-data-import
-Version: 5.4.0
+Version: 5.4.1
 Summary: A set of tools for OS2MO data import and export
 Home-page: https://git.magenta.dk/rammearkitektur/os2mo_data_import
 License: MPL-2.0
 Keywords: os2mo,dipex
 Author: Magenta
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
```

