# Comparing `tmp/androtools-0.1.5.tar.gz` & `tmp/androtools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "androtools-0.1.5.tar", max compression
+gzip compressed data, was "androtools-0.1.6.tar", max compression
```

## Comparing `androtools-0.1.5.tar` & `androtools-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.5/LICENSE
--rw-r--r--   0        0        0      509 2023-07-10 07:45:39.944213 androtools-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.5/androtools/__init__.py
--rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.5/androtools/__main__.py
--rw-r--r--   0        0        0     1808 2023-06-30 08:37:58.985005 androtools-0.1.5/androtools/android_sdk/__init__.py
--rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.5/androtools/android_sdk/build_tools.py
--rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.5/androtools/android_sdk/emulator.py
--rw-r--r--   0        0        0     3148 2023-07-07 09:32:34.474354 androtools-0.1.5/androtools/android_sdk/platform_tools.py
--rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.5/androtools/android_sdk/tools.py
--rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.5/androtools/core/__init__.py
--rw-r--r--   0        0        0     8246 2023-07-10 07:50:33.481661 androtools-0.1.5/androtools/core/device.py
--rw-r--r--   0        0        0      889 2023-07-10 07:51:00.995522 androtools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 androtools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.6/LICENSE
+-rw-r--r--   0        0        0      509 2023-07-10 07:45:39.944213 androtools-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.6/androtools/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.6/androtools/__main__.py
+-rw-r--r--   0        0        0     1808 2023-06-30 08:37:58.985005 androtools-0.1.6/androtools/android_sdk/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.6/androtools/android_sdk/build_tools.py
+-rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.6/androtools/android_sdk/emulator.py
+-rw-r--r--   0        0        0     3148 2023-07-07 09:32:34.474354 androtools-0.1.6/androtools/android_sdk/platform_tools.py
+-rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.6/androtools/android_sdk/tools.py
+-rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.6/androtools/core/__init__.py
+-rw-r--r--   0        0        0     8205 2023-07-10 07:57:12.593185 androtools-0.1.6/androtools/core/device.py
+-rw-r--r--   0        0        0      889 2023-07-10 07:57:34.778381 androtools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 androtools-0.1.6/PKG-INFO
```

### Comparing `androtools-0.1.5/LICENSE` & `androtools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `androtools-0.1.5/androtools/android_sdk/__init__.py` & `androtools-0.1.6/androtools/android_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.5/androtools/android_sdk/build_tools.py` & `androtools-0.1.6/androtools/android_sdk/build_tools.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.5/androtools/android_sdk/platform_tools.py` & `androtools-0.1.6/androtools/android_sdk/platform_tools.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.5/androtools/core/device.py` & `androtools-0.1.6/androtools/core/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     def _is_offline(self):
         output, error = self.adb.run_cmd(["get-state"])
         # output: ['device']
         # error: error: device offline
         # error: device 'emulator-5556' not found
         if f"error: device '{self.name}' not found" in error:
             logging.error(f"device '{self.name}' not found")
-            raise RuntimeError(f"device '{self.name}' not found")
+            return False
         return "device" not in output
 
     def _init_sdk(self):
         output, error = self.adb.run_shell_cmd(["getprop", "ro.build.version.sdk"])
         if isinstance(output, str):
             self.sdk = int(output)
         elif isinstance(output, list):
```

### Comparing `androtools-0.1.5/pyproject.toml` & `androtools-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "androtools"
-version = "0.1.5"
+version = "0.1.6"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Natural Language :: Chinese (Simplified)",
```

### Comparing `androtools-0.1.5/PKG-INFO` & `androtools-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: androtools
-Version: 0.1.5
+Version: 0.1.6
 Summary: 一个对Android SDK相关的命令封装的库
 Home-page: https://gitee.com/kin9-0rz/apkutils
 License: MIT
 Author: kin9-0rz
 Author-email: kin9-0rz@outlook.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
```

