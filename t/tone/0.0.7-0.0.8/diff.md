# Comparing `tmp/tone-0.0.7.tar.gz` & `tmp/tone-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tone-0.0.7.tar", last modified: Mon Jul 10 23:06:49 2023, max compression
+gzip compressed data, was "tone-0.0.8.tar", last modified: Tue Jul 11 03:30:39 2023, max compression
```

## Comparing `tone-0.0.7.tar` & `tone-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 23:06:49.368329 tone-0.0.7/
--rw-r--r--   0 steven    (1000) root         (0)     1063 2023-07-10 20:38:25.000000 tone-0.0.7/LICENSE
--rw-r--r--   0 steven    (1000) root         (0)       36 2023-07-10 20:38:25.000000 tone-0.0.7/MANIFEST.in
--rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-10 23:06:49.368329 tone-0.0.7/PKG-INFO
--rw-r--r--   0 steven    (1000) root         (0)       98 2023-07-10 20:38:25.000000 tone-0.0.7/README
--rw-r--r--   0 steven    (1000) root         (0)       38 2023-07-10 23:06:49.368329 tone-0.0.7/setup.cfg
--rw-r--r--   0 steven    (1000) root         (0)     1205 2023-07-10 22:23:33.000000 tone-0.0.7/setup.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 23:06:49.368329 tone-0.0.7/tests/
--rw-r--r--   0 steven    (1000) root         (0)      421 2023-07-10 20:38:25.000000 tone-0.0.7/tests/test_all.py
--rw-r--r--   0 steven    (1000) root         (0)      402 2023-07-10 20:38:25.000000 tone-0.0.7/tests/test_base.py
--rw-r--r--   0 steven    (1000) root         (0)      266 2023-07-10 20:38:25.000000 tone-0.0.7/tests/test_tone.py
--rw-r--r--   0 steven    (1000) root         (0)     3904 2023-07-10 20:38:25.000000 tone-0.0.7/tests/test_utils_attrdict.py
--rw-r--r--   0 steven    (1000) root         (0)      554 2023-07-10 20:38:25.000000 tone-0.0.7/tests/test_utils_logger.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 23:06:49.368329 tone-0.0.7/tone/
--rw-r--r--   0 steven    (1000) root         (0)       84 2023-07-10 23:06:09.000000 tone-0.0.7/tone/__init__.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 23:06:49.368329 tone-0.0.7/tone/utils/
--rw-r--r--   0 steven    (1000) root         (0)      147 2023-07-10 22:22:09.000000 tone-0.0.7/tone/utils/__init__.py
--rw-r--r--   0 steven    (1000) root         (0)     1502 2023-07-10 20:38:25.000000 tone-0.0.7/tone/utils/attrdict.py
--rw-r--r--   0 steven    (1000) root         (0)      700 2023-07-10 23:06:01.000000 tone-0.0.7/tone/utils/ipython.py
--rw-r--r--   0 steven    (1000) root         (0)      620 2023-07-10 22:22:14.000000 tone-0.0.7/tone/utils/learning.py
--rw-r--r--   0 steven    (1000) root         (0)     1029 2023-07-10 20:38:25.000000 tone-0.0.7/tone/utils/logger.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 23:06:49.368329 tone-0.0.7/tone.egg-info/
--rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-10 23:06:49.000000 tone-0.0.7/tone.egg-info/PKG-INFO
--rw-r--r--   0 steven    (1000) root         (0)      411 2023-07-10 23:06:49.000000 tone-0.0.7/tone.egg-info/SOURCES.txt
--rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-10 23:06:49.000000 tone-0.0.7/tone.egg-info/dependency_links.txt
--rw-r--r--   0 steven    (1000) root         (0)        5 2023-07-10 23:06:49.000000 tone-0.0.7/tone.egg-info/top_level.txt
--rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-10 23:06:49.000000 tone-0.0.7/tone.egg-info/zip-safe
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:30:39.390932 tone-0.0.8/
+-rw-r--r--   0 steven    (1000) root         (0)     1063 2023-07-10 20:38:25.000000 tone-0.0.8/LICENSE
+-rw-r--r--   0 steven    (1000) root         (0)       36 2023-07-10 20:38:25.000000 tone-0.0.8/MANIFEST.in
+-rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-11 03:30:39.390932 tone-0.0.8/PKG-INFO
+-rw-r--r--   0 steven    (1000) root         (0)       98 2023-07-10 20:38:25.000000 tone-0.0.8/README
+-rw-r--r--   0 steven    (1000) root         (0)       38 2023-07-11 03:30:39.390932 tone-0.0.8/setup.cfg
+-rw-r--r--   0 steven    (1000) root         (0)     1205 2023-07-10 22:23:33.000000 tone-0.0.8/setup.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:30:39.387598 tone-0.0.8/tests/
+-rw-r--r--   0 steven    (1000) root         (0)      421 2023-07-10 20:38:25.000000 tone-0.0.8/tests/test_all.py
+-rw-r--r--   0 steven    (1000) root         (0)      402 2023-07-10 20:38:25.000000 tone-0.0.8/tests/test_base.py
+-rw-r--r--   0 steven    (1000) root         (0)      437 2023-07-11 03:29:57.000000 tone-0.0.8/tests/test_learning.py
+-rw-r--r--   0 steven    (1000) root         (0)      266 2023-07-10 20:38:25.000000 tone-0.0.8/tests/test_tone.py
+-rw-r--r--   0 steven    (1000) root         (0)     3904 2023-07-10 20:38:25.000000 tone-0.0.8/tests/test_utils_attrdict.py
+-rw-r--r--   0 steven    (1000) root         (0)      554 2023-07-10 20:38:25.000000 tone-0.0.8/tests/test_utils_logger.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:30:39.390932 tone-0.0.8/tone/
+-rw-r--r--   0 steven    (1000) root         (0)       84 2023-07-11 03:30:22.000000 tone-0.0.8/tone/__init__.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:30:39.390932 tone-0.0.8/tone/utils/
+-rw-r--r--   0 steven    (1000) root         (0)      147 2023-07-10 22:22:09.000000 tone-0.0.8/tone/utils/__init__.py
+-rw-r--r--   0 steven    (1000) root         (0)     1502 2023-07-10 20:38:25.000000 tone-0.0.8/tone/utils/attrdict.py
+-rw-r--r--   0 steven    (1000) root         (0)      700 2023-07-10 23:06:01.000000 tone-0.0.8/tone/utils/ipython.py
+-rw-r--r--   0 steven    (1000) root         (0)     1453 2023-07-11 03:29:24.000000 tone-0.0.8/tone/utils/learning.py
+-rw-r--r--   0 steven    (1000) root         (0)     1029 2023-07-10 20:38:25.000000 tone-0.0.8/tone/utils/logger.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-11 03:30:39.390932 tone-0.0.8/tone.egg-info/
+-rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-11 03:30:39.000000 tone-0.0.8/tone.egg-info/PKG-INFO
+-rw-r--r--   0 steven    (1000) root         (0)      434 2023-07-11 03:30:39.000000 tone-0.0.8/tone.egg-info/SOURCES.txt
+-rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-11 03:30:39.000000 tone-0.0.8/tone.egg-info/dependency_links.txt
+-rw-r--r--   0 steven    (1000) root         (0)        5 2023-07-11 03:30:39.000000 tone-0.0.8/tone.egg-info/top_level.txt
+-rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-11 03:30:39.000000 tone-0.0.8/tone.egg-info/zip-safe
```

### Comparing `tone-0.0.7/LICENSE` & `tone-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tone-0.0.7/setup.py` & `tone-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.7/tests/test_utils_attrdict.py` & `tone-0.0.8/tests/test_utils_attrdict.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.7/tests/test_utils_logger.py` & `tone-0.0.8/tests/test_utils_logger.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.7/tone/utils/attrdict.py` & `tone-0.0.8/tone/utils/attrdict.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.7/tone/utils/ipython.py` & `tone-0.0.8/tone/utils/ipython.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.7/tone/utils/logger.py` & `tone-0.0.8/tone/utils/logger.py`

 * *Files identical despite different names*

