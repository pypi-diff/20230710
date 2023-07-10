# Comparing `tmp/androtools-0.1.4.tar.gz` & `tmp/androtools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "androtools-0.1.4.tar", max compression
+gzip compressed data, was "androtools-0.1.5.tar", max compression
```

## Comparing `androtools-0.1.4.tar` & `androtools-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.4/LICENSE
--rw-r--r--   0        0        0      509 2023-07-10 02:24:06.729804 androtools-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.4/androtools/__init__.py
--rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.4/androtools/__main__.py
--rw-r--r--   0        0        0     1808 2023-06-30 08:37:58.985005 androtools-0.1.4/androtools/android_sdk/__init__.py
--rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.4/androtools/android_sdk/build_tools.py
--rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.4/androtools/android_sdk/emulator.py
--rw-r--r--   0        0        0     3148 2023-07-07 09:32:34.474354 androtools-0.1.4/androtools/android_sdk/platform_tools.py
--rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.4/androtools/android_sdk/tools.py
--rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.4/androtools/core/__init__.py
--rw-r--r--   0        0        0     7526 2023-07-10 03:22:44.635778 androtools-0.1.4/androtools/core/device.py
--rw-r--r--   0        0        0      889 2023-07-10 03:33:03.885278 androtools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 androtools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.5/LICENSE
+-rw-r--r--   0        0        0      509 2023-07-10 07:45:39.944213 androtools-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.5/androtools/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.5/androtools/__main__.py
+-rw-r--r--   0        0        0     1808 2023-06-30 08:37:58.985005 androtools-0.1.5/androtools/android_sdk/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.5/androtools/android_sdk/build_tools.py
+-rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.5/androtools/android_sdk/emulator.py
+-rw-r--r--   0        0        0     3148 2023-07-07 09:32:34.474354 androtools-0.1.5/androtools/android_sdk/platform_tools.py
+-rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.5/androtools/android_sdk/tools.py
+-rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.5/androtools/core/__init__.py
+-rw-r--r--   0        0        0     8246 2023-07-10 07:50:33.481661 androtools-0.1.5/androtools/core/device.py
+-rw-r--r--   0        0        0      889 2023-07-10 07:51:00.995522 androtools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 androtools-0.1.5/PKG-INFO
```

### Comparing `androtools-0.1.4/LICENSE` & `androtools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `androtools-0.1.4/androtools/android_sdk/__init__.py` & `androtools-0.1.5/androtools/android_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.4/androtools/android_sdk/build_tools.py` & `androtools-0.1.5/androtools/android_sdk/build_tools.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.4/androtools/android_sdk/platform_tools.py` & `androtools-0.1.5/androtools/android_sdk/platform_tools.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.4/androtools/core/device.py` & `androtools-0.1.5/androtools/core/device.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from enum import Enum
 from time import sleep
 
 from androtools.android_sdk.platform_tools import ADB, DeviceType
 
 # API等级，SDK，CodeName
 # https://apilevels.com/
 Android_API_MAP = {
@@ -26,14 +27,29 @@
     31: ("Android 12", "Snow Cone"),
     32: ("Android 12L", "Snow Cone"),
     33: ("Android 13", "TIRAMISU"),
     34: ("Android 14", "Upside Down Cake"),
 }
 
 
+class STATE(Enum):
+    DEVICE = "device"
+    RECOVERY = "recovery"
+    RESCUE = "rescue"
+    SIDELOADING = "sideload"
+    BOOTLOADER = "bootloader"
+    DISCONNECT = "disconnect"
+
+
+class TRANSPORT(Enum):
+    USB = "usb"
+    LOCAL = "local"
+    ANY = "any"
+
+
 class Device:
     def __init__(self, device_name, device_type: DeviceType = DeviceType.Serial):
         self.name = device_name
         self.adb = ADB()
         self.adb.set_target_device(device_name, device_type)
 
         counter = 0
@@ -106,14 +122,22 @@
         output = "".join(output)
         if "pulled" in output:
             return True
         logging.error("".join(cmd))
         logging.error(output)
         logging.error(error)
 
+    def wait_for(self, state: STATE, transport: TRANSPORT = TRANSPORT.ANY):
+        cmd = "wait-for"
+        if transport != TRANSPORT.ANY:
+            cmd += f"-{transport.value}"
+        cmd += f"-{state}"
+        output, error = self.adb.run_cmd([cmd])
+        return output, error
+
     # ------------------------------- am 命令，控制应用 ------------------------------ #
 
     def start_activity(self, package_name, activity_name):
         # adb shell am start -n com.example.myapp/com.example.myapp.MainActivity
         cmd = ["am", "start", "-n", f"{package_name}/{activity_name}"]
         self.adb.run_shell_cmd(cmd)
 
@@ -149,14 +173,24 @@
         output, _ = self.adb.run_shell_cmd(["killall", process_name])
         return output
 
     def kill(self, pid):
         cmd = ["kill", str(pid)]
         self.adb.run_shell_cmd(cmd)
 
+    def reboot(self, seconds: int = 60):
+        self.adb.run_shell_cmd(["reboot"])
+        self.wait_for(STATE.DEVICE)
+
+        count = 0
+        while self._is_offline():
+            count += 1
+            if count > seconds:
+                break
+
     # ------------------------------ dumpsys command ----------------------------- #
 
     def dumpsys_window_windows(self):
         # adb shell dumpsys window windows | grep -E 'mCurrentFocus|mFocusedApp'
         cmd = ["dumpsys", "window", "windows"]
         output, _ = self.adb.run_shell_cmd(cmd)
         return output
@@ -166,26 +200,24 @@
     def tap(self, x, y):
         cmd = ["input", "tap", str(x), str(y)]
         self.adb.run_shell_cmd(cmd)
         # 点击太快,模拟器可能反应不过来.
         sleep(1)
 
     def home(self):
-        # adb shell input keyevent KEYCODE_HOME
         cmd = ["input", "keyevent", "KEYCODE_HOME"]
         self.adb.run_shell_cmd(cmd)
         sleep(1)
 
     def swipe(self, x1, y1, x2, y2):
         cmd = ["input", "swipe", str(x1), str(y1), str(x2), str(y2)]
         self.adb.run_shell_cmd(cmd)
         sleep(1)
 
     def back(self):
-        # adb shell input keyevent KEYCODE_BACK
         cmd = ["input", "keyevent", "KEYCODE_BACK"]
         self.adb.run_shell_cmd(cmd)
         sleep(1)
 
     # TODO 清理最近的任务，有可能高级版本才支持
     # adb shell input keyevent KEYCODE_APP_SWITCH
     # && sleep 1 &&
```

### Comparing `androtools-0.1.4/pyproject.toml` & `androtools-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "androtools"
-version = "0.1.4"
+version = "0.1.5"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Natural Language :: Chinese (Simplified)",
```

### Comparing `androtools-0.1.4/PKG-INFO` & `androtools-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: androtools
-Version: 0.1.4
+Version: 0.1.5
 Summary: 一个对Android SDK相关的命令封装的库
 Home-page: https://gitee.com/kin9-0rz/apkutils
 License: MIT
 Author: kin9-0rz
 Author-email: kin9-0rz@outlook.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
```

