# Comparing `tmp/influxdb3-python-0.1.5.tar.gz` & `tmp/influxdb3-python-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-0.1.5.tar", last modified: Mon Jul  3 14:10:43 2023, max compression
+gzip compressed data, was "influxdb3-python-0.1.6.tar", last modified: Mon Jul 10 11:50:48 2023, max compression
```

## Comparing `influxdb3-python-0.1.5.tar` & `influxdb3-python-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:43.538594 influxdb3-python-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 14:10:30.000000 influxdb3-python-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-03 14:10:43.538594 influxdb3-python-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-03 14:10:30.000000 influxdb3-python-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:43.538594 influxdb3-python-0.1.5/influxdb3_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-03 14:10:43.000000 influxdb3-python-0.1.5/influxdb3_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-03 14:10:43.000000 influxdb3-python-0.1.5/influxdb3_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:10:43.000000 influxdb3-python-0.1.5/influxdb3_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 14:10:43.000000 influxdb3-python-0.1.5/influxdb3_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 14:10:43.000000 influxdb3-python-0.1.5/influxdb3_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:43.538594 influxdb3-python-0.1.5/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-03 14:10:30.000000 influxdb3-python-0.1.5/influxdb_client_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-03 14:10:30.000000 influxdb3-python-0.1.5/influxdb_client_3/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:10:43.538594 influxdb3-python-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-03 14:10:30.000000 influxdb3-python-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:43.538594 influxdb3-python-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-03 14:10:30.000000 influxdb3-python-0.1.5/tests/test_influxdb_client_3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:50:48.201254 influxdb3-python-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 11:50:38.000000 influxdb3-python-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-10 11:50:48.201254 influxdb3-python-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-10 11:50:38.000000 influxdb3-python-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:50:48.201254 influxdb3-python-0.1.6/influxdb3_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-10 11:50:48.000000 influxdb3-python-0.1.6/influxdb3_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-10 11:50:48.000000 influxdb3-python-0.1.6/influxdb3_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 11:50:48.000000 influxdb3-python-0.1.6/influxdb3_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 11:50:48.000000 influxdb3-python-0.1.6/influxdb3_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 11:50:48.000000 influxdb3-python-0.1.6/influxdb3_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:50:48.201254 influxdb3-python-0.1.6/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-10 11:50:38.000000 influxdb3-python-0.1.6/influxdb_client_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-10 11:50:38.000000 influxdb3-python-0.1.6/influxdb_client_3/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 11:50:48.201254 influxdb3-python-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-10 11:50:38.000000 influxdb3-python-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:50:48.201254 influxdb3-python-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-10 11:50:38.000000 influxdb3-python-0.1.6/tests/test_influxdb_client_3.py
```

### Comparing `influxdb3-python-0.1.5/LICENSE` & `influxdb3-python-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.5/PKG-INFO` & `influxdb3-python-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `influxdb3-python-0.1.5/README.md` & `influxdb3-python-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.5/influxdb3_python.egg-info/PKG-INFO` & `influxdb3-python-0.1.6/influxdb3_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `influxdb3-python-0.1.5/influxdb_client_3/__init__.py` & `influxdb3-python-0.1.6/influxdb_client_3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         :type write_client_options: dict
         :param flight_client_options: Options for the FlightClient.
         :type flight_client_options: dict
         :param kwargs: Additional arguments for the InfluxDB Client.
         """
         self._org = org
         self._database = database
-        self._write_client_options = write_client_options or {'write_options': SYNCHRONOUS}
+        self._write_client_options = write_client_options or write_client_options(write_options=SYNCHRONOUS)
 
         # Extracting the hostname from URL if provided
         parsed_url = urllib.parse.urlparse(host)
         host = parsed_url.hostname or host
 
         self._client = _InfluxDBClient(
             url=f"https://{host}",
```

### Comparing `influxdb3-python-0.1.5/influxdb_client_3/read_file.py` & `influxdb3-python-0.1.6/influxdb_client_3/read_file.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.5/setup.py` & `influxdb3-python-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.5/tests/test_influxdb_client_3.py` & `influxdb3-python-0.1.6/tests/test_influxdb_client_3.py`

 * *Files identical despite different names*

