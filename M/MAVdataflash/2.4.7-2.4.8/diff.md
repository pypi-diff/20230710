# Comparing `tmp/MAVdataflash-2.4.7.tar.gz` & `tmp/MAVdataflash-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MAVdataflash-2.4.7.tar", last modified: Mon Jul 10 09:59:10 2023, max compression
+gzip compressed data, was "MAVdataflash-2.4.8.tar", last modified: Mon Jul 10 12:03:03 2023, max compression
```

## Comparing `MAVdataflash-2.4.7.tar` & `MAVdataflash-2.4.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 09:59:10.894749 MAVdataflash-2.4.7/
--rw-rw-rw-   0        0        0    35823 2023-04-26 15:30:20.000000 MAVdataflash-2.4.7/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-10 09:59:10.880750 MAVdataflash-2.4.7/MAVdataflash/
--rw-rw-rw-   0        0        0     7032 2023-04-26 15:30:20.000000 MAVdataflash-2.4.7/MAVdataflash/DataFlashDict.py
--rw-rw-rw-   0        0        0     6887 2023-04-26 15:30:20.000000 MAVdataflash-2.4.7/MAVdataflash/MAVdataflash.py
--rw-rw-rw-   0        0        0       35 2023-04-26 15:30:20.000000 MAVdataflash-2.4.7/MAVdataflash/__init__.py
--rw-rw-rw-   0        0        0       21 2023-07-10 09:51:14.000000 MAVdataflash-2.4.7/MAVdataflash/__version__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:59:10.891749 MAVdataflash-2.4.7/MAVdataflash.egg-info/
--rw-rw-rw-   0        0        0     2954 2023-07-10 09:59:10.000000 MAVdataflash-2.4.7/MAVdataflash.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-07-10 09:59:10.000000 MAVdataflash-2.4.7/MAVdataflash.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 09:59:10.000000 MAVdataflash-2.4.7/MAVdataflash.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-10 09:59:10.000000 MAVdataflash-2.4.7/MAVdataflash.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-10 09:59:10.000000 MAVdataflash-2.4.7/MAVdataflash.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2954 2023-07-10 09:59:10.893749 MAVdataflash-2.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     2628 2023-04-26 15:30:20.000000 MAVdataflash-2.4.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 09:59:10.894749 MAVdataflash-2.4.7/setup.cfg
--rw-rw-rw-   0        0        0      681 2023-04-26 15:30:20.000000 MAVdataflash-2.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:03:03.149091 MAVdataflash-2.4.8/
+-rw-rw-rw-   0        0        0    35823 2023-04-26 15:30:20.000000 MAVdataflash-2.4.8/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-10 12:03:03.128092 MAVdataflash-2.4.8/MAVdataflash/
+-rw-rw-rw-   0        0        0     7032 2023-04-26 15:30:20.000000 MAVdataflash-2.4.8/MAVdataflash/DataFlashDict.py
+-rw-rw-rw-   0        0        0     6884 2023-07-10 12:00:13.000000 MAVdataflash-2.4.8/MAVdataflash/MAVdataflash.py
+-rw-rw-rw-   0        0        0       35 2023-04-26 15:30:20.000000 MAVdataflash-2.4.8/MAVdataflash/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-07-10 12:00:07.000000 MAVdataflash-2.4.8/MAVdataflash/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:03:03.145090 MAVdataflash-2.4.8/MAVdataflash.egg-info/
+-rw-rw-rw-   0        0        0     2954 2023-07-10 12:03:02.000000 MAVdataflash-2.4.8/MAVdataflash.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-07-10 12:03:02.000000 MAVdataflash-2.4.8/MAVdataflash.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 12:03:02.000000 MAVdataflash-2.4.8/MAVdataflash.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-10 12:03:02.000000 MAVdataflash-2.4.8/MAVdataflash.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-10 12:03:02.000000 MAVdataflash-2.4.8/MAVdataflash.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2954 2023-07-10 12:03:03.148091 MAVdataflash-2.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2628 2023-04-26 15:30:20.000000 MAVdataflash-2.4.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 12:03:03.149091 MAVdataflash-2.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      681 2023-04-26 15:30:20.000000 MAVdataflash-2.4.8/setup.py
```

### Comparing `MAVdataflash-2.4.7/LICENSE` & `MAVdataflash-2.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `MAVdataflash-2.4.7/MAVdataflash/DataFlashDict.py` & `MAVdataflash-2.4.8/MAVdataflash/DataFlashDict.py`

 * *Files identical despite different names*

### Comparing `MAVdataflash-2.4.7/MAVdataflash/MAVdataflash.py` & `MAVdataflash-2.4.8/MAVdataflash/MAVdataflash.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 if 'mavpackettype' in DFdict: del DFdict['mavpackettype']
                 DFdict = {'DateTime': datetime.datetime.fromtimestamp(DFmsg._timestamp), **DFdict}
                 # list append of DFmsg
                 DFlist.append(DFdict)
             if len(DFlist) != 0:
                 # updating dataframe from DF list
                 Data = pl.DataFrame(DFlist)
-                Data = Data.with_columns(pl.col("DateTime").dt.cast_time_unit(tu="ms"))
+                Data = Data.with_columns(pl.col("DateTime").dt.cast_time_unit("ms"))
                 self.DFdict[dtype] = pl.concat([self.DFdict[dtype], Data], how='diagonal')
             else: return None
     
     # Return column name of Instance.
     def _getInstance(self, dtype):
         column = self.GetColumns(dtype)
         if ('Instance' in column) or ('I' in column):
```

### Comparing `MAVdataflash-2.4.7/MAVdataflash.egg-info/PKG-INFO` & `MAVdataflash-2.4.8/MAVdataflash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MAVdataflash
-Version: 2.4.7
+Version: 2.4.8
 Summary: Read, analyze and visualize *.bin flight data logs recorded by ArduPilot
 Home-page: https://github.com/generalaeronautics/MAVdataflash
 Author: General Aeronautics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `MAVdataflash-2.4.7/PKG-INFO` & `MAVdataflash-2.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MAVdataflash
-Version: 2.4.7
+Version: 2.4.8
 Summary: Read, analyze and visualize *.bin flight data logs recorded by ArduPilot
 Home-page: https://github.com/generalaeronautics/MAVdataflash
 Author: General Aeronautics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `MAVdataflash-2.4.7/README.md` & `MAVdataflash-2.4.8/README.md`

 * *Files identical despite different names*

### Comparing `MAVdataflash-2.4.7/setup.py` & `MAVdataflash-2.4.8/setup.py`

 * *Files identical despite different names*

