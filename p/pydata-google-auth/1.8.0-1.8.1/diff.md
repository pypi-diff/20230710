# Comparing `tmp/pydata-google-auth-1.8.0.tar.gz` & `tmp/pydata-google-auth-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydata-google-auth-1.8.0.tar", last modified: Tue May  9 16:30:24 2023, max compression
+gzip compressed data, was "pydata-google-auth-1.8.1.tar", last modified: Mon Jul 10 15:11:24 2023, max compression
```

## Comparing `pydata-google-auth-1.8.0.tar` & `pydata-google-auth-1.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 swast    (212416) primarygroup (89939)        0 2023-05-09 16:30:24.769804 pydata-google-auth-1.8.0/
--rw-r--r--   0 swast    (212416) primarygroup (89939)     2283 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.0/AUTHORS.md
--rw-r--r--   0 swast    (212416) primarygroup (89939)     1582 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.0/LICENSE.txt
--rw-r--r--   0 swast    (212416) primarygroup (89939)      331 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.0/MANIFEST.in
--rw-r--r--   0 swast    (212416) primarygroup (89939)     2906 2023-05-09 16:30:24.769988 pydata-google-auth-1.8.0/PKG-INFO
--rw-r--r--   0 swast    (212416) primarygroup (89939)     1795 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.0/README.rst
-drwxr-xr-x   0 swast    (212416) primarygroup (89939)        0 2023-05-09 16:30:24.771634 pydata-google-auth-1.8.0/pydata_google_auth/
--rw-r--r--   0 swast    (212416) primarygroup (89939)      662 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.0/pydata_google_auth/__init__.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)     3706 2022-03-10 20:53:17.000000 pydata-google-auth-1.8.0/pydata_google_auth/__main__.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)      497 2023-05-09 16:30:24.771815 pydata-google-auth-1.8.0/pydata_google_auth/_version.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)     2319 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.0/pydata_google_auth/_webserver.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)    19443 2023-05-09 16:29:08.000000 pydata-google-auth-1.8.0/pydata_google_auth/auth.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)     8789 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.0/pydata_google_auth/cache.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)      262 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.0/pydata_google_auth/exceptions.py
-drwxr-xr-x   0 swast    (212416) primarygroup (89939)        0 2023-05-09 16:30:24.769132 pydata-google-auth-1.8.0/pydata_google_auth.egg-info/
--rw-r--r--   0 swast    (212416) primarygroup (89939)     2906 2023-05-09 16:30:24.000000 pydata-google-auth-1.8.0/pydata_google_auth.egg-info/PKG-INFO
--rw-r--r--   0 swast    (212416) primarygroup (89939)      501 2023-05-09 16:30:24.000000 pydata-google-auth-1.8.0/pydata_google_auth.egg-info/SOURCES.txt
--rw-r--r--   0 swast    (212416) primarygroup (89939)        1 2023-05-09 16:30:24.000000 pydata-google-auth-1.8.0/pydata_google_auth.egg-info/dependency_links.txt
--rw-r--r--   0 swast    (212416) primarygroup (89939)      188 2023-05-09 16:30:24.000000 pydata-google-auth-1.8.0/pydata_google_auth.egg-info/requires.txt
--rw-r--r--   0 swast    (212416) primarygroup (89939)       19 2023-05-09 16:30:24.000000 pydata-google-auth-1.8.0/pydata_google_auth.egg-info/top_level.txt
--rw-r--r--   0 swast    (212416) primarygroup (89939)      356 2023-05-09 16:30:24.770634 pydata-google-auth-1.8.0/setup.cfg
--rw-r--r--   0 swast    (212416) primarygroup (89939)     1859 2021-12-03 19:00:07.000000 pydata-google-auth-1.8.0/setup.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)    68752 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.0/versioneer.py
+drwxr-xr-x   0 swast    (212416) primarygroup (89939)        0 2023-07-10 15:11:24.264217 pydata-google-auth-1.8.1/
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     2283 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/AUTHORS.md
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     1582 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/LICENSE.txt
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      331 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/MANIFEST.in
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     2906 2023-07-10 15:11:24.264391 pydata-google-auth-1.8.1/PKG-INFO
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     1795 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/README.rst
+drwxr-xr-x   0 swast    (212416) primarygroup (89939)        0 2023-07-10 15:11:24.265661 pydata-google-auth-1.8.1/pydata_google_auth/
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      662 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/pydata_google_auth/__init__.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     3706 2022-03-10 20:53:17.000000 pydata-google-auth-1.8.1/pydata_google_auth/__main__.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      497 2023-07-10 15:11:24.265795 pydata-google-auth-1.8.1/pydata_google_auth/_version.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     2319 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/pydata_google_auth/_webserver.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)    20022 2023-07-10 15:01:28.000000 pydata-google-auth-1.8.1/pydata_google_auth/auth.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     8789 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/pydata_google_auth/cache.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      262 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/pydata_google_auth/exceptions.py
+drwxr-xr-x   0 swast    (212416) primarygroup (89939)        0 2023-07-10 15:11:24.263839 pydata-google-auth-1.8.1/pydata_google_auth.egg-info/
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     2906 2023-07-10 15:11:24.000000 pydata-google-auth-1.8.1/pydata_google_auth.egg-info/PKG-INFO
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      501 2023-07-10 15:11:24.000000 pydata-google-auth-1.8.1/pydata_google_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 swast    (212416) primarygroup (89939)        1 2023-07-10 15:11:24.000000 pydata-google-auth-1.8.1/pydata_google_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      188 2023-07-10 15:11:24.000000 pydata-google-auth-1.8.1/pydata_google_auth.egg-info/requires.txt
+-rw-r--r--   0 swast    (212416) primarygroup (89939)       19 2023-07-10 15:11:24.000000 pydata-google-auth-1.8.1/pydata_google_auth.egg-info/top_level.txt
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      356 2023-07-10 15:11:24.265066 pydata-google-auth-1.8.1/setup.cfg
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     1859 2021-12-03 19:00:07.000000 pydata-google-auth-1.8.1/setup.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)    68752 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/versioneer.py
```

### Comparing `pydata-google-auth-1.8.0/AUTHORS.md` & `pydata-google-auth-1.8.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.0/LICENSE.txt` & `pydata-google-auth-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.0/PKG-INFO` & `pydata-google-auth-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydata-google-auth
-Version: 1.8.0
+Version: 1.8.1
 Summary: PyData helpers for authenticating to Google APIs
 Home-page: https://github.com/pydata/pydata-google-auth
 Author: The PyData Development Team
 Author-email: pydata@googlegroups.com
 License: BSD License
 Keywords: data
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pydata-google-auth-1.8.0/README.rst` & `pydata-google-auth-1.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.0/pydata_google_auth/__init__.py` & `pydata-google-auth-1.8.1/pydata_google_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.0/pydata_google_auth/__main__.py` & `pydata-google-auth-1.8.1/pydata_google_auth/__main__.py`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.0/pydata_google_auth/_webserver.py` & `pydata-google-auth-1.8.1/pydata_google_auth/_webserver.py`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.0/pydata_google_auth/auth.py` & `pydata-google-auth-1.8.1/pydata_google_auth/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,15 +161,25 @@
     # This is a special handling for google colab environment where we want to
     # use the colab specific authentication flow
     # https://github.com/googlecolab/colabtools/blob/3c8772efd332289e1c6d1204826b0915d22b5b95/google/colab/auth.py#L209
     try:
         from google.colab import auth
 
         auth.authenticate_user()
-    except ImportError:
+    except Exception:
+        # We are catching a broad exception class here because we want to be
+        # agnostic to anything that could internally go wrong in the google
+        # colab auth. Some of the known exception we want to pass on are:
+        #
+        # ModuleNotFoundError: No module named 'google.colab'
+        # ImportError: cannot import name 'auth' from 'google.cloud'
+        # MessageError: Error: credential propagation was unsuccessful
+        #
+        # The MessageError happens on Vertex Colab when it fails to resolve auth
+        # from the Compute Engine Metadata server.
         pass
 
 
 def get_application_default_credentials(scopes):
     """
     This method tries to retrieve the "default application credentials".
     This could be useful for running code on Google Cloud Platform.
```

### Comparing `pydata-google-auth-1.8.0/pydata_google_auth/cache.py` & `pydata-google-auth-1.8.1/pydata_google_auth/cache.py`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.0/pydata_google_auth.egg-info/PKG-INFO` & `pydata-google-auth-1.8.1/pydata_google_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydata-google-auth
-Version: 1.8.0
+Version: 1.8.1
 Summary: PyData helpers for authenticating to Google APIs
 Home-page: https://github.com/pydata/pydata-google-auth
 Author: The PyData Development Team
 Author-email: pydata@googlegroups.com
 License: BSD License
 Keywords: data
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pydata-google-auth-1.8.0/setup.py` & `pydata-google-auth-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.0/versioneer.py` & `pydata-google-auth-1.8.1/versioneer.py`

 * *Files identical despite different names*

