# Comparing `tmp/performancetest-0.0.16.tar.gz` & `tmp/performancetest-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "performancetest-0.0.16.tar", last modified: Mon Jul 10 03:57:03 2023, max compression
+gzip compressed data, was "performancetest-0.0.17.tar", last modified: Mon Jul 10 04:29:05 2023, max compression
```

## Comparing `performancetest-0.0.16.tar` & `performancetest-0.0.17.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 03:57:03.641266 performancetest-0.0.16/
--rw-rw-rw-   0        0        0      516 2023-07-10 03:57:03.641266 performancetest-0.0.16/PKG-INFO
--rw-rw-rw-   0        0        0     4346 2023-06-27 05:36:55.000000 performancetest-0.0.16/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 03:57:03.499046 performancetest-0.0.16/performancetest/
--rw-rw-rw-   0        0        0       49 2023-06-21 09:23:31.000000 performancetest-0.0.16/performancetest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 03:57:03.602372 performancetest-0.0.16/performancetest/core/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.16/performancetest/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 03:57:03.614338 performancetest-0.0.16/performancetest/core/base/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.16/performancetest/core/base/__init__.py
--rw-rw-rw-   0        0        0      289 2023-05-04 05:59:55.000000 performancetest-0.0.16/performancetest/core/base/actuator.py
--rw-rw-rw-   0        0        0      325 2023-05-04 05:59:55.000000 performancetest-0.0.16/performancetest/core/base/monitor.py
--rw-rw-rw-   0        0        0     3562 2023-06-21 12:46:09.000000 performancetest-0.0.16/performancetest/core/command.py
--rw-rw-rw-   0        0        0     4277 2023-06-27 06:56:49.000000 performancetest-0.0.16/performancetest/core/cpu.py
--rw-rw-rw-   0        0        0     6451 2023-07-04 03:26:18.000000 performancetest-0.0.16/performancetest/core/device.py
--rw-rw-rw-   0        0        0     4268 2023-06-21 12:46:09.000000 performancetest-0.0.16/performancetest/core/devicebattery.py
--rw-rw-rw-   0        0        0    19366 2023-07-03 10:04:25.000000 performancetest-0.0.16/performancetest/core/fps.py
--rw-rw-rw-   0        0        0      678 2023-06-21 12:46:09.000000 performancetest-0.0.16/performancetest/core/global_data.py
--rw-rw-rw-   0        0        0     3882 2023-06-27 06:56:49.000000 performancetest-0.0.16/performancetest/core/gpu.py
--rw-rw-rw-   0        0        0     6646 2023-06-21 12:47:53.000000 performancetest-0.0.16/performancetest/core/iosperf.py
--rw-rw-rw-   0        0        0     3928 2023-06-27 06:56:49.000000 performancetest-0.0.16/performancetest/core/memory.py
--rw-rw-rw-   0        0        0     4315 2023-06-23 08:54:45.000000 performancetest-0.0.16/performancetest/core/snapshot.py
--rw-rw-rw-   0        0        0     4375 2023-07-10 03:46:07.000000 performancetest-0.0.16/performancetest/core/task_handle.py
-drwxrwxrwx   0        0        0        0 2023-07-10 03:57:03.625309 performancetest-0.0.16/performancetest/test/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.16/performancetest/test/__init__.py
--rw-rw-rw-   0        0        0     1133 2023-05-04 05:59:55.000000 performancetest-0.0.16/performancetest/test/all_property_test.py
-drwxrwxrwx   0        0        0        0 2023-07-10 03:57:03.639276 performancetest-0.0.16/performancetest/web/
--rw-rw-rw-   0        0        0       25 2023-05-05 12:26:54.000000 performancetest-0.0.16/performancetest/web/__init__.py
--rw-rw-rw-   0        0        0     1852 2023-06-21 12:46:09.000000 performancetest-0.0.16/performancetest/web/dao.py
--rw-rw-rw-   0        0        0      408 2023-06-21 10:25:13.000000 performancetest-0.0.16/performancetest/web/entity.py
--rw-rw-rw-   0        0        0     9209 2023-07-10 03:54:05.000000 performancetest-0.0.16/performancetest/web/main.py
--rw-rw-rw-   0        0        0    11864 2023-06-25 06:05:19.000000 performancetest-0.0.16/performancetest/web/util.py
-drwxrwxrwx   0        0        0        0 2023-07-10 03:57:03.526008 performancetest-0.0.16/performancetest.egg-info/
--rw-rw-rw-   0        0        0      516 2023-07-10 03:57:03.000000 performancetest-0.0.16/performancetest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2023-07-10 03:57:03.000000 performancetest-0.0.16/performancetest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 03:57:03.000000 performancetest-0.0.16/performancetest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-07-10 03:57:03.000000 performancetest-0.0.16/performancetest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-10 03:57:03.000000 performancetest-0.0.16/performancetest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 03:57:03.642263 performancetest-0.0.16/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-07-10 03:23:53.000000 performancetest-0.0.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.241722 performancetest-0.0.17/
+-rw-rw-rw-   0        0        0      516 2023-07-10 04:29:05.239784 performancetest-0.0.17/PKG-INFO
+-rw-rw-rw-   0        0        0     4346 2023-06-27 05:36:55.000000 performancetest-0.0.17/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.077478 performancetest-0.0.17/performancetest/
+-rw-rw-rw-   0        0        0       49 2023-06-21 09:23:31.000000 performancetest-0.0.17/performancetest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.192655 performancetest-0.0.17/performancetest/core/
+-rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.17/performancetest/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.201441 performancetest-0.0.17/performancetest/core/base/
+-rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.17/performancetest/core/base/__init__.py
+-rw-rw-rw-   0        0        0      289 2023-05-04 05:59:55.000000 performancetest-0.0.17/performancetest/core/base/actuator.py
+-rw-rw-rw-   0        0        0      325 2023-05-04 05:59:55.000000 performancetest-0.0.17/performancetest/core/base/monitor.py
+-rw-rw-rw-   0        0        0     3637 2023-07-10 04:22:08.000000 performancetest-0.0.17/performancetest/core/command.py
+-rw-rw-rw-   0        0        0     4277 2023-06-27 06:56:49.000000 performancetest-0.0.17/performancetest/core/cpu.py
+-rw-rw-rw-   0        0        0     6451 2023-07-04 03:26:18.000000 performancetest-0.0.17/performancetest/core/device.py
+-rw-rw-rw-   0        0        0     4268 2023-06-21 12:46:09.000000 performancetest-0.0.17/performancetest/core/devicebattery.py
+-rw-rw-rw-   0        0        0    19366 2023-07-03 10:04:25.000000 performancetest-0.0.17/performancetest/core/fps.py
+-rw-rw-rw-   0        0        0      678 2023-06-21 12:46:09.000000 performancetest-0.0.17/performancetest/core/global_data.py
+-rw-rw-rw-   0        0        0     3882 2023-06-27 06:56:49.000000 performancetest-0.0.17/performancetest/core/gpu.py
+-rw-rw-rw-   0        0        0     6646 2023-06-21 12:47:53.000000 performancetest-0.0.17/performancetest/core/iosperf.py
+-rw-rw-rw-   0        0        0     3928 2023-06-27 06:56:49.000000 performancetest-0.0.17/performancetest/core/memory.py
+-rw-rw-rw-   0        0        0     4315 2023-06-23 08:54:45.000000 performancetest-0.0.17/performancetest/core/snapshot.py
+-rw-rw-rw-   0        0        0     4294 2023-07-10 04:22:56.000000 performancetest-0.0.17/performancetest/core/task_handle.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.211463 performancetest-0.0.17/performancetest/test/
+-rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.17/performancetest/test/__init__.py
+-rw-rw-rw-   0        0        0     1133 2023-05-04 05:59:55.000000 performancetest-0.0.17/performancetest/test/all_property_test.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.232936 performancetest-0.0.17/performancetest/web/
+-rw-rw-rw-   0        0        0       25 2023-05-05 12:26:54.000000 performancetest-0.0.17/performancetest/web/__init__.py
+-rw-rw-rw-   0        0        0     1852 2023-06-21 12:46:09.000000 performancetest-0.0.17/performancetest/web/dao.py
+-rw-rw-rw-   0        0        0      408 2023-06-21 10:25:13.000000 performancetest-0.0.17/performancetest/web/entity.py
+-rw-rw-rw-   0        0        0     9209 2023-07-10 03:54:05.000000 performancetest-0.0.17/performancetest/web/main.py
+-rw-rw-rw-   0        0        0    11864 2023-06-25 06:05:19.000000 performancetest-0.0.17/performancetest/web/util.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.150687 performancetest-0.0.17/performancetest.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-07-10 04:29:04.000000 performancetest-0.0.17/performancetest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      959 2023-07-10 04:29:04.000000 performancetest-0.0.17/performancetest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 04:29:04.000000 performancetest-0.0.17/performancetest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-07-10 04:29:04.000000 performancetest-0.0.17/performancetest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-10 04:29:04.000000 performancetest-0.0.17/performancetest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 04:29:05.243670 performancetest-0.0.17/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-07-10 04:28:27.000000 performancetest-0.0.17/setup.py
```

### Comparing `performancetest-0.0.16/PKG-INFO` & `performancetest-0.0.17/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: performancetest
-Version: 0.0.16
+Version: 0.0.17
 Summary: Android, IOS app_performance
 Home-page: https://github.com/1033866383/perf-orange-cat
 Author: bozhou.fan
 Author-email: 15525730080@163.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `performancetest-0.0.16/README.md` & `performancetest-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest/core/command.py` & `performancetest-0.0.17/performancetest/core/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding=utf-8
 import subprocess
 import traceback
 from builtins import *
 
+import airtest.core.android.adb
 import requests
 
 from performancetest.core.global_data import logger
 
 
 def split_cmd(cmds):
     return cmds.split() if isinstance(cmds, str) else list(cmds)
@@ -25,15 +26,15 @@
 
     return stdout, stderr
 
 
 class ADB(object):
     def __init__(self, serialno=None, adb_path=None, server_addr=None):
         self.serialno = serialno
-        self.adb_path = adb_path or "adb"
+        self.adb_path = adb_path or airtest.core.android.adb.ADB.builtin_adb_path()
         self._set_cmd_options(server_addr)
         self.server_addr = server_addr
 
     def _set_cmd_options(self, server_addr=None):
         logger.info(server_addr)
         self.host = server_addr[0] if server_addr[0] else "127.0.0.1"
         self.port = server_addr[1] if server_addr[1] else 5037
```

### Comparing `performancetest-0.0.16/performancetest/core/cpu.py` & `performancetest-0.0.17/performancetest/core/cpu.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest/core/device.py` & `performancetest-0.0.17/performancetest/core/device.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest/core/devicebattery.py` & `performancetest-0.0.17/performancetest/core/devicebattery.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest/core/fps.py` & `performancetest-0.0.17/performancetest/core/fps.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest/core/global_data.py` & `performancetest-0.0.17/performancetest/core/global_data.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest/core/gpu.py` & `performancetest-0.0.17/performancetest/core/gpu.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest/core/iosperf.py` & `performancetest-0.0.17/performancetest/core/iosperf.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest/core/memory.py` & `performancetest-0.0.17/performancetest/core/memory.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest/core/snapshot.py` & `performancetest-0.0.17/performancetest/core/snapshot.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest/core/task_handle.py` & `performancetest-0.0.17/performancetest/core/task_handle.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,16 +36,14 @@
 
     def start(self):
         logger.info("join task handle")
         super().start()
 
     def run(self):
         logger.info("join task handle run")
-        adb_path = ADB.builtin_adb_path()
-        os.environ['adb'] = adb_path
         with connect() as session:
             current_task_running = session.query(Task).filter(
                 Task.id == self.task_id).first()
             if current_task_running:
                 current_task_running.status = 1
                 current_task_running.pid = self.pid
             else:
```

### Comparing `performancetest-0.0.16/performancetest/test/all_property_test.py` & `performancetest-0.0.17/performancetest/test/all_property_test.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest/web/dao.py` & `performancetest-0.0.17/performancetest/web/dao.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest/web/main.py` & `performancetest-0.0.17/performancetest/web/main.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest/web/util.py` & `performancetest-0.0.17/performancetest/web/util.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/performancetest.egg-info/PKG-INFO` & `performancetest-0.0.17/performancetest.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: performancetest
-Version: 0.0.16
+Version: 0.0.17
 Summary: Android, IOS app_performance
 Home-page: https://github.com/1033866383/perf-orange-cat
 Author: bozhou.fan
 Author-email: 15525730080@163.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `performancetest-0.0.16/performancetest.egg-info/SOURCES.txt` & `performancetest-0.0.17/performancetest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.16/setup.py` & `performancetest-0.0.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # # _*_ coding: utf-8 _*_
 from setuptools import setup, find_packages
 
 setup(
        name='performancetest',
-       version='0.0.16',
+       version='0.0.17',
        url='https://github.com/1033866383/perf-orange-cat',
        author='bozhou.fan',
        author_email='15525730080@163.com',
        description='Android, IOS app_performance',
        packages=find_packages(),
        install_requires=[
            "psutil", "airtest", "fastapi", "tidevice", "func-timeout", "sqlalchemy", "sqlalchemy-serializer", "uvicorn"
```

