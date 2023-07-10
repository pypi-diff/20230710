# Comparing `tmp/template_pypackage_builder-0.3.tar.gz` & `tmp/template_pypackage_builder-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "template_pypackage_builder-0.3.tar", last modified: Mon Jul 10 15:32:58 2023, max compression
+gzip compressed data, was "template_pypackage_builder-0.4.tar", last modified: Mon Jul 10 15:44:30 2023, max compression
```

## Comparing `template_pypackage_builder-0.3.tar` & `template_pypackage_builder-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:32:58.878257 template_pypackage_builder-0.3/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       48 2023-07-10 14:46:28.000000 template_pypackage_builder-0.3/MANIFEST.in
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     3998 2023-07-10 15:32:58.878257 template_pypackage_builder-0.3/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     3583 2023-07-10 14:47:06.000000 template_pypackage_builder-0.3/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-10 15:32:58.878257 template_pypackage_builder-0.3/setup.cfg
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      719 2023-07-10 15:32:39.000000 template_pypackage_builder-0.3/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:32:58.878257 template_pypackage_builder-0.3/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:32:58.878257 template_pypackage_builder-0.3/src/template_pypackage_builder/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    13080 2023-07-10 14:10:03.000000 template_pypackage_builder-0.3/src/template_pypackage_builder/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:32:58.878257 template_pypackage_builder-0.3/src/template_pypackage_builder.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     3998 2023-07-10 15:32:58.000000 template_pypackage_builder-0.3/src/template_pypackage_builder.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      342 2023-07-10 15:32:58.000000 template_pypackage_builder-0.3/src/template_pypackage_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-10 15:32:58.000000 template_pypackage_builder-0.3/src/template_pypackage_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       24 2023-07-10 15:32:58.000000 template_pypackage_builder-0.3/src/template_pypackage_builder.egg-info/requires.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       27 2023-07-10 15:32:58.000000 template_pypackage_builder-0.3/src/template_pypackage_builder.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:44:30.499620 template_pypackage_builder-0.4/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       48 2023-07-10 14:46:28.000000 template_pypackage_builder-0.4/MANIFEST.in
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4050 2023-07-10 15:44:30.499620 template_pypackage_builder-0.4/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     3583 2023-07-10 14:47:06.000000 template_pypackage_builder-0.4/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-10 15:44:30.499620 template_pypackage_builder-0.4/setup.cfg
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      755 2023-07-10 15:44:26.000000 template_pypackage_builder-0.4/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:44:30.495620 template_pypackage_builder-0.4/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:44:30.499620 template_pypackage_builder-0.4/src/template_pypackage_builder/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    13080 2023-07-10 14:10:03.000000 template_pypackage_builder-0.4/src/template_pypackage_builder/__init__.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:44:30.499620 template_pypackage_builder-0.4/src/template_pypackage_builder.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4050 2023-07-10 15:44:30.000000 template_pypackage_builder-0.4/src/template_pypackage_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      342 2023-07-10 15:44:30.000000 template_pypackage_builder-0.4/src/template_pypackage_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-10 15:44:30.000000 template_pypackage_builder-0.4/src/template_pypackage_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       10 2023-07-10 15:44:30.000000 template_pypackage_builder-0.4/src/template_pypackage_builder.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       27 2023-07-10 15:44:30.000000 template_pypackage_builder-0.4/src/template_pypackage_builder.egg-info/top_level.txt
```

### Comparing `template_pypackage_builder-0.3/PKG-INFO` & `template_pypackage_builder-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: template_pypackage_builder
-Version: 0.3
+Version: 0.4
 Summary: A simple tool for packaging python
+Home-page: https://github.com/dipson94/packagemaker
 Author: Dipson
 License: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `template_pypackage_builder-0.3/README.md` & `template_pypackage_builder-0.4/README.md`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.3/setup.py` & `template_pypackage_builder-0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup
 with open("README.md", "r") as f:
     long_description = f.read()
 setup(
     name="template_pypackage_builder",
-    version="0.3",
+    version="0.4",
     description="A simple tool for packaging python",
     package_dir={"": "src"},
     include_package_data=True,
+    url="https://github.com/dipson94/packagemaker",
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

### Comparing `template_pypackage_builder-0.3/src/template_pypackage_builder/__init__.py` & `template_pypackage_builder-0.4/src/template_pypackage_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.3/src/template_pypackage_builder.egg-info/PKG-INFO` & `template_pypackage_builder-0.4/src/template_pypackage_builder.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: template-pypackage-builder
-Version: 0.3
+Version: 0.4
 Summary: A simple tool for packaging python
+Home-page: https://github.com/dipson94/packagemaker
 Author: Dipson
 License: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

