# Comparing `tmp/androtools-0.1.7.tar.gz` & `tmp/androtools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "androtools-0.1.7.tar", max compression
+gzip compressed data, was "androtools-0.1.8.tar", max compression
```

## Comparing `androtools-0.1.7.tar` & `androtools-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.7/LICENSE
--rw-r--r--   0        0        0      509 2023-07-10 07:45:39.944213 androtools-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.7/androtools/__init__.py
--rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.7/androtools/__main__.py
--rw-r--r--   0        0        0     1808 2023-06-30 08:37:58.985005 androtools-0.1.7/androtools/android_sdk/__init__.py
--rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.7/androtools/android_sdk/build_tools.py
--rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.7/androtools/android_sdk/emulator.py
--rw-r--r--   0        0        0     3258 2023-07-10 08:09:07.675769 androtools-0.1.7/androtools/android_sdk/platform_tools.py
--rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.7/androtools/android_sdk/tools.py
--rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.7/androtools/core/__init__.py
--rw-r--r--   0        0        0     8229 2023-07-10 08:09:30.967661 androtools-0.1.7/androtools/core/device.py
--rw-r--r--   0        0        0      889 2023-07-10 08:10:12.776123 androtools-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 androtools-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.8/LICENSE
+-rw-r--r--   0        0        0      509 2023-07-10 07:45:39.944213 androtools-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.8/androtools/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.8/androtools/__main__.py
+-rw-r--r--   0        0        0     1808 2023-06-30 08:37:58.985005 androtools-0.1.8/androtools/android_sdk/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.8/androtools/android_sdk/build_tools.py
+-rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.8/androtools/android_sdk/emulator.py
+-rw-r--r--   0        0        0     3258 2023-07-10 08:09:07.675769 androtools-0.1.8/androtools/android_sdk/platform_tools.py
+-rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.8/androtools/android_sdk/tools.py
+-rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.8/androtools/core/__init__.py
+-rw-r--r--   0        0        0     8551 2023-07-10 08:26:19.575847 androtools-0.1.8/androtools/core/device.py
+-rw-r--r--   0        0        0      889 2023-07-10 08:26:28.879886 androtools-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 androtools-0.1.8/PKG-INFO
```

### Comparing `androtools-0.1.7/LICENSE` & `androtools-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `androtools-0.1.7/androtools/android_sdk/__init__.py` & `androtools-0.1.8/androtools/android_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.7/androtools/android_sdk/build_tools.py` & `androtools-0.1.8/androtools/android_sdk/build_tools.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.7/androtools/android_sdk/platform_tools.py` & `androtools-0.1.8/androtools/android_sdk/platform_tools.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.7/androtools/core/device.py` & `androtools-0.1.8/androtools/core/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,25 @@
 
         count = 0
         while self._is_offline():
             count += 1
             if count > seconds:
                 break
 
+        while True:
+            if self.is_boot_completed():
+                break
+            sleep(1)
+        sleep(3)
+
+    def is_boot_completed(self) -> bool:
+        """判断设备是否处于开机状态"""
+        output, _ = self.adb.run_shell_cmd(["getprop", "sys.boot_completed"])
+        return "1" in output
+
     # ------------------------------ dumpsys command ----------------------------- #
 
     def dumpsys_window_windows(self):
         # adb shell dumpsys window windows | grep -E 'mCurrentFocus|mFocusedApp'
         cmd = ["dumpsys", "window", "windows"]
         output, _ = self.adb.run_shell_cmd(cmd)
         return output
```

### Comparing `androtools-0.1.7/pyproject.toml` & `androtools-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "androtools"
-version = "0.1.7"
+version = "0.1.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Natural Language :: Chinese (Simplified)",
```

### Comparing `androtools-0.1.7/PKG-INFO` & `androtools-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: androtools
-Version: 0.1.7
+Version: 0.1.8
 Summary: 一个对Android SDK相关的命令封装的库
 Home-page: https://gitee.com/kin9-0rz/apkutils
 License: MIT
 Author: kin9-0rz
 Author-email: kin9-0rz@outlook.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
```

