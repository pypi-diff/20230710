# Comparing `tmp/template-pypackage-tool-0.1.tar.gz` & `tmp/template-pypackage-tool-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "template-pypackage-tool-0.1.tar", last modified: Mon Jul 10 15:06:15 2023, max compression
+gzip compressed data, was "template-pypackage-tool-0.2.tar", last modified: Mon Jul 10 15:07:57 2023, max compression
```

## Comparing `template-pypackage-tool-0.1.tar` & `template-pypackage-tool-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:06:15.891897 template-pypackage-tool-0.1/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       48 2023-07-10 14:46:28.000000 template-pypackage-tool-0.1/MANIFEST.in
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     3995 2023-07-10 15:06:15.891897 template-pypackage-tool-0.1/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     3583 2023-07-10 14:47:06.000000 template-pypackage-tool-0.1/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-10 15:06:15.891897 template-pypackage-tool-0.1/setup.cfg
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      716 2023-07-10 15:05:27.000000 template-pypackage-tool-0.1/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:06:15.887897 template-pypackage-tool-0.1/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:06:15.887897 template-pypackage-tool-0.1/src/template-pypackage-tool/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    13080 2023-07-10 14:10:03.000000 template-pypackage-tool-0.1/src/template-pypackage-tool/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:06:15.891897 template-pypackage-tool-0.1/src/template-pypackage-tool/types/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    11357 2023-07-09 20:17:56.000000 template-pypackage-tool-0.1/src/template-pypackage-tool/types/Apache Version 2.0.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    35150 2023-07-09 20:14:37.000000 template-pypackage-tool-0.1/src/template-pypackage-tool/types/GNU GPLv3.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1070 2023-07-09 20:15:41.000000 template-pypackage-tool-0.1/src/template-pypackage-tool/types/MIT License.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    16725 2023-07-09 20:21:23.000000 template-pypackage-tool-0.1/src/template-pypackage-tool/types/Mozilla Public License 2.0.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1211 2023-07-09 20:22:37.000000 template-pypackage-tool-0.1/src/template-pypackage-tool/types/The Unlicense.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        0 2023-07-09 21:14:00.000000 template-pypackage-tool-0.1/src/template-pypackage-tool/types/user_defined.txt
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:06:15.891897 template-pypackage-tool-0.1/src/template_pypackage_tool.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     3995 2023-07-10 15:06:15.000000 template-pypackage-tool-0.1/src/template_pypackage_tool.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      647 2023-07-10 15:06:15.000000 template-pypackage-tool-0.1/src/template_pypackage_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-10 15:06:15.000000 template-pypackage-tool-0.1/src/template_pypackage_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       24 2023-07-10 15:06:15.000000 template-pypackage-tool-0.1/src/template_pypackage_tool.egg-info/requires.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       24 2023-07-10 15:06:15.000000 template-pypackage-tool-0.1/src/template_pypackage_tool.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:07:57.281449 template-pypackage-tool-0.2/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       48 2023-07-10 14:46:28.000000 template-pypackage-tool-0.2/MANIFEST.in
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     3995 2023-07-10 15:07:57.281449 template-pypackage-tool-0.2/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     3583 2023-07-10 14:47:06.000000 template-pypackage-tool-0.2/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-10 15:07:57.281449 template-pypackage-tool-0.2/setup.cfg
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      700 2023-07-10 15:07:35.000000 template-pypackage-tool-0.2/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:07:57.277449 template-pypackage-tool-0.2/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:07:57.277449 template-pypackage-tool-0.2/src/template-pypackage-tool/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    13080 2023-07-10 14:10:03.000000 template-pypackage-tool-0.2/src/template-pypackage-tool/__init__.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:07:57.277449 template-pypackage-tool-0.2/src/template-pypackage-tool/types/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    11357 2023-07-09 20:17:56.000000 template-pypackage-tool-0.2/src/template-pypackage-tool/types/Apache Version 2.0.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    35150 2023-07-09 20:14:37.000000 template-pypackage-tool-0.2/src/template-pypackage-tool/types/GNU GPLv3.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1070 2023-07-09 20:15:41.000000 template-pypackage-tool-0.2/src/template-pypackage-tool/types/MIT License.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    16725 2023-07-09 20:21:23.000000 template-pypackage-tool-0.2/src/template-pypackage-tool/types/Mozilla Public License 2.0.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1211 2023-07-09 20:22:37.000000 template-pypackage-tool-0.2/src/template-pypackage-tool/types/The Unlicense.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        0 2023-07-09 21:14:00.000000 template-pypackage-tool-0.2/src/template-pypackage-tool/types/user_defined.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:07:57.281449 template-pypackage-tool-0.2/src/template_pypackage_tool.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     3995 2023-07-10 15:07:57.000000 template-pypackage-tool-0.2/src/template_pypackage_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      647 2023-07-10 15:07:57.000000 template-pypackage-tool-0.2/src/template_pypackage_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-10 15:07:57.000000 template-pypackage-tool-0.2/src/template_pypackage_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       10 2023-07-10 15:07:57.000000 template-pypackage-tool-0.2/src/template_pypackage_tool.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       24 2023-07-10 15:07:57.000000 template-pypackage-tool-0.2/src/template_pypackage_tool.egg-info/top_level.txt
```

### Comparing `template-pypackage-tool-0.1/PKG-INFO` & `template-pypackage-tool-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pypackage-tool
-Version: 0.1
+Version: 0.2
 Summary: A simple tool for packaging python
 Author: Dipson
 License: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `template-pypackage-tool-0.1/README.md` & `template-pypackage-tool-0.2/README.md`

 * *Files identical despite different names*

### Comparing `template-pypackage-tool-0.1/setup.py` & `template-pypackage-tool-0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 with open("README.md", "r") as f:
     long_description = f.read()
 setup(
     name="template-pypackage-tool",
-    version="0.1",
+    version="0.2",
     description="A simple tool for packaging python",
     package_dir={"": "src"},
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Dipson",
     license="GNU General Public License v3 (GPLv3)",
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
-    install_requires=['pyperclip','pkg_resources'],
+    install_requires=['pyperclip'],
     python_requires=">=3.10",
 )
```

### Comparing `template-pypackage-tool-0.1/src/template-pypackage-tool/__init__.py` & `template-pypackage-tool-0.2/src/template-pypackage-tool/__init__.py`

 * *Files identical despite different names*

### Comparing `template-pypackage-tool-0.1/src/template-pypackage-tool/types/Apache Version 2.0.txt` & `template-pypackage-tool-0.2/src/template-pypackage-tool/types/Apache Version 2.0.txt`

 * *Files identical despite different names*

### Comparing `template-pypackage-tool-0.1/src/template-pypackage-tool/types/GNU GPLv3.txt` & `template-pypackage-tool-0.2/src/template-pypackage-tool/types/GNU GPLv3.txt`

 * *Files identical despite different names*

### Comparing `template-pypackage-tool-0.1/src/template-pypackage-tool/types/MIT License.txt` & `template-pypackage-tool-0.2/src/template-pypackage-tool/types/MIT License.txt`

 * *Files identical despite different names*

### Comparing `template-pypackage-tool-0.1/src/template-pypackage-tool/types/Mozilla Public License 2.0.txt` & `template-pypackage-tool-0.2/src/template-pypackage-tool/types/Mozilla Public License 2.0.txt`

 * *Files identical despite different names*

### Comparing `template-pypackage-tool-0.1/src/template-pypackage-tool/types/The Unlicense.txt` & `template-pypackage-tool-0.2/src/template-pypackage-tool/types/The Unlicense.txt`

 * *Files identical despite different names*

### Comparing `template-pypackage-tool-0.1/src/template_pypackage_tool.egg-info/PKG-INFO` & `template-pypackage-tool-0.2/src/template_pypackage_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pypackage-tool
-Version: 0.1
+Version: 0.2
 Summary: A simple tool for packaging python
 Author: Dipson
 License: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `template-pypackage-tool-0.1/src/template_pypackage_tool.egg-info/SOURCES.txt` & `template-pypackage-tool-0.2/src/template_pypackage_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

