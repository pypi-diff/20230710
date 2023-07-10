# Comparing `tmp/tone-0.0.5.tar.gz` & `tmp/tone-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tone-0.0.5.tar", last modified: Mon Jul 10 20:41:48 2023, max compression
+gzip compressed data, was "tone-0.0.6.tar", last modified: Mon Jul 10 22:22:42 2023, max compression
```

## Comparing `tone-0.0.5.tar` & `tone-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 20:41:48.548729 tone-0.0.5/
--rw-r--r--   0 steven    (1000) root         (0)     1063 2023-07-10 20:38:25.000000 tone-0.0.5/LICENSE
--rw-r--r--   0 steven    (1000) root         (0)       36 2023-07-10 20:38:25.000000 tone-0.0.5/MANIFEST.in
--rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-10 20:41:48.548729 tone-0.0.5/PKG-INFO
--rw-r--r--   0 steven    (1000) root         (0)       98 2023-07-10 20:38:25.000000 tone-0.0.5/README
--rw-r--r--   0 steven    (1000) root         (0)       38 2023-07-10 20:41:48.548729 tone-0.0.5/setup.cfg
--rw-r--r--   0 steven    (1000) root         (0)     1209 2023-07-10 20:38:25.000000 tone-0.0.5/setup.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 20:41:48.548729 tone-0.0.5/tests/
--rw-r--r--   0 steven    (1000) root         (0)      421 2023-07-10 20:38:25.000000 tone-0.0.5/tests/test_all.py
--rw-r--r--   0 steven    (1000) root         (0)      402 2023-07-10 20:38:25.000000 tone-0.0.5/tests/test_base.py
--rw-r--r--   0 steven    (1000) root         (0)      266 2023-07-10 20:38:25.000000 tone-0.0.5/tests/test_tone.py
--rw-r--r--   0 steven    (1000) root         (0)     3904 2023-07-10 20:38:25.000000 tone-0.0.5/tests/test_utils_attrdict.py
--rw-r--r--   0 steven    (1000) root         (0)      554 2023-07-10 20:38:25.000000 tone-0.0.5/tests/test_utils_logger.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 20:41:48.548729 tone-0.0.5/tone/
--rw-r--r--   0 steven    (1000) root         (0)       84 2023-07-10 20:40:01.000000 tone-0.0.5/tone/__init__.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 20:41:48.548729 tone-0.0.5/tone/utils/
--rw-r--r--   0 steven    (1000) root         (0)      108 2023-07-10 20:41:10.000000 tone-0.0.5/tone/utils/__init__.py
--rw-r--r--   0 steven    (1000) root         (0)     1502 2023-07-10 20:38:25.000000 tone-0.0.5/tone/utils/attrdict.py
--rw-r--r--   0 steven    (1000) root         (0)      618 2023-07-10 20:40:50.000000 tone-0.0.5/tone/utils/ipython.py
--rw-r--r--   0 steven    (1000) root         (0)     1029 2023-07-10 20:38:25.000000 tone-0.0.5/tone/utils/logger.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 20:41:48.548729 tone-0.0.5/tone.egg-info/
--rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-10 20:41:48.000000 tone-0.0.5/tone.egg-info/PKG-INFO
--rw-r--r--   0 steven    (1000) root         (0)      388 2023-07-10 20:41:48.000000 tone-0.0.5/tone.egg-info/SOURCES.txt
--rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-10 20:41:48.000000 tone-0.0.5/tone.egg-info/dependency_links.txt
--rw-r--r--   0 steven    (1000) root         (0)        5 2023-07-10 20:41:48.000000 tone-0.0.5/tone.egg-info/top_level.txt
--rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-10 20:41:48.000000 tone-0.0.5/tone.egg-info/zip-safe
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 22:22:42.575118 tone-0.0.6/
+-rw-r--r--   0 steven    (1000) root         (0)     1063 2023-07-10 20:38:25.000000 tone-0.0.6/LICENSE
+-rw-r--r--   0 steven    (1000) root         (0)       36 2023-07-10 20:38:25.000000 tone-0.0.6/MANIFEST.in
+-rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-10 22:22:42.575118 tone-0.0.6/PKG-INFO
+-rw-r--r--   0 steven    (1000) root         (0)       98 2023-07-10 20:38:25.000000 tone-0.0.6/README
+-rw-r--r--   0 steven    (1000) root         (0)       38 2023-07-10 22:22:42.575118 tone-0.0.6/setup.cfg
+-rw-r--r--   0 steven    (1000) root         (0)     1209 2023-07-10 20:38:25.000000 tone-0.0.6/setup.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 22:22:42.575118 tone-0.0.6/tests/
+-rw-r--r--   0 steven    (1000) root         (0)      421 2023-07-10 20:38:25.000000 tone-0.0.6/tests/test_all.py
+-rw-r--r--   0 steven    (1000) root         (0)      402 2023-07-10 20:38:25.000000 tone-0.0.6/tests/test_base.py
+-rw-r--r--   0 steven    (1000) root         (0)      266 2023-07-10 20:38:25.000000 tone-0.0.6/tests/test_tone.py
+-rw-r--r--   0 steven    (1000) root         (0)     3904 2023-07-10 20:38:25.000000 tone-0.0.6/tests/test_utils_attrdict.py
+-rw-r--r--   0 steven    (1000) root         (0)      554 2023-07-10 20:38:25.000000 tone-0.0.6/tests/test_utils_logger.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 22:22:42.575118 tone-0.0.6/tone/
+-rw-r--r--   0 steven    (1000) root         (0)       84 2023-07-10 22:22:29.000000 tone-0.0.6/tone/__init__.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 22:22:42.575118 tone-0.0.6/tone/utils/
+-rw-r--r--   0 steven    (1000) root         (0)      147 2023-07-10 22:22:09.000000 tone-0.0.6/tone/utils/__init__.py
+-rw-r--r--   0 steven    (1000) root         (0)     1502 2023-07-10 20:38:25.000000 tone-0.0.6/tone/utils/attrdict.py
+-rw-r--r--   0 steven    (1000) root         (0)      618 2023-07-10 20:40:50.000000 tone-0.0.6/tone/utils/ipython.py
+-rw-r--r--   0 steven    (1000) root         (0)      620 2023-07-10 22:22:14.000000 tone-0.0.6/tone/utils/learning.py
+-rw-r--r--   0 steven    (1000) root         (0)     1029 2023-07-10 20:38:25.000000 tone-0.0.6/tone/utils/logger.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 22:22:42.575118 tone-0.0.6/tone.egg-info/
+-rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-10 22:22:42.000000 tone-0.0.6/tone.egg-info/PKG-INFO
+-rw-r--r--   0 steven    (1000) root         (0)      411 2023-07-10 22:22:42.000000 tone-0.0.6/tone.egg-info/SOURCES.txt
+-rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-10 22:22:42.000000 tone-0.0.6/tone.egg-info/dependency_links.txt
+-rw-r--r--   0 steven    (1000) root         (0)        5 2023-07-10 22:22:42.000000 tone-0.0.6/tone.egg-info/top_level.txt
+-rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-10 22:22:42.000000 tone-0.0.6/tone.egg-info/zip-safe
```

### Comparing `tone-0.0.5/LICENSE` & `tone-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tone-0.0.5/setup.py` & `tone-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.5/tests/test_utils_attrdict.py` & `tone-0.0.6/tests/test_utils_attrdict.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.5/tests/test_utils_logger.py` & `tone-0.0.6/tests/test_utils_logger.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.5/tone/utils/attrdict.py` & `tone-0.0.6/tone/utils/attrdict.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.5/tone/utils/ipython.py` & `tone-0.0.6/tone/utils/ipython.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.5/tone/utils/logger.py` & `tone-0.0.6/tone/utils/logger.py`

 * *Files identical despite different names*

