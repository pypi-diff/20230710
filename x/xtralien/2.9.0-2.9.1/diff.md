# Comparing `tmp/xtralien-2.9.0.tar.gz` & `tmp/xtralien-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xtralien-2.9.0.tar", last modified: Fri Apr  7 08:52:54 2017, max compression
+gzip compressed data, was "dist/xtralien-2.9.1.tar", last modified: Fri Apr  7 09:41:31 2017, max compression
```

## Comparing `xtralien-2.9.0.tar` & `xtralien-2.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-07 08:52:54.000000 xtralien-2.9.0/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-07 08:52:54.000000 xtralien-2.9.0/xtralien/
--rw-r--r--   0 travis    (1000) travis    (1000)    12690 2017-04-07 08:52:41.000000 xtralien-2.9.0/xtralien/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)       49 2017-04-07 08:52:41.000000 xtralien-2.9.0/xtralien/__main__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      365 2017-04-07 08:52:41.000000 xtralien-2.9.0/xtralien/discover.py
--rw-r--r--   0 travis    (1000) travis    (1000)      336 2017-04-07 08:52:41.000000 xtralien-2.9.0/xtralien/experiment.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2779 2017-04-07 08:52:41.000000 xtralien-2.9.0/xtralien/imports.py
--rw-r--r--   0 travis    (1000) travis    (1000)      691 2017-04-07 08:52:41.000000 xtralien-2.9.0/xtralien/mixins.py
--rw-r--r--   0 travis    (1000) travis    (1000)      666 2017-04-07 08:52:41.000000 xtralien-2.9.0/xtralien/prompt.py
--rw-r--r--   0 travis    (1000) travis    (1000)      963 2017-04-07 08:52:41.000000 xtralien-2.9.0/xtralien/serial_utils.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1230 2017-04-07 08:52:41.000000 xtralien-2.9.0/xtralien/smartboard.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-07 08:52:54.000000 xtralien-2.9.0/xtralien.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     1380 2017-04-07 08:52:54.000000 xtralien-2.9.0/xtralien.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      359 2017-04-07 08:52:54.000000 xtralien-2.9.0/xtralien.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-04-07 08:52:54.000000 xtralien-2.9.0/xtralien.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       59 2017-04-07 08:52:54.000000 xtralien-2.9.0/xtralien.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        9 2017-04-07 08:52:54.000000 xtralien-2.9.0/xtralien.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      597 2017-04-07 08:52:41.000000 xtralien-2.9.0/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1380 2017-04-07 08:52:54.000000 xtralien-2.9.0/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)       59 2017-04-07 08:52:54.000000 xtralien-2.9.0/setup.cfg
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-07 09:41:31.000000 xtralien-2.9.1/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-07 09:41:31.000000 xtralien-2.9.1/xtralien/
+-rw-r--r--   0 travis    (1000) travis    (1000)    12655 2017-04-07 09:41:20.000000 xtralien-2.9.1/xtralien/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)       49 2017-04-07 09:41:20.000000 xtralien-2.9.1/xtralien/__main__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      365 2017-04-07 09:41:20.000000 xtralien-2.9.1/xtralien/discover.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      336 2017-04-07 09:41:20.000000 xtralien-2.9.1/xtralien/experiment.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2779 2017-04-07 09:41:20.000000 xtralien-2.9.1/xtralien/imports.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      691 2017-04-07 09:41:20.000000 xtralien-2.9.1/xtralien/mixins.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      666 2017-04-07 09:41:20.000000 xtralien-2.9.1/xtralien/prompt.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      963 2017-04-07 09:41:20.000000 xtralien-2.9.1/xtralien/serial_utils.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1230 2017-04-07 09:41:20.000000 xtralien-2.9.1/xtralien/smartboard.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-07 09:41:31.000000 xtralien-2.9.1/xtralien.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1380 2017-04-07 09:41:31.000000 xtralien-2.9.1/xtralien.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      359 2017-04-07 09:41:31.000000 xtralien-2.9.1/xtralien.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-04-07 09:41:31.000000 xtralien-2.9.1/xtralien.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       59 2017-04-07 09:41:31.000000 xtralien-2.9.1/xtralien.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        9 2017-04-07 09:41:31.000000 xtralien-2.9.1/xtralien.egg-info/top_level.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      597 2017-04-07 09:41:20.000000 xtralien-2.9.1/setup.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1380 2017-04-07 09:41:31.000000 xtralien-2.9.1/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)       59 2017-04-07 09:41:31.000000 xtralien-2.9.1/setup.cfg
```

### Comparing `xtralien-2.9.0/xtralien/__init__.py` & `xtralien-2.9.1/xtralien/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import logging
 import os
 import time
 import re
 import threading
 import random
 import datetime
+import sys
+import socket
 
 from xtralien.serial_utils import serial_ports
 
 log_levels = {
     'debug': logging.DEBUG,
     'info': logging.INFO,
     'warn': logging.WARNING,
@@ -28,29 +30,25 @@
 )
 
 try:
     import numpy
 except ImportError:
     logger.warn("Numpy not found, narray and nmatrix will fail")
 
-import sys
 
 if sys.version_info.major < 3:
     logger.warn("Module not supported on Python 2.x")
 
 # Try and import the serial module (supports USB-serial communication)
 try:
     import serial
 except ImportError:
     serial = None
     logger.warn("The serial module was not found, USB not supported")
 
-# Import useful BILs
-import socket
-
 
 def process_strip(x):
     return x.strip('\n[];')
 
 
 def process_array(x):
     data = [float(y) for y in x.strip('\n[];').split(';')]
@@ -66,14 +64,15 @@
         for y in x.strip('\n[];').split(';')
     ]
     try:
         return numpy.array(data)
     except NameError:
         return data
 
+
 number_regex = r"(\-|\+)?[0-9]+(\.[0-9]+)?(e-?[0-9]+(\.[0-9]+)?)?"
 re_matrix = re.compile(
     r'(\[({number},{number}(;?))+\])\n?'.format(number=number_regex)
 )
 re_array = re.compile(r'(\[({number}(;?))+\])\n?'.format(number=number_regex))
 re_number = re.compile(r'{number}\n?'.format(number=number_regex))
 
@@ -160,36 +159,37 @@
 
     def close(self):
         for conn in self.connections:
             conn.close()
 
     @property
     def serial(self):
-        _serial = int('0x' + self.cmd("serial", format=None), 16)
+        _serial = int('0x' + self("serial", format=None), 16)
         return {
             # 16 bits
             "board_number": (_serial & 0x00000000FFFF),
             # 6 bits
             "week": (_serial & 0x0000003F0000) >> 16,
             # 8 bits
             "year": (_serial & 0x00003FC00000) >> 22,
             # 8 bits
             "model": (_serial & 0x003FC0000000) >> 30,
             # 10 bits
             "product": (_serial & 0xFFC000000000) >> 38
         }
 
     @serial.setter
-    def setSerial(self, board, week=None, year=None, model=None, product=None):
+    def serial(self, serial_dict):
         # Set defaults
         dt = datetime.datetime.now()
-        week = week if week is not None else int(dt.strftime("%W"))
-        year = year if year is not None else int(dt.strftime("%Y"))
-        model = model if model is not None else 0
-        product = product if product is not None else 0
+        week = serial_dict.get("week", int(dt.strftime("%W")))
+        year = serial_dict.get("year", dt.year - 2000)
+        model = serial_dict.get('model', 0)
+        product = serial_dict.get('product', 0)
+        board = serial_dict.get('board_number', 0)
         # Create Serial
         _serial = 0x000000000000
         _serial |= board & 0xffff
         _serial |= (week & 0x3f) << 16
         _serial |= (year & 0xff) << 22
         _serial |= (model & 0xff) << 30
         _serial |= (product & 0x3ff) << 38
@@ -215,15 +215,17 @@
     def __call__(self, *args, **kwargs):
         sleep_time = kwargs.get("sleep_time", 0.001)
         self.current_selection += args
         returns = kwargs.get('response', True) or kwargs.get('callback', False)
         command = ' '.join([str(x) for x in self.current_selection])
         self.current_selection = []
 
-        formatter = lambda x: x
+        def formatter(x):
+            return x
+
         if returns:
             try:
                 formatter = self.formatters.get(
                     kwargs.get('format', 'auto'),
                     formatter
                 )
             except KeyError:
```

### Comparing `xtralien-2.9.0/xtralien/imports.py` & `xtralien-2.9.1/xtralien/imports.py`

 * *Files identical despite different names*

### Comparing `xtralien-2.9.0/xtralien/mixins.py` & `xtralien-2.9.1/xtralien/mixins.py`

 * *Files identical despite different names*

### Comparing `xtralien-2.9.0/xtralien/prompt.py` & `xtralien-2.9.1/xtralien/prompt.py`

 * *Files identical despite different names*

### Comparing `xtralien-2.9.0/xtralien/serial_utils.py` & `xtralien-2.9.1/xtralien/serial_utils.py`

 * *Files identical despite different names*

### Comparing `xtralien-2.9.0/xtralien/smartboard.py` & `xtralien-2.9.1/xtralien/smartboard.py`

 * *Files identical despite different names*

### Comparing `xtralien-2.9.0/xtralien.egg-info/PKG-INFO` & `xtralien-2.9.1/xtralien.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: xtralien
-Version: 2.9.0
+Version: 2.9.1
 Summary: A connector to implement connecting to CLOI-based instruments
 Home-page: https://github.com/xtralien/pyxtralien.git
 Author: Xtralien
 Author-email: jack@xtralien.com
 License: GPLv3
 Description: pyxtralien
         ======
```

### Comparing `xtralien-2.9.0/setup.py` & `xtralien-2.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open('README.md') as f:
         long_description = f.read()
 except:
     long_description = ''
 
 setup(
     name='xtralien',
-    version='2.9.0',
+    version='2.9.1',
     description='A connector to implement connecting to CLOI-based instruments',
     long_description=long_description,
     author='Xtralien',
     author_email='jack@xtralien.com',
     url='https://github.com/xtralien/pyxtralien.git',
     packages=['xtralien'],
     extras_require={
```

### Comparing `xtralien-2.9.0/PKG-INFO` & `xtralien-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: xtralien
-Version: 2.9.0
+Version: 2.9.1
 Summary: A connector to implement connecting to CLOI-based instruments
 Home-page: https://github.com/xtralien/pyxtralien.git
 Author: Xtralien
 Author-email: jack@xtralien.com
 License: GPLv3
 Description: pyxtralien
         ======
```

