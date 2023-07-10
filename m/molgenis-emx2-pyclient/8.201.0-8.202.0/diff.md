# Comparing `tmp/molgenis_emx2_pyclient-8.201.0.tar.gz` & `tmp/molgenis_emx2_pyclient-8.202.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgenis_emx2_pyclient-8.201.0.tar", last modified: Thu Jul  6 18:00:29 2023, max compression
+gzip compressed data, was "molgenis_emx2_pyclient-8.202.0.tar", last modified: Mon Jul 10 11:26:23 2023, max compression
```

## Comparing `molgenis_emx2_pyclient-8.201.0.tar` & `molgenis_emx2_pyclient-8.202.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:00:29.304258 molgenis_emx2_pyclient-8.201.0/
--rw-r--r--   0 root         (0) root         (0)     7631 2023-07-06 17:52:32.000000 molgenis_emx2_pyclient-8.201.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1342 2023-07-06 18:00:29.304258 molgenis_emx2_pyclient-8.201.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-07-06 17:52:33.000000 molgenis_emx2_pyclient-8.201.0/README.md
--rw-r--r--   0 root         (0) root         (0)      634 2023-07-06 17:52:33.000000 molgenis_emx2_pyclient-8.201.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-06 17:52:33.000000 molgenis_emx2_pyclient-8.201.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 18:00:29.304258 molgenis_emx2_pyclient-8.201.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:00:29.300258 molgenis_emx2_pyclient-8.201.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:00:29.304258 molgenis_emx2_pyclient-8.201.0/src/molgenis_emx2_pyclient/
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-06 17:52:33.000000 molgenis_emx2_pyclient-8.201.0/src/molgenis_emx2_pyclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2781 2023-07-06 17:52:33.000000 molgenis_emx2_pyclient-8.201.0/src/molgenis_emx2_pyclient/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:00:29.304258 molgenis_emx2_pyclient-8.201.0/src/molgenis_emx2_pyclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1342 2023-07-06 18:00:29.000000 molgenis_emx2_pyclient-8.201.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      386 2023-07-06 18:00:29.000000 molgenis_emx2_pyclient-8.201.0/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 18:00:29.000000 molgenis_emx2_pyclient-8.201.0/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-06 18:00:29.000000 molgenis_emx2_pyclient-8.201.0/src/molgenis_emx2_pyclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-06 18:00:29.000000 molgenis_emx2_pyclient-8.201.0/src/molgenis_emx2_pyclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 17:54:03.000000 molgenis_emx2_pyclient-8.201.0/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:26:23.516791 molgenis_emx2_pyclient-8.202.0/
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-07-10 11:18:45.000000 molgenis_emx2_pyclient-8.202.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-10 11:26:23.516791 molgenis_emx2_pyclient-8.202.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-07-10 11:18:45.000000 molgenis_emx2_pyclient-8.202.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-10 11:18:45.000000 molgenis_emx2_pyclient-8.202.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-10 11:18:45.000000 molgenis_emx2_pyclient-8.202.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 11:26:23.516791 molgenis_emx2_pyclient-8.202.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:26:23.516791 molgenis_emx2_pyclient-8.202.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:26:23.516791 molgenis_emx2_pyclient-8.202.0/src/molgenis_emx2_pyclient/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-10 11:18:45.000000 molgenis_emx2_pyclient-8.202.0/src/molgenis_emx2_pyclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-07-10 11:18:45.000000 molgenis_emx2_pyclient-8.202.0/src/molgenis_emx2_pyclient/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:26:23.516791 molgenis_emx2_pyclient-8.202.0/src/molgenis_emx2_pyclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-10 11:26:23.000000 molgenis_emx2_pyclient-8.202.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      386 2023-07-10 11:26:23.000000 molgenis_emx2_pyclient-8.202.0/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 11:26:23.000000 molgenis_emx2_pyclient-8.202.0/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-10 11:26:23.000000 molgenis_emx2_pyclient-8.202.0/src/molgenis_emx2_pyclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-10 11:26:23.000000 molgenis_emx2_pyclient-8.202.0/src/molgenis_emx2_pyclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 11:20:11.000000 molgenis_emx2_pyclient-8.202.0/version.txt
```

### Comparing `molgenis_emx2_pyclient-8.201.0/LICENSE` & `molgenis_emx2_pyclient-8.202.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.201.0/PKG-INFO` & `molgenis_emx2_pyclient-8.202.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis_emx2_pyclient
-Version: 8.201.0
+Version: 8.202.0
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molgenis_emx2_pyclient-8.201.0/README.md` & `molgenis_emx2_pyclient-8.202.0/README.md`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.201.0/pyproject.toml` & `molgenis_emx2_pyclient-8.202.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.201.0/src/molgenis_emx2_pyclient/client.py` & `molgenis_emx2_pyclient-8.202.0/src/molgenis_emx2_pyclient/client.py`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.201.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO` & `molgenis_emx2_pyclient-8.202.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-pyclient
-Version: 8.201.0
+Version: 8.202.0
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

