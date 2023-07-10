# Comparing `tmp/bondzai.davinsy-py-0.0.4.tar.gz` & `tmp/bondzai.davinsy-py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.davinsy-py-0.0.4.tar", last modified: Tue Jul  4 09:33:29 2023, max compression
+gzip compressed data, was "bondzai.davinsy-py-0.0.5.tar", last modified: Mon Jul 10 17:59:10 2023, max compression
```

## Comparing `bondzai.davinsy-py-0.0.4.tar` & `bondzai.davinsy-py-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:29.964277 bondzai.davinsy-py-0.0.4/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      491 2023-07-04 09:33:29.964376 bondzai.davinsy-py-0.0.4/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)       72 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/README.md
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:29.958034 bondzai.davinsy-py-0.0.4/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:29.961634 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/
--rw-r--r--   0 theo       (501) staff       (20)       24 2023-07-04 09:33:20.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     3989 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/davinsy.py
--rw-r--r--   0 theo       (501) staff       (20)     6661 2023-07-04 09:33:20.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/enums.py
--rw-r--r--   0 theo       (501) staff       (20)      333 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/logger.py
--rw-r--r--   0 theo       (501) staff       (20)    21765 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/model.py
--rw-r--r--   0 theo       (501) staff       (20)    24433 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/operations.py
--rw-r--r--   0 theo       (501) staff       (20)     3342 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/preproc.py
--rw-r--r--   0 theo       (501) staff       (20)     1034 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/utils.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:29.964050 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      491 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      591 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)       26 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      700 2023-07-04 09:33:29.964990 bondzai.davinsy-py-0.0.4/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:10.537632 bondzai.davinsy-py-0.0.5/
+-rwxrwxrwx   0 root         (0) root         (0)      547 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/NOTICE
+-rwxrwxrwx   0 root         (0) root         (0)      491 2023-07-10 17:59:10.538632 bondzai.davinsy-py-0.0.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:09.990473 bondzai.davinsy-py-0.0.5/bondzai/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:10.324985 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/
+-rwxrwxrwx   0 root         (0) root         (0)       24 2023-07-10 17:58:59.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3989 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/davinsy.py
+-rwxrwxrwx   0 root         (0) root         (0)     6693 2023-07-10 17:58:59.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/enums.py
+-rwxrwxrwx   0 root         (0) root         (0)      333 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)    21765 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/model.py
+-rwxrwxrwx   0 root         (0) root         (0)    24433 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/operations.py
+-rwxrwxrwx   0 root         (0) root         (0)     3346 2023-07-10 17:58:59.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/preproc.py
+-rwxrwxrwx   0 root         (0) root         (0)     1034 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:10.513627 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      491 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      591 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/namespace_packages.txt
+-rwxrwxrwx   0 root         (0) root         (0)       26 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)      700 2023-07-10 17:59:10.543147 bondzai.davinsy-py-0.0.5/setup.cfg
```

### Comparing `bondzai.davinsy-py-0.0.4/NOTICE` & `bondzai.davinsy-py-0.0.5/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/davinsy.py` & `bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/davinsy.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/enums.py` & `bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,15 @@
     OP_PARAM_PWSPAN = 0x90001302
     OP_PARAM_COMPRESS = 0x90001402
     OP_PARAM_MATRIX = 0x90001403
     OP_PARAM_EMPTY = 0x90008000
     OP_PARAM_MODE = 0x90008001
     OP_PARAM_REMOVENFIRST = 0x90008003
     OP_PARAM_SHAPE = 0x90008005
+    OP_PARAM_SLICE = 0x90008006
 
 
 class KPITypes(Enum):
     KPI_FREE = 0
     KPI_TRAINING_TIME_START = 1
     KPI_TRAINING_TIME_STOP = 2
     KPI_TRAINING_DATASET_SIZE = 3
```

### Comparing `bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/model.py` & `bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/model.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/operations.py` & `bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/operations.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/preproc.py` & `bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/preproc.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             res1 = zeclass.from_buffer(res)
             logger.debug("PD %08x"%res1.data)
             data = (c_float * int(dim_out)).from_buffer(res[header_size:])
 
             # import numpy as np
             # print("VECTOR1DF32 data "+ np.array(data, dtype='float32'))
             datalist = [f for f in data]
-            logger.debug("VECTOR1DF32 data "+ str(datalist))
+            # logger.debug("VECTOR1DF32 data "+ str(datalist))
         elif PPParam(res1.typeid) == PPParam.OP_INOUT_VECT2D:
             res1 = VECTOR2DF32_factory(0).from_buffer(res)
             header_size = sizeof(res1)
             nb_it = res1.len[0]
             dim_out = res1.len[1]
             logger.debug("VECTOR2DF32 dim_out "+ str(dim_out) + " by nb_it "+str(nb_it))
             logger.debug("VECTOR1DF32 size "+ str(res1.size))
@@ -77,12 +77,12 @@
             data = (c_float * int(dim_out*nb_it)).from_buffer(res[header_size:])
             
             datalist = []
             for k in range(nb_it):
                 datalisttmp = [f for f in data[k*dim_out:(k+1)*dim_out]]
                 datalist.append(datalisttmp)
             # how to reshape ?
-            logger.debug("VECTOR2DF32 data "+ str(datalist))
+            # logger.debug("VECTOR2DF32 data "+ str(datalist))
         else:
             raise(Exception("Unknown signature output type"))
 
         return data
```

### Comparing `bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/utils.py` & `bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/SOURCES.txt` & `bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.4/setup.cfg` & `bondzai.davinsy-py-0.0.5/setup.cfg`

 * *Files identical despite different names*

