# Comparing `tmp/kthbuild-3.2.0.tar.gz` & `tmp/kthbuild-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kthbuild-3.2.0.tar", last modified: Mon Jul 10 08:46:28 2023, max compression
+gzip compressed data, was "kthbuild-3.3.0.tar", last modified: Mon Jul 10 10:14:00 2023, max compression
```

## Comparing `kthbuild-3.2.0.tar` & `kthbuild-3.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:46:28.632326 kthbuild-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-10 08:46:07.000000 kthbuild-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-10 08:46:28.632326 kthbuild-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-10 08:46:07.000000 kthbuild-3.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:46:28.632326 kthbuild-3.2.0/kthbuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-10 08:46:28.000000 kthbuild-3.2.0/kthbuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-10 08:46:28.000000 kthbuild-3.2.0/kthbuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-10 08:46:28.000000 kthbuild-3.2.0/kthbuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-10 08:46:28.000000 kthbuild-3.2.0/kthbuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-10 08:46:28.000000 kthbuild-3.2.0/kthbuild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    42265 2023-07-10 08:46:07.000000 kthbuild-3.2.0/kthbuild.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 08:46:28.632326 kthbuild-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-07-10 08:46:07.000000 kthbuild-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:14:00.058287 kthbuild-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-10 10:13:31.000000 kthbuild-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-10 10:14:00.058287 kthbuild-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-10 10:13:31.000000 kthbuild-3.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:14:00.058287 kthbuild-3.3.0/kthbuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-10 10:14:00.000000 kthbuild-3.3.0/kthbuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-10 10:14:00.000000 kthbuild-3.3.0/kthbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-10 10:14:00.000000 kthbuild-3.3.0/kthbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-10 10:14:00.000000 kthbuild-3.3.0/kthbuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-10 10:14:00.000000 kthbuild-3.3.0/kthbuild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    42295 2023-07-10 10:13:31.000000 kthbuild-3.3.0/kthbuild.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 10:14:00.058287 kthbuild-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-07-10 10:13:31.000000 kthbuild-3.3.0/setup.py
```

### Comparing `kthbuild-3.2.0/LICENSE` & `kthbuild-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kthbuild-3.2.0/PKG-INFO` & `kthbuild-3.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthbuild
-Version: 3.2.0
+Version: 3.3.0
 Summary: Knuth node build tools
 Home-page: https://github.com/k-nuth/kthbuild
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kthbuild-3.2.0/kthbuild.egg-info/PKG-INFO` & `kthbuild-3.3.0/kthbuild.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthbuild
-Version: 3.2.0
+Version: 3.3.0
 Summary: Knuth node build tools
 Home-page: https://github.com/k-nuth/kthbuild
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kthbuild-3.2.0/kthbuild.py` & `kthbuild-3.3.0/kthbuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -954,29 +954,29 @@
 
         if self.info.options.get_safe("cmake_export_compile_commands") is not None:
             self.info.options.cmake_export_compile_commands = "ANY"
 
         if self.info.options.get_safe("march_strategy") is not None:
             self.info.options.march_strategy = "ANY"
 
-    def _cmake_database(self, tc):
-        if self.options.get_safe("db") is None:
-            return
-
-        if self.options.db == "dynamic":
-            tc.variables["DB_TRANSACTION_UNCONFIRMED"] = option_on_off(False)
-            tc.variables["DB_SPENDS"] = option_on_off(False)
-            tc.variables["DB_HISTORY"] = option_on_off(False)
-            tc.variables["DB_STEALTH"] = option_on_off(False)
-            tc.variables["DB_UNSPENT_LEGACY"] = option_on_off(False)
-            tc.variables["DB_LEGACY"] = option_on_off(False)
-            tc.variables["DB_NEW"] = option_on_off(False)
-            tc.variables["DB_NEW_BLOCKS"] = option_on_off(False)
-            tc.variables["DB_NEW_FULL"] = option_on_off(False)
-            tc.variables["DB_DYNAMIC"] = option_on_off(True)
+    # def _cmake_database(self, tc):
+    #     if self.options.get_safe("db") is None:
+    #         return
+
+    #     if self.options.db == "dynamic":
+    #         tc.variables["DB_TRANSACTION_UNCONFIRMED"] = option_on_off(False)
+    #         tc.variables["DB_SPENDS"] = option_on_off(False)
+    #         tc.variables["DB_HISTORY"] = option_on_off(False)
+    #         tc.variables["DB_STEALTH"] = option_on_off(False)
+    #         tc.variables["DB_UNSPENT_LEGACY"] = option_on_off(False)
+    #         tc.variables["DB_LEGACY"] = option_on_off(False)
+    #         tc.variables["DB_NEW"] = option_on_off(False)
+    #         tc.variables["DB_NEW_BLOCKS"] = option_on_off(False)
+    #         tc.variables["DB_NEW_FULL"] = option_on_off(False)
+    #         tc.variables["DB_DYNAMIC"] = option_on_off(True)
 
     def cmake_toolchain_basis(self, pure_c=False):
         tc = CMakeToolchain(self)
         tc.variables["USE_CONAN"] = option_on_off(True)
         tc.variables["NO_CONAN_AT_ALL"] = option_on_off(False)
         # cmake.verbose = self.options.verbose
         tc.variables["ENABLE_SHARED"] = option_on_off(self.is_shared)
@@ -1010,15 +1010,15 @@
         tc.variables["MARCH_NAMES_FULL_STR"] = self.march_names_full_str
 
         tc.variables["KTH_PROJECT_VERSION"] = self.version
 
         if self.options.get_safe("currency") is not None:
             tc.variables["CURRENCY"] = self.options.currency
 
-        self._cmake_database(tc)
+        # self._cmake_database(tc)
 
         if self.options.get_safe("cmake_export_compile_commands") is not None and self.options.cmake_export_compile_commands:
             tc.variables["CMAKE_EXPORT_COMPILE_COMMANDS"] = option_on_off(self.options.cmake_export_compile_commands)
 
         pass_march_to_compiler(self, tc)
         return tc
```

### Comparing `kthbuild-3.2.0/setup.py` & `kthbuild-3.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import subprocess
 import os
 import platform
 
 __title__ = "kthbuild"
 __summary__ = "Knuth node build tools"
 __uri__ = "https://github.com/k-nuth/kthbuild"
-__version__ = "3.2.0"
+__version__ = "3.3.0"
 __author__ = "Fernando Pelliccioni"
 __email__ = "fpelliccioni@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2019-2023 Knuth Project"
 
 
 install_requires = [
```

