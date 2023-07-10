# Comparing `tmp/androtools-0.1.3.tar.gz` & `tmp/androtools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "androtools-0.1.3.tar", max compression
+gzip compressed data, was "androtools-0.1.4.tar", max compression
```

## Comparing `androtools-0.1.3.tar` & `androtools-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.3/LICENSE
--rw-r--r--   0        0        0      509 2023-07-10 02:24:06.729804 androtools-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.3/androtools/__init__.py
--rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.3/androtools/__main__.py
--rw-r--r--   0        0        0     1808 2023-06-30 08:37:58.985005 androtools-0.1.3/androtools/android_sdk/__init__.py
--rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.3/androtools/android_sdk/build_tools.py
--rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.3/androtools/android_sdk/emulator.py
--rw-r--r--   0        0        0     3148 2023-07-07 09:32:34.474354 androtools-0.1.3/androtools/android_sdk/platform_tools.py
--rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.3/androtools/android_sdk/tools.py
--rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.3/androtools/core/__init__.py
--rw-r--r--   0        0        0     7508 2023-07-07 09:35:52.554824 androtools-0.1.3/androtools/core/device.py
--rw-r--r--   0        0        0      889 2023-07-10 02:24:50.460839 androtools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 androtools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.4/LICENSE
+-rw-r--r--   0        0        0      509 2023-07-10 02:24:06.729804 androtools-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.4/androtools/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.4/androtools/__main__.py
+-rw-r--r--   0        0        0     1808 2023-06-30 08:37:58.985005 androtools-0.1.4/androtools/android_sdk/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.4/androtools/android_sdk/build_tools.py
+-rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.4/androtools/android_sdk/emulator.py
+-rw-r--r--   0        0        0     3148 2023-07-07 09:32:34.474354 androtools-0.1.4/androtools/android_sdk/platform_tools.py
+-rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.4/androtools/android_sdk/tools.py
+-rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.4/androtools/core/__init__.py
+-rw-r--r--   0        0        0     7526 2023-07-10 03:22:44.635778 androtools-0.1.4/androtools/core/device.py
+-rw-r--r--   0        0        0      889 2023-07-10 03:33:03.885278 androtools-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 androtools-0.1.4/PKG-INFO
```

### Comparing `androtools-0.1.3/LICENSE` & `androtools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `androtools-0.1.3/androtools/android_sdk/__init__.py` & `androtools-0.1.4/androtools/android_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.3/androtools/android_sdk/build_tools.py` & `androtools-0.1.4/androtools/android_sdk/build_tools.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.3/androtools/android_sdk/platform_tools.py` & `androtools-0.1.4/androtools/android_sdk/platform_tools.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.3/androtools/core/device.py` & `androtools-0.1.4/androtools/core/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,25 +71,29 @@
             self.sdk = int(output)
         elif isinstance(output, list):
             self.sdk = int(output[0])
         return self.sdk
 
     # ---------------------------------- adb 命令 ---------------------------------- #
 
-    def install_apk(self, apk_path):
+    def install_apk(self, apk_path: str):
+        """安装apk
+
+        Args:
+            apk_path (str): apk 路径
+
+        Returns:
+            tuple: (is_success, output)
+        """
         cmd = ["install", "-r", "-g", "-t", apk_path]
         if self.sdk < 26:
             cmd = ["install", "-r", "-t", apk_path]
-        output, error = self.adb.run_cmd(cmd)
-        if "Success" in output:
-            return True
-        logging.error("".join(cmd))
-        logging.error(output)
-        logging.error(error)
-        return False
+        output, _ = self.adb.run_cmd(cmd)
+
+        return "Success" in output, output
 
     def uninstall_apk(self, package_name):
         cmd = ["uninstall", package_name]
         output, error = self.adb.run_cmd(cmd)
         if "Success" in output:
             return True
         logging.error("".join(cmd))
```

### Comparing `androtools-0.1.3/pyproject.toml` & `androtools-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "androtools"
-version = "0.1.3"
+version = "0.1.4"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Natural Language :: Chinese (Simplified)",
```

### Comparing `androtools-0.1.3/PKG-INFO` & `androtools-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: androtools
-Version: 0.1.3
+Version: 0.1.4
 Summary: 一个对Android SDK相关的命令封装的库
 Home-page: https://gitee.com/kin9-0rz/apkutils
 License: MIT
 Author: kin9-0rz
 Author-email: kin9-0rz@outlook.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
```

