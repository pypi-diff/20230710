# Comparing `tmp/micropython-icm20948-0.2.1.tar.gz` & `tmp/micropython-icm20948-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-icm20948-0.2.1.tar", last modified: Sat Jun 17 15:13:32 2023, max compression
+gzip compressed data, was "micropython-icm20948-0.2.2.tar", last modified: Mon Jul 10 12:50:00 2023, max compression
```

## Comparing `micropython-icm20948-0.2.1.tar` & `micropython-icm20948-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.918759 micropython-icm20948-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.918759 micropython-icm20948-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-17 15:13:25.000000 micropython-icm20948-0.2.1/examples/icm20948_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/micropython_icm20948/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:25.000000 micropython-icm20948-0.2.1/micropython_icm20948/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:13:25.000000 micropython-icm20948-0.2.1/micropython_icm20948/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23487 2023-06-17 15:13:25.000000 micropython-icm20948-0.2.1/micropython_icm20948/icm20948.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/micropython_icm20948.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-17 15:13:32.000000 micropython-icm20948-0.2.1/micropython_icm20948.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-17 15:13:32.000000 micropython-icm20948-0.2.1/micropython_icm20948.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:13:32.000000 micropython-icm20948-0.2.1/micropython_icm20948.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:13:32.000000 micropython-icm20948-0.2.1/micropython_icm20948.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-17 15:13:32.000000 micropython-icm20948-0.2.1/micropython_icm20948.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-17 15:13:25.000000 micropython-icm20948-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:50:00.123845 micropython-icm20948-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:50:00.119845 micropython-icm20948-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:50:00.119845 micropython-icm20948-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-10 12:50:00.123845 micropython-icm20948-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:50:00.119845 micropython-icm20948-0.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:50:00.119845 micropython-icm20948-0.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:50:00.119845 micropython-icm20948-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-10 12:49:52.000000 micropython-icm20948-0.2.2/examples/icm20948_acc_dlpf_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-10 12:49:52.000000 micropython-icm20948-0.2.2/examples/icm20948_accelerometer_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-10 12:49:52.000000 micropython-icm20948-0.2.2/examples/icm20948_clock_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-10 12:49:52.000000 micropython-icm20948-0.2.2/examples/icm20948_gyro_dlpf_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-10 12:49:52.000000 micropython-icm20948-0.2.2/examples/icm20948_gyro_full_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-10 12:49:52.000000 micropython-icm20948-0.2.2/examples/icm20948_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-10 12:49:52.000000 micropython-icm20948-0.2.2/examples/icm20948_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:50:00.123845 micropython-icm20948-0.2.2/micropython_icm20948/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 12:49:52.000000 micropython-icm20948-0.2.2/micropython_icm20948/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-10 12:49:52.000000 micropython-icm20948-0.2.2/micropython_icm20948/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26553 2023-07-10 12:49:52.000000 micropython-icm20948-0.2.2/micropython_icm20948/icm20948.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:50:00.123845 micropython-icm20948-0.2.2/micropython_icm20948.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-10 12:50:00.000000 micropython-icm20948-0.2.2/micropython_icm20948.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-10 12:50:00.000000 micropython-icm20948-0.2.2/micropython_icm20948.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:50:00.000000 micropython-icm20948-0.2.2/micropython_icm20948.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-10 12:50:00.000000 micropython-icm20948-0.2.2/micropython_icm20948.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-10 12:49:52.000000 micropython-icm20948-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 12:49:44.000000 micropython-icm20948-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 12:50:00.123845 micropython-icm20948-0.2.2/setup.cfg
```

### Comparing `micropython-icm20948-0.2.1/.gitignore` & `micropython-icm20948-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.1/.pre-commit-config.yaml` & `micropython-icm20948-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.1/LICENSE` & `micropython-icm20948-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.1/PKG-INFO` & `micropython-icm20948-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-icm20948
-Version: 0.2.1
+Version: 0.2.2
 Summary: MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor
 Author-email: "Jose D. Montoya" <icm20948@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ICM20948
 Keywords: micropython,icm20948,gyro,accelerometer,acceleration,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-icm20948-0.2.1/README.rst` & `micropython-icm20948-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.1/docs/_static/Logo.png` & `micropython-icm20948-0.2.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.1/docs/_static/favicon.ico` & `micropython-icm20948-0.2.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.1/docs/conf.py` & `micropython-icm20948-0.2.2/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,40 @@
-# -*- coding: utf-8 -*-
-
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
 import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
+try:
+    # Inject mock modules so that we can build the
+    # documentation without having the real stuff available
+    from mock import Mock
+
+    to_be_mocked = [
+        "micropython",
+        "machine",
+    ]
+    for module in to_be_mocked:
+        sys.modules[module] = Mock()
+        print("Mocked '{}' module".format(module))
+
+    import micropython_icm20948
+except ImportError:
+    raise SystemExit("micropython_icm20948 has to be importable")
+
 # -- General configuration ------------------------------------------------
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
-    "sphinx.ext.todo",
     "sphinx.ext.viewcode",
     "sphinx_immaterial",
 ]
 
 autodoc_preserve_defaults = True
 
 intersphinx_mapping = {
```

### Comparing `micropython-icm20948-0.2.1/micropython_icm20948/i2c_helpers.py` & `micropython-icm20948-0.2.2/micropython_icm20948/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.1/micropython_icm20948/icm20948.py` & `micropython-icm20948-0.2.2/micropython_icm20948/icm20948.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,26 @@
 
 **Software and Dependencies:**
 
 This library depends on Micropython
 
 """
 
-# pylint: disable=too-many-arguments, line-too-long, too-many-instance-attributes
+# pylint: disable=line-too-long
 
 from time import sleep
 from micropython import const
 from micropython_icm20948.i2c_helpers import CBits, RegisterStruct
 
-__version__ = "0.2.1"
+try:
+    from typing import Tuple
+except ImportError:
+    pass
+
+__version__ = "0.2.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_ICM20948.git"
 
 _REG_WHOAMI = const(0x69)
 _DEVICE_ID = const(0x00)
 
 _PWR_MGMT_1 = const(0x06)
 _PWR_MGMT_2 = const(0x07)
@@ -43,43 +48,39 @@
 _GYRO_XOUT_H = const(0x33)  # first byte of accel data
 _TEMP_OUT = const(0x3A)
 
 # ICM20948
 CLK_SELECT_INTERNAL = const(0b000)
 CLK_SELECT_BEST = const(0b001)
 CLK_SELECT_STOP = const(0b111)
-# End
 clk_values = (CLK_SELECT_INTERNAL, CLK_SELECT_BEST, CLK_SELECT_STOP)
 
 # ICM20948
 ACC_DISABLED = const(0b111)
 GYRO_DISABLED = const(0b111)
 ACC_ENABLED = const(0b000)
 GYRO_ENABLED = const(0b000)
 TEMP_ENABLED = const(0b0)
 TEMP_DISABLED = const(0b1)
-# End
 gyro_en_values = (GYRO_DISABLED, GYRO_ENABLED)
 acc_en_values = (ACC_DISABLED, ACC_ENABLED)
 temperature_en_values = (TEMP_DISABLED, TEMP_ENABLED)
 
 # ICM20948 USer Bank
 USER_BANK_0 = const(0)
 USER_BANK_1 = const(1)
 USER_BANK_2 = const(2)
 USER_BANK_3 = const(3)
-# End
 user_bank_values = (USER_BANK_0, USER_BANK_1, USER_BANK_2, USER_BANK_3)
 
-# User Bank ICM20948
+# ACC Range ICM20948
 RANGE_2G = const(0b00)
 RANGE_4G = const(0b01)
 RANGE_8G = const(0b10)
 RANGE_16G = const(0b11)
-
 acc_range_values = (RANGE_2G, RANGE_4G, RANGE_8G, RANGE_16G)
 acc_range_sensitivity = (16384, 8192, 4096, 2048)
 
 # Acceleration Rate Divisor Values
 acc_rate_values = {
     140.6: 7,
     102.3: 10,
@@ -214,15 +215,15 @@
         from machine import Pin, I2C
         import micropython_icm20948.icm20948 as icm20948
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin(8), scl=Pin(9))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         icm = icm20948.ICM20948(i2c)
 
     Now you have access to the :attr:`acceleration` attribute and :attr:`gyro` attribute
 
     .. code-block:: python
 
         accx, accy, accz = icm.accelerometer
@@ -267,15 +268,15 @@
 
     # _GYRO_CONFIG_1 (0x01)
     # |----|----|GYRO_DLPFCFG(2)|GYRO_DLPFCFG(1)|GYRO_DLPFCFG(0)|GYRO_FS_SEL[(1)|GYRO_FS_SEL[(0)|GYRO_FCHOICE|
     _gyro_choice = CBits(0, _GYRO_CONFIG_1, 0)
     _gyro_full_scale = CBits(2, _GYRO_CONFIG_1, 1)
     _gyro_dplcfg = CBits(3, _GYRO_CONFIG_1, 3)
 
-    def __init__(self, i2c, address=_REG_WHOAMI):
+    def __init__(self, i2c, address=0x69):
         self._i2c = i2c
         self._address = address
 
         if self._device_id != 0xEA:
             raise RuntimeError("Failed to find the ICM20948 sensor!")
 
         self.reset = True
@@ -289,18 +290,19 @@
         self.gyro_data_rate_divisor = 10
         print("ACC data rate", self.acc_data_rate)
 
     @property
     def clock_select(self):
         """
         CLK_SELECT_INTERNAL: Internal 20 MHz oscillator
-        CLK_SELECT_BEST: Auto selects the best available clock source – PLL if ready, else use the
-        Internal oscillator
+        CLK_SELECT_BEST: Auto selects the best available clock source - PLL if
+        ready, else use the Internal oscillator
         CLK_SELECT_STOP: Stops the clock and keeps timing generator in reset
-        NOTE: CLKSEL should be set to ``CLK_SELECT_BEST`` to achieve full gyroscope performance.
+        NOTE: CLKSEL should be set to ``CLK_SELECT_BEST`` to achieve full
+        gyroscope performance.
 
         +------------------------------------------+-------------------+
         | Mode                                     | Value             |
         +==========================================+===================+
         | :py:const:`icm20948.CLK_SELECT_INTERNAL` | :py:const:`0b000` |
         +------------------------------------------+-------------------+
         | :py:const:`icm20948.CLK_SELECT_BEST`     | :py:const:`0b001` |
@@ -317,29 +319,29 @@
     @clock_select.setter
     def clock_select(self, value):
         if value not in clk_values:
             raise ValueError("Select a valid Clock Select setting")
         self._clock_select = value
 
     @property
-    def reset(self):
+    def reset(self) -> int:
         """
         Reset the internal registers and restores the default settings. Write a 1 to set the
         reset, the bit will auto clear
         """
 
         return self._reset
 
     @reset.setter
-    def reset(self, value=1):
+    def reset(self, value: int = 1) -> None:
         self._reset = value
         sleep(1)
 
     @property
-    def gyro_enabled(self):
+    def gyro_enabled(self) -> str:
         """
         Gyro Enabled
 
         +------------------------------------+------------------------------------------------------+
         | Mode                               | Value                                                |
         +====================================+======================================================+
         | :py:const:`icm20948.GYRO_ENABLED`  | :py:const:`0b000` Gyroscope (all axes) on            |
@@ -348,21 +350,21 @@
         +------------------------------------+------------------------------------------------------+
 
         """
         values = {0: "GYRO_DISABLED", 7: "GYRO_ENABLED"}
         return values[self._gyro_enable]
 
     @gyro_enabled.setter
-    def gyro_enabled(self, value):
+    def gyro_enabled(self, value: int) -> None:
         if value not in gyro_en_values:
             raise ValueError("Value must be a valid Gyro Enabled setting")
         self._gyro_enable = value
 
     @property
-    def acc_enabled(self):
+    def acc_enabled(self) -> str:
         """
         Accelerometer enabled
 
         +------------------------------------+------------------------------------------------------+
         | Mode                               | Value                                                |
         +====================================+======================================================+
         | :py:const:`icm20948.ACC_ENABLED`   | :py:const:`0b000` Accelerometer (all axes) on        |
@@ -371,44 +373,44 @@
         +------------------------------------+------------------------------------------------------+
 
         """
         values = {0: "ACC_DISABLED", 7: "ACC_ENABLED"}
         return values[self._acc_enable]
 
     @acc_enabled.setter
-    def acc_enabled(self, value):
+    def acc_enabled(self, value: int) -> None:
         if value not in acc_en_values:
             raise ValueError("Value must be a valid Accelerometer Enabled setting")
         self._acc_enable = value
 
     @property
-    def temperature_enabled(self):
+    def temperature_enabled(self) -> str:
         """
         Temperature Enabled. When set to 1, this bit disables the temperature sensor.
 
-        +------------------------------------+------------------------------------------------------+
-        | Mode                               | Value                                                |
-        +====================================+======================================================+
-        | :py:const:`icm20948.TEMP_ENABLED`  | :py:const:`0b0` Temperature on                       |
-        +------------------------------------+------------------------------------------------------+
-        | :py:const:`icm20948.TEMP_DISABLED` | :py:const:`0b1` Temperature disabled                 |
-        +------------------------------------+------------------------------------------------------+
+        +------------------------------------+----------------------------------------+
+        | Mode                               | Value                                  |
+        +====================================+========================================+
+        | :py:const:`icm20948.TEMP_ENABLED`  | :py:const:`0b0` Temperature on         |
+        +------------------------------------+----------------------------------------+
+        | :py:const:`icm20948.TEMP_DISABLED` | :py:const:`0b1` Temperature disabled   |
+        +------------------------------------+----------------------------------------+
 
         """
-        values = {0: "TEMP_DISABLED", 1: "TEMP_ENABLED"}
+        values = ("TEMP_DISABLED", "TEMP_ENABLED")
         return values[self._temp_enabled]
 
     @temperature_enabled.setter
-    def temperature_enabled(self, value):
+    def temperature_enabled(self, value: int) -> None:
         if value not in temperature_en_values:
             raise ValueError("Value must be a valid Temperature Enabled setting")
         self._temp_enabled = value
 
     @property
-    def acceleration(self):
+    def acceleration(self) -> Tuple[float, float, float]:
         """
         Acceleration Property. The x, y, z acceleration values returned in a 3-tuple
         and are in :math:`m / s ^ 2.`
         :return: Acceleration Values
         """
         raw_measurement = self._raw_accel_data
         sleep(0.005)
@@ -427,15 +429,15 @@
             / acc_range_sensitivity[self._memory_accel_range]
             * 9.80665
         )
 
         return x, y, z
 
     @property
-    def gyro(self):
+    def gyro(self) -> Tuple[float, float, float]:
         """
         Gyro Property. The x, y, z angular velocity values returned in a 3-tuple and
         are in :math:`degrees / second`
         :return: Angular velocity Values
         """
         raw_measurement = self._raw_gyro_data
         sleep(0.005)
@@ -454,27 +456,27 @@
             / gyro_full_scale_sensitivity[self._memory_gyro_fs]
             * 0.017453293
         )
 
         return x, y, z
 
     @property
-    def power_bank(self):
+    def power_bank(self) -> int:
         """
         Power bank selected
         """
         return self._user_bank
 
     @power_bank.setter
-    def power_bank(self, value):
+    def power_bank(self, value: int) -> None:
         self._user_bank = value
         sleep(0.005)
 
     @property
-    def accelerometer_range(self):
+    def accelerometer_range(self) -> str:
         """
         Sensor acceleration_range
 
         +--------------------------------+------------------+
         | Mode                           | Value            |
         +================================+==================+
         | :py:const:`icm20948.RANGE_2G`  | :py:const:`0b00` |
@@ -487,25 +489,25 @@
         +--------------------------------+------------------+
 
         """
         values = ("RANGE_2G", "RANGE_4G", "RANGE_8G", "RANGE_16G")
         return values[self._memory_accel_range]
 
     @accelerometer_range.setter
-    def accelerometer_range(self, value):
+    def accelerometer_range(self, value: int) -> None:
         if value not in acc_range_values:
             raise ValueError("Value must be a valid Accelerometer Range Setting")
         self._user_bank = 2
         self._acc_data_range = value
         sleep(0.005)
         self._memory_accel_range = value
         self._user_bank = 0
 
     @property
-    def gyro_full_scale(self):
+    def gyro_full_scale(self) -> str:
         """
         Sensor gyro_full_scale
 
         +----------------------------------+------------------+
         | Mode                             | Value            |
         +==================================+==================+
         | :py:const:`icm20948.FS_250_DPS`  | :py:const:`0b00` |
@@ -517,42 +519,43 @@
         | :py:const:`icm20948.FS_2000_DPS` | :py:const:`0b11` |
         +----------------------------------+------------------+
         """
         values = ("FS_250_DPS", "FS_500_DPS", "FS_1000_DPS", "FS_2000_DPS")
         return values[self._memory_gyro_fs]
 
     @gyro_full_scale.setter
-    def gyro_full_scale(self, value):
+    def gyro_full_scale(self, value: int) -> None:
         if value not in gyro_full_scale_values:
             raise ValueError("Value must be a valid gyro_full_scale setting")
         self._user_bank = 2
         self._gyro_full_scale = value
         sleep(0.005)
         self._memory_gyro_fs = value
         self._user_bank = 0
         sleep(0.1)
 
     @property
-    def temperature(self):
+    def temperature(self) -> float:
         """
-        Temperature Value. In the setup tested, there is the need to read either the values from acceleration,
-        gyro and temperature or gyro and temperature at the same time in order to have a logic temperature value.
+        Temperature Value. In the setup tested, there is the need to read either the values
+        from acceleration, gyro and temperature or gyro and temperature at the same time
+        in order to have a logic temperature value.
 
         """
         return (self._raw_temp_data[3] / 333.87) + 21
 
     @property
     def gyro_data_rate(self):
         """The rate at which gyro measurements are taken in Hz"""
         return list(gyro_rate_values.keys())[
             list(gyro_rate_values.values()).index(self.gyro_data_rate_divisor)
         ]
 
     @gyro_data_rate.setter
-    def gyro_data_rate(self, value):
+    def gyro_data_rate(self, value: int) -> None:
         """
         .. note::
 
             The data rates are set indirectly by setting a rate divisor according to the
             following formula:
 
             .. math::
@@ -584,15 +587,15 @@
         """
         if value not in gyro_data_rate_values:
             raise ValueError("Gyro data rate must be a valid setting")
 
         self.gyro_data_rate_divisor = gyro_rate_values[value]
 
     @property
-    def gyro_data_rate_divisor(self):
+    def gyro_data_rate_divisor(self) -> int:
         """
         Accepted values are:
 
         | * 1
         | * 2
         | * 3
         | * 4
@@ -614,15 +617,15 @@
         self._user_bank = 2
         raw_rate_divisor = self._gyro_rate_divisor
         sleep(0.005)
         self._user_bank = 0
         return raw_rate_divisor
 
     @gyro_data_rate_divisor.setter
-    def gyro_data_rate_divisor(self, value):
+    def gyro_data_rate_divisor(self, value: int) -> None:
         if value not in gyro_rate_divisor_values:
             raise ValueError("Value must be a valid gyro data rate divisor setting")
         self._user_bank = 2
         sleep(0.005)
         self._gyro_rate_divisor = value
         sleep(0.005)
 
@@ -630,15 +633,15 @@
     def acc_data_rate(self):
         """The rate at which accelerometer measurements are taken in Hz"""
         return list(acc_rate_values.keys())[
             list(acc_rate_values.values()).index(self.acc_data_rate_divisor)
         ]
 
     @acc_data_rate.setter
-    def acc_data_rate(self, value):
+    def acc_data_rate(self, value: int) -> None:
         """
         .. note::
 
             The data rates are set indirectly by setting a rate divisor according to the
             following formula:
 
             .. math::
@@ -666,15 +669,15 @@
         """
         if value not in acc_data_rate_values:
             raise ValueError("Accelerometer data rate must be a valid setting")
 
         self.acc_data_rate_divisor = acc_rate_values[value]
 
     @property
-    def acc_data_rate_divisor(self):
+    def acc_data_rate_divisor(self) -> int:
         """
         Accepted values are:
 
         | * 7
         | * 10
         | * 15
         | * 22
@@ -692,104 +695,157 @@
         self._user_bank = 2
         raw_rate_divisor = self._acc_rate_divisor
         sleep(0.005)
         self._user_bank = 0
         return raw_rate_divisor
 
     @acc_data_rate_divisor.setter
-    def acc_data_rate_divisor(self, value):
+    def acc_data_rate_divisor(self, value: int) -> None:
         if value not in acc_rate_divisor_values:
             raise ValueError(
                 "Value must be a valid acceleration data rate divisor setting"
             )
         self._user_bank = 2
         sleep(0.005)
         self._acc_rate_divisor = value
         sleep(0.005)
 
     @property
-    def acc_dlpf_cutoff(self):
+    def acc_dlpf_cutoff(self) -> int:
         """The cutoff frequency for the accelerometer's digital low pass filter. Signals
         above the given frequency will be filtered out.
 
         .. note::
             Readings immediately following setting a cutoff frequency will be
             inaccurate due to the filter "warming up"
 
-        """
-
+        +---------------------------------+-------------------+
+        | Mode                            | Value             |
+        +=================================+===================+
+        | :py:const:`icm20948.FREQ_246_0` | :py:const:`0b001` |
+        +---------------------------------+-------------------+
+        | :py:const:`icm20948.FREQ_111_4` | :py:const:`0b010` |
+        +---------------------------------+-------------------+
+        | :py:const:`icm20948.FREQ_50_4`  | :py:const:`0b011` |
+        +---------------------------------+-------------------+
+        | :py:const:`icm20948.FREQ_23_9`  | :py:const:`0b100` |
+        +---------------------------------+-------------------+
+        | :py:const:`icm20948.FREQ_11_5`  | :py:const:`0b101` |
+        +---------------------------------+-------------------+
+        | :py:const:`icm20948.FREQ_5_7`   | :py:const:`0b110` |
+        +---------------------------------+-------------------+
+        | :py:const:`icm20948.FREQ_473`   | :py:const:`0b111` |
+        +---------------------------------+-------------------+
+        """
+        values = (
+            "FREQ_246_0",
+            "FREQ_111_4",
+            "FREQ_50_4",
+            "FREQ_23_9",
+            "FREQ_11_5",
+            "FREQ_5_7",
+            "FREQ_473",
+        )
         self._user_bank = 2
         sleep(0.005)
         raw_value = self._acc_dplcfg
         self._user_bank = 0
-        return raw_value
+        return values[raw_value]
 
     @acc_dlpf_cutoff.setter
-    def acc_dlpf_cutoff(self, value):
+    def acc_dlpf_cutoff(self, value: int) -> None:
         if value not in acc_filter_values:
             raise ValueError("Value must be a valid dlpf setting")
         self._user_bank = 2
         sleep(0.005)
         self._acc_dplcfg = value
         self._user_bank = 0
         sleep(0.005)
 
     @property
-    def acc_filter_choice(self):
+    def acc_filter_choice(self) -> int:
         """Enables accelerometer DLPF"""
         self._user_bank = 2
         sleep(0.005)
         raw_value = self._acc_choice
         self._user_bank = 0
         return raw_value
 
     @acc_filter_choice.setter
-    def acc_filter_choice(self, value):
+    def acc_filter_choice(self, value: int) -> None:
         self._user_bank = 2
         sleep(0.005)
         self._acc_choice = value
         self._user_bank = 0
         sleep(0.05)
 
     @property
-    def gyro_dlpf_cutoff(self):
+    def gyro_dlpf_cutoff(self) -> int:
         """The cutoff frequency for the gyro's digital low pass filter. Signals
         above the given frequency will be filtered out.
 
         .. note::
             Readings immediately following setting a cutoff frequency will be
             inaccurate due to the filter "warming up"
 
-        """
-
+        +-----------------------------------+-------------------+
+        | Mode                              | Value             |
+        +===================================+===================+
+        | :py:const:`icm20948.G_FREQ_196_6` | :py:const:`0b000` |
+        +-----------------------------------+-------------------+
+        | :py:const:`icm20948.G_FREQ_151_8` | :py:const:`0b001` |
+        +-----------------------------------+-------------------+
+        | :py:const:`icm20948.G_FREQ_119_5` | :py:const:`0b010` |
+        +-----------------------------------+-------------------+
+        | :py:const:`icm20948.G_FREQ_51_2`  | :py:const:`0b011` |
+        +-----------------------------------+-------------------+
+        | :py:const:`icm20948.G_FREQ_23_9`  | :py:const:`0b100` |
+        +-----------------------------------+-------------------+
+        | :py:const:`icm20948.G_FREQ_11_6`  | :py:const:`0b101` |
+        +-----------------------------------+-------------------+
+        | :py:const:`icm20948.G_FREQ_5_7`   | :py:const:`0b110` |
+        +-----------------------------------+-------------------+
+        | :py:const:`icm20948.G_FREQ_361_4` | :py:const:`0b111` |
+        +-----------------------------------+-------------------+
+        """
+        values = (
+            "G_FREQ_196_6",
+            "G_FREQ_151_8",
+            "G_FREQ_119_5",
+            "G_FREQ_51_2",
+            "G_FREQ_23_9",
+            "G_FREQ_11_6",
+            "G_FREQ_5_7",
+            "G_FREQ_361_4",
+        )
         self._user_bank = 2
         sleep(0.005)
         raw_value = self._gyro_dplcfg
         self._user_bank = 0
-        return raw_value
+        return values[raw_value]
 
     @gyro_dlpf_cutoff.setter
-    def gyro_dlpf_cutoff(self, value):
+    def gyro_dlpf_cutoff(self, value: int) -> None:
         if value not in gyro_filter_values:
             raise ValueError("Value must be a valid dlpf setting")
         self._user_bank = 2
         sleep(0.005)
         self._gyro_dplcfg = value
         self._user_bank = 0
         sleep(0.005)
 
     @property
-    def gyro_filter_choice(self):
+    def gyro_filter_choice(self) -> int:
         """Enables gyro DLPF"""
         self._user_bank = 2
         sleep(0.005)
         raw_value = self._gyro_choice
         self._user_bank = 0
         return raw_value
 
     @gyro_filter_choice.setter
-    def gyro_filter_choice(self, value):
+    def gyro_filter_choice(self, value: int) -> None:
         self._user_bank = 2
         sleep(0.005)
         self._gyro_choice = value
         self._user_bank = 0
         sleep(0.05)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `micropython-icm20948-0.2.1/micropython_icm20948.egg-info/PKG-INFO` & `micropython-icm20948-0.2.2/micropython_icm20948.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-icm20948
-Version: 0.2.1
+Version: 0.2.2
 Summary: MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor
 Author-email: "Jose D. Montoya" <icm20948@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ICM20948
 Keywords: micropython,icm20948,gyro,accelerometer,acceleration,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-icm20948-0.2.1/pyproject.toml` & `micropython-icm20948-0.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-icm20948"
 description = "MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor"
-version = "0.2.1"
+version = "0.2.2"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "icm20948@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_ICM20948"}
 keywords = [
     "micropython",
```

