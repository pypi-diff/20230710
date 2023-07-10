# Comparing `tmp/CTid-programmer-1.4.1.tar.gz` & `tmp/CTid-programmer-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTid-programmer-1.4.1.tar", last modified: Thu Apr 27 20:37:16 2023, max compression
+gzip compressed data, was "CTid-programmer-1.4.2.tar", last modified: Mon Jul 10 21:39:52 2023, max compression
```

## Comparing `CTid-programmer-1.4.1.tar` & `CTid-programmer-1.4.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.335142 CTid-programmer-1.4.1/
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.255143 CTid-programmer-1.4.1/CTid_programmer.egg-info/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1413 2023-04-27 20:37:16.000000 CTid-programmer-1.4.1/CTid_programmer.egg-info/PKG-INFO
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1063 2023-04-27 20:37:16.000000 CTid-programmer-1.4.1/CTid_programmer.egg-info/SOURCES.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)        1 2023-04-27 20:37:16.000000 CTid-programmer-1.4.1/CTid_programmer.egg-info/dependency_links.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       69 2023-04-27 20:37:16.000000 CTid-programmer-1.4.1/CTid_programmer.egg-info/entry_points.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       54 2023-04-27 20:37:16.000000 CTid-programmer-1.4.1/CTid_programmer.egg-info/requires.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       16 2023-04-27 20:37:16.000000 CTid-programmer-1.4.1/CTid_programmer.egg-info/top_level.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1122 2020-03-07 04:32:39.000000 CTid-programmer-1.4.1/LICENSE
--rw-r--r--   0 davidm    (1000) davidm    (1000)      101 2020-03-07 04:32:39.000000 CTid-programmer-1.4.1/MANIFEST.in
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1413 2023-04-27 20:37:16.335142 CTid-programmer-1.4.1/PKG-INFO
--rw-rw-r--   0 davidm    (1000) davidm    (1000)      677 2020-10-07 01:16:20.000000 CTid-programmer-1.4.1/README.rst
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.283143 CTid-programmer-1.4.1/ctid_programmer/
--rw-r--r--   0 davidm    (1000) davidm    (1000)        0 2020-03-07 04:32:39.000000 CTid-programmer-1.4.1/ctid_programmer/__init__.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.319142 CTid-programmer-1.4.1/ctid_programmer/gui/
--rw-rw-r--   0 davidm    (1000) davidm    (1000)        0 2020-10-03 17:39:49.000000 CTid-programmer-1.4.1/ctid_programmer/gui/__init__.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.323142 CTid-programmer-1.4.1/ctid_programmer/gui/images/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     5957 2020-03-07 04:32:39.000000 CTid-programmer-1.4.1/ctid_programmer/gui/images/ctid-logo.svg
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    14163 2022-05-05 19:33:57.000000 CTid-programmer-1.4.1/ctid_programmer/gui/main_window.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     5128 2020-10-07 04:04:20.000000 CTid-programmer-1.4.1/ctid_programmer/gui/main_window_rc.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    14134 2022-05-13 18:49:59.000000 CTid-programmer-1.4.1/ctid_programmer/gui/param_ct.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4416 2021-04-26 21:41:35.000000 CTid-programmer-1.4.1/ctid_programmer/gui/param_linear.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     6693 2020-10-07 04:04:19.000000 CTid-programmer-1.4.1/ctid_programmer/gui/param_ntc.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4749 2020-10-07 04:04:20.000000 CTid-programmer-1.4.1/ctid_programmer/gui/param_pulse.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     3141 2020-10-07 04:04:20.000000 CTid-programmer-1.4.1/ctid_programmer/gui/param_temp.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4153 2020-10-07 04:04:19.000000 CTid-programmer-1.4.1/ctid_programmer/gui/param_volt.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     3619 2020-10-07 04:04:20.000000 CTid-programmer-1.4.1/ctid_programmer/gui/preferences_dialog.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     3796 2020-10-07 04:04:20.000000 CTid-programmer-1.4.1/ctid_programmer/gui/template_dialog.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     2140 2023-04-27 17:10:07.000000 CTid-programmer-1.4.1/ctid_programmer/preferences.py
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)    36022 2023-04-27 20:36:40.000000 CTid-programmer-1.4.1/ctid_programmer/programmer.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.323142 CTid-programmer-1.4.1/ctid_programmer/qt4/
--rw-rw-r--   0 davidm    (1000) davidm    (1000)        0 2020-10-03 17:37:26.000000 CTid-programmer-1.4.1/ctid_programmer/qt4/__init__.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.227144 CTid-programmer-1.4.1/ctid_programmer/resources/
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.331142 CTid-programmer-1.4.1/ctid_programmer/resources/code/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1249 2020-03-07 04:32:39.000000 CTid-programmer-1.4.1/ctid_programmer/resources/code/ac.hex
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1482 2022-05-05 14:42:37.000000 CTid-programmer-1.4.1/ctid_programmer/resources/code/powered.hex
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    15071 2023-04-27 17:10:08.000000 CTid-programmer-1.4.1/ctid_programmer/sensor_params.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4969 2023-04-27 17:10:07.000000 CTid-programmer-1.4.1/ctid_programmer/sn.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     7654 2023-04-27 17:10:07.000000 CTid-programmer-1.4.1/ctid_programmer/sn_egauge.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4075 2023-04-27 17:10:07.000000 CTid-programmer-1.4.1/ctid_programmer/sn_local.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     2410 2023-04-27 17:10:07.000000 CTid-programmer-1.4.1/ctid_programmer/template.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       55 2023-04-27 17:09:38.000000 CTid-programmer-1.4.1/pyproject.toml
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       38 2023-04-27 20:37:16.335142 CTid-programmer-1.4.1/setup.cfg
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1407 2023-04-27 20:35:22.000000 CTid-programmer-1.4.1/setup.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.245325 CTid-programmer-1.4.2/
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.157327 CTid-programmer-1.4.2/CTid_programmer.egg-info/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1393 2023-07-10 21:39:52.000000 CTid-programmer-1.4.2/CTid_programmer.egg-info/PKG-INFO
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1063 2023-07-10 21:39:52.000000 CTid-programmer-1.4.2/CTid_programmer.egg-info/SOURCES.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)        1 2023-07-10 21:39:52.000000 CTid-programmer-1.4.2/CTid_programmer.egg-info/dependency_links.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       68 2023-07-10 21:39:52.000000 CTid-programmer-1.4.2/CTid_programmer.egg-info/entry_points.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       54 2023-07-10 21:39:52.000000 CTid-programmer-1.4.2/CTid_programmer.egg-info/requires.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       16 2023-07-10 21:39:52.000000 CTid-programmer-1.4.2/CTid_programmer.egg-info/top_level.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1122 2020-03-07 04:32:39.000000 CTid-programmer-1.4.2/LICENSE
+-rw-r--r--   0 davidm    (1000) davidm    (1000)      101 2020-03-07 04:32:39.000000 CTid-programmer-1.4.2/MANIFEST.in
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     1393 2023-07-10 21:39:52.245325 CTid-programmer-1.4.2/PKG-INFO
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)      677 2020-10-07 01:16:20.000000 CTid-programmer-1.4.2/README.rst
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.185326 CTid-programmer-1.4.2/ctid_programmer/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)        0 2020-03-07 04:32:39.000000 CTid-programmer-1.4.2/ctid_programmer/__init__.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.225326 CTid-programmer-1.4.2/ctid_programmer/gui/
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)        0 2020-10-03 17:39:49.000000 CTid-programmer-1.4.2/ctid_programmer/gui/__init__.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.233326 CTid-programmer-1.4.2/ctid_programmer/gui/images/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     5957 2020-03-07 04:32:39.000000 CTid-programmer-1.4.2/ctid_programmer/gui/images/ctid-logo.svg
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    14163 2022-05-05 19:33:57.000000 CTid-programmer-1.4.2/ctid_programmer/gui/main_window.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     5128 2020-10-07 04:04:20.000000 CTid-programmer-1.4.2/ctid_programmer/gui/main_window_rc.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    14134 2023-07-10 17:59:24.000000 CTid-programmer-1.4.2/ctid_programmer/gui/param_ct.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4416 2021-04-26 21:41:35.000000 CTid-programmer-1.4.2/ctid_programmer/gui/param_linear.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     6693 2020-10-07 04:04:19.000000 CTid-programmer-1.4.2/ctid_programmer/gui/param_ntc.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4749 2020-10-07 04:04:20.000000 CTid-programmer-1.4.2/ctid_programmer/gui/param_pulse.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     3141 2020-10-07 04:04:20.000000 CTid-programmer-1.4.2/ctid_programmer/gui/param_temp.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4153 2020-10-07 04:04:19.000000 CTid-programmer-1.4.2/ctid_programmer/gui/param_volt.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     3619 2020-10-07 04:04:20.000000 CTid-programmer-1.4.2/ctid_programmer/gui/preferences_dialog.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     3796 2020-10-07 04:04:20.000000 CTid-programmer-1.4.2/ctid_programmer/gui/template_dialog.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     2140 2023-04-27 17:10:07.000000 CTid-programmer-1.4.2/ctid_programmer/preferences.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)    35995 2023-07-10 17:58:46.000000 CTid-programmer-1.4.2/ctid_programmer/programmer.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.233326 CTid-programmer-1.4.2/ctid_programmer/qt4/
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)        0 2020-10-03 17:37:26.000000 CTid-programmer-1.4.2/ctid_programmer/qt4/__init__.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.117327 CTid-programmer-1.4.2/ctid_programmer/resources/
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-07-10 21:39:52.241325 CTid-programmer-1.4.2/ctid_programmer/resources/code/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1249 2020-03-07 04:32:39.000000 CTid-programmer-1.4.2/ctid_programmer/resources/code/ac.hex
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     1482 2022-05-05 14:42:37.000000 CTid-programmer-1.4.2/ctid_programmer/resources/code/powered.hex
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    15071 2023-04-27 17:10:08.000000 CTid-programmer-1.4.2/ctid_programmer/sensor_params.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4969 2023-04-27 17:10:07.000000 CTid-programmer-1.4.2/ctid_programmer/sn.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     7654 2023-04-27 17:10:07.000000 CTid-programmer-1.4.2/ctid_programmer/sn_egauge.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4075 2023-04-27 17:10:07.000000 CTid-programmer-1.4.2/ctid_programmer/sn_local.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     2410 2023-04-27 17:10:07.000000 CTid-programmer-1.4.2/ctid_programmer/template.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       55 2023-04-27 17:09:38.000000 CTid-programmer-1.4.2/pyproject.toml
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       38 2023-07-10 21:39:52.245325 CTid-programmer-1.4.2/setup.cfg
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     1407 2023-07-10 18:19:50.000000 CTid-programmer-1.4.2/setup.py
```

### Comparing `CTid-programmer-1.4.1/CTid_programmer.egg-info/PKG-INFO` & `CTid-programmer-1.4.2/CTid_programmer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: CTid-programmer
-Version: 1.4.1
+Version: 1.4.2
 Summary: A graphical user interface for programming CTid sensors.
 Home-page: https://bitbucket.org/egauge/CTid-programmer/
 Author: David Mosberger-Tang
 Author-email: davidm@egauge.net
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -38,9 +37,7 @@
 The programmer uses an enhanced version avrdude which can be found here:
 
     https://bitbucket.org/egauge/avrdude/src/upstream/
 
 Apart from all the normal avrdude features, this version enables
 programming of ATtiny microcontrollers with a standard FTDI serial
 cable.
-
-
```

### Comparing `CTid-programmer-1.4.1/CTid_programmer.egg-info/SOURCES.txt` & `CTid-programmer-1.4.2/CTid_programmer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/LICENSE` & `CTid-programmer-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/PKG-INFO` & `CTid-programmer-1.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: CTid-programmer
-Version: 1.4.1
+Version: 1.4.2
 Summary: A graphical user interface for programming CTid sensors.
 Home-page: https://bitbucket.org/egauge/CTid-programmer/
 Author: David Mosberger-Tang
 Author-email: davidm@egauge.net
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -38,9 +37,7 @@
 The programmer uses an enhanced version avrdude which can be found here:
 
     https://bitbucket.org/egauge/avrdude/src/upstream/
 
 Apart from all the normal avrdude features, this version enables
 programming of ATtiny microcontrollers with a standard FTDI serial
 cable.
-
-
```

### Comparing `CTid-programmer-1.4.1/README.rst` & `CTid-programmer-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/gui/images/ctid-logo.svg` & `CTid-programmer-1.4.2/ctid_programmer/gui/images/ctid-logo.svg`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/gui/main_window.py` & `CTid-programmer-1.4.2/ctid_programmer/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/gui/main_window_rc.py` & `CTid-programmer-1.4.2/ctid_programmer/gui/main_window_rc.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/gui/param_ct.py` & `CTid-programmer-1.4.2/ctid_programmer/gui/param_ct.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,61 +141,61 @@
 
         self.params = QGridLayout()
         self.params.setObjectName(u"params")
         self.calp3 = QDoubleSpinBox(Param_CT)
         self.calp3.setObjectName(u"calp3")
         self.calp3.setMinimum(-5.120000000000000)
         self.calp3.setMaximum(5.110000000000000)
-        self.calp3.setSingleStep(0.020000000000000)
+        self.calp3.setSingleStep(0.010000000000000)
 
         self.params.addWidget(self.calp3, 3, 3, 1, 1)
 
         self.label_14 = QLabel(Param_CT)
         self.label_14.setObjectName(u"label_14")
         self.label_14.setFont(font)
         self.label_14.setAlignment(Qt.AlignRight|Qt.AlignTrailing|Qt.AlignVCenter)
 
         self.params.addWidget(self.label_14, 1, 1, 1, 1)
 
         self.calv3 = QDoubleSpinBox(Param_CT)
         self.calv3.setObjectName(u"calv3")
         self.calv3.setMinimum(-5.120000000000000)
         self.calv3.setMaximum(5.110000000000000)
-        self.calv3.setSingleStep(0.020000000000000)
+        self.calv3.setSingleStep(0.010000000000000)
 
         self.params.addWidget(self.calv3, 3, 2, 1, 1)
 
         self.label_17 = QLabel(Param_CT)
         self.label_17.setObjectName(u"label_17")
         self.label_17.setFont(font)
         self.label_17.setAlignment(Qt.AlignRight|Qt.AlignTrailing|Qt.AlignVCenter)
 
         self.params.addWidget(self.label_17, 4, 1, 1, 1)
 
         self.calv2 = QDoubleSpinBox(Param_CT)
         self.calv2.setObjectName(u"calv2")
         self.calv2.setMinimum(-5.120000000000000)
         self.calv2.setMaximum(5.110000000000000)
-        self.calv2.setSingleStep(0.020000000000000)
+        self.calv2.setSingleStep(0.010000000000000)
 
         self.params.addWidget(self.calv2, 2, 2, 1, 1)
 
         self.calv1 = QDoubleSpinBox(Param_CT)
         self.calv1.setObjectName(u"calv1")
         self.calv1.setMinimum(-5.120000000000000)
         self.calv1.setMaximum(5.110000000000000)
-        self.calv1.setSingleStep(0.020000000000000)
+        self.calv1.setSingleStep(0.010000000000000)
 
         self.params.addWidget(self.calv1, 1, 2, 1, 1)
 
         self.calp2 = QDoubleSpinBox(Param_CT)
         self.calp2.setObjectName(u"calp2")
         self.calp2.setMinimum(-5.120000000000000)
         self.calp2.setMaximum(5.110000000000000)
-        self.calp2.setSingleStep(0.020000000000000)
+        self.calp2.setSingleStep(0.010000000000000)
 
         self.params.addWidget(self.calp2, 2, 3, 1, 1)
 
         self.label_16 = QLabel(Param_CT)
         self.label_16.setObjectName(u"label_16")
         self.label_16.setFont(font)
         self.label_16.setAlignment(Qt.AlignRight|Qt.AlignTrailing|Qt.AlignVCenter)
@@ -209,38 +209,38 @@
 
         self.params.addWidget(self.label_15, 2, 1, 1, 1)
 
         self.calp4 = QDoubleSpinBox(Param_CT)
         self.calp4.setObjectName(u"calp4")
         self.calp4.setMinimum(-5.120000000000000)
         self.calp4.setMaximum(5.110000000000000)
-        self.calp4.setSingleStep(0.020000000000000)
+        self.calp4.setSingleStep(0.010000000000000)
 
         self.params.addWidget(self.calp4, 4, 3, 1, 1)
 
         self.label_20 = QLabel(Param_CT)
         self.label_20.setObjectName(u"label_20")
         self.label_20.setFont(font)
         self.label_20.setAlignment(Qt.AlignRight|Qt.AlignTrailing|Qt.AlignVCenter)
 
         self.params.addWidget(self.label_20, 0, 1, 1, 1)
 
         self.calp1 = QDoubleSpinBox(Param_CT)
         self.calp1.setObjectName(u"calp1")
         self.calp1.setMinimum(-5.120000000000000)
         self.calp1.setMaximum(5.110000000000000)
-        self.calp1.setSingleStep(0.020000000000000)
+        self.calp1.setSingleStep(0.010000000000000)
 
         self.params.addWidget(self.calp1, 1, 3, 1, 1)
 
         self.calv4 = QDoubleSpinBox(Param_CT)
         self.calv4.setObjectName(u"calv4")
         self.calv4.setMinimum(-5.120000000000000)
         self.calv4.setMaximum(5.110000000000000)
-        self.calv4.setSingleStep(0.020000000000000)
+        self.calv4.setSingleStep(0.010000000000000)
 
         self.params.addWidget(self.calv4, 4, 2, 1, 1)
 
         self.label_18 = QLabel(Param_CT)
         self.label_18.setObjectName(u"label_18")
         self.label_18.setFont(font)
```

### Comparing `CTid-programmer-1.4.1/ctid_programmer/gui/param_linear.py` & `CTid-programmer-1.4.2/ctid_programmer/gui/param_linear.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/gui/param_ntc.py` & `CTid-programmer-1.4.2/ctid_programmer/gui/param_ntc.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/gui/param_pulse.py` & `CTid-programmer-1.4.2/ctid_programmer/gui/param_pulse.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/gui/param_temp.py` & `CTid-programmer-1.4.2/ctid_programmer/gui/param_temp.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/gui/param_volt.py` & `CTid-programmer-1.4.2/ctid_programmer/gui/param_volt.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/gui/preferences_dialog.py` & `CTid-programmer-1.4.2/ctid_programmer/gui/preferences_dialog.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/gui/template_dialog.py` & `CTid-programmer-1.4.2/ctid_programmer/gui/template_dialog.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/preferences.py` & `CTid-programmer-1.4.2/ctid_programmer/preferences.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/programmer.py` & `CTid-programmer-1.4.2/ctid_programmer/programmer.py`

 * *Files 0% similar despite different names*

```diff
@@ -719,15 +719,14 @@
 
         # now that we have created the actual hexfile, it's safe to close
         # the original (empty) file created by mkstemp():
         os.close(output[0])
         return output[1]
 
     def detect_chip_type(self):
-        print('detecting')
         self.cmd_start(
             CMD_AVRDUDE + ["-pt9", "-nq"],
             [r"[dD]evice signature = 0x([0-9a-f]+)"],
         )
         chip_id = None
         for _, match in self.cmd:
             chip_id = int(match.group(1), base=16)
```

### Comparing `CTid-programmer-1.4.1/ctid_programmer/resources/code/ac.hex` & `CTid-programmer-1.4.2/ctid_programmer/resources/code/ac.hex`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/resources/code/powered.hex` & `CTid-programmer-1.4.2/ctid_programmer/resources/code/powered.hex`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/sensor_params.py` & `CTid-programmer-1.4.2/ctid_programmer/sensor_params.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/sn.py` & `CTid-programmer-1.4.2/ctid_programmer/sn.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/sn_egauge.py` & `CTid-programmer-1.4.2/ctid_programmer/sn_egauge.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/sn_local.py` & `CTid-programmer-1.4.2/ctid_programmer/sn_local.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/ctid_programmer/template.py` & `CTid-programmer-1.4.2/ctid_programmer/template.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.1/setup.py` & `CTid-programmer-1.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,20 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name='CTid-programmer',
-    version='1.4.1',
+    version='1.4.2',
     packages=setuptools.find_packages(),
     package_data={
         '': ['resources/code/*.hex']
     },
-    install_requires=['egauge-python>=0.7.2,!=0.21',
+    install_requires=['egauge-python>=0.7.3,!=0.21',
                       'importlib_resources', 'wheel'],
     entry_points={
         'console_scripts': [
             'CTid-programmer = ctid_programmer.programmer:main'
         ]
     },
     license='MIT License',  # example license
```

