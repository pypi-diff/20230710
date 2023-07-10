# Comparing `tmp/ciscopykit-1.3.1.tar.gz` & `tmp/ciscopykit-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciscopykit-1.3.1.tar", last modified: Fri Jul  7 15:30:29 2023, max compression
+gzip compressed data, was "ciscopykit-1.4.1.tar", last modified: Mon Jul 10 01:13:44 2023, max compression
```

## Comparing `ciscopykit-1.3.1.tar` & `ciscopykit-1.4.1.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/ciscopykit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/ciscopykit/switch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/switch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/switch/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/switch/l2_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/switch/l3_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/switch/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/ciscopykit/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/templates/generate_router_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/templates/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/ciscopykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-07 15:30:29.000000 ciscopykit-1.3.1/ciscopykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-07 15:30:29.000000 ciscopykit-1.3.1/ciscopykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:30:29.000000 ciscopykit-1.3.1/ciscopykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 15:30:29.000000 ciscopykit-1.3.1/ciscopykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 15:30:29.000000 ciscopykit-1.3.1/ciscopykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 15:30:29.000000 ciscopykit-1.3.1/ciscopykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 01:13:44.478575 ciscopykit-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-10 01:13:44.478575 ciscopykit-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 01:13:44.478575 ciscopykit-1.4.1/ciscopykit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 01:13:44.478575 ciscopykit-1.4.1/ciscopykit/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/services/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/services/dhcp_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/services/pat_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 01:13:44.478575 ciscopykit-1.4.1/ciscopykit/switch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/switch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/switch/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/switch/l2_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/switch/l3_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/switch/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 01:13:44.478575 ciscopykit-1.4.1/ciscopykit/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/templates/generate_router_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/ciscopykit/templates/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 01:13:44.478575 ciscopykit-1.4.1/ciscopykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-10 01:13:44.000000 ciscopykit-1.4.1/ciscopykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-10 01:13:44.000000 ciscopykit-1.4.1/ciscopykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 01:13:44.000000 ciscopykit-1.4.1/ciscopykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-10 01:13:44.000000 ciscopykit-1.4.1/ciscopykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 01:13:44.000000 ciscopykit-1.4.1/ciscopykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 01:13:44.000000 ciscopykit-1.4.1/ciscopykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 01:13:44.478575 ciscopykit-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-10 01:13:29.000000 ciscopykit-1.4.1/setup.py
```

### Comparing `ciscopykit-1.3.1/LICENSE.md` & `ciscopykit-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.3.1/PKG-INFO` & `ciscopykit-1.4.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscopykit
-Version: 1.3.1
+Version: 1.4.1
 Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer
 Home-page: https://github.com/Vincent-de-Torres-Portfolio/ciscopykit
 Author: devinci-it
 Author-email: vince.dev@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ciscopykit-1.3.1/README.md` & `ciscopykit-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.3.1/ciscopykit/app.py` & `ciscopykit-1.4.1/ciscopykit/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.3.1/ciscopykit/device.py` & `ciscopykit-1.4.1/ciscopykit/device.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.3.1/ciscopykit/entry_point.py` & `ciscopykit-1.4.1/ciscopykit/entry_point.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.3.1/ciscopykit/interface.py` & `ciscopykit-1.4.1/ciscopykit/interface.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.3.1/ciscopykit/switch/app.py` & `ciscopykit-1.4.1/ciscopykit/switch/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.3.1/ciscopykit/switch/l3_switch.py` & `ciscopykit-1.4.1/ciscopykit/switch/l3_switch.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.3.1/ciscopykit/switch/switch.py` & `ciscopykit-1.4.1/ciscopykit/switch/switch.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.3.1/ciscopykit/templates/generate_router_config.py` & `ciscopykit-1.4.1/ciscopykit/templates/generate_router_config.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.3.1/ciscopykit.egg-info/PKG-INFO` & `ciscopykit-1.4.1/ciscopykit.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscopykit
-Version: 1.3.1
+Version: 1.4.1
 Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer
 Home-page: https://github.com/Vincent-de-Torres-Portfolio/ciscopykit
 Author: devinci-it
 Author-email: vince.dev@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ciscopykit-1.3.1/ciscopykit.egg-info/SOURCES.txt` & `ciscopykit-1.4.1/ciscopykit.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 ciscopykit/interface.py
 ciscopykit.egg-info/PKG-INFO
 ciscopykit.egg-info/SOURCES.txt
 ciscopykit.egg-info/dependency_links.txt
 ciscopykit.egg-info/entry_points.txt
 ciscopykit.egg-info/requires.txt
 ciscopykit.egg-info/top_level.txt
+ciscopykit/services/__init__.py
+ciscopykit/services/app.py
+ciscopykit/services/dhcp_service.py
+ciscopykit/services/pat_service.py
 ciscopykit/switch/__init__.py
 ciscopykit/switch/app.py
 ciscopykit/switch/l2_switch.py
 ciscopykit/switch/l3_switch.py
 ciscopykit/switch/switch.py
 ciscopykit/templates/generate_router_config.py
 ciscopykit/templates/placeholder.txt
```

### Comparing `ciscopykit-1.3.1/setup.py` & `ciscopykit-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ciscopykit',
-    version='1.3.1',
+    version='1.4.1',
     author='devinci-it',
     author_email='vince.dev@icloud.com',
     description='A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer',
     long_description='''A network management toolkit for Cisco devices. It provides classes and methods to manage network devices, interfaces, and configurations.''',
     url='https://github.com/Vincent-de-Torres-Portfolio/ciscopykit',
     packages=find_packages(),
     classifiers=[
@@ -28,11 +28,12 @@
         'matplotlib',
         'ipaddress',
         'argeparse'
     ],
     entry_points={
         'console_scripts': [
             'ciscopykit = ciscopykit.entry_point:main',
-            'switch = ciscopykit.switch.app:main'
+            'switch = ciscopykit.switch.app:main',
+            'services=ciscopykit.services.app:main'
         ],
     },
 )
```

