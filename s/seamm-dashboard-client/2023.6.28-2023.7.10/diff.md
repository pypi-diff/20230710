# Comparing `tmp/seamm_dashboard_client-2023.6.28.tar.gz` & `tmp/seamm_dashboard_client-2023.7.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamm_dashboard_client-2023.6.28.tar", last modified: Wed Jun 28 12:35:35 2023, max compression
+gzip compressed data, was "seamm_dashboard_client-2023.7.10.tar", last modified: Mon Jul 10 20:44:56 2023, max compression
```

## Comparing `seamm_dashboard_client-2023.6.28.tar` & `seamm_dashboard_client-2023.7.10.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:35:35.796145 seamm_dashboard_client-2023.6.28/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-28 12:35:35.796145 seamm_dashboard_client-2023.6.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:35:35.788145 seamm_dashboard_client-2023.6.28/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     8842 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:35:35.792145 seamm_dashboard_client-2023.6.28/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/developer/cms_plots.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/developer/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/developer/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/developer/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/developer/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/developer/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:35:35.792145 seamm_dashboard_client-2023.6.28/docs/user/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/docs/user/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/requirements_dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:35:35.796145 seamm_dashboard_client-2023.6.28/seamm_dashboard_client/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/seamm_dashboard_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-28 12:35:35.796145 seamm_dashboard_client-2023.6.28/seamm_dashboard_client/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/seamm_dashboard_client/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:35:35.796145 seamm_dashboard_client-2023.6.28/seamm_dashboard_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-28 12:35:35.000000 seamm_dashboard_client-2023.6.28/seamm_dashboard_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-28 12:35:35.000000 seamm_dashboard_client-2023.6.28/seamm_dashboard_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 12:35:35.000000 seamm_dashboard_client-2023.6.28/seamm_dashboard_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-28 12:35:35.000000 seamm_dashboard_client-2023.6.28/seamm_dashboard_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-28 12:35:35.000000 seamm_dashboard_client-2023.6.28/seamm_dashboard_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 12:35:18.000000 seamm_dashboard_client-2023.6.28/seamm_dashboard_client.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-28 12:35:35.796145 seamm_dashboard_client-2023.6.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:35:35.796145 seamm_dashboard_client-2023.6.28/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31497 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-28 12:35:11.000000 seamm_dashboard_client-2023.6.28/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:44:56.574455 seamm_dashboard_client-2023.7.10/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-10 20:44:56.574455 seamm_dashboard_client-2023.7.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:44:56.574455 seamm_dashboard_client-2023.7.10/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8842 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:44:56.574455 seamm_dashboard_client-2023.7.10/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/developer/cms_plots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/developer/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/developer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/developer/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/developer/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/developer/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:44:56.574455 seamm_dashboard_client-2023.7.10/docs/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/docs/user/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:44:56.578455 seamm_dashboard_client-2023.7.10/seamm_dashboard_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/seamm_dashboard_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-10 20:44:56.578455 seamm_dashboard_client-2023.7.10/seamm_dashboard_client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28115 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/seamm_dashboard_client/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:44:56.574455 seamm_dashboard_client-2023.7.10/seamm_dashboard_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-10 20:44:56.000000 seamm_dashboard_client-2023.7.10/seamm_dashboard_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-10 20:44:56.000000 seamm_dashboard_client-2023.7.10/seamm_dashboard_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:44:56.000000 seamm_dashboard_client-2023.7.10/seamm_dashboard_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-10 20:44:56.000000 seamm_dashboard_client-2023.7.10/seamm_dashboard_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 20:44:56.000000 seamm_dashboard_client-2023.7.10/seamm_dashboard_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:44:47.000000 seamm_dashboard_client-2023.7.10/seamm_dashboard_client.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-10 20:44:56.578455 seamm_dashboard_client-2023.7.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:44:56.574455 seamm_dashboard_client-2023.7.10/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31497 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-10 20:44:43.000000 seamm_dashboard_client-2023.7.10/versioneer.py
```

### Comparing `seamm_dashboard_client-2023.6.28/CONTRIBUTING.rst` & `seamm_dashboard_client-2023.7.10/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2023.6.28/LICENSE` & `seamm_dashboard_client-2023.7.10/LICENSE`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2023.6.28/PKG-INFO` & `seamm_dashboard_client-2023.7.10/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_dashboard_client
-Version: 2023.6.28
+Version: 2023.7.10
 Summary: A Python client for the SEAMM Dashboard RESTful API.
 Home-page: https://github.com/molssi-seamm/seamm_dashboard_client
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMDashboard,RESTful,client
 Platform: Linux
@@ -86,13 +86,17 @@
 .. _MolSSI: https://molssi.org
 
 
 =======
 History
 =======
 
+2023.7.10 -- Corrected handling of control parameters
+   * Now handle control parameters with multiple values.
+   * Separate the options from required parameters with '--' as required.
+     
 2023.6.28 -- Improved error messages for login failures.
 
 2022.8.13 (13 August 2022)
 --------------------------
 
 * First release of a working version on PyPI.
```

### Comparing `seamm_dashboard_client-2023.6.28/README.rst` & `seamm_dashboard_client-2023.7.10/README.rst`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2023.6.28/docs/Makefile` & `seamm_dashboard_client-2023.7.10/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2023.6.28/docs/conf.py` & `seamm_dashboard_client-2023.7.10/docs/conf.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2023.6.28/docs/developer/cms_plots.rst` & `seamm_dashboard_client-2023.7.10/docs/developer/cms_plots.rst`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2023.6.28/docs/developer/installation.rst` & `seamm_dashboard_client-2023.7.10/docs/developer/installation.rst`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2023.6.28/docs/index.rst` & `seamm_dashboard_client-2023.7.10/docs/index.rst`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2023.6.28/docs/make.bat` & `seamm_dashboard_client-2023.7.10/docs/make.bat`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2023.6.28/seamm_dashboard_client/__init__.py` & `seamm_dashboard_client-2023.7.10/seamm_dashboard_client/__init__.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2023.6.28/seamm_dashboard_client/dashboard.py` & `seamm_dashboard_client-2023.7.10/seamm_dashboard_client/dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,15 +468,18 @@
                                 optional.append(f"--{name}")
                                 for filename in shlex.split(values[name]):
                                     if filename not in files:
                                         files[filename] = safe_filename(filename)
                                     optional.append(files[filename])
                         else:
                             optional.append(f"--{name}")
-                            optional.append(values[name])
+                            if data["nargs"] == "a single value":
+                                optional.append(values[name])
+                            else:
+                                optional.extend(shlex.split(values[name]))
                     else:
                         if data["type"] == "file":
                             if data["nargs"] == "a single value":
                                 filename = values[name]
                                 if filename not in files:
                                     files[filename] = safe_filename(filename)
                                 required.append(files[filename])
@@ -485,15 +488,16 @@
                                     if filename not in files:
                                         files[filename] = safe_filename(filename)
                                     required.append(files[filename])
                         else:
                             if data["nargs"] == "a single value":
                                 required.append(values[name])
                             else:
-                                required = shlex.split(values[name])
+                                required.extend(shlex.split(values[name]))
+            optional.append("--")
             cmdline = optional + required
 
         # Prepare the data
         data = {
             "flowchart": flowchart.to_text(),
             "project": project,
             "title": title,
```

### Comparing `seamm_dashboard_client-2023.6.28/seamm_dashboard_client.egg-info/PKG-INFO` & `seamm_dashboard_client-2023.7.10/seamm_dashboard_client.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm-dashboard-client
-Version: 2023.6.28
+Version: 2023.7.10
 Summary: A Python client for the SEAMM Dashboard RESTful API.
 Home-page: https://github.com/molssi-seamm/seamm_dashboard_client
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMDashboard,RESTful,client
 Platform: Linux
@@ -86,13 +86,17 @@
 .. _MolSSI: https://molssi.org
 
 
 =======
 History
 =======
 
+2023.7.10 -- Corrected handling of control parameters
+   * Now handle control parameters with multiple values.
+   * Separate the options from required parameters with '--' as required.
+     
 2023.6.28 -- Improved error messages for login failures.
 
 2022.8.13 (13 August 2022)
 --------------------------
 
 * First release of a working version on PyPI.
```

### Comparing `seamm_dashboard_client-2023.6.28/seamm_dashboard_client.egg-info/SOURCES.txt` & `seamm_dashboard_client-2023.7.10/seamm_dashboard_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2023.6.28/setup.py` & `seamm_dashboard_client-2023.7.10/setup.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2023.6.28/tests/test_dashboard.py` & `seamm_dashboard_client-2023.7.10/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2023.6.28/versioneer.py` & `seamm_dashboard_client-2023.7.10/versioneer.py`

 * *Files identical despite different names*

