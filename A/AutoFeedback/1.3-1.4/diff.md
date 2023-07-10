# Comparing `tmp/AutoFeedback-1.3.tar.gz` & `tmp/AutoFeedback-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoFeedback-1.3.tar", last modified: Thu Jul  6 16:22:41 2023, max compression
+gzip compressed data, was "AutoFeedback-1.4.tar", last modified: Mon Jul 10 12:06:50 2023, max compression
```

## Comparing `AutoFeedback-1.3.tar` & `AutoFeedback-1.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-06 16:22:41.735893 AutoFeedback-1.3/
--rw-r--r--   0 abrown41   (502) staff       (20)      162 2023-03-20 10:13:58.000000 AutoFeedback-1.3/AUTHORS.rst
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-06 16:22:41.736636 AutoFeedback-1.3/AutoFeedback/
--rw-r--r--   0 abrown41   (502) staff       (20)      260 2023-07-06 16:17:28.000000 AutoFeedback-1.3/AutoFeedback/__init__.py
--rw-r--r--   0 abrown41   (502) staff       (20)      495 2023-07-06 16:22:41.736702 AutoFeedback-1.3/AutoFeedback/_version.py
--rw-r--r--   0 abrown41   (502) staff       (20)      283 2023-03-20 10:13:58.000000 AutoFeedback-1.3/AutoFeedback/bcolors.py
--rw-r--r--   0 abrown41   (502) staff       (20)     7052 2023-06-22 17:57:56.000000 AutoFeedback-1.3/AutoFeedback/funcchecks.py
--rw-r--r--   0 abrown41   (502) staff       (20)     4557 2023-03-20 10:13:58.000000 AutoFeedback-1.3/AutoFeedback/function_error_messages.py
--rw-r--r--   0 abrown41   (502) staff       (20)     4374 2023-06-22 18:26:48.000000 AutoFeedback-1.3/AutoFeedback/plot_error_messages.py
--rw-r--r--   0 abrown41   (502) staff       (20)     9009 2023-06-22 18:35:21.000000 AutoFeedback-1.3/AutoFeedback/plotchecks.py
--rw-r--r--   0 abrown41   (502) staff       (20)     4391 2023-03-20 10:13:58.000000 AutoFeedback-1.3/AutoFeedback/plotclass.py
--rw-r--r--   0 abrown41   (502) staff       (20)    16126 2023-03-20 10:13:58.000000 AutoFeedback-1.3/AutoFeedback/randomclass.py
--rw-r--r--   0 abrown41   (502) staff       (20)      431 2023-06-22 17:57:56.000000 AutoFeedback-1.3/AutoFeedback/utils.py
--rw-r--r--   0 abrown41   (502) staff       (20)     4119 2023-06-22 17:57:56.000000 AutoFeedback-1.3/AutoFeedback/varchecks.py
--rw-r--r--   0 abrown41   (502) staff       (20)     3986 2023-03-20 10:13:58.000000 AutoFeedback-1.3/AutoFeedback/variable_error_messages.py
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-06 16:22:41.732773 AutoFeedback-1.3/AutoFeedback.egg-info/
--rw-r--r--   0 abrown41   (502) staff       (20)     2712 2023-07-06 16:22:41.000000 AutoFeedback-1.3/AutoFeedback.egg-info/PKG-INFO
--rw-r--r--   0 abrown41   (502) staff       (20)      999 2023-07-06 16:22:41.000000 AutoFeedback-1.3/AutoFeedback.egg-info/SOURCES.txt
--rw-r--r--   0 abrown41   (502) staff       (20)        1 2023-07-06 16:22:41.000000 AutoFeedback-1.3/AutoFeedback.egg-info/dependency_links.txt
--rw-r--r--   0 abrown41   (502) staff       (20)       20 2023-07-06 16:22:41.000000 AutoFeedback-1.3/AutoFeedback.egg-info/entry_points.txt
--rw-r--r--   0 abrown41   (502) staff       (20)       63 2023-07-06 16:22:41.000000 AutoFeedback-1.3/AutoFeedback.egg-info/requires.txt
--rw-r--r--   0 abrown41   (502) staff       (20)       18 2023-07-06 16:22:41.000000 AutoFeedback-1.3/AutoFeedback.egg-info/top_level.txt
--rw-r--r--   0 abrown41   (502) staff       (20)     3081 2023-03-20 10:13:58.000000 AutoFeedback-1.3/CONTRIBUTING.rst
--rw-r--r--   0 abrown41   (502) staff       (20)     1520 2023-03-20 10:13:58.000000 AutoFeedback-1.3/LICENSE
--rw-r--r--   0 abrown41   (502) staff       (20)      398 2023-03-20 10:13:58.000000 AutoFeedback-1.3/MANIFEST.in
--rw-r--r--   0 abrown41   (502) staff       (20)     2712 2023-07-06 16:22:41.735973 AutoFeedback-1.3/PKG-INFO
--rw-r--r--   0 abrown41   (502) staff       (20)     2157 2023-03-20 10:13:58.000000 AutoFeedback-1.3/README.rst
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-06 16:22:41.733255 AutoFeedback-1.3/docs/
--rw-r--r--   0 abrown41   (502) staff       (20)      673 2023-03-20 10:13:58.000000 AutoFeedback-1.3/docs/Makefile
--rw-r--r--   0 abrown41   (502) staff       (20)      797 2023-03-20 10:13:58.000000 AutoFeedback-1.3/docs/make.bat
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-06 16:22:41.734021 AutoFeedback-1.3/docs/source/
--rw-r--r--   0 abrown41   (502) staff       (20)     6730 2023-03-20 10:13:58.000000 AutoFeedback-1.3/docs/source/conf.py
--rw-r--r--   0 abrown41   (502) staff       (20)      396 2023-03-20 10:13:58.000000 AutoFeedback-1.3/docs/source/index.rst
--rw-r--r--   0 abrown41   (502) staff       (20)     1083 2023-03-20 10:13:58.000000 AutoFeedback-1.3/docs/source/min_versions.rst
--rw-r--r--   0 abrown41   (502) staff       (20)    30606 2023-06-22 17:57:56.000000 AutoFeedback-1.3/docs/source/usage.rst
--rw-r--r--   0 abrown41   (502) staff       (20)       29 2023-06-22 17:57:53.000000 AutoFeedback-1.3/requirements.txt
--rw-r--r--   0 abrown41   (502) staff       (20)      408 2023-07-06 16:22:41.736281 AutoFeedback-1.3/setup.cfg
--rw-r--r--   0 abrown41   (502) staff       (20)     2414 2023-03-20 10:13:58.000000 AutoFeedback-1.3/setup.py
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-06 16:22:41.735767 AutoFeedback-1.3/test/
--rw-r--r--   0 abrown41   (502) staff       (20)        0 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/__init__.py
--rw-r--r--   0 abrown41   (502) staff       (20)       32 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/printtest.py
--rw-r--r--   0 abrown41   (502) staff       (20)     9518 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/testerrors.py
--rw-r--r--   0 abrown41   (502) staff       (20)     3525 2023-06-22 17:57:56.000000 AutoFeedback-1.3/test/testfuncs.py
--rw-r--r--   0 abrown41   (502) staff       (20)     3497 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/testplot.py
--rw-r--r--   0 abrown41   (502) staff       (20)     2780 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/testplotclass.py
--rw-r--r--   0 abrown41   (502) staff       (20)      578 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/testprint.py
--rw-r--r--   0 abrown41   (502) staff       (20)    11743 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/testrandomclass.py
--rw-r--r--   0 abrown41   (502) staff       (20)     1976 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/testsymp.py
--rw-r--r--   0 abrown41   (502) staff       (20)      970 2023-06-22 17:57:56.000000 AutoFeedback-1.3/test/testutils.py
--rw-r--r--   0 abrown41   (502) staff       (20)     2224 2023-06-22 17:57:56.000000 AutoFeedback-1.3/test/testvars.py
--rw-r--r--   0 abrown41   (502) staff       (20)    78254 2023-03-20 10:13:58.000000 AutoFeedback-1.3/versioneer.py
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-10 12:06:50.185565 AutoFeedback-1.4/
+-rw-r--r--   0 abrown41   (502) staff       (20)      162 2023-03-20 10:13:58.000000 AutoFeedback-1.4/AUTHORS.rst
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-10 12:06:50.186226 AutoFeedback-1.4/AutoFeedback/
+-rw-r--r--   0 abrown41   (502) staff       (20)      260 2023-07-06 16:17:28.000000 AutoFeedback-1.4/AutoFeedback/__init__.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      495 2023-07-10 12:06:50.186263 AutoFeedback-1.4/AutoFeedback/_version.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      283 2023-03-20 10:13:58.000000 AutoFeedback-1.4/AutoFeedback/bcolors.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     7052 2023-06-22 17:57:56.000000 AutoFeedback-1.4/AutoFeedback/funcchecks.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     4557 2023-03-20 10:13:58.000000 AutoFeedback-1.4/AutoFeedback/function_error_messages.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     4359 2023-07-10 11:39:39.000000 AutoFeedback-1.4/AutoFeedback/plot_error_messages.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     9172 2023-07-10 11:57:02.000000 AutoFeedback-1.4/AutoFeedback/plotchecks.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     4391 2023-03-20 10:13:58.000000 AutoFeedback-1.4/AutoFeedback/plotclass.py
+-rw-r--r--   0 abrown41   (502) staff       (20)    16126 2023-03-20 10:13:58.000000 AutoFeedback-1.4/AutoFeedback/randomclass.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      431 2023-06-22 17:57:56.000000 AutoFeedback-1.4/AutoFeedback/utils.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     4119 2023-07-10 10:44:54.000000 AutoFeedback-1.4/AutoFeedback/varchecks.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     3986 2023-03-20 10:13:58.000000 AutoFeedback-1.4/AutoFeedback/variable_error_messages.py
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-10 12:06:50.182918 AutoFeedback-1.4/AutoFeedback.egg-info/
+-rw-r--r--   0 abrown41   (502) staff       (20)     2712 2023-07-10 12:06:50.000000 AutoFeedback-1.4/AutoFeedback.egg-info/PKG-INFO
+-rw-r--r--   0 abrown41   (502) staff       (20)      999 2023-07-10 12:06:50.000000 AutoFeedback-1.4/AutoFeedback.egg-info/SOURCES.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)        1 2023-07-10 12:06:50.000000 AutoFeedback-1.4/AutoFeedback.egg-info/dependency_links.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)       20 2023-07-10 12:06:50.000000 AutoFeedback-1.4/AutoFeedback.egg-info/entry_points.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)       63 2023-07-10 12:06:50.000000 AutoFeedback-1.4/AutoFeedback.egg-info/requires.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)       18 2023-07-10 12:06:50.000000 AutoFeedback-1.4/AutoFeedback.egg-info/top_level.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)     3081 2023-03-20 10:13:58.000000 AutoFeedback-1.4/CONTRIBUTING.rst
+-rw-r--r--   0 abrown41   (502) staff       (20)     1520 2023-03-20 10:13:58.000000 AutoFeedback-1.4/LICENSE
+-rw-r--r--   0 abrown41   (502) staff       (20)      398 2023-03-20 10:13:58.000000 AutoFeedback-1.4/MANIFEST.in
+-rw-r--r--   0 abrown41   (502) staff       (20)     2712 2023-07-10 12:06:50.185628 AutoFeedback-1.4/PKG-INFO
+-rw-r--r--   0 abrown41   (502) staff       (20)     2157 2023-03-20 10:13:58.000000 AutoFeedback-1.4/README.rst
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-10 12:06:50.183303 AutoFeedback-1.4/docs/
+-rw-r--r--   0 abrown41   (502) staff       (20)      673 2023-03-20 10:13:58.000000 AutoFeedback-1.4/docs/Makefile
+-rw-r--r--   0 abrown41   (502) staff       (20)      797 2023-03-20 10:13:58.000000 AutoFeedback-1.4/docs/make.bat
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-10 12:06:50.183956 AutoFeedback-1.4/docs/source/
+-rw-r--r--   0 abrown41   (502) staff       (20)     6730 2023-03-20 10:13:58.000000 AutoFeedback-1.4/docs/source/conf.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      396 2023-03-20 10:13:58.000000 AutoFeedback-1.4/docs/source/index.rst
+-rw-r--r--   0 abrown41   (502) staff       (20)     1083 2023-03-20 10:13:58.000000 AutoFeedback-1.4/docs/source/min_versions.rst
+-rw-r--r--   0 abrown41   (502) staff       (20)    30606 2023-06-22 17:57:56.000000 AutoFeedback-1.4/docs/source/usage.rst
+-rw-r--r--   0 abrown41   (502) staff       (20)       29 2023-06-22 17:57:53.000000 AutoFeedback-1.4/requirements.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)      408 2023-07-10 12:06:50.185911 AutoFeedback-1.4/setup.cfg
+-rw-r--r--   0 abrown41   (502) staff       (20)     2414 2023-03-20 10:13:58.000000 AutoFeedback-1.4/setup.py
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-10 12:06:50.185443 AutoFeedback-1.4/test/
+-rw-r--r--   0 abrown41   (502) staff       (20)        0 2023-03-20 10:13:58.000000 AutoFeedback-1.4/test/__init__.py
+-rw-r--r--   0 abrown41   (502) staff       (20)       32 2023-03-20 10:13:58.000000 AutoFeedback-1.4/test/printtest.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     9536 2023-07-10 12:05:46.000000 AutoFeedback-1.4/test/testerrors.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     3525 2023-06-22 17:57:56.000000 AutoFeedback-1.4/test/testfuncs.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     3497 2023-03-20 10:13:58.000000 AutoFeedback-1.4/test/testplot.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     2780 2023-03-20 10:13:58.000000 AutoFeedback-1.4/test/testplotclass.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      578 2023-03-20 10:13:58.000000 AutoFeedback-1.4/test/testprint.py
+-rw-r--r--   0 abrown41   (502) staff       (20)    11743 2023-03-20 10:13:58.000000 AutoFeedback-1.4/test/testrandomclass.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     1976 2023-03-20 10:13:58.000000 AutoFeedback-1.4/test/testsymp.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      970 2023-06-22 17:57:56.000000 AutoFeedback-1.4/test/testutils.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     2224 2023-06-22 17:57:56.000000 AutoFeedback-1.4/test/testvars.py
+-rw-r--r--   0 abrown41   (502) staff       (20)    78254 2023-03-20 10:13:58.000000 AutoFeedback-1.4/versioneer.py
```

### Comparing `AutoFeedback-1.3/AutoFeedback/funcchecks.py` & `AutoFeedback-1.4/AutoFeedback/funcchecks.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/AutoFeedback/function_error_messages.py` & `AutoFeedback-1.4/AutoFeedback/function_error_messages.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/AutoFeedback/plot_error_messages.py` & `AutoFeedback-1.4/AutoFeedback/plot_error_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,10 +102,10 @@
         emsg = eval(f"error_message().{error}")
         print(f"{bcolors.OKGREEN}{emsg}{bcolors.ENDC}")
     elif hasattr(expline, "diagnosis") and expline.diagnosis != "ok":
         emsg = expline.get_error(
             str(error).replace("_data(", "").replace(")", ""))
         print(f"{bcolors.FAIL}{emsg}{bcolors.ENDC}")
     else:
-        emsg = eval(f"error_message().{error}(expline.label)")
+        emsg = eval(f"error_message().{error}")
         print(f"{bcolors.FAIL}{emsg}{bcolors.ENDC}")
     print(f"{bcolors.WARNING}{30*'='}\n{bcolors.ENDC}")
```

### Comparing `AutoFeedback-1.3/AutoFeedback/plotchecks.py` & `AutoFeedback-1.4/AutoFeedback/plotchecks.py`

 * *Files 8% similar despite different names*

```diff
@@ -198,17 +198,17 @@
                                    axislabels=bool(explabels),
                                    legend=explegend)
         explegends = [line.label for line in explines
                       if line.label is not None]
         expline = explines[0]
         if not check_partial:
             if explines:
-                assert (len(lines) == len(explines)), "_datasets"
+                assert (len(lines) == len(explines)), _e_string("_datasets", "")
             if explegend:
-                assert (len(legends) == len(explegends)), "_legend"
+                assert (len(legends) == len(explegends)), _e_string("_legend", "")
 
         if (explines and not lines):
             assert (False), "_datasets"
 
         if (explines):
             lines = _reorder(explines, lines)
 
@@ -224,34 +224,35 @@
                                 ), _e_string("_marker", expline.label)
                     if expline.colour:
                         assert (_check_colour(line, expline.colour)
                                 ), _e_string("_colour", expline.label)
                     if expline.label and explegend:
                         if line.get_label()[0] != "_":
                             assert (_check_legend(line.get_label(),
-                                                  expline.label)), "_legend"
+                                                  expline.label)),\
+                                                  _e_string("_legend", expline.label)
                         else:
                             assert (_check_legend(legend, expline.label)),\
-                                "_legend"
+                                _e_string("_legend", expline.label)
                     if output:
                         print_error_message(
                             _e_string("_partial", expline.label), expline)
         if (exppatch):
             expline = exppatch
             assert (_check_patchdata(patch, exppatch)), _e_string("_data", "")
             if output:
                 print_error_message(_e_string("_partial", ""), exppatch)
         if not explines and not exppatch:
             assert (False), "_data"
         if explabels:
             if len(explabels) == 2:
                 explabels.append("")
-            assert (_check_axes(labels, explabels)), "_labels"
+            assert (_check_axes(labels, explabels)), _e_string("_labels", "")
         if expaxes:
-            assert (_check_axes(axes, expaxes)), "_axes"
+            assert (_check_axes(axes, expaxes)), _e_string("_axes", "")
         if output:
             print_error_message("_success", expline)
         return True
     except AssertionError as error:
         if output:
             print_error_message(error, expline)
         return False
```

### Comparing `AutoFeedback-1.3/AutoFeedback/plotclass.py` & `AutoFeedback-1.4/AutoFeedback/plotclass.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/AutoFeedback/randomclass.py` & `AutoFeedback-1.4/AutoFeedback/randomclass.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/AutoFeedback/varchecks.py` & `AutoFeedback-1.4/AutoFeedback/varchecks.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/AutoFeedback/variable_error_messages.py` & `AutoFeedback-1.4/AutoFeedback/variable_error_messages.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/AutoFeedback.egg-info/PKG-INFO` & `AutoFeedback-1.4/AutoFeedback.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoFeedback
-Version: 1.3
+Version: 1.4
 Summary: check basic python exercises with pretty feedback
 Home-page: https://github.com/abrown41/AutoFeedback
 Author: Andrew Brown
 Author-email: andrew.brown@qub.ac.uk
 License: BSD (3-clause)
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `AutoFeedback-1.3/AutoFeedback.egg-info/SOURCES.txt` & `AutoFeedback-1.4/AutoFeedback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/CONTRIBUTING.rst` & `AutoFeedback-1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/LICENSE` & `AutoFeedback-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/PKG-INFO` & `AutoFeedback-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoFeedback
-Version: 1.3
+Version: 1.4
 Summary: check basic python exercises with pretty feedback
 Home-page: https://github.com/abrown41/AutoFeedback
 Author: Andrew Brown
 Author-email: andrew.brown@qub.ac.uk
 License: BSD (3-clause)
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `AutoFeedback-1.3/README.rst` & `AutoFeedback-1.4/README.rst`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/docs/Makefile` & `AutoFeedback-1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/docs/make.bat` & `AutoFeedback-1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/docs/source/conf.py` & `AutoFeedback-1.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/docs/source/min_versions.rst` & `AutoFeedback-1.4/docs/source/min_versions.rst`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/docs/source/usage.rst` & `AutoFeedback-1.4/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/setup.py` & `AutoFeedback-1.4/setup.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/test/testerrors.py` & `AutoFeedback-1.4/test/testerrors.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 
 class PlotErrorTests(unittest.TestCase):
     def checkprint(self, estring, error_message, line=myline):
         """ estring is the string passed to print_error_message,
         error_message is the expected error message that is printed"""
         f = io.StringIO()
         with contextlib.redirect_stdout(f):
-            pr(estring, line)
+            pr(f"{estring}('googlyboo')", line)
         printed = f.getvalue()
         expected = colour_message(error_message)
         return printed == expected
 
     def test_plot_data(self):
         error_message = """Data set googlyboo is plotted with incorrect data.
     Check that all variables are correctly defined, and that you are plotting
```

### Comparing `AutoFeedback-1.3/test/testfuncs.py` & `AutoFeedback-1.4/test/testfuncs.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/test/testplot.py` & `AutoFeedback-1.4/test/testplot.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/test/testplotclass.py` & `AutoFeedback-1.4/test/testplotclass.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/test/testprint.py` & `AutoFeedback-1.4/test/testprint.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/test/testrandomclass.py` & `AutoFeedback-1.4/test/testrandomclass.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/test/testsymp.py` & `AutoFeedback-1.4/test/testsymp.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/test/testutils.py` & `AutoFeedback-1.4/test/testutils.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/test/testvars.py` & `AutoFeedback-1.4/test/testvars.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.3/versioneer.py` & `AutoFeedback-1.4/versioneer.py`

 * *Files identical despite different names*

