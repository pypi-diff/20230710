# Comparing `tmp/lvhao_lib-0.3.0.tar.gz` & `tmp/lvhao_lib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lvhao_lib-0.3.0.tar", max compression
+gzip compressed data, was "lvhao_lib-0.7.0.tar", max compression
```

## Comparing `lvhao_lib-0.3.0.tar` & `lvhao_lib-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-07-10 02:55:19.579447 lvhao_lib-0.3.0/README.md
--rw-r--r--   0        0        0  1368592 2023-07-06 23:47:26.000000 lvhao_lib-0.3.0/lib/linux_x86_64/libpnd.so
--rw-r--r--   0        0        0  1368592 2023-07-06 23:47:26.000000 lvhao_lib-0.3.0/lib/linux_x86_64/libpnd.so.1.0.0
--rw-r--r--   0        0        0  1004584 2023-07-06 23:48:36.000000 lvhao_lib-0.3.0/lib/mac_x86_64/libpnd.1.0.0.dylib
--rw-r--r--   0        0        0  1004584 2023-07-06 23:48:38.000000 lvhao_lib-0.3.0/lib/mac_x86_64/libpnd.dylib
--rw-r--r--   0        0        0   639488 2023-07-06 23:49:48.000000 lvhao_lib-0.3.0/lib/win_x64/pnd.dll
--rw-r--r--   0        0        0    10122 2023-07-06 23:49:48.000000 lvhao_lib-0.3.0/lib/win_x64/pnd.lib
--rw-r--r--   0        0        0        0 2023-07-10 02:55:19.579408 lvhao_lib-0.3.0/my_lib/__init__.py
--rw-r--r--   0        0        0      340 2023-07-10 03:46:53.486010 lvhao_lib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 lvhao_lib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-10 04:36:58.117404 lvhao_lib-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 04:36:58.117367 lvhao_lib-0.7.0/lvhao_lib/__init__.py
+-rw-r--r--   0        0        0  1368592 2023-07-06 23:47:26.000000 lvhao_lib-0.7.0/lvhao_lib/lib/linux_x86_64/libpnd.so
+-rw-r--r--   0        0        0  1368592 2023-07-06 23:47:26.000000 lvhao_lib-0.7.0/lvhao_lib/lib/linux_x86_64/libpnd.so.1.0.0
+-rw-r--r--   0        0        0  1004584 2023-07-06 23:48:36.000000 lvhao_lib-0.7.0/lvhao_lib/lib/mac_x86_64/libpnd.1.0.0.dylib
+-rw-r--r--   0        0        0  1004584 2023-07-06 23:48:38.000000 lvhao_lib-0.7.0/lvhao_lib/lib/mac_x86_64/libpnd.dylib
+-rw-r--r--   0        0        0   639488 2023-07-06 23:49:48.000000 lvhao_lib-0.7.0/lvhao_lib/lib/win_x64/pnd.dll
+-rw-r--r--   0        0        0    10122 2023-07-06 23:49:48.000000 lvhao_lib-0.7.0/lvhao_lib/lib/win_x64/pnd.lib
+-rw-r--r--   0        0        0      298 2023-07-10 04:38:18.996765 lvhao_lib-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      331 1970-01-01 00:00:00.000000 lvhao_lib-0.7.0/PKG-INFO
```

### Comparing `lvhao_lib-0.3.0/lib/linux_x86_64/libpnd.so` & `lvhao_lib-0.7.0/lvhao_lib/lib/linux_x86_64/libpnd.so`

 * *Files identical despite different names*

### Comparing `lvhao_lib-0.3.0/lib/linux_x86_64/libpnd.so.1.0.0` & `lvhao_lib-0.7.0/lvhao_lib/lib/linux_x86_64/libpnd.so.1.0.0`

 * *Files identical despite different names*

### Comparing `lvhao_lib-0.3.0/lib/mac_x86_64/libpnd.1.0.0.dylib` & `lvhao_lib-0.7.0/lvhao_lib/lib/mac_x86_64/libpnd.1.0.0.dylib`

 * *Files identical despite different names*

### Comparing `lvhao_lib-0.3.0/lib/mac_x86_64/libpnd.dylib` & `lvhao_lib-0.7.0/lvhao_lib/lib/mac_x86_64/libpnd.dylib`

 * *Files identical despite different names*

### Comparing `lvhao_lib-0.3.0/lib/win_x64/pnd.dll` & `lvhao_lib-0.7.0/lvhao_lib/lib/win_x64/pnd.dll`

 * *Files identical despite different names*

### Comparing `lvhao_lib-0.3.0/lib/win_x64/pnd.lib` & `lvhao_lib-0.7.0/lvhao_lib/lib/win_x64/pnd.lib`

 * *Files identical despite different names*

