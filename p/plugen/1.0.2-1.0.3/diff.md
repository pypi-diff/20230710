# Comparing `tmp/plugen-1.0.2.tar.gz` & `tmp/plugen-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugen-1.0.2.tar", last modified: Mon Jul 10 05:14:05 2023, max compression
+gzip compressed data, was "plugen-1.0.3.tar", last modified: Mon Jul 10 05:15:31 2023, max compression
```

## Comparing `plugen-1.0.2.tar` & `plugen-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:14:05.698514 plugen-1.0.2/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      215 2023-07-10 05:14:05.694514 plugen-1.0.2/PKG-INFO
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     3774 2023-07-09 18:55:27.000000 plugen-1.0.2/README.md
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:14:05.694514 plugen-1.0.2/plugen/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.2/plugen/__init__.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:14:05.694514 plugen-1.0.2/plugen/lib/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       41 2023-07-09 05:59:38.000000 plugen-1.0.2/plugen/lib/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      942 2023-07-09 18:33:02.000000 plugen-1.0.2/plugen/lib/build.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1968 2023-07-09 18:38:01.000000 plugen-1.0.2/plugen/lib/plugin.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2526 2023-07-09 18:33:02.000000 plugen-1.0.2/plugen/lib/serve.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      522 2023-07-09 09:14:03.000000 plugen-1.0.2/plugen/lib/utils.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1742 2023-07-09 18:34:51.000000 plugen-1.0.2/plugen/main.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:14:05.694514 plugen-1.0.2/plugen/plugins/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.2/plugen/plugins/__init__.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:14:05.694514 plugen-1.0.2/plugen/plugins/copydest/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.2/plugen/plugins/copydest/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      362 2023-07-09 09:15:39.000000 plugen-1.0.2/plugen/plugins/copydest/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:14:05.694514 plugen-1.0.2/plugen/plugins/hotreload/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.2/plugen/plugins/hotreload/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1820 2023-07-09 09:36:13.000000 plugen-1.0.2/plugen/plugins/hotreload/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:14:05.694514 plugen-1.0.2/plugen/plugins/imagecompressor/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.2/plugen/plugins/imagecompressor/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:18.000000 plugen-1.0.2/plugen/plugins/imagecompressor/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:14:05.694514 plugen-1.0.2/plugen/plugins/sass/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.2/plugen/plugins/sass/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      534 2023-07-09 10:19:25.000000 plugen-1.0.2/plugen/plugins/sass/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:14:05.694514 plugen-1.0.2/plugen/plugins/tailwind/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.2/plugen/plugins/tailwind/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:22.000000 plugen-1.0.2/plugen/plugins/tailwind/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:14:05.694514 plugen-1.0.2/plugen.egg-info/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      215 2023-07-10 05:14:05.000000 plugen-1.0.2/plugen.egg-info/PKG-INFO
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      771 2023-07-10 05:14:05.000000 plugen-1.0.2/plugen.egg-info/SOURCES.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        1 2023-07-10 05:14:05.000000 plugen-1.0.2/plugen.egg-info/dependency_links.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       39 2023-07-10 05:14:05.000000 plugen-1.0.2/plugen.egg-info/entry_points.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        7 2023-07-10 05:14:05.000000 plugen-1.0.2/plugen.egg-info/requires.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        7 2023-07-10 05:14:05.000000 plugen-1.0.2/plugen.egg-info/top_level.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       38 2023-07-10 05:14:05.698514 plugen-1.0.2/setup.cfg
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      481 2023-07-10 05:14:03.000000 plugen-1.0.2/setup.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:15:31.577340 plugen-1.0.3/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      215 2023-07-10 05:15:31.577340 plugen-1.0.3/PKG-INFO
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     3774 2023-07-09 18:55:27.000000 plugen-1.0.3/README.md
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:15:31.577340 plugen-1.0.3/plugen/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       19 2023-07-10 05:15:24.000000 plugen-1.0.3/plugen/__init__.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:15:31.577340 plugen-1.0.3/plugen/lib/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       41 2023-07-09 05:59:38.000000 plugen-1.0.3/plugen/lib/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      942 2023-07-09 18:33:02.000000 plugen-1.0.3/plugen/lib/build.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1968 2023-07-09 18:38:01.000000 plugen-1.0.3/plugen/lib/plugin.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2526 2023-07-09 18:33:02.000000 plugen-1.0.3/plugen/lib/serve.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      522 2023-07-09 09:14:03.000000 plugen-1.0.3/plugen/lib/utils.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1742 2023-07-10 05:14:56.000000 plugen-1.0.3/plugen/main.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:15:31.577340 plugen-1.0.3/plugen/plugins/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.3/plugen/plugins/__init__.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:15:31.577340 plugen-1.0.3/plugen/plugins/copydest/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.3/plugen/plugins/copydest/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      362 2023-07-09 09:15:39.000000 plugen-1.0.3/plugen/plugins/copydest/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:15:31.577340 plugen-1.0.3/plugen/plugins/hotreload/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.3/plugen/plugins/hotreload/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1820 2023-07-09 09:36:13.000000 plugen-1.0.3/plugen/plugins/hotreload/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:15:31.577340 plugen-1.0.3/plugen/plugins/imagecompressor/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.3/plugen/plugins/imagecompressor/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:18.000000 plugen-1.0.3/plugen/plugins/imagecompressor/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:15:31.577340 plugen-1.0.3/plugen/plugins/sass/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.3/plugen/plugins/sass/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      534 2023-07-09 10:19:25.000000 plugen-1.0.3/plugen/plugins/sass/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:15:31.577340 plugen-1.0.3/plugen/plugins/tailwind/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.3/plugen/plugins/tailwind/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:22.000000 plugen-1.0.3/plugen/plugins/tailwind/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:15:31.577340 plugen-1.0.3/plugen.egg-info/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      215 2023-07-10 05:15:31.000000 plugen-1.0.3/plugen.egg-info/PKG-INFO
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      771 2023-07-10 05:15:31.000000 plugen-1.0.3/plugen.egg-info/SOURCES.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        1 2023-07-10 05:15:31.000000 plugen-1.0.3/plugen.egg-info/dependency_links.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       39 2023-07-10 05:15:31.000000 plugen-1.0.3/plugen.egg-info/entry_points.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        7 2023-07-10 05:15:31.000000 plugen-1.0.3/plugen.egg-info/requires.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        7 2023-07-10 05:15:31.000000 plugen-1.0.3/plugen.egg-info/top_level.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       38 2023-07-10 05:15:31.577340 plugen-1.0.3/setup.cfg
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      481 2023-07-10 05:15:28.000000 plugen-1.0.3/setup.py
```

### Comparing `plugen-1.0.2/README.md` & `plugen-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `plugen-1.0.2/plugen/lib/build.py` & `plugen-1.0.3/plugen/lib/build.py`

 * *Files identical despite different names*

### Comparing `plugen-1.0.2/plugen/lib/plugin.py` & `plugen-1.0.3/plugen/lib/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-1.0.2/plugen/lib/serve.py` & `plugen-1.0.3/plugen/lib/serve.py`

 * *Files identical despite different names*

### Comparing `plugen-1.0.2/plugen/lib/utils.py` & `plugen-1.0.3/plugen/lib/utils.py`

 * *Files identical despite different names*

### Comparing `plugen-1.0.2/plugen/main.py` & `plugen-1.0.3/plugen/main.py`

 * *Files identical despite different names*

### Comparing `plugen-1.0.2/plugen/plugins/hotreload/plugin.py` & `plugen-1.0.3/plugen/plugins/hotreload/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-1.0.2/plugen/plugins/sass/plugin.py` & `plugen-1.0.3/plugen/plugins/sass/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-1.0.2/plugen.egg-info/SOURCES.txt` & `plugen-1.0.3/plugen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

