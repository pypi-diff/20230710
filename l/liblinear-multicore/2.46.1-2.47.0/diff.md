# Comparing `tmp/liblinear-multicore-2.46.1.tar.gz` & `tmp/liblinear-multicore-2.47.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liblinear-multicore-2.46.1.tar", last modified: Sun Feb 26 06:45:44 2023, max compression
+gzip compressed data, was "liblinear-multicore-2.47.0.tar", last modified: Sun Jul  2 11:30:17 2023, max compression
```

## Comparing `liblinear-multicore-2.46.1.tar` & `liblinear-multicore-2.47.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-02-26 06:45:44.539519 liblinear-multicore-2.46.1/
--rw-rw-rw-   0        0        0     1517 2023-02-26 06:41:40.000000 liblinear-multicore-2.46.1/LICENSE
--rw-rw-rw-   0        0        0       48 2023-02-26 06:37:23.000000 liblinear-multicore-2.46.1/MANIFEST.in
--rw-rw-rw-   0        0        0    18212 2023-02-26 06:45:44.538523 liblinear-multicore-2.46.1/PKG-INFO
--rw-rw-rw-   0        0        0    17870 2023-02-26 06:37:23.000000 liblinear-multicore-2.46.1/README
-drwxrwxrwx   0        0        0        0 2023-02-26 06:45:44.490014 liblinear-multicore-2.46.1/cpp-source/
-drwxrwxrwx   0        0        0        0 2023-02-26 06:45:44.503975 liblinear-multicore-2.46.1/cpp-source/blas/
--rw-rw-rw-   0        0        0      727 2023-02-26 06:41:40.000000 liblinear-multicore-2.46.1/cpp-source/blas/blas.h
--rw-rw-rw-   0        0        0    16959 2023-02-26 06:41:40.000000 liblinear-multicore-2.46.1/cpp-source/blas/blasp.h
--rw-rw-rw-   0        0        0     1322 2023-02-26 06:41:40.000000 liblinear-multicore-2.46.1/cpp-source/blas/daxpy.c
--rw-rw-rw-   0        0        0     1329 2023-02-26 06:41:40.000000 liblinear-multicore-2.46.1/cpp-source/blas/ddot.c
--rw-rw-rw-   0        0        0     1427 2023-02-26 06:41:40.000000 liblinear-multicore-2.46.1/cpp-source/blas/dnrm2.c
--rw-rw-rw-   0        0        0     1144 2023-02-26 06:41:40.000000 liblinear-multicore-2.46.1/cpp-source/blas/dscal.c
--rw-rw-rw-   0        0        0    93589 2023-02-26 06:41:40.000000 liblinear-multicore-2.46.1/cpp-source/linear.cpp
--rw-rw-rw-   0        0        0      526 2023-02-26 06:41:40.000000 liblinear-multicore-2.46.1/cpp-source/linear.def
--rw-rw-rw-   0        0        0     2805 2023-02-26 06:41:40.000000 liblinear-multicore-2.46.1/cpp-source/linear.h
--rw-rw-rw-   0        0        0     5414 2023-02-26 06:41:40.000000 liblinear-multicore-2.46.1/cpp-source/newton.cpp
--rw-rw-rw-   0        0        0      925 2023-02-26 06:41:40.000000 liblinear-multicore-2.46.1/cpp-source/newton.h
-drwxrwxrwx   0        0        0        0 2023-02-26 06:45:44.512951 liblinear-multicore-2.46.1/liblinear/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:37:23.000000 liblinear-multicore-2.46.1/liblinear/__init__.py
--rw-rw-rw-   0        0        0     6384 2023-02-26 06:37:23.000000 liblinear-multicore-2.46.1/liblinear/commonutil.py
--rw-rw-rw-   0        0        0    18120 2023-02-26 06:37:23.000000 liblinear-multicore-2.46.1/liblinear/liblinear.py
--rw-rw-rw-   0        0        0    11678 2023-02-26 06:37:23.000000 liblinear-multicore-2.46.1/liblinear/liblinearutil.py
-drwxrwxrwx   0        0        0        0 2023-02-26 06:45:44.536527 liblinear-multicore-2.46.1/liblinear_multicore.egg-info/
--rw-rw-rw-   0        0        0    18212 2023-02-26 06:45:43.000000 liblinear-multicore-2.46.1/liblinear_multicore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-02-26 06:45:44.000000 liblinear-multicore-2.46.1/liblinear_multicore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-26 06:45:43.000000 liblinear-multicore-2.46.1/liblinear_multicore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-02-26 06:45:43.000000 liblinear-multicore-2.46.1/liblinear_multicore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-26 06:45:43.000000 liblinear-multicore-2.46.1/liblinear_multicore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-26 06:45:44.540524 liblinear-multicore-2.46.1/setup.cfg
--rw-rw-rw-   0        0        0     3841 2023-02-26 06:37:23.000000 liblinear-multicore-2.46.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:30:17.655479 liblinear-multicore-2.47.0/
+-rw-rw-rw-   0        0        0     1517 2023-07-02 11:30:16.000000 liblinear-multicore-2.47.0/LICENSE
+-rw-rw-rw-   0        0        0       48 2023-07-01 06:01:07.000000 liblinear-multicore-2.47.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    18212 2023-07-02 11:30:17.653442 liblinear-multicore-2.47.0/PKG-INFO
+-rw-rw-rw-   0        0        0    17870 2023-07-01 06:01:22.000000 liblinear-multicore-2.47.0/README
+drwxrwxrwx   0        0        0        0 2023-07-02 11:30:17.507622 liblinear-multicore-2.47.0/cpp-source/
+drwxrwxrwx   0        0        0        0 2023-07-02 11:30:17.544957 liblinear-multicore-2.47.0/cpp-source/blas/
+-rw-rw-rw-   0        0        0      727 2023-07-02 11:30:16.000000 liblinear-multicore-2.47.0/cpp-source/blas/blas.h
+-rw-rw-rw-   0        0        0    16959 2023-07-02 11:30:16.000000 liblinear-multicore-2.47.0/cpp-source/blas/blasp.h
+-rw-rw-rw-   0        0        0     1322 2023-07-02 11:30:16.000000 liblinear-multicore-2.47.0/cpp-source/blas/daxpy.c
+-rw-rw-rw-   0        0        0     1329 2023-07-02 11:30:16.000000 liblinear-multicore-2.47.0/cpp-source/blas/ddot.c
+-rw-rw-rw-   0        0        0     1427 2023-07-02 11:30:16.000000 liblinear-multicore-2.47.0/cpp-source/blas/dnrm2.c
+-rw-rw-rw-   0        0        0     1144 2023-07-02 11:30:16.000000 liblinear-multicore-2.47.0/cpp-source/blas/dscal.c
+-rw-rw-rw-   0        0        0    93589 2023-07-02 11:30:16.000000 liblinear-multicore-2.47.0/cpp-source/linear.cpp
+-rw-rw-rw-   0        0        0      526 2023-07-02 11:30:16.000000 liblinear-multicore-2.47.0/cpp-source/linear.def
+-rw-rw-rw-   0        0        0     2805 2023-07-02 11:30:16.000000 liblinear-multicore-2.47.0/cpp-source/linear.h
+-rw-rw-rw-   0        0        0     5414 2023-07-02 11:30:16.000000 liblinear-multicore-2.47.0/cpp-source/newton.cpp
+-rw-rw-rw-   0        0        0      925 2023-07-02 11:30:16.000000 liblinear-multicore-2.47.0/cpp-source/newton.h
+drwxrwxrwx   0        0        0        0 2023-07-02 11:30:17.579976 liblinear-multicore-2.47.0/liblinear/
+-rw-rw-rw-   0        0        0        0 2023-07-01 06:01:07.000000 liblinear-multicore-2.47.0/liblinear/__init__.py
+-rw-rw-rw-   0        0        0     6384 2023-07-01 06:01:07.000000 liblinear-multicore-2.47.0/liblinear/commonutil.py
+-rw-rw-rw-   0        0        0    18328 2023-07-01 06:01:32.000000 liblinear-multicore-2.47.0/liblinear/liblinear.py
+-rw-rw-rw-   0        0        0    11678 2023-07-01 06:01:22.000000 liblinear-multicore-2.47.0/liblinear/liblinearutil.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:30:17.649587 liblinear-multicore-2.47.0/liblinear_multicore.egg-info/
+-rw-rw-rw-   0        0        0    18212 2023-07-02 11:30:17.000000 liblinear-multicore-2.47.0/liblinear_multicore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-07-02 11:30:17.000000 liblinear-multicore-2.47.0/liblinear_multicore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 11:30:17.000000 liblinear-multicore-2.47.0/liblinear_multicore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 11:30:17.000000 liblinear-multicore-2.47.0/liblinear_multicore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-02 11:30:17.000000 liblinear-multicore-2.47.0/liblinear_multicore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 11:30:17.655479 liblinear-multicore-2.47.0/setup.cfg
+-rw-rw-rw-   0        0        0     3841 2023-07-01 06:25:03.000000 liblinear-multicore-2.47.0/setup.py
```

### Comparing `liblinear-multicore-2.46.1/LICENSE` & `liblinear-multicore-2.47.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/PKG-INFO` & `liblinear-multicore-2.47.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liblinear-multicore
-Version: 2.46.1
+Version: 2.47.0
 Summary: Python binding of multi-core LIBLINEAR
 Home-page: https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/multicore-liblinear
 Author: ML group @ National Taiwan University
 Author-email: cjlin@csie.ntu.edu.tw
 Description-Content-Type: text/plain
 License-File: LICENSE
```

### Comparing `liblinear-multicore-2.46.1/README` & `liblinear-multicore-2.47.0/README`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/cpp-source/blas/blas.h` & `liblinear-multicore-2.47.0/cpp-source/blas/blas.h`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/cpp-source/blas/blasp.h` & `liblinear-multicore-2.47.0/cpp-source/blas/blasp.h`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/cpp-source/blas/daxpy.c` & `liblinear-multicore-2.47.0/cpp-source/blas/daxpy.c`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/cpp-source/blas/ddot.c` & `liblinear-multicore-2.47.0/cpp-source/blas/ddot.c`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/cpp-source/blas/dnrm2.c` & `liblinear-multicore-2.47.0/cpp-source/blas/dnrm2.c`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/cpp-source/blas/dscal.c` & `liblinear-multicore-2.47.0/cpp-source/blas/dscal.c`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/cpp-source/linear.cpp` & `liblinear-multicore-2.47.0/cpp-source/linear.cpp`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/cpp-source/linear.def` & `liblinear-multicore-2.47.0/cpp-source/linear.def`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/cpp-source/linear.h` & `liblinear-multicore-2.47.0/cpp-source/linear.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef _LIBLINEAR_H
 #define _LIBLINEAR_H
 
-#define LIBLINEAR_VERSION 246
+#define LIBLINEAR_VERSION 247
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 extern int liblinear_version;
```

### Comparing `liblinear-multicore-2.46.1/cpp-source/newton.cpp` & `liblinear-multicore-2.47.0/cpp-source/newton.cpp`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/cpp-source/newton.h` & `liblinear-multicore-2.47.0/cpp-source/newton.h`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/liblinear/commonutil.py` & `liblinear-multicore-2.47.0/liblinear/commonutil.py`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/liblinear/liblinear.py` & `liblinear-multicore-2.47.0/liblinear/liblinear.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,17 @@
         prob_slice = slice(prob_rowptr[i], prob_rowptr[i+1]-2)
         prob_ind[prob_slice] = x_ind[x_slice]+1
         prob_val[prob_slice] = x_val[x_slice]
 
 def csr_to_problem(x, prob):
     # Extra space for termination node and (possibly) bias term
     x_space = prob.x_space = np.empty((x.nnz+x.shape[0]*2), dtype=feature_node)
-    prob.rowptr = x.indptr.copy()
+    # rowptr has to be a 64bit integer because it will later be used for pointer arithmetic,
+    # which overflows when the added pointer points to an address that is numerically high.
+    prob.rowptr = x.indptr.astype(np.int64, copy=True)
     prob.rowptr[1:] += 2*np.arange(1,x.shape[0]+1)
     prob_ind = x_space["index"]
     prob_val = x_space["value"]
     prob_ind[:] = -1
     if jit_enabled:
         csr_to_problem_jit(x.shape[0], x.data, x.indices, x.indptr, prob_val, prob_ind, prob.rowptr)
     else:
```

### Comparing `liblinear-multicore-2.46.1/liblinear/liblinearutil.py` & `liblinear-multicore-2.47.0/liblinear/liblinearutil.py`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/liblinear_multicore.egg-info/PKG-INFO` & `liblinear-multicore-2.47.0/liblinear_multicore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liblinear-multicore
-Version: 2.46.1
+Version: 2.47.0
 Summary: Python binding of multi-core LIBLINEAR
 Home-page: https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/multicore-liblinear
 Author: ML group @ National Taiwan University
 Author-email: cjlin@csie.ntu.edu.tw
 Description-Content-Type: text/plain
 License-File: LICENSE
```

### Comparing `liblinear-multicore-2.46.1/liblinear_multicore.egg-info/SOURCES.txt` & `liblinear-multicore-2.47.0/liblinear_multicore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liblinear-multicore-2.46.1/setup.py` & `liblinear-multicore-2.47.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from distutils.command.build_ext import build_ext
 
 build_ext.get_export_symbols = lambda x, y: []
 
 
 PACKAGE_DIR = "liblinear"
 PACKAGE_NAME = "liblinear-multicore"
-VERSION = "2.46.1"
+VERSION = "2.47.0"
 cpp_dir = "cpp-source"
 # should be consistent with dynamic_lib_name in liblinear/liblinear.py
 dynamic_lib_name = "clib"
 
 # sources to be included to build the shared library
 source_codes = [
     path.join("blas", "daxpy.c"),
```

