# Comparing `tmp/androtools-0.1.2.tar.gz` & `tmp/androtools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "androtools-0.1.2.tar", max compression
+gzip compressed data, was "androtools-0.1.3.tar", max compression
```

## Comparing `androtools-0.1.2.tar` & `androtools-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.2/LICENSE
--rw-r--r--   0        0        0      680 2023-07-07 07:04:49.932174 androtools-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.2/androtools/__init__.py
--rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.2/androtools/__main__.py
--rw-r--r--   0        0        0     1808 2023-06-30 08:37:58.985005 androtools-0.1.2/androtools/android_sdk/__init__.py
--rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.2/androtools/android_sdk/build_tools.py
--rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.2/androtools/android_sdk/emulator.py
--rw-r--r--   0        0        0     3148 2023-07-07 09:32:34.474354 androtools-0.1.2/androtools/android_sdk/platform_tools.py
--rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.2/androtools/android_sdk/tools.py
--rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.2/androtools/core/__init__.py
--rw-r--r--   0        0        0     7508 2023-07-07 09:35:52.554824 androtools-0.1.2/androtools/core/device.py
--rw-r--r--   0        0        0      791 2023-07-07 09:35:59.039728 androtools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1624 1970-01-01 00:00:00.000000 androtools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-19 09:41:52.401698 androtools-0.1.3/LICENSE
+-rw-r--r--   0        0        0      509 2023-07-10 02:24:06.729804 androtools-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 09:44:13.647842 androtools-0.1.3/androtools/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-19 10:26:22.117797 androtools-0.1.3/androtools/__main__.py
+-rw-r--r--   0        0        0     1808 2023-06-30 08:37:58.985005 androtools-0.1.3/androtools/android_sdk/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-30 08:38:11.610147 androtools-0.1.3/androtools/android_sdk/build_tools.py
+-rw-r--r--   0        0        0        0 2023-06-19 10:27:54.144068 androtools-0.1.3/androtools/android_sdk/emulator.py
+-rw-r--r--   0        0        0     3148 2023-07-07 09:32:34.474354 androtools-0.1.3/androtools/android_sdk/platform_tools.py
+-rw-r--r--   0        0        0      407 2023-06-19 10:35:05.259843 androtools-0.1.3/androtools/android_sdk/tools.py
+-rw-r--r--   0        0        0      169 2023-07-07 09:33:48.479529 androtools-0.1.3/androtools/core/__init__.py
+-rw-r--r--   0        0        0     7508 2023-07-07 09:35:52.554824 androtools-0.1.3/androtools/core/device.py
+-rw-r--r--   0        0        0      889 2023-07-10 02:24:50.460839 androtools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 androtools-0.1.3/PKG-INFO
```

### Comparing `androtools-0.1.2/LICENSE` & `androtools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `androtools-0.1.2/androtools/android_sdk/__init__.py` & `androtools-0.1.3/androtools/android_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.2/androtools/android_sdk/build_tools.py` & `androtools-0.1.3/androtools/android_sdk/build_tools.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.2/androtools/android_sdk/platform_tools.py` & `androtools-0.1.3/androtools/android_sdk/platform_tools.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.2/androtools/core/device.py` & `androtools-0.1.3/androtools/core/device.py`

 * *Files identical despite different names*

### Comparing `androtools-0.1.2/PKG-INFO` & `androtools-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: androtools
-Version: 0.1.2
-Summary: 
+Version: 0.1.3
+Summary: 一个对Android SDK相关的命令封装的库
+Home-page: https://gitee.com/kin9-0rz/apkutils
 License: MIT
 Author: kin9-0rz
 Author-email: kin9-0rz@outlook.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
@@ -17,23 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
+Project-URL: Repository, https://gitee.com/kin9-0rz/apkutils
 Description-Content-Type: text/markdown
 
 # androtools
 
-[![PyPI](https://img.shields.io/pypi/v/androtools?style=for-the-badge)](https://pypi.org/project/androtools/) ![PyPI - Status](https://img.shields.io/pypi/status/androtools?style=for-the-badge) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/androtools?style=for-the-badge)  ![PyPI - Downloads](https://img.shields.io/pypi/dw/androtools?style=for-the-badge) ![PyPI - License](https://img.shields.io/pypi/l/androtools?style=for-the-badge)
+[![PyPI](https://img.shields.io/pypi/v/androtools?style=flat-square)](https://pypi.org/project/androtools/) ![PyPI - Status](https://img.shields.io/pypi/status/androtools?style=flat-square) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/androtools?style=flat-square)  ![PyPI - Downloads](https://img.shields.io/pypi/dw/androtools?style=flat-square) ![PyPI - License](https://img.shields.io/pypi/l/androtools?style=flat-square)
 
-- 命令封装
-    - 优先 adb
-- 业务逻辑封装，business
-- adb 连接多个模拟器
-  - usb 的方式
-  - 本地模拟器
-  - 稳定连接
-
-参考：
-- https://github.com/Genymobile/scrcpy，控制手机
+一个对Android SDK相关的命令封装的库。
```

