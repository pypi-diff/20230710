# Comparing `tmp/esp-coredump-1.5.2.tar.gz` & `tmp/esp-coredump-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/esp-coredump-1.5.2.tar", last modified: Thu Jun 29 17:21:03 2023, max compression
+gzip compressed data, was "dist/esp-coredump-1.6.0.tar", last modified: Mon Jul 10 15:32:10 2023, max compression
```

## Comparing `esp-coredump-1.5.2.tar` & `esp-coredump-1.6.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2471 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump/
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/cli_ext.py
--rwxrwxrwx   0 root         (0) root         (0)    22322 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/coredump.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump/corefile/
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2019 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/_parse_soc_header.py
--rw-rw-rw-   0 root         (0) root         (0)    12070 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/elf.py
--rw-rw-rw-   0 root         (0) root         (0)     5339 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/gdb.py
--rw-rw-rw-   0 root         (0) root         (0)    28537 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/riscv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32c2.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32c3.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32c6.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32h2.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32s2.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32s3.py
--rw-rw-rw-   0 root         (0) root         (0)    11177 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/xtensa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/scripts/espcoredump.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/scripts/run_tests.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2471 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1088 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4334 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/tests/test_espcoredump.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/esp_coredump/
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/cli_ext.py
+-rwxrwxrwx   0 root         (0) root         (0)    22601 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/coredump.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/esp_coredump/corefile/
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/_parse_soc_header.py
+-rw-rw-rw-   0 root         (0) root         (0)    12070 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/elf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5339 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/gdb.py
+-rw-rw-rw-   0 root         (0) root         (0)    28537 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/riscv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/esp_coredump/corefile/soc_headers/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/soc_headers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/soc_headers/esp32.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/soc_headers/esp32c2.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/soc_headers/esp32c3.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/soc_headers/esp32c6.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/soc_headers/esp32h2.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/soc_headers/esp32s2.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/soc_headers/esp32s3.py
+-rw-rw-rw-   0 root         (0) root         (0)    11177 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/corefile/xtensa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/esp_coredump/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/scripts/espcoredump.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/scripts/run_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/esp_coredump/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/esp_coredump.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/esp_coredump.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/esp_coredump.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/esp_coredump.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/esp_coredump.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/esp_coredump.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/esp_coredump.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 15:32:10.000000 esp-coredump-1.6.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4334 2023-07-10 15:21:58.000000 esp-coredump-1.6.0/tests/test_espcoredump.py
```

### Comparing `esp-coredump-1.5.2/LICENSE` & `esp-coredump-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/PKG-INFO` & `esp-coredump-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-coredump
-Version: 1.5.2
+Version: 1.6.0
 Summary: Generate core dumps on unrecoverable software errors
 Home-page: https://github.com/espressif/esp-idf
 Author: Espressif Systems
 Author-email: aleksei.apaseev@espressif.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `esp-coredump-1.5.2/README.md` & `esp-coredump-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/esp_coredump/__init__.py` & `esp-coredump-1.6.0/esp_coredump/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
 from .coredump import CoreDump
 
 __all__ = [
     'CoreDump',
 ]
 
-__version__ = '1.5.2'
+__version__ = '1.6.0'
```

### Comparing `esp-coredump-1.5.2/esp_coredump/cli_ext.py` & `esp-coredump-1.6.0/esp_coredump/cli_ext.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/esp_coredump/coredump.py` & `esp-coredump-1.6.0/esp_coredump/coredump.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,23 @@
 
             if chip_version == EspCoreDumpVersion.ESP32S3:
                 return 'esp32s3'
 
             if chip_version == EspCoreDumpVersion.ESP32C3:
                 return 'esp32c3'
 
+            if chip_version == EspCoreDumpVersion.ESP32C2:
+                return 'esp32c2'
+
+            if chip_version == EspCoreDumpVersion.ESP32C6:
+                return 'esp32c6'
+
+            if chip_version == EspCoreDumpVersion.ESP32H2:
+                return 'esp32h2'
+
         target = None
         try:
             inst = detect_chip(self.port, self.baud)
         except serial.serialutil.SerialException:
             print('Unable to identify the chip type. '
                   'Please use the --chip option to specify the chip type or '
                   'connect the board and provide the --port option to have the chip type determined automatically.',
```

### Comparing `esp-coredump-1.5.2/esp_coredump/corefile/__init__.py` & `esp-coredump-1.6.0/esp_coredump/corefile/__init__.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/esp_coredump/corefile/_parse_soc_header.py` & `esp-coredump-1.6.0/esp_coredump/corefile/_parse_soc_header.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/esp_coredump/corefile/elf.py` & `esp-coredump-1.6.0/esp_coredump/corefile/elf.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/esp_coredump/corefile/gdb.py` & `esp-coredump-1.6.0/esp_coredump/corefile/gdb.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/esp_coredump/corefile/loader.py` & `esp-coredump-1.6.0/esp_coredump/corefile/loader.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/esp_coredump/corefile/riscv.py` & `esp-coredump-1.6.0/esp_coredump/corefile/riscv.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/esp_coredump/corefile/xtensa.py` & `esp-coredump-1.6.0/esp_coredump/corefile/xtensa.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/esp_coredump/scripts/espcoredump.py` & `esp-coredump-1.6.0/esp_coredump/scripts/espcoredump.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/esp_coredump/scripts/run_tests.py` & `esp-coredump-1.6.0/esp_coredump/scripts/run_tests.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/esp_coredump.egg-info/PKG-INFO` & `esp-coredump-1.6.0/esp_coredump.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-coredump
-Version: 1.5.2
+Version: 1.6.0
 Summary: Generate core dumps on unrecoverable software errors
 Home-page: https://github.com/espressif/esp-idf
 Author: Espressif Systems
 Author-email: aleksei.apaseev@espressif.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `esp-coredump-1.5.2/esp_coredump.egg-info/SOURCES.txt` & `esp-coredump-1.6.0/esp_coredump.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/setup.py` & `esp-coredump-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.2/tests/test_espcoredump.py` & `esp-coredump-1.6.0/tests/test_espcoredump.py`

 * *Files identical despite different names*

