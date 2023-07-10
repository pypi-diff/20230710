# Comparing `tmp/egauge-python-0.7.3.tar.gz` & `tmp/egauge-python-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egauge-python-0.7.3.tar", last modified: Fri Apr 21 02:04:10 2023, max compression
+gzip compressed data, was "egauge-python-0.7.4.tar", last modified: Mon Jul 10 18:16:35 2023, max compression
```

## Comparing `egauge-python-0.7.3.tar` & `egauge-python-0.7.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.242138 egauge-python-0.7.3/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1090 2023-02-23 18:58:55.000000 egauge-python-0.7.3/LICENSE
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     2956 2023-04-21 02:04:10.242138 egauge-python-0.7.3/PKG-INFO
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     2301 2023-04-20 23:53:17.000000 egauge-python-0.7.3/README.md
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/ctid/
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       71 2022-05-10 19:26:55.000000 egauge-python-0.7.3/egauge/ctid/__init__.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     2234 2022-04-22 23:39:14.000000 egauge-python-0.7.3/egauge/ctid/bit_stuffer.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    29354 2022-05-14 04:25:32.000000 egauge-python-0.7.3/egauge/ctid/ctid.py
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)    12370 2022-05-14 04:25:14.000000 egauge-python-0.7.3/egauge/ctid/encoder.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     8791 2022-05-10 19:45:02.000000 egauge-python-0.7.3/egauge/ctid/waveform.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/pyside2/
--rw-r--r--   0 davidm    (1000) davidm    (1000)        0 2020-03-06 20:43:49.000000 egauge-python-0.7.3/egauge/pyside2/__init__.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     3643 2022-04-22 23:39:14.000000 egauge-python-0.7.3/egauge/pyside2/ansi2html.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    10640 2022-04-22 23:39:14.000000 egauge-python-0.7.3/egauge/pyside2/terminal.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/webapi/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1346 2020-07-16 19:02:13.000000 egauge-python-0.7.3/egauge/webapi/__init__.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     8335 2022-05-04 18:07:16.000000 egauge-python-0.7.3/egauge/webapi/auth.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/webapi/cloud/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1293 2020-03-12 14:56:16.000000 egauge-python-0.7.3/egauge/webapi/cloud/__init__.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4069 2022-05-04 18:28:54.000000 egauge-python-0.7.3/egauge/webapi/cloud/credentials.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/webapi/cloud/gui/
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     3950 2022-04-22 23:52:29.000000 egauge-python-0.7.3/egauge/webapi/cloud/gui/credentials_dialog.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     7561 2022-05-05 19:36:33.000000 egauge-python-0.7.3/egauge/webapi/cloud/serial_number.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/webapi/device/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1502 2022-09-19 21:16:17.000000 egauge-python-0.7.3/egauge/webapi/device/__init__.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    13955 2023-03-01 22:13:47.000000 egauge-python-0.7.3/egauge/webapi/device/capture.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    16279 2022-04-22 23:39:14.000000 egauge-python-0.7.3/egauge/webapi/device/ctid_info.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     7548 2023-04-21 02:01:09.000000 egauge-python-0.7.3/egauge/webapi/device/device.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     6603 2023-03-01 22:14:28.000000 egauge-python-0.7.3/egauge/webapi/device/local.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    12412 2022-09-20 20:05:39.000000 egauge-python-0.7.3/egauge/webapi/device/physical_quantity.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    14201 2022-09-20 18:48:03.000000 egauge-python-0.7.3/egauge/webapi/device/physical_units.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     9065 2022-09-19 15:49:48.000000 egauge-python-0.7.3/egauge/webapi/device/register.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     5356 2023-03-02 00:28:30.000000 egauge-python-0.7.3/egauge/webapi/device/register_row.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    30705 2023-02-23 21:18:54.000000 egauge-python-0.7.3/egauge/webapi/device/register_type.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     9308 2023-03-01 22:33:44.000000 egauge-python-0.7.3/egauge/webapi/device/virtual_register.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1405 2022-04-22 23:39:14.000000 egauge-python-0.7.3/egauge/webapi/error.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     9209 2023-04-20 23:53:17.000000 egauge-python-0.7.3/egauge/webapi/json_api.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge_python.egg-info/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     2956 2023-04-21 02:04:10.000000 egauge-python-0.7.3/egauge_python.egg-info/PKG-INFO
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1222 2023-04-21 02:04:10.000000 egauge-python-0.7.3/egauge_python.egg-info/SOURCES.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)        1 2023-04-21 02:04:10.000000 egauge-python-0.7.3/egauge_python.egg-info/dependency_links.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       59 2023-04-21 02:04:10.000000 egauge-python-0.7.3/egauge_python.egg-info/entry_points.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       94 2023-04-21 02:04:10.000000 egauge-python-0.7.3/egauge_python.egg-info/requires.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       21 2023-04-21 02:04:10.000000 egauge-python-0.7.3/egauge_python.egg-info/top_level.txt
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/examples/
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)     2224 2023-03-10 21:32:59.000000 egauge-python-0.7.3/examples/test_capture.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)      716 2023-03-02 01:05:11.000000 egauge-python-0.7.3/examples/test_common.py
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)     2236 2023-03-10 21:33:26.000000 egauge-python-0.7.3/examples/test_ctid.py
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)     4775 2023-03-10 20:47:54.000000 egauge-python-0.7.3/examples/test_local.py
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)     3214 2023-03-10 22:06:39.000000 egauge-python-0.7.3/examples/test_register.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       55 2022-05-11 01:22:07.000000 egauge-python-0.7.3/pyproject.toml
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       38 2023-04-21 02:04:10.242138 egauge-python-0.7.3/setup.cfg
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1440 2023-04-21 02:02:35.000000 egauge-python-0.7.3/setup.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 18:16:35.677543 egauge-python-0.7.4/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1090 2023-02-23 18:58:55.000000 egauge-python-0.7.4/LICENSE
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     2936 2023-07-10 18:16:35.677543 egauge-python-0.7.4/PKG-INFO
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     2301 2023-04-10 19:09:39.000000 egauge-python-0.7.4/README.md
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 18:16:35.501546 egauge-python-0.7.4/egauge/
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 18:16:35.541546 egauge-python-0.7.4/egauge/ctid/
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       71 2022-05-10 19:26:55.000000 egauge-python-0.7.4/egauge/ctid/__init__.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     2234 2022-04-22 23:39:14.000000 egauge-python-0.7.4/egauge/ctid/bit_stuffer.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    29206 2023-07-10 18:08:22.000000 egauge-python-0.7.4/egauge/ctid/ctid.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)    12370 2023-07-10 18:06:03.000000 egauge-python-0.7.4/egauge/ctid/encoder.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     8791 2022-05-10 19:45:02.000000 egauge-python-0.7.4/egauge/ctid/waveform.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 18:16:35.553546 egauge-python-0.7.4/egauge/pyside2/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)        0 2020-03-06 20:43:49.000000 egauge-python-0.7.4/egauge/pyside2/__init__.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     3643 2022-04-22 23:39:14.000000 egauge-python-0.7.4/egauge/pyside2/ansi2html.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    10640 2022-04-22 23:39:14.000000 egauge-python-0.7.4/egauge/pyside2/terminal.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 18:16:35.565545 egauge-python-0.7.4/egauge/webapi/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1346 2020-07-16 19:02:13.000000 egauge-python-0.7.4/egauge/webapi/__init__.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     8335 2022-05-04 18:07:16.000000 egauge-python-0.7.4/egauge/webapi/auth.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 18:16:35.577545 egauge-python-0.7.4/egauge/webapi/cloud/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1293 2020-03-12 14:56:16.000000 egauge-python-0.7.4/egauge/webapi/cloud/__init__.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4069 2022-05-04 18:28:54.000000 egauge-python-0.7.4/egauge/webapi/cloud/credentials.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 18:16:35.581545 egauge-python-0.7.4/egauge/webapi/cloud/gui/
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     3950 2022-04-22 23:52:29.000000 egauge-python-0.7.4/egauge/webapi/cloud/gui/credentials_dialog.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     7561 2022-05-05 19:36:33.000000 egauge-python-0.7.4/egauge/webapi/cloud/serial_number.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 18:16:35.629544 egauge-python-0.7.4/egauge/webapi/device/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1502 2022-09-19 21:16:17.000000 egauge-python-0.7.4/egauge/webapi/device/__init__.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    13955 2023-03-01 22:13:47.000000 egauge-python-0.7.4/egauge/webapi/device/capture.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    16279 2023-03-18 20:49:18.000000 egauge-python-0.7.4/egauge/webapi/device/ctid_info.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     7548 2023-05-25 18:24:12.000000 egauge-python-0.7.4/egauge/webapi/device/device.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     6603 2023-03-01 22:14:28.000000 egauge-python-0.7.4/egauge/webapi/device/local.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    12412 2022-09-20 20:05:39.000000 egauge-python-0.7.4/egauge/webapi/device/physical_quantity.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    14201 2022-09-20 18:48:03.000000 egauge-python-0.7.4/egauge/webapi/device/physical_units.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     9065 2022-09-19 15:49:48.000000 egauge-python-0.7.4/egauge/webapi/device/register.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     5356 2023-03-02 00:28:30.000000 egauge-python-0.7.4/egauge/webapi/device/register_row.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    30705 2023-06-05 15:20:41.000000 egauge-python-0.7.4/egauge/webapi/device/register_type.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     9308 2023-03-01 22:33:44.000000 egauge-python-0.7.4/egauge/webapi/device/virtual_register.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1405 2022-04-22 23:39:14.000000 egauge-python-0.7.4/egauge/webapi/error.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     9209 2023-04-10 18:59:44.000000 egauge-python-0.7.4/egauge/webapi/json_api.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 18:16:35.653544 egauge-python-0.7.4/egauge_python.egg-info/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     2936 2023-07-10 18:16:35.000000 egauge-python-0.7.4/egauge_python.egg-info/PKG-INFO
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1222 2023-07-10 18:16:35.000000 egauge-python-0.7.4/egauge_python.egg-info/SOURCES.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)        1 2023-07-10 18:16:35.000000 egauge-python-0.7.4/egauge_python.egg-info/dependency_links.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       58 2023-07-10 18:16:35.000000 egauge-python-0.7.4/egauge_python.egg-info/entry_points.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       94 2023-07-10 18:16:35.000000 egauge-python-0.7.4/egauge_python.egg-info/requires.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       21 2023-07-10 18:16:35.000000 egauge-python-0.7.4/egauge_python.egg-info/top_level.txt
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 18:16:35.673543 egauge-python-0.7.4/examples/
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)     2224 2023-03-10 21:32:59.000000 egauge-python-0.7.4/examples/test_capture.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)      716 2023-03-02 01:05:11.000000 egauge-python-0.7.4/examples/test_common.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)     2236 2023-03-10 21:33:26.000000 egauge-python-0.7.4/examples/test_ctid.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)     4775 2023-03-10 20:47:54.000000 egauge-python-0.7.4/examples/test_local.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)     3214 2023-03-10 22:06:39.000000 egauge-python-0.7.4/examples/test_register.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       55 2022-05-11 01:22:07.000000 egauge-python-0.7.4/pyproject.toml
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       38 2023-07-10 18:16:35.677543 egauge-python-0.7.4/setup.cfg
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     1440 2023-07-10 18:10:28.000000 egauge-python-0.7.4/setup.py
```

### Comparing `egauge-python-0.7.3/LICENSE` & `egauge-python-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/PKG-INFO` & `egauge-python-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: egauge-python
-Version: 0.7.3
+Version: 0.7.4
 Summary: .
 Home-page: https://bitbucket.org/egauge/python/
 Author: David Mosberger-Tang
 Author-email: davidm@egauge.net
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -83,9 +82,7 @@
 formatted data tables, you can make judicious use of ``# fmt: off`` and
 ``# fmt: on`` to disable formatting for the relevant lines.
 
 Source code should be syntax checked with pylint.  Pylint can be
 installed with ``pip install pylint``.  You can make judicious use
 of ``# pylint: disable=``\ *warning-name* to temporarily disable
 warnings that can safely be ignored.
-
-
```

### Comparing `egauge-python-0.7.3/README.md` & `egauge-python-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/ctid/bit_stuffer.py` & `egauge-python-0.7.4/egauge/ctid/bit_stuffer.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/ctid/ctid.py` & `egauge-python-0.7.4/egauge/ctid/ctid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2016-2017, 2019-2022 eGauge Systems LLC
+# Copyright (c) 2016-2017, 2019-2023 eGauge Systems LLC
 # 	1644 Conestoga St, Suite 2
 # 	Boulder, CO 80301
 # 	voice: 720-545-9767
 # 	email: davidm@egauge.net
 #
 #  All rights reserved.
 #
@@ -742,18 +742,15 @@
                     self.m_s8("cal_table", 0.02, "%", idx1=k, idx2=0)
                     self.m_s8("cal_table", 0.02, "°", idx1=k, idx2=1)
                 self.m_u8("reserved")
                 self.m_u8("mfg_info")
                 if self.version > 1:
                     self.m_f12_f12("r_source", "Ω", "r_load", "Ω")
 
-    # TODO: Default to version 4 for now.  Once eGauge firmware v4.1.3
-    # or later is widely in use, we can switch this back to
-    # version=CTID_VERSION.
-    def encode(self, version=4):
+    def encode(self, version=CTID_VERSION):
         """Encode the table contents and store is as a sequence of bytes in
         property ``raw_data''.
 
         """
         self.encoding = True
         self._raw_data = b""
         self._raw_offset = 0
```

### Comparing `egauge-python-0.7.3/egauge/ctid/encoder.py` & `egauge-python-0.7.4/egauge/ctid/encoder.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/ctid/waveform.py` & `egauge-python-0.7.4/egauge/ctid/waveform.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/pyside2/ansi2html.py` & `egauge-python-0.7.4/egauge/pyside2/ansi2html.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/pyside2/terminal.py` & `egauge-python-0.7.4/egauge/pyside2/terminal.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/__init__.py` & `egauge-python-0.7.4/egauge/webapi/__init__.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/auth.py` & `egauge-python-0.7.4/egauge/webapi/auth.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/cloud/__init__.py` & `egauge-python-0.7.4/egauge/webapi/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/cloud/credentials.py` & `egauge-python-0.7.4/egauge/webapi/cloud/credentials.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/cloud/gui/credentials_dialog.py` & `egauge-python-0.7.4/egauge/webapi/cloud/gui/credentials_dialog.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/cloud/serial_number.py` & `egauge-python-0.7.4/egauge/webapi/cloud/serial_number.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/device/__init__.py` & `egauge-python-0.7.4/egauge/webapi/device/__init__.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/device/capture.py` & `egauge-python-0.7.4/egauge/webapi/device/capture.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/device/ctid_info.py` & `egauge-python-0.7.4/egauge/webapi/device/ctid_info.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/device/device.py` & `egauge-python-0.7.4/egauge/webapi/device/device.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/device/local.py` & `egauge-python-0.7.4/egauge/webapi/device/local.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/device/physical_quantity.py` & `egauge-python-0.7.4/egauge/webapi/device/physical_quantity.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/device/physical_units.py` & `egauge-python-0.7.4/egauge/webapi/device/physical_units.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/device/register.py` & `egauge-python-0.7.4/egauge/webapi/device/register.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/device/register_row.py` & `egauge-python-0.7.4/egauge/webapi/device/register_row.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/device/register_type.py` & `egauge-python-0.7.4/egauge/webapi/device/register_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,32 +237,32 @@
     pus.add_scaled(p15, "EΩ", 1 / 1e+18, "exa")
     pus.add_scaled(p15, "ZΩ", 1 / 1e+21, "zetta")
     pus.add_scaled(p15, "YΩ", 1 / 1e+24, "yotta")
 
     p16 = PrimaryUnit("Ω·s")
     pus.add(p16)
 
-    p17 = PrimaryUnit("W/m^2", "Irradiance")
+    p17 = PrimaryUnit("W/m²", "Irradiance")
     pus.add(p17)
-    pus.add_scaled(p17, "yW/m^2", 1e+24, "yocto")
-    pus.add_scaled(p17, "zW/m^2", 1e+21, "zepto")
-    pus.add_scaled(p17, "aW/m^2", 1e+18, "atto")
-    pus.add_scaled(p17, "fW/m^2", 1000000000000000, "femto")
-    pus.add_scaled(p17, "pW/m^2", 1000000000000, "pico")
-    pus.add_scaled(p17, "nW/m^2", 1000000000, "nano")
-    pus.add_scaled(p17, "μW/m^2", 1000000, "micro")
-    pus.add_scaled(p17, "mW/m^2", 1000, "milli")
-    pus.add_scaled(p17, "kW/m^2", 1 / 1000, "kilo")
-    pus.add_scaled(p17, "MW/m^2", 1 / 1000000, "mega")
-    pus.add_scaled(p17, "GW/m^2", 1 / 1000000000, "giga")
-    pus.add_scaled(p17, "TW/m^2", 1 / 1000000000000, "tera")
-    pus.add_scaled(p17, "PW/m^2", 1 / 1000000000000000, "peta")
-    pus.add_scaled(p17, "EW/m^2", 1 / 1e+18, "exa")
-    pus.add_scaled(p17, "ZW/m^2", 1 / 1e+21, "zetta")
-    pus.add_scaled(p17, "YW/m^2", 1 / 1e+24, "yotta")
+    pus.add_scaled(p17, "yW/m²", 1e+24, "yocto")
+    pus.add_scaled(p17, "zW/m²", 1e+21, "zepto")
+    pus.add_scaled(p17, "aW/m²", 1e+18, "atto")
+    pus.add_scaled(p17, "fW/m²", 1000000000000000, "femto")
+    pus.add_scaled(p17, "pW/m²", 1000000000000, "pico")
+    pus.add_scaled(p17, "nW/m²", 1000000000, "nano")
+    pus.add_scaled(p17, "μW/m²", 1000000, "micro")
+    pus.add_scaled(p17, "mW/m²", 1000, "milli")
+    pus.add_scaled(p17, "kW/m²", 1 / 1000, "kilo")
+    pus.add_scaled(p17, "MW/m²", 1 / 1000000, "mega")
+    pus.add_scaled(p17, "GW/m²", 1 / 1000000000, "giga")
+    pus.add_scaled(p17, "TW/m²", 1 / 1000000000000, "tera")
+    pus.add_scaled(p17, "PW/m²", 1 / 1000000000000000, "peta")
+    pus.add_scaled(p17, "EW/m²", 1 / 1e+18, "exa")
+    pus.add_scaled(p17, "ZW/m²", 1 / 1e+21, "zetta")
+    pus.add_scaled(p17, "YW/m²", 1 / 1e+24, "yotta")
 
     p18 = PrimaryUnit("var", "Reactive Power")
     pus.add(p18)
     pus.add_scaled(p18, "yvar", 1e+24, "yocto")
     pus.add_scaled(p18, "zvar", 1e+21, "zepto")
     pus.add_scaled(p18, "avar", 1e+18, "atto")
     pus.add_scaled(p18, "fvar", 1000000000000000, "femto")
@@ -287,15 +287,15 @@
 
     p21 = PrimaryUnit("°", "Angle")
     pus.add(p21)
 
     p22 = PrimaryUnit("°·s")
     pus.add(p22)
 
-    p23 = PrimaryUnit("m^3/s", "Volumetric flow")
+    p23 = PrimaryUnit("m³/s", "Volumetric flow")
     pus.add(p23)
 
     p24 = PrimaryUnit("Pa", "Pressure")
     pus.add(p24)
 
     p25 = PrimaryUnit("Pa·s")
     pus.add(p25)
@@ -473,34 +473,34 @@
     c4 = PhysicalUnitConversion(False,
         lambda x, t=None: 0.000947817077749151*x,
         lambda x, t=None: 1055.0559*x
     )
     au = AlternateUnit("Btu", p34, c4)
     pus.add(au)
 
-    p35 = PrimaryUnit("W·s/m^2")
+    p35 = PrimaryUnit("W·s/m²")
     pus.add(p35)
-    au = AlternateUnit("Wh/m^2", p35, c2)
+    au = AlternateUnit("Wh/m²", p35, c2)
     pus.add(au)
-    pus.add_scaled(au, "yWh/m^2", 1e+24, "yocto")
-    pus.add_scaled(au, "zWh/m^2", 1e+21, "zepto")
-    pus.add_scaled(au, "aWh/m^2", 1e+18, "atto")
-    pus.add_scaled(au, "fWh/m^2", 1000000000000000, "femto")
-    pus.add_scaled(au, "pWh/m^2", 1000000000000, "pico")
-    pus.add_scaled(au, "nWh/m^2", 1000000000, "nano")
-    pus.add_scaled(au, "μWh/m^2", 1000000, "micro")
-    pus.add_scaled(au, "mWh/m^2", 1000, "milli")
-    pus.add_scaled(au, "kWh/m^2", 1 / 1000, "kilo")
-    pus.add_scaled(au, "MWh/m^2", 1 / 1000000, "mega")
-    pus.add_scaled(au, "GWh/m^2", 1 / 1000000000, "giga")
-    pus.add_scaled(au, "TWh/m^2", 1 / 1000000000000, "tera")
-    pus.add_scaled(au, "PWh/m^2", 1 / 1000000000000000, "peta")
-    pus.add_scaled(au, "EWh/m^2", 1 / 1e+18, "exa")
-    pus.add_scaled(au, "ZWh/m^2", 1 / 1e+21, "zetta")
-    pus.add_scaled(au, "YWh/m^2", 1 / 1e+24, "yotta")
+    pus.add_scaled(au, "yWh/m²", 1e+24, "yocto")
+    pus.add_scaled(au, "zWh/m²", 1e+21, "zepto")
+    pus.add_scaled(au, "aWh/m²", 1e+18, "atto")
+    pus.add_scaled(au, "fWh/m²", 1000000000000000, "femto")
+    pus.add_scaled(au, "pWh/m²", 1000000000000, "pico")
+    pus.add_scaled(au, "nWh/m²", 1000000000, "nano")
+    pus.add_scaled(au, "μWh/m²", 1000000, "micro")
+    pus.add_scaled(au, "mWh/m²", 1000, "milli")
+    pus.add_scaled(au, "kWh/m²", 1 / 1000, "kilo")
+    pus.add_scaled(au, "MWh/m²", 1 / 1000000, "mega")
+    pus.add_scaled(au, "GWh/m²", 1 / 1000000000, "giga")
+    pus.add_scaled(au, "TWh/m²", 1 / 1000000000000, "tera")
+    pus.add_scaled(au, "PWh/m²", 1 / 1000000000000000, "peta")
+    pus.add_scaled(au, "EWh/m²", 1 / 1e+18, "exa")
+    pus.add_scaled(au, "ZWh/m²", 1 / 1e+21, "zetta")
+    pus.add_scaled(au, "YWh/m²", 1 / 1e+24, "yotta")
 
     c18 = PhysicalUnitConversion(False,
         lambda x, t=None: 0.00220462*x,
         lambda x, t=None: 453.59290943564*x
     )
     au = AlternateUnit("lbs", p27, c18)
     pus.add(au)
@@ -568,15 +568,15 @@
     c14 = PhysicalUnitConversion(False,
         lambda x, t=None: 2.2369362920544*x,
         lambda x, t=None: 0.44704*x
     )
     au = AlternateUnit("mph", p11, c14)
     pus.add(au)
 
-    p36 = PrimaryUnit("m^3")
+    p36 = PrimaryUnit("m³")
     pus.add(p36)
 
     c20 = PhysicalUnitConversion(False,
         lambda x, t=None: 1000.0*x,
         lambda x, t=None: 0.001*x
     )
     au = AlternateUnit("L", p36, c20)
@@ -708,18 +708,18 @@
         self.inverse = inverse
 
 class Units:
 
     # Preferred units for METRIC and IMPERIAL systems:
     preferred = [
         ['kW', 'kWh', 'kVA', 'kVAh', 'kvar', 'kvahr', 'kg', 'kg/s',
-         'kWh/m^2', 'km/h', 'hPa', 'Ah', 'Vh', 'L/m', 'L', '°C',
+         'kWh/m²', 'km/h', 'hPa', 'Ah', 'Vh', 'L/m', 'L', '°C',
          '°C·d'],
         ['kW', 'kWh', 'kVA', 'kVAh', 'kvar', 'kvahr', 'lbs', 'lbs/s',
-         'kWh/m^2', 'mph', 'inHg', 'Ah', 'Vh', 'ft', '°F', '°F·d',
+         'kWh/m²', 'mph', 'inHg', 'Ah', 'Vh', 'ft', '°F', '°F·d',
          'lbs·s', 'inHg·s', 'ft·s', 'gpm', 'gal']
     ]
 
     table = {
         'P': UnitTableEntry(fix_scale=1, rate_unit='W',
                             cumul_scale=1 / 3600000, cumul_unit='kWh',
                             name='Power'),
@@ -749,30 +749,30 @@
                             name='Speed'),
         '#': UnitTableEntry(fix_scale=1, rate_unit='',
                             cumul_scale=1, cumul_unit='s',
                             name='Whole number'),
         'R': UnitTableEntry(fix_scale=1, rate_unit='Ω',
                             cumul_scale=1, cumul_unit='Ω·s',
                             name='Resistance'),
-        'Ee': UnitTableEntry(fix_scale=1, rate_unit='W/m^2',
-                             cumul_scale=1 / 3600000, cumul_unit='kWh/m^2',
+        'Ee': UnitTableEntry(fix_scale=1, rate_unit='W/m²',
+                             cumul_scale=1 / 3600000, cumul_unit='kWh/m²',
                              name='Irradiance'),
         'PQ': UnitTableEntry(fix_scale=1, rate_unit='var',
                              cumul_scale=1 / 3600000, cumul_unit='kvahr',
                              name='Reactive Power'),
         '$': UnitTableEntry(fix_scale=536870912, rate_unit='${currency}/s',
                             cumul_scale=1 / 536870912, cumul_unit='${currency}',
                             name='Monetary'),
         'a': UnitTableEntry(fix_scale=1000, rate_unit='°',
                             cumul_scale=1 / 1000, cumul_unit='°·s',
                             name='Angle'),
         'h': UnitTableEntry(fix_scale=1000, rate_unit='%',
                             cumul_scale=1 / 1000, cumul_unit='%·s',
                             name='Humidity'),
-        'Qv': UnitTableEntry(fix_scale=1000000000, rate_unit='m^3/s',
+        'Qv': UnitTableEntry(fix_scale=1000000000, rate_unit='m³/s',
                              cumul_scale=1 / 1000000, cumul_unit='L',
                              name='Volumetric flow'),
         'Pa': UnitTableEntry(fix_scale=1, rate_unit='Pa',
                              cumul_scale=1, cumul_unit='Pa·s',
                              name='Pressure'),
         'Qe': UnitTableEntry(fix_scale=1000, rate_unit='Ah',
                              cumul_scale=1 / 1000, cumul_unit='Ah·s',
```

### Comparing `egauge-python-0.7.3/egauge/webapi/device/virtual_register.py` & `egauge-python-0.7.4/egauge/webapi/device/virtual_register.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/error.py` & `egauge-python-0.7.4/egauge/webapi/error.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge/webapi/json_api.py` & `egauge-python-0.7.4/egauge/webapi/json_api.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/egauge_python.egg-info/PKG-INFO` & `egauge-python-0.7.4/egauge_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: egauge-python
-Version: 0.7.3
+Version: 0.7.4
 Summary: .
 Home-page: https://bitbucket.org/egauge/python/
 Author: David Mosberger-Tang
 Author-email: davidm@egauge.net
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -83,9 +82,7 @@
 formatted data tables, you can make judicious use of ``# fmt: off`` and
 ``# fmt: on`` to disable formatting for the relevant lines.
 
 Source code should be syntax checked with pylint.  Pylint can be
 installed with ``pip install pylint``.  You can make judicious use
 of ``# pylint: disable=``\ *warning-name* to temporarily disable
 warnings that can safely be ignored.
-
-
```

### Comparing `egauge-python-0.7.3/egauge_python.egg-info/SOURCES.txt` & `egauge-python-0.7.4/egauge_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/examples/test_capture.py` & `egauge-python-0.7.4/examples/test_capture.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/examples/test_common.py` & `egauge-python-0.7.4/examples/test_common.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/examples/test_ctid.py` & `egauge-python-0.7.4/examples/test_ctid.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/examples/test_local.py` & `egauge-python-0.7.4/examples/test_local.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/examples/test_register.py` & `egauge-python-0.7.4/examples/test_register.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.3/setup.py` & `egauge-python-0.7.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name="egauge-python",
-    version="0.7.3",
+    version="0.7.4",
     packages=setuptools.find_namespace_packages(include="egauge.*"),
     install_requires=[
         "crcmod",
         "deprecated",
         "intelhex",
         "wheel",
         "pexpect",
```

