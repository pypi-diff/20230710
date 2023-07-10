# Comparing `tmp/yaccounts-1.1.2.tar.gz` & `tmp/yaccounts-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaccounts-1.1.2.tar", last modified: Mon Jul 10 15:17:38 2023, max compression
+gzip compressed data, was "yaccounts-1.1.3.tar", last modified: Mon Jul 10 21:17:42 2023, max compression
```

## Comparing `yaccounts-1.1.2.tar` & `yaccounts-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 15:17:38.957820 yaccounts-1.1.2/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-10 15:17:38.957820 yaccounts-1.1.2/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-10 15:17:38.957820 yaccounts-1.1.2/setup.cfg
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      395 2023-07-10 15:17:36.000000 yaccounts-1.1.2/setup.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 15:17:38.947820 yaccounts-1.1.2/test/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1199 2023-07-10 14:33:50.000000 yaccounts-1.1.2/test/test.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 15:17:38.957820 yaccounts-1.1.2/yaccounts/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-10 14:33:38.000000 yaccounts-1.1.2/yaccounts/__init__.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3628 2023-07-10 15:17:36.000000 yaccounts-1.1.2/yaccounts/analyzer.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2001 2023-07-10 15:17:36.000000 yaccounts-1.1.2/yaccounts/config.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     9762 2023-07-10 15:17:36.000000 yaccounts-1.1.2/yaccounts/operating_unit.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      290 2023-07-10 14:33:38.000000 yaccounts-1.1.2/yaccounts/utils.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1097 2023-07-10 14:33:38.000000 yaccounts-1.1.2/yaccounts/workbook.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2683 2023-07-10 15:17:36.000000 yaccounts-1.1.2/yaccounts/worksheet.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 15:17:38.957820 yaccounts-1.1.2/yaccounts.egg-info/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-10 15:17:38.000000 yaccounts-1.1.2/yaccounts.egg-info/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      341 2023-07-10 15:17:38.000000 yaccounts-1.1.2/yaccounts.egg-info/SOURCES.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-07-10 15:17:38.000000 yaccounts-1.1.2/yaccounts.egg-info/dependency_links.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       45 2023-07-10 15:17:38.000000 yaccounts-1.1.2/yaccounts.egg-info/requires.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       10 2023-07-10 15:17:38.000000 yaccounts-1.1.2/yaccounts.egg-info/top_level.txt
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 21:17:42.596136 yaccounts-1.1.3/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-10 21:17:42.596136 yaccounts-1.1.3/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-10 21:17:42.596136 yaccounts-1.1.3/setup.cfg
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      395 2023-07-10 21:16:52.000000 yaccounts-1.1.3/setup.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 21:17:42.596136 yaccounts-1.1.3/test/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1199 2023-07-10 14:33:50.000000 yaccounts-1.1.3/test/test.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 21:17:42.596136 yaccounts-1.1.3/yaccounts/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-10 14:33:38.000000 yaccounts-1.1.3/yaccounts/__init__.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3628 2023-07-10 15:17:36.000000 yaccounts-1.1.3/yaccounts/analyzer.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     4702 2023-07-10 21:16:42.000000 yaccounts-1.1.3/yaccounts/config.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     9762 2023-07-10 15:17:36.000000 yaccounts-1.1.3/yaccounts/operating_unit.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      290 2023-07-10 14:33:38.000000 yaccounts-1.1.3/yaccounts/utils.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1097 2023-07-10 14:33:38.000000 yaccounts-1.1.3/yaccounts/workbook.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2683 2023-07-10 15:17:36.000000 yaccounts-1.1.3/yaccounts/worksheet.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 21:17:42.596136 yaccounts-1.1.3/yaccounts.egg-info/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-10 21:17:42.000000 yaccounts-1.1.3/yaccounts.egg-info/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      341 2023-07-10 21:17:42.000000 yaccounts-1.1.3/yaccounts.egg-info/SOURCES.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-07-10 21:17:42.000000 yaccounts-1.1.3/yaccounts.egg-info/dependency_links.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       45 2023-07-10 21:17:42.000000 yaccounts-1.1.3/yaccounts.egg-info/requires.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       10 2023-07-10 21:17:42.000000 yaccounts-1.1.3/yaccounts.egg-info/top_level.txt
```

### Comparing `yaccounts-1.1.2/test/test.py` & `yaccounts-1.1.3/test/test.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.2/yaccounts/analyzer.py` & `yaccounts-1.1.3/yaccounts/analyzer.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.2/yaccounts/operating_unit.py` & `yaccounts-1.1.3/yaccounts/operating_unit.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.2/yaccounts/workbook.py` & `yaccounts-1.1.3/yaccounts/workbook.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.2/yaccounts/worksheet.py` & `yaccounts-1.1.3/yaccounts/worksheet.py`

 * *Files identical despite different names*

