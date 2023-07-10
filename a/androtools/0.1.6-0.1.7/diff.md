# Comparing `tmp/androtools-0.1.6.tar.gz` & `tmp/androtools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "androtools-0.1.6.tar", max compression
+gzip compressed data, was "androtools-0.1.7.tar", max compression
```

## Comparing `androtools-0.1.6.tar` & `androtools-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.6/LICENSE
--rw-r--r--   0        0        0      509 2023-07-10 07:45:39.944213 androtools-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.6/androtools/__init__.py
--rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.6/androtools/__main__.py
--rw-r--r--   0        0        0     1808 2023-06-30 08:37:58.985005 androtools-0.1.6/androtools/android_sdk/__init__.py
--rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.6/androtools/android_sdk/build_tools.py
--rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.6/androtools/android_sdk/emulator.py
--rw-r--r--   0        0        0     3148 2023-07-07 09:32:34.474354 androtools-0.1.6/androtools/android_sdk/platform_tools.py
--rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.6/androtools/android_sdk/tools.py
--rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.6/androtools/core/__init__.py
--rw-r--r--   0        0        0     8205 2023-07-10 07:57:12.593185 androtools-0.1.6/androtools/core/device.py
--rw-r--r--   0        0        0      889 2023-07-10 07:57:34.778381 androtools-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 androtools-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.7/LICENSE
+-rw-r--r--   0        0        0      509 2023-07-10 07:45:39.944213 androtools-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.7/androtools/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.7/androtools/__main__.py
+-rw-r--r--   0        0        0     1808 2023-06-30 08:37:58.985005 androtools-0.1.7/androtools/android_sdk/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.7/androtools/android_sdk/build_tools.py
+-rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.7/androtools/android_sdk/emulator.py
+-rw-r--r--   0        0        0     3258 2023-07-10 08:09:07.675769 androtools-0.1.7/androtools/android_sdk/platform_tools.py
+-rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.7/androtools/android_sdk/tools.py
+-rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.7/androtools/core/__init__.py
+-rw-r--r--   0        0        0     8229 2023-07-10 08:09:30.967661 androtools-0.1.7/androtools/core/device.py
+-rw-r--r--   0        0        0      889 2023-07-10 08:10:12.776123 androtools-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 androtools-0.1.7/PKG-INFO
```

### Comparing `androtools-0.1.6/LICENSE` & `androtools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `androtools-0.1.6/androtools/android_sdk/__init__.py` & `androtools-0.1.7/androtools/android_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.6/androtools/android_sdk/build_tools.py` & `androtools-0.1.7/androtools/android_sdk/build_tools.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.6/androtools/android_sdk/platform_tools.py` & `androtools-0.1.7/androtools/android_sdk/platform_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,19 @@
                 self._cmd_target_device.append(device_name)
 
     def run_shell_cmd(self, cmd: list):
         assert isinstance(cmd, list)
         return self.run_cmd(self._cmd_target_device + ["shell"] + cmd)
 
     def get_devices(self):
-        output, error = self.run_cmd(["devices", "-l"])
+        self.run_cmd(["devices", "-l"])
+        sleep(1)
+        self.run_cmd(["devices", "-l"])
+        sleep(1)
+        output, _ = self.run_cmd(["devices", "-l"])
         devices = []
         transport_ids = []
 
         lines = output.strip().splitlines()
         if len(lines) <= 1:
             return None, None
```

### Comparing `androtools-0.1.6/androtools/core/device.py` & `androtools-0.1.7/androtools/core/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,18 +232,18 @@
 class DeviceManager:
     def __init__(self, force: bool = False):
         self._adb = ADB()
         self._adb.restart_server(force)
         self._devices = {}
         self.update()
 
-    def get_total(self):
+    def get_total(self) -> int:
         return len(self._devices)
 
-    def get_free_device(self):
+    def get_free_device(self) -> Device | None:
         for device in self._devices:
             if self._devices[device] == DeviceState.Free:
                 self._devices[device] = DeviceState.Busy
                 logging.debug(f"free device: {device}")
                 return device
 
     def free_busy_device(self, device: Device):
```

### Comparing `androtools-0.1.6/pyproject.toml` & `androtools-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "androtools"
-version = "0.1.6"
+version = "0.1.7"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Natural Language :: Chinese (Simplified)",
```

### Comparing `androtools-0.1.6/PKG-INFO` & `androtools-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: androtools
-Version: 0.1.6
+Version: 0.1.7
 Summary: 一个对Android SDK相关的命令封装的库
 Home-page: https://gitee.com/kin9-0rz/apkutils
 License: MIT
 Author: kin9-0rz
 Author-email: kin9-0rz@outlook.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
```

