# Comparing `tmp/tone-0.0.6.tar.gz` & `tmp/tone-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tone-0.0.6.tar", last modified: Mon Jul 10 22:22:42 2023, max compression
+gzip compressed data, was "tone-0.0.7.tar", last modified: Mon Jul 10 23:06:49 2023, max compression
```

## Comparing `tone-0.0.6.tar` & `tone-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 22:22:42.575118 tone-0.0.6/
--rw-r--r--   0 steven    (1000) root         (0)     1063 2023-07-10 20:38:25.000000 tone-0.0.6/LICENSE
--rw-r--r--   0 steven    (1000) root         (0)       36 2023-07-10 20:38:25.000000 tone-0.0.6/MANIFEST.in
--rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-10 22:22:42.575118 tone-0.0.6/PKG-INFO
--rw-r--r--   0 steven    (1000) root         (0)       98 2023-07-10 20:38:25.000000 tone-0.0.6/README
--rw-r--r--   0 steven    (1000) root         (0)       38 2023-07-10 22:22:42.575118 tone-0.0.6/setup.cfg
--rw-r--r--   0 steven    (1000) root         (0)     1209 2023-07-10 20:38:25.000000 tone-0.0.6/setup.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 22:22:42.575118 tone-0.0.6/tests/
--rw-r--r--   0 steven    (1000) root         (0)      421 2023-07-10 20:38:25.000000 tone-0.0.6/tests/test_all.py
--rw-r--r--   0 steven    (1000) root         (0)      402 2023-07-10 20:38:25.000000 tone-0.0.6/tests/test_base.py
--rw-r--r--   0 steven    (1000) root         (0)      266 2023-07-10 20:38:25.000000 tone-0.0.6/tests/test_tone.py
--rw-r--r--   0 steven    (1000) root         (0)     3904 2023-07-10 20:38:25.000000 tone-0.0.6/tests/test_utils_attrdict.py
--rw-r--r--   0 steven    (1000) root         (0)      554 2023-07-10 20:38:25.000000 tone-0.0.6/tests/test_utils_logger.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 22:22:42.575118 tone-0.0.6/tone/
--rw-r--r--   0 steven    (1000) root         (0)       84 2023-07-10 22:22:29.000000 tone-0.0.6/tone/__init__.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 22:22:42.575118 tone-0.0.6/tone/utils/
--rw-r--r--   0 steven    (1000) root         (0)      147 2023-07-10 22:22:09.000000 tone-0.0.6/tone/utils/__init__.py
--rw-r--r--   0 steven    (1000) root         (0)     1502 2023-07-10 20:38:25.000000 tone-0.0.6/tone/utils/attrdict.py
--rw-r--r--   0 steven    (1000) root         (0)      618 2023-07-10 20:40:50.000000 tone-0.0.6/tone/utils/ipython.py
--rw-r--r--   0 steven    (1000) root         (0)      620 2023-07-10 22:22:14.000000 tone-0.0.6/tone/utils/learning.py
--rw-r--r--   0 steven    (1000) root         (0)     1029 2023-07-10 20:38:25.000000 tone-0.0.6/tone/utils/logger.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 22:22:42.575118 tone-0.0.6/tone.egg-info/
--rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-10 22:22:42.000000 tone-0.0.6/tone.egg-info/PKG-INFO
--rw-r--r--   0 steven    (1000) root         (0)      411 2023-07-10 22:22:42.000000 tone-0.0.6/tone.egg-info/SOURCES.txt
--rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-10 22:22:42.000000 tone-0.0.6/tone.egg-info/dependency_links.txt
--rw-r--r--   0 steven    (1000) root         (0)        5 2023-07-10 22:22:42.000000 tone-0.0.6/tone.egg-info/top_level.txt
--rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-10 22:22:42.000000 tone-0.0.6/tone.egg-info/zip-safe
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 23:06:49.368329 tone-0.0.7/
+-rw-r--r--   0 steven    (1000) root         (0)     1063 2023-07-10 20:38:25.000000 tone-0.0.7/LICENSE
+-rw-r--r--   0 steven    (1000) root         (0)       36 2023-07-10 20:38:25.000000 tone-0.0.7/MANIFEST.in
+-rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-10 23:06:49.368329 tone-0.0.7/PKG-INFO
+-rw-r--r--   0 steven    (1000) root         (0)       98 2023-07-10 20:38:25.000000 tone-0.0.7/README
+-rw-r--r--   0 steven    (1000) root         (0)       38 2023-07-10 23:06:49.368329 tone-0.0.7/setup.cfg
+-rw-r--r--   0 steven    (1000) root         (0)     1205 2023-07-10 22:23:33.000000 tone-0.0.7/setup.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 23:06:49.368329 tone-0.0.7/tests/
+-rw-r--r--   0 steven    (1000) root         (0)      421 2023-07-10 20:38:25.000000 tone-0.0.7/tests/test_all.py
+-rw-r--r--   0 steven    (1000) root         (0)      402 2023-07-10 20:38:25.000000 tone-0.0.7/tests/test_base.py
+-rw-r--r--   0 steven    (1000) root         (0)      266 2023-07-10 20:38:25.000000 tone-0.0.7/tests/test_tone.py
+-rw-r--r--   0 steven    (1000) root         (0)     3904 2023-07-10 20:38:25.000000 tone-0.0.7/tests/test_utils_attrdict.py
+-rw-r--r--   0 steven    (1000) root         (0)      554 2023-07-10 20:38:25.000000 tone-0.0.7/tests/test_utils_logger.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 23:06:49.368329 tone-0.0.7/tone/
+-rw-r--r--   0 steven    (1000) root         (0)       84 2023-07-10 23:06:09.000000 tone-0.0.7/tone/__init__.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 23:06:49.368329 tone-0.0.7/tone/utils/
+-rw-r--r--   0 steven    (1000) root         (0)      147 2023-07-10 22:22:09.000000 tone-0.0.7/tone/utils/__init__.py
+-rw-r--r--   0 steven    (1000) root         (0)     1502 2023-07-10 20:38:25.000000 tone-0.0.7/tone/utils/attrdict.py
+-rw-r--r--   0 steven    (1000) root         (0)      700 2023-07-10 23:06:01.000000 tone-0.0.7/tone/utils/ipython.py
+-rw-r--r--   0 steven    (1000) root         (0)      620 2023-07-10 22:22:14.000000 tone-0.0.7/tone/utils/learning.py
+-rw-r--r--   0 steven    (1000) root         (0)     1029 2023-07-10 20:38:25.000000 tone-0.0.7/tone/utils/logger.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 23:06:49.368329 tone-0.0.7/tone.egg-info/
+-rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-10 23:06:49.000000 tone-0.0.7/tone.egg-info/PKG-INFO
+-rw-r--r--   0 steven    (1000) root         (0)      411 2023-07-10 23:06:49.000000 tone-0.0.7/tone.egg-info/SOURCES.txt
+-rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-10 23:06:49.000000 tone-0.0.7/tone.egg-info/dependency_links.txt
+-rw-r--r--   0 steven    (1000) root         (0)        5 2023-07-10 23:06:49.000000 tone-0.0.7/tone.egg-info/top_level.txt
+-rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-10 23:06:49.000000 tone-0.0.7/tone.egg-info/zip-safe
```

### Comparing `tone-0.0.6/LICENSE` & `tone-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tone-0.0.6/setup.py` & `tone-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,9 +40,9 @@
     zip_safe=True,
     platforms="any",
 )
 
 
 # python setup.py sdist bdist_wheel --universal
 # twine upload dist/*
-# pip2 install dandan --upgrade -i https://pypi.python.org/simple
-# pip3 install dandan --upgrade -i https://pypi.python.org/simple
+# pip2 install tone --upgrade -i https://pypi.python.org/simple
+# pip3 install tone --upgrade -i https://pypi.python.org/simple
```

### Comparing `tone-0.0.6/tests/test_utils_attrdict.py` & `tone-0.0.7/tests/test_utils_attrdict.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.6/tests/test_utils_logger.py` & `tone-0.0.7/tests/test_utils_logger.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.6/tone/utils/attrdict.py` & `tone-0.0.7/tone/utils/attrdict.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.6/tone/utils/ipython.py` & `tone-0.0.7/tone/utils/ipython.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,7 +16,13 @@
 
     ipy = get_ipython()
     if 'IPython.extensions.autoreload' not in ipy.extension_manager.loaded:
         ipy.run_line_magic('load_ext', 'autoreload')
 
     ipy.run_line_magic('autoreload', '1')
     ipy.run_line_magic('aimport', module)
+
+
+class StopExecution(Exception):
+
+    def _render_traceback_(self):
+        pass
```

### Comparing `tone-0.0.6/tone/utils/learning.py` & `tone-0.0.7/tone/utils/learning.py`

 * *Files identical despite different names*

### Comparing `tone-0.0.6/tone/utils/logger.py` & `tone-0.0.7/tone/utils/logger.py`

 * *Files identical despite different names*

