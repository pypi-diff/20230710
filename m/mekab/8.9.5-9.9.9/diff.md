# Comparing `tmp/mekab-8.9.5.tar.gz` & `tmp/mekab-9.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mekab-8.9.5.tar", last modified: Mon Jul 10 12:04:26 2023, max compression
+gzip compressed data, was "mekab-9.9.9.tar", last modified: Mon Jul 10 12:26:55 2023, max compression
```

## Comparing `mekab-8.9.5.tar` & `mekab-9.9.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 12:04:26.402769 mekab-8.9.5/
--rw-r--r--   0 root         (0) root         (0)     2511 2023-07-10 12:04:26.402769 mekab-8.9.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1584 2023-07-09 09:20:41.000000 mekab-8.9.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 12:04:26.402769 mekab-8.9.5/mekab.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2511 2023-07-10 12:04:26.000000 mekab-8.9.5/mekab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      162 2023-07-10 12:04:26.000000 mekab-8.9.5/mekab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 12:04:26.000000 mekab-8.9.5/mekab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-10 12:04:26.000000 mekab-8.9.5/mekab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 12:04:26.000000 mekab-8.9.5/mekab.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 12:04:26.402769 mekab-8.9.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 12:03:58.000000 mekab-8.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 12:26:55.374895 mekab-9.9.9/
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-07-10 12:26:55.374895 mekab-9.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-07-09 09:20:41.000000 mekab-9.9.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 12:26:55.374895 mekab-9.9.9/mekab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-07-10 12:26:55.000000 mekab-9.9.9/mekab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-10 12:26:55.000000 mekab-9.9.9/mekab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 12:26:55.000000 mekab-9.9.9/mekab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-10 12:26:55.000000 mekab-9.9.9/mekab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 12:26:55.000000 mekab-9.9.9/mekab.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 12:26:55.374895 mekab-9.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 12:03:58.000000 mekab-9.9.9/setup.py
```

### Comparing `mekab-8.9.5/PKG-INFO` & `mekab-9.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mekab
-Version: 8.9.5
+Version: 9.9.9
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: cariin
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `mekab-8.9.5/README.md` & `mekab-9.9.9/README.md`

 * *Files identical despite different names*

### Comparing `mekab-8.9.5/mekab.egg-info/PKG-INFO` & `mekab-9.9.9/mekab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mekab
-Version: 8.9.5
+Version: 9.9.9
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: cariin
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `mekab-8.9.5/setup.py` & `mekab-9.9.9/setup.py`

 * *Files identical despite different names*

