# Comparing `tmp/disk_treemap-1.0.8.tar.gz` & `tmp/disk_treemap-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disk_treemap-1.0.8.tar", last modified: Sun Dec  5 18:59:16 2021, max compression
+gzip compressed data, was "disk_treemap-1.0.9.tar", last modified: Sun Dec  5 19:22:22 2021, max compression
```

## Comparing `disk_treemap-1.0.8.tar` & `disk_treemap-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 18:59:16.821935 disk_treemap-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-12-05 18:57:37.000000 disk_treemap-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-12-05 18:57:37.000000 disk_treemap-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5777 2021-12-05 18:59:16.821935 disk_treemap-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4815 2021-12-05 18:57:37.000000 disk_treemap-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 18:59:16.817935 disk_treemap-1.0.8/disk_treemap/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-12-05 18:57:37.000000 disk_treemap-1.0.8/disk_treemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4943 2021-12-05 18:57:37.000000 disk_treemap-1.0.8/disk_treemap/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     2510 2021-12-05 18:57:37.000000 disk_treemap-1.0.8/disk_treemap/scan_everything.py
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-12-05 18:57:37.000000 disk_treemap-1.0.8/disk_treemap/scan_fs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-12-05 18:57:37.000000 disk_treemap-1.0.8/disk_treemap/scan_s3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 18:59:16.817935 disk_treemap-1.0.8/disk_treemap/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 18:59:16.817935 disk_treemap-1.0.8/disk_treemap/static/dist/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 18:59:16.821935 disk_treemap-1.0.8/disk_treemap/static/dist/webapp/
--rw-r--r--   0 runner    (1001) docker     (121)    24667 2021-12-05 18:59:15.000000 disk_treemap-1.0.8/disk_treemap/static/dist/webapp/3rdpartylicenses.txt
--rw-r--r--   0 runner    (1001) docker     (121)      948 2021-12-05 18:59:16.000000 disk_treemap-1.0.8/disk_treemap/static/dist/webapp/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      700 2021-12-05 18:59:16.000000 disk_treemap-1.0.8/disk_treemap/static/dist/webapp/index.html
--rw-r--r--   0 runner    (1001) docker     (121)   262874 2021-12-05 18:59:15.000000 disk_treemap-1.0.8/disk_treemap/static/dist/webapp/main.5cc76c324311214514de.js
--rw-r--r--   0 runner    (1001) docker     (121)    45513 2021-12-05 18:59:15.000000 disk_treemap-1.0.8/disk_treemap/static/dist/webapp/polyfills.aff2eefe283ca9600825.js
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-12-05 18:59:15.000000 disk_treemap-1.0.8/disk_treemap/static/dist/webapp/runtime.ae823e292a77cd950d0a.js
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-12-05 18:59:15.000000 disk_treemap-1.0.8/disk_treemap/static/dist/webapp/styles.fd7e0e557b99d505e7ac.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 18:59:16.821935 disk_treemap-1.0.8/disk_treemap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5777 2021-12-05 18:59:16.000000 disk_treemap-1.0.8/disk_treemap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      808 2021-12-05 18:59:16.000000 disk_treemap-1.0.8/disk_treemap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-05 18:59:16.000000 disk_treemap-1.0.8/disk_treemap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-05 18:59:16.000000 disk_treemap-1.0.8/disk_treemap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-12-05 18:59:16.000000 disk_treemap-1.0.8/disk_treemap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-05 18:59:16.000000 disk_treemap-1.0.8/disk_treemap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-05 18:59:16.000000 disk_treemap-1.0.8/disk_treemap.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-05 18:59:16.821935 disk_treemap-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2021-12-05 18:57:37.000000 disk_treemap-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 19:22:22.292967 disk_treemap-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-12-05 19:21:05.000000 disk_treemap-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2021-12-05 19:21:05.000000 disk_treemap-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5777 2021-12-05 19:22:22.292967 disk_treemap-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4815 2021-12-05 19:21:05.000000 disk_treemap-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 19:22:22.288967 disk_treemap-1.0.9/disk_treemap/
+-rw-r--r--   0 runner    (1001) docker     (121)    93000 2021-12-05 19:21:05.000000 disk_treemap-1.0.9/disk_treemap/Everything64.dll
+-rw-r--r--   0 runner    (1001) docker     (121)     2636 2021-12-05 19:21:05.000000 disk_treemap-1.0.9/disk_treemap/Everything_license.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2021-12-05 19:21:05.000000 disk_treemap-1.0.9/disk_treemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4943 2021-12-05 19:21:05.000000 disk_treemap-1.0.9/disk_treemap/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2510 2021-12-05 19:21:05.000000 disk_treemap-1.0.9/disk_treemap/scan_everything.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-12-05 19:21:05.000000 disk_treemap-1.0.9/disk_treemap/scan_fs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-12-05 19:21:05.000000 disk_treemap-1.0.9/disk_treemap/scan_s3.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 19:22:22.288967 disk_treemap-1.0.9/disk_treemap/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 19:22:22.288967 disk_treemap-1.0.9/disk_treemap/static/dist/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 19:22:22.292967 disk_treemap-1.0.9/disk_treemap/static/dist/webapp/
+-rw-r--r--   0 runner    (1001) docker     (121)    24667 2021-12-05 19:22:21.000000 disk_treemap-1.0.9/disk_treemap/static/dist/webapp/3rdpartylicenses.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      948 2021-12-05 19:22:21.000000 disk_treemap-1.0.9/disk_treemap/static/dist/webapp/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2021-12-05 19:22:21.000000 disk_treemap-1.0.9/disk_treemap/static/dist/webapp/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)   262874 2021-12-05 19:22:21.000000 disk_treemap-1.0.9/disk_treemap/static/dist/webapp/main.5cc76c324311214514de.js
+-rw-r--r--   0 runner    (1001) docker     (121)    45513 2021-12-05 19:22:21.000000 disk_treemap-1.0.9/disk_treemap/static/dist/webapp/polyfills.aff2eefe283ca9600825.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-12-05 19:22:21.000000 disk_treemap-1.0.9/disk_treemap/static/dist/webapp/runtime.ae823e292a77cd950d0a.js
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-12-05 19:22:21.000000 disk_treemap-1.0.9/disk_treemap/static/dist/webapp/styles.fd7e0e557b99d505e7ac.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 19:22:22.288967 disk_treemap-1.0.9/disk_treemap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5777 2021-12-05 19:22:22.000000 disk_treemap-1.0.9/disk_treemap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2021-12-05 19:22:22.000000 disk_treemap-1.0.9/disk_treemap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-05 19:22:22.000000 disk_treemap-1.0.9/disk_treemap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-05 19:22:22.000000 disk_treemap-1.0.9/disk_treemap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-12-05 19:22:22.000000 disk_treemap-1.0.9/disk_treemap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-05 19:22:22.000000 disk_treemap-1.0.9/disk_treemap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-05 19:22:22.000000 disk_treemap-1.0.9/disk_treemap.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-05 19:22:22.292967 disk_treemap-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1951 2021-12-05 19:21:05.000000 disk_treemap-1.0.9/setup.py
```

### Comparing `disk_treemap-1.0.8/LICENSE` & `disk_treemap-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `disk_treemap-1.0.8/PKG-INFO` & `disk_treemap-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disk_treemap
-Version: 1.0.8
+Version: 1.0.9
 Summary: Just another disk usage analyzer with treemap GUI.
 Home-page: https://github.com/exzhawk/disk_treemap
 Author: Epix Zhang
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `disk_treemap-1.0.8/README.md` & `disk_treemap-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `disk_treemap-1.0.8/disk_treemap/main.py` & `disk_treemap-1.0.9/disk_treemap/main.py`

 * *Files identical despite different names*

### Comparing `disk_treemap-1.0.8/disk_treemap/scan_everything.py` & `disk_treemap-1.0.9/disk_treemap/scan_everything.py`

 * *Files identical despite different names*

### Comparing `disk_treemap-1.0.8/disk_treemap/scan_fs.py` & `disk_treemap-1.0.9/disk_treemap/scan_fs.py`

 * *Files identical despite different names*

### Comparing `disk_treemap-1.0.8/disk_treemap/scan_s3.py` & `disk_treemap-1.0.9/disk_treemap/scan_s3.py`

 * *Files identical despite different names*

### Comparing `disk_treemap-1.0.8/disk_treemap/static/dist/webapp/3rdpartylicenses.txt` & `disk_treemap-1.0.9/disk_treemap/static/dist/webapp/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `disk_treemap-1.0.8/disk_treemap/static/dist/webapp/favicon.ico` & `disk_treemap-1.0.9/disk_treemap/static/dist/webapp/favicon.ico`

 * *Files identical despite different names*

### Comparing `disk_treemap-1.0.8/disk_treemap/static/dist/webapp/index.html` & `disk_treemap-1.0.9/disk_treemap/static/dist/webapp/index.html`

 * *Files identical despite different names*

### Comparing `disk_treemap-1.0.8/disk_treemap/static/dist/webapp/main.5cc76c324311214514de.js` & `disk_treemap-1.0.9/disk_treemap/static/dist/webapp/main.5cc76c324311214514de.js`

 * *Files identical despite different names*

### Comparing `disk_treemap-1.0.8/disk_treemap/static/dist/webapp/polyfills.aff2eefe283ca9600825.js` & `disk_treemap-1.0.9/disk_treemap/static/dist/webapp/polyfills.aff2eefe283ca9600825.js`

 * *Files identical despite different names*

### Comparing `disk_treemap-1.0.8/disk_treemap/static/dist/webapp/runtime.ae823e292a77cd950d0a.js` & `disk_treemap-1.0.9/disk_treemap/static/dist/webapp/runtime.ae823e292a77cd950d0a.js`

 * *Files identical despite different names*

### Comparing `disk_treemap-1.0.8/disk_treemap.egg-info/PKG-INFO` & `disk_treemap-1.0.9/disk_treemap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disk-treemap
-Version: 1.0.8
+Version: 1.0.9
 Summary: Just another disk usage analyzer with treemap GUI.
 Home-page: https://github.com/exzhawk/disk_treemap
 Author: Epix Zhang
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `disk_treemap-1.0.8/disk_treemap.egg-info/SOURCES.txt` & `disk_treemap-1.0.9/disk_treemap.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+disk_treemap/Everything64.dll
+disk_treemap/Everything_license.txt
 disk_treemap/__init__.py
 disk_treemap/main.py
 disk_treemap/scan_everything.py
 disk_treemap/scan_fs.py
 disk_treemap/scan_s3.py
 disk_treemap.egg-info/PKG-INFO
 disk_treemap.egg-info/SOURCES.txt
```

### Comparing `disk_treemap-1.0.8/setup.py` & `disk_treemap-1.0.9/setup.py`

 * *Files identical despite different names*

