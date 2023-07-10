# Comparing `tmp/discoverable_garage_door-0.1.1.tar.gz` & `tmp/discoverable_garage_door-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoverable_garage_door-0.1.1.tar", max compression
+gzip compressed data, was "discoverable_garage_door-0.1.3.tar", max compression
```

## Comparing `discoverable_garage_door-0.1.1.tar` & `discoverable_garage_door-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-07-05 15:01:59.971398 discoverable_garage_door-0.1.1/LICENSE
--rw-r--r--   0        0        0     3950 2023-07-05 15:01:59.971398 discoverable_garage_door-0.1.1/README.md
--rw-r--r--   0        0        0      455 2023-07-05 15:01:59.971398 discoverable_garage_door-0.1.1/discoverable_garage_door/.config.yaml
--rw-r--r--   0        0        0      157 2023-07-07 01:12:50.933164 discoverable_garage_door-0.1.1/discoverable_garage_door/__init__.py
--rw-r--r--   0        0        0      801 2023-07-07 01:13:37.469035 discoverable_garage_door-0.1.1/discoverable_garage_door/__main__.py
--rw-r--r--   0        0        0     2857 2023-07-05 15:08:13.229050 discoverable_garage_door-0.1.1/discoverable_garage_door/config.py
--rw-r--r--   0        0        0     3013 2023-07-05 15:08:13.161050 discoverable_garage_door-0.1.1/discoverable_garage_door/cover.py
--rw-r--r--   0        0        0      439 2023-07-05 15:01:59.975398 discoverable_garage_door-0.1.1/discoverable_garage_door/logger.conf
--rw-r--r--   0        0        0      333 2023-07-05 15:08:12.673053 discoverable_garage_door-0.1.1/discoverable_garage_door/util.py
--rw-r--r--   0        0        0      410 2023-07-08 23:17:38.047140 discoverable_garage_door-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4394 1970-01-01 00:00:00.000000 discoverable_garage_door-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-05 15:01:59.971398 discoverable_garage_door-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4359 2023-07-10 16:03:23.211414 discoverable_garage_door-0.1.3/README.md
+-rw-r--r--   0        0        0      455 2023-07-05 15:01:59.971398 discoverable_garage_door-0.1.3/discoverable_garage_door/.config.yaml
+-rw-r--r--   0        0        0      157 2023-07-07 01:12:50.933164 discoverable_garage_door-0.1.3/discoverable_garage_door/__init__.py
+-rw-r--r--   0        0        0      801 2023-07-07 01:13:37.469035 discoverable_garage_door-0.1.3/discoverable_garage_door/__main__.py
+-rw-r--r--   0        0        0     2857 2023-07-05 15:08:13.229050 discoverable_garage_door-0.1.3/discoverable_garage_door/config.py
+-rw-r--r--   0        0        0     3013 2023-07-05 15:08:13.161050 discoverable_garage_door-0.1.3/discoverable_garage_door/cover.py
+-rw-r--r--   0        0        0      439 2023-07-05 15:01:59.975398 discoverable_garage_door-0.1.3/discoverable_garage_door/logging.conf
+-rw-r--r--   0        0        0      333 2023-07-05 15:08:12.673053 discoverable_garage_door-0.1.3/discoverable_garage_door/util.py
+-rw-r--r--   0        0        0      410 2023-07-10 16:02:55.827602 discoverable_garage_door-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4803 1970-01-01 00:00:00.000000 discoverable_garage_door-0.1.3/PKG-INFO
```

### Comparing `discoverable_garage_door-0.1.1/LICENSE` & `discoverable_garage_door-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `discoverable_garage_door-0.1.1/README.md` & `discoverable_garage_door-0.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,18 @@
   - [Debian](#debian)
   - [Python](#python)
 - [Installing](#installing)
   - [installation](#installation)
 - [Usage](#usage)
 - [Configuration](#configuration)
   - [Format](#format)
+- [Version History](#version-history)
+  - [Version 0.1.1 - Complete build config](#version-011---complete-build-config)
+  - [Version 0.1.2 - Add Lovelace UI exampe](#version-012---add-lovelace-ui-exampe)
+- [Uses ha-mqtt-discoverable](#uses-ha-mqtt-discoverable)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 ## Requirements
 
 ### Raspberry PI
 
 discoverable_garage_door is designed to run on a PI Zero, Pi 3B+ or PI 4B it may run on other models.
@@ -82,10 +86,18 @@
 <p><strong><em>gpio.contact_pullup - </em></strong>whether to use a pullup for the GPIO inputs(true) or whether a pullup will be externally used (false)<br></p>
 <p><strong><em>gpio.doors - </em></strong>a list of door descriptions<br></p>
 <p><strong><em>door.name - </em></strong>the name of the garage door<br></p>
 <p><strong><em>door.button_pin - </em></strong>the number of the pin used for the button (GPIO numbering)<br></p>
 <p><strong><em>door.closed_contact_pin - </em></strong>the number of the pin used for the closed contact (GPIO numbering)<br></p>
 <p><strong><em>door.opened_contact_pin - </em></strong>the number of the pin used for the opened contact (GPIO numbering)<br></p>
 
+## Version History
+
+### Version 0.1.1 - Complete build config
+
+### Version 0.1.2 - Add Lovelace UI exampe
+
+### Version 0.1.3 - Rename logger.conf
+
 ## Uses ha-mqtt-discoverable
 
 - [ha-mqtt-discoverable-cli](https://github.com/unixorn/ha-mqtt-discoverable-cli)
```

### Comparing `discoverable_garage_door-0.1.1/discoverable_garage_door/__main__.py` & `discoverable_garage_door-0.1.3/discoverable_garage_door/__main__.py`

 * *Files identical despite different names*

### Comparing `discoverable_garage_door-0.1.1/discoverable_garage_door/config.py` & `discoverable_garage_door-0.1.3/discoverable_garage_door/config.py`

 * *Files identical despite different names*

### Comparing `discoverable_garage_door-0.1.1/discoverable_garage_door/cover.py` & `discoverable_garage_door-0.1.3/discoverable_garage_door/cover.py`

 * *Files identical despite different names*

### Comparing `discoverable_garage_door-0.1.1/PKG-INFO` & `discoverable_garage_door-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discoverable-garage-door
-Version: 0.1.1
+Version: 0.1.3
 Summary: 
 Author: Tim Daley
 Author-email: timdaley@earthling.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ha-mqtt-discoverable (>=0.9.0,<0.10.0)
@@ -29,14 +29,18 @@
   - [Debian](#debian)
   - [Python](#python)
 - [Installing](#installing)
   - [installation](#installation)
 - [Usage](#usage)
 - [Configuration](#configuration)
   - [Format](#format)
+- [Version History](#version-history)
+  - [Version 0.1.1 - Complete build config](#version-011---complete-build-config)
+  - [Version 0.1.2 - Add Lovelace UI exampe](#version-012---add-lovelace-ui-exampe)
+- [Uses ha-mqtt-discoverable](#uses-ha-mqtt-discoverable)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 ## Requirements
 
 ### Raspberry PI
 
 discoverable_garage_door is designed to run on a PI Zero, Pi 3B+ or PI 4B it may run on other models.
@@ -96,11 +100,19 @@
 <p><strong><em>gpio.contact_pullup - </em></strong>whether to use a pullup for the GPIO inputs(true) or whether a pullup will be externally used (false)<br></p>
 <p><strong><em>gpio.doors - </em></strong>a list of door descriptions<br></p>
 <p><strong><em>door.name - </em></strong>the name of the garage door<br></p>
 <p><strong><em>door.button_pin - </em></strong>the number of the pin used for the button (GPIO numbering)<br></p>
 <p><strong><em>door.closed_contact_pin - </em></strong>the number of the pin used for the closed contact (GPIO numbering)<br></p>
 <p><strong><em>door.opened_contact_pin - </em></strong>the number of the pin used for the opened contact (GPIO numbering)<br></p>
 
+## Version History
+
+### Version 0.1.1 - Complete build config
+
+### Version 0.1.2 - Add Lovelace UI exampe
+
+### Version 0.1.3 - Rename logger.conf
+
 ## Uses ha-mqtt-discoverable
 
 - [ha-mqtt-discoverable-cli](https://github.com/unixorn/ha-mqtt-discoverable-cli)
```

