# Comparing `tmp/androtools-0.1.8.tar.gz` & `tmp/androtools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "androtools-0.1.8.tar", max compression
+gzip compressed data, was "androtools-0.1.9.tar", max compression
```

## Comparing `androtools-0.1.8.tar` & `androtools-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.8/LICENSE
--rw-r--r--   0        0        0      509 2023-07-10 07:45:39.944213 androtools-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.8/androtools/__init__.py
--rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.8/androtools/__main__.py
--rw-r--r--   0        0        0     1808 2023-06-30 08:37:58.985005 androtools-0.1.8/androtools/android_sdk/__init__.py
--rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.8/androtools/android_sdk/build_tools.py
--rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.8/androtools/android_sdk/emulator.py
--rw-r--r--   0        0        0     3258 2023-07-10 08:09:07.675769 androtools-0.1.8/androtools/android_sdk/platform_tools.py
--rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.8/androtools/android_sdk/tools.py
--rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.8/androtools/core/__init__.py
--rw-r--r--   0        0        0     8551 2023-07-10 08:26:19.575847 androtools-0.1.8/androtools/core/device.py
--rw-r--r--   0        0        0      889 2023-07-10 08:26:28.879886 androtools-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 androtools-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.9/LICENSE
+-rw-r--r--   0        0        0      509 2023-07-10 07:45:39.944213 androtools-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.9/androtools/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.9/androtools/__main__.py
+-rw-r--r--   0        0        0     1894 2023-07-10 10:28:37.824161 androtools-0.1.9/androtools/android_sdk/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.9/androtools/android_sdk/build_tools.py
+-rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.9/androtools/android_sdk/emulator.py
+-rw-r--r--   0        0        0     3314 2023-07-10 10:32:54.929659 androtools-0.1.9/androtools/android_sdk/platform_tools.py
+-rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.9/androtools/android_sdk/tools.py
+-rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.9/androtools/core/__init__.py
+-rw-r--r--   0        0        0     8650 2023-07-10 10:33:09.809716 androtools-0.1.9/androtools/core/device.py
+-rw-r--r--   0        0        0      889 2023-07-10 10:33:59.693867 androtools-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 androtools-0.1.9/PKG-INFO
```

### Comparing `androtools-0.1.8/LICENSE` & `androtools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `androtools-0.1.8/androtools/android_sdk/__init__.py` & `androtools-0.1.9/androtools/android_sdk/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import logging
+import os
 import shutil
 import subprocess
 from enum import Enum
 
 
 class SubSubCommand(Enum):
     """命令的子命令的子命令"""
 
     pass
 
 
 class CMD:
-    def __init__(self, path) -> None:
-        self.bin_path = shutil.which(path)
+    def __init__(self, path: str) -> None:
+        assert isinstance(path, str)
+        self.bin_path = path if os.path.exists(path) else shutil.which(path)
 
     def _build_cmds(self, cmd: list):
         return [self.bin_path] + cmd
 
     def _run(self, cmd: list, shell: bool = False):
         """运行阻塞命令"""
         assert isinstance(cmd, list)
```

### Comparing `androtools-0.1.8/androtools/android_sdk/build_tools.py` & `androtools-0.1.9/androtools/android_sdk/build_tools.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.8/androtools/android_sdk/platform_tools.py` & `androtools-0.1.9/androtools/android_sdk/platform_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,17 @@
     Raises:
         ValueError: _description_
 
     Returns:
         _type_: _description_
     """
 
-    def __init__(self, path=shutil.which("adb")) -> None:
+    def __init__(self, path: str = None) -> None:
+        if path is None:
+            path = shutil.which("adb")
         super().__init__(path)
         self._cmd_target_device = []
 
     def run_cmd(self, cmd: list):
         assert isinstance(cmd, list)
         logging.debug("run_cmd: %s", cmd)
         return self._run(cmd)
```

### Comparing `androtools-0.1.8/androtools/core/device.py` & `androtools-0.1.9/androtools/core/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,22 @@
 class TRANSPORT(Enum):
     USB = "usb"
     LOCAL = "local"
     ANY = "any"
 
 
 class Device:
-    def __init__(self, device_name, device_type: DeviceType = DeviceType.Serial):
+    def __init__(
+        self,
+        device_name,
+        device_type: DeviceType = DeviceType.Serial,
+        adb_path: str = None,
+    ):
         self.name = device_name
-        self.adb = ADB()
+        self.adb = ADB(adb_path)
         self.adb.set_target_device(device_name, device_type)
 
         counter = 0
         while self._is_offline():
             if ":" in self.name:  # 如果是网络设备，不等待
                 raise RuntimeError("device offline")
 
@@ -237,16 +242,16 @@
 
 class DeviceState:
     Free = 0
     Busy = 1
 
 
 class DeviceManager:
-    def __init__(self, force: bool = False):
-        self._adb = ADB()
+    def __init__(self, adb_path: str = None, force: bool = False):
+        self._adb = ADB(adb_path)
         self._adb.restart_server(force)
         self._devices = {}
         self.update()
 
     def get_total(self) -> int:
         return len(self._devices)
```

### Comparing `androtools-0.1.8/pyproject.toml` & `androtools-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "androtools"
-version = "0.1.8"
+version = "0.1.9"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Natural Language :: Chinese (Simplified)",
```

### Comparing `androtools-0.1.8/PKG-INFO` & `androtools-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: androtools
-Version: 0.1.8
+Version: 0.1.9
 Summary: 一个对Android SDK相关的命令封装的库
 Home-page: https://gitee.com/kin9-0rz/apkutils
 License: MIT
 Author: kin9-0rz
 Author-email: kin9-0rz@outlook.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
```

