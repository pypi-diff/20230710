# Comparing `tmp/performancetest-0.0.17.tar.gz` & `tmp/performancetest-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "performancetest-0.0.17.tar", last modified: Mon Jul 10 04:29:05 2023, max compression
+gzip compressed data, was "performancetest-0.0.18.tar", last modified: Mon Jul 10 04:44:54 2023, max compression
```

## Comparing `performancetest-0.0.17.tar` & `performancetest-0.0.18.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.241722 performancetest-0.0.17/
--rw-rw-rw-   0        0        0      516 2023-07-10 04:29:05.239784 performancetest-0.0.17/PKG-INFO
--rw-rw-rw-   0        0        0     4346 2023-06-27 05:36:55.000000 performancetest-0.0.17/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.077478 performancetest-0.0.17/performancetest/
--rw-rw-rw-   0        0        0       49 2023-06-21 09:23:31.000000 performancetest-0.0.17/performancetest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.192655 performancetest-0.0.17/performancetest/core/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.17/performancetest/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.201441 performancetest-0.0.17/performancetest/core/base/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.17/performancetest/core/base/__init__.py
--rw-rw-rw-   0        0        0      289 2023-05-04 05:59:55.000000 performancetest-0.0.17/performancetest/core/base/actuator.py
--rw-rw-rw-   0        0        0      325 2023-05-04 05:59:55.000000 performancetest-0.0.17/performancetest/core/base/monitor.py
--rw-rw-rw-   0        0        0     3637 2023-07-10 04:22:08.000000 performancetest-0.0.17/performancetest/core/command.py
--rw-rw-rw-   0        0        0     4277 2023-06-27 06:56:49.000000 performancetest-0.0.17/performancetest/core/cpu.py
--rw-rw-rw-   0        0        0     6451 2023-07-04 03:26:18.000000 performancetest-0.0.17/performancetest/core/device.py
--rw-rw-rw-   0        0        0     4268 2023-06-21 12:46:09.000000 performancetest-0.0.17/performancetest/core/devicebattery.py
--rw-rw-rw-   0        0        0    19366 2023-07-03 10:04:25.000000 performancetest-0.0.17/performancetest/core/fps.py
--rw-rw-rw-   0        0        0      678 2023-06-21 12:46:09.000000 performancetest-0.0.17/performancetest/core/global_data.py
--rw-rw-rw-   0        0        0     3882 2023-06-27 06:56:49.000000 performancetest-0.0.17/performancetest/core/gpu.py
--rw-rw-rw-   0        0        0     6646 2023-06-21 12:47:53.000000 performancetest-0.0.17/performancetest/core/iosperf.py
--rw-rw-rw-   0        0        0     3928 2023-06-27 06:56:49.000000 performancetest-0.0.17/performancetest/core/memory.py
--rw-rw-rw-   0        0        0     4315 2023-06-23 08:54:45.000000 performancetest-0.0.17/performancetest/core/snapshot.py
--rw-rw-rw-   0        0        0     4294 2023-07-10 04:22:56.000000 performancetest-0.0.17/performancetest/core/task_handle.py
-drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.211463 performancetest-0.0.17/performancetest/test/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.17/performancetest/test/__init__.py
--rw-rw-rw-   0        0        0     1133 2023-05-04 05:59:55.000000 performancetest-0.0.17/performancetest/test/all_property_test.py
-drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.232936 performancetest-0.0.17/performancetest/web/
--rw-rw-rw-   0        0        0       25 2023-05-05 12:26:54.000000 performancetest-0.0.17/performancetest/web/__init__.py
--rw-rw-rw-   0        0        0     1852 2023-06-21 12:46:09.000000 performancetest-0.0.17/performancetest/web/dao.py
--rw-rw-rw-   0        0        0      408 2023-06-21 10:25:13.000000 performancetest-0.0.17/performancetest/web/entity.py
--rw-rw-rw-   0        0        0     9209 2023-07-10 03:54:05.000000 performancetest-0.0.17/performancetest/web/main.py
--rw-rw-rw-   0        0        0    11864 2023-06-25 06:05:19.000000 performancetest-0.0.17/performancetest/web/util.py
-drwxrwxrwx   0        0        0        0 2023-07-10 04:29:05.150687 performancetest-0.0.17/performancetest.egg-info/
--rw-rw-rw-   0        0        0      516 2023-07-10 04:29:04.000000 performancetest-0.0.17/performancetest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2023-07-10 04:29:04.000000 performancetest-0.0.17/performancetest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 04:29:04.000000 performancetest-0.0.17/performancetest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-07-10 04:29:04.000000 performancetest-0.0.17/performancetest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-10 04:29:04.000000 performancetest-0.0.17/performancetest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 04:29:05.243670 performancetest-0.0.17/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-07-10 04:28:27.000000 performancetest-0.0.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:44:54.454645 performancetest-0.0.18/
+-rw-rw-rw-   0        0        0      516 2023-07-10 04:44:54.452696 performancetest-0.0.18/PKG-INFO
+-rw-rw-rw-   0        0        0     4346 2023-06-27 05:36:55.000000 performancetest-0.0.18/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 04:44:54.318428 performancetest-0.0.18/performancetest/
+-rw-rw-rw-   0        0        0       49 2023-06-21 09:23:31.000000 performancetest-0.0.18/performancetest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:44:54.423431 performancetest-0.0.18/performancetest/core/
+-rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.18/performancetest/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:44:54.432196 performancetest-0.0.18/performancetest/core/base/
+-rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.18/performancetest/core/base/__init__.py
+-rw-rw-rw-   0        0        0      289 2023-05-04 05:59:55.000000 performancetest-0.0.18/performancetest/core/base/actuator.py
+-rw-rw-rw-   0        0        0      325 2023-05-04 05:59:55.000000 performancetest-0.0.18/performancetest/core/base/monitor.py
+-rw-rw-rw-   0        0        0     3637 2023-07-10 04:22:08.000000 performancetest-0.0.18/performancetest/core/command.py
+-rw-rw-rw-   0        0        0     4277 2023-06-27 06:56:49.000000 performancetest-0.0.18/performancetest/core/cpu.py
+-rw-rw-rw-   0        0        0     6451 2023-07-04 03:26:18.000000 performancetest-0.0.18/performancetest/core/device.py
+-rw-rw-rw-   0        0        0     4268 2023-06-21 12:46:09.000000 performancetest-0.0.18/performancetest/core/devicebattery.py
+-rw-rw-rw-   0        0        0    19375 2023-07-10 04:42:07.000000 performancetest-0.0.18/performancetest/core/fps.py
+-rw-rw-rw-   0        0        0      678 2023-06-21 12:46:09.000000 performancetest-0.0.18/performancetest/core/global_data.py
+-rw-rw-rw-   0        0        0     3882 2023-06-27 06:56:49.000000 performancetest-0.0.18/performancetest/core/gpu.py
+-rw-rw-rw-   0        0        0     6646 2023-06-21 12:47:53.000000 performancetest-0.0.18/performancetest/core/iosperf.py
+-rw-rw-rw-   0        0        0     3928 2023-06-27 06:56:49.000000 performancetest-0.0.18/performancetest/core/memory.py
+-rw-rw-rw-   0        0        0     4315 2023-06-23 08:54:45.000000 performancetest-0.0.18/performancetest/core/snapshot.py
+-rw-rw-rw-   0        0        0     4294 2023-07-10 04:22:56.000000 performancetest-0.0.18/performancetest/core/task_handle.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:44:54.437080 performancetest-0.0.18/performancetest/test/
+-rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.18/performancetest/test/__init__.py
+-rw-rw-rw-   0        0        0     1133 2023-05-04 05:59:55.000000 performancetest-0.0.18/performancetest/test/all_property_test.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:44:54.449762 performancetest-0.0.18/performancetest/web/
+-rw-rw-rw-   0        0        0       25 2023-05-05 12:26:54.000000 performancetest-0.0.18/performancetest/web/__init__.py
+-rw-rw-rw-   0        0        0     1852 2023-06-21 12:46:09.000000 performancetest-0.0.18/performancetest/web/dao.py
+-rw-rw-rw-   0        0        0      408 2023-06-21 10:25:13.000000 performancetest-0.0.18/performancetest/web/entity.py
+-rw-rw-rw-   0        0        0     9209 2023-07-10 03:54:05.000000 performancetest-0.0.18/performancetest/web/main.py
+-rw-rw-rw-   0        0        0    11864 2023-06-25 06:05:19.000000 performancetest-0.0.18/performancetest/web/util.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:44:54.365271 performancetest-0.0.18/performancetest.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-07-10 04:44:54.000000 performancetest-0.0.18/performancetest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      959 2023-07-10 04:44:54.000000 performancetest-0.0.18/performancetest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 04:44:54.000000 performancetest-0.0.18/performancetest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-07-10 04:44:54.000000 performancetest-0.0.18/performancetest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-10 04:44:54.000000 performancetest-0.0.18/performancetest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 04:44:54.455622 performancetest-0.0.18/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-07-10 04:44:30.000000 performancetest-0.0.18/setup.py
```

### Comparing `performancetest-0.0.17/PKG-INFO` & `performancetest-0.0.18/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: performancetest
-Version: 0.0.17
+Version: 0.0.18
 Summary: Android, IOS app_performance
 Home-page: https://github.com/1033866383/perf-orange-cat
 Author: bozhou.fan
 Author-email: 15525730080@163.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `performancetest-0.0.17/README.md` & `performancetest-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/core/command.py` & `performancetest-0.0.18/performancetest/core/command.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/core/cpu.py` & `performancetest-0.0.18/performancetest/core/cpu.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/core/device.py` & `performancetest-0.0.18/performancetest/core/device.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/core/devicebattery.py` & `performancetest-0.0.18/performancetest/core/devicebattery.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/core/fps.py` & `performancetest-0.0.18/performancetest/core/fps.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
                 self.m_surface_view_name = i.strip()
         logger.info("获取到的surface_view信息是：{}".format(self.m_surface_view_name))
 
     def get_surfaceview_activity(self):
         activity_name = ''
         activity_line = ''
         try:
-            dumpsys_result = G.device.adb.raw_shell('dumpsys SurfaceFlinger --list | {} {}'.format(('grep', 'findstr')[platform.system() == "Windows"], G.device.package))
+            dumpsys_result = G.device.adb.raw_shell('dumpsys SurfaceFlinger --list | {} {}'.format(('grep', 'findstr')[platform.system() == "Windows"], G.device.package)).decode()
             dumpsys_result_list = dumpsys_result.split('\n')
             for line in dumpsys_result_list:
                 if line.startswith('SurfaceView') and line.find(G.device.package) != -1:
                     activity_line = line.strip()
                     break
             if activity_line:
                 if activity_line.find(' ') != -1:
```

### Comparing `performancetest-0.0.17/performancetest/core/global_data.py` & `performancetest-0.0.18/performancetest/core/global_data.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/core/gpu.py` & `performancetest-0.0.18/performancetest/core/gpu.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/core/iosperf.py` & `performancetest-0.0.18/performancetest/core/iosperf.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/core/memory.py` & `performancetest-0.0.18/performancetest/core/memory.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/core/snapshot.py` & `performancetest-0.0.18/performancetest/core/snapshot.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/core/task_handle.py` & `performancetest-0.0.18/performancetest/core/task_handle.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/test/all_property_test.py` & `performancetest-0.0.18/performancetest/test/all_property_test.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/web/dao.py` & `performancetest-0.0.18/performancetest/web/dao.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/web/main.py` & `performancetest-0.0.18/performancetest/web/main.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest/web/util.py` & `performancetest-0.0.18/performancetest/web/util.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/performancetest.egg-info/PKG-INFO` & `performancetest-0.0.18/performancetest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: performancetest
-Version: 0.0.17
+Version: 0.0.18
 Summary: Android, IOS app_performance
 Home-page: https://github.com/1033866383/perf-orange-cat
 Author: bozhou.fan
 Author-email: 15525730080@163.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `performancetest-0.0.17/performancetest.egg-info/SOURCES.txt` & `performancetest-0.0.18/performancetest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.17/setup.py` & `performancetest-0.0.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # # _*_ coding: utf-8 _*_
 from setuptools import setup, find_packages
 
 setup(
        name='performancetest',
-       version='0.0.17',
+       version='0.0.18',
        url='https://github.com/1033866383/perf-orange-cat',
        author='bozhou.fan',
        author_email='15525730080@163.com',
        description='Android, IOS app_performance',
        packages=find_packages(),
        install_requires=[
            "psutil", "airtest", "fastapi", "tidevice", "func-timeout", "sqlalchemy", "sqlalchemy-serializer", "uvicorn"
```

