# Comparing `tmp/xeus-python-shell-0.5.0.tar.gz` & `tmp/xeus-python-shell-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeus-python-shell-0.5.0.tar", last modified: Tue Aug 23 08:25:24 2022, max compression
+gzip compressed data, was "xeus-python-shell-0.6.0.tar", last modified: Mon Jul 10 14:44:54 2023, max compression
```

## Comparing `xeus-python-shell-0.5.0.tar` & `xeus-python-shell-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2022-08-23 08:25:24.343137 xeus-python-shell-0.5.0/
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     1518 2021-08-13 10:02:56.000000 xeus-python-shell-0.5.0/LICENSE
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)       16 2021-08-19 09:11:29.000000 xeus-python-shell-0.5.0/MANIFEST.in
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      852 2022-08-23 08:25:24.343137 xeus-python-shell-0.5.0/PKG-INFO
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)      101 2021-08-19 08:49:07.000000 xeus-python-shell-0.5.0/README.md
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       38 2022-08-23 08:25:24.343137 xeus-python-shell-0.5.0/setup.cfg
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1130 2022-08-23 08:24:41.000000 xeus-python-shell-0.5.0/setup.py
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2022-08-23 08:25:24.342137 xeus-python-shell-0.5.0/xeus_python_shell/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        0 2022-08-05 13:17:28.000000 xeus-python-shell-0.5.0/xeus_python_shell/__init__.py
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)      587 2022-06-29 10:04:57.000000 xeus-python-shell-0.5.0/xeus_python_shell/compiler.py
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     3805 2022-08-09 09:38:41.000000 xeus-python-shell-0.5.0/xeus_python_shell/debugger.py
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     1383 2022-06-29 10:04:57.000000 xeus-python-shell-0.5.0/xeus_python_shell/display.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3145 2022-08-05 13:09:27.000000 xeus-python-shell-0.5.0/xeus_python_shell/lite_mocks.py
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)      255 2022-06-29 10:00:05.000000 xeus-python-shell-0.5.0/xeus_python_shell/lite_webbrowser.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3642 2022-08-23 08:15:05.000000 xeus-python-shell-0.5.0/xeus_python_shell/shell.py
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2022-08-23 08:25:24.343137 xeus-python-shell-0.5.0/xeus_python_shell.egg-info/
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)      852 2022-08-23 08:25:24.000000 xeus-python-shell-0.5.0/xeus_python_shell.egg-info/PKG-INFO
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)      457 2022-08-23 08:25:24.000000 xeus-python-shell-0.5.0/xeus_python_shell.egg-info/SOURCES.txt
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)        1 2022-08-23 08:25:24.000000 xeus-python-shell-0.5.0/xeus_python_shell.egg-info/dependency_links.txt
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)       59 2022-08-23 08:25:24.000000 xeus-python-shell-0.5.0/xeus_python_shell.egg-info/requires.txt
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)       18 2022-08-23 08:25:24.000000 xeus-python-shell-0.5.0/xeus_python_shell.egg-info/top_level.txt
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-10 14:44:54.241876 xeus-python-shell-0.6.0/
+-rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     1518 2021-08-13 10:02:56.000000 xeus-python-shell-0.6.0/LICENSE
+-rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)       16 2021-08-19 09:11:29.000000 xeus-python-shell-0.6.0/MANIFEST.in
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      852 2023-07-10 14:44:54.240876 xeus-python-shell-0.6.0/PKG-INFO
+-rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)      101 2021-08-19 08:49:07.000000 xeus-python-shell-0.6.0/README.md
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       38 2023-07-10 14:44:54.241876 xeus-python-shell-0.6.0/setup.cfg
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1144 2023-07-10 14:43:23.000000 xeus-python-shell-0.6.0/setup.py
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-10 14:44:54.239876 xeus-python-shell-0.6.0/xeus_python_shell/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        0 2022-08-05 13:17:28.000000 xeus-python-shell-0.6.0/xeus_python_shell/__init__.py
+-rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)      587 2022-06-29 10:04:57.000000 xeus-python-shell-0.6.0/xeus_python_shell/compiler.py
+-rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     3805 2022-08-09 09:38:41.000000 xeus-python-shell-0.6.0/xeus_python_shell/debugger.py
+-rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     1383 2022-06-29 10:04:57.000000 xeus-python-shell-0.6.0/xeus_python_shell/display.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3481 2023-07-10 14:43:11.000000 xeus-python-shell-0.6.0/xeus_python_shell/shell.py
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-10 14:44:54.240876 xeus-python-shell-0.6.0/xeus_python_shell.egg-info/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      852 2023-07-10 14:44:54.000000 xeus-python-shell-0.6.0/xeus_python_shell.egg-info/PKG-INFO
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      388 2023-07-10 14:44:54.000000 xeus-python-shell-0.6.0/xeus_python_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-07-10 14:44:54.000000 xeus-python-shell-0.6.0/xeus_python_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       73 2023-07-10 14:44:54.000000 xeus-python-shell-0.6.0/xeus_python_shell.egg-info/requires.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       18 2023-07-10 14:44:54.000000 xeus-python-shell-0.6.0/xeus_python_shell.egg-info/top_level.txt
```

### Comparing `xeus-python-shell-0.5.0/LICENSE` & `xeus-python-shell-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xeus-python-shell-0.5.0/PKG-INFO` & `xeus-python-shell-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeus-python-shell
-Version: 0.5.0
+Version: 0.6.0
 Summary: The xeus-python core python logic.
 Home-page: https://github.com/jupyter-xeus/xeus-python-shell
 Author: QuantStack dev team
 Maintainer: QuantStack dev team
 License: BSD 3-Clause
 Keywords: python ipython xeus-python
 Platform: any
```

### Comparing `xeus-python-shell-0.5.0/setup.py` & `xeus-python-shell-0.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 from setuptools import setup, find_packages
 
 __AUTHOR__ = 'QuantStack dev team'
 
 setup(
     name='xeus-python-shell',
-    version='0.5.0',
+    version='0.6.0',
     description='The xeus-python core python logic.',
     author=__AUTHOR__,
     maintainer=__AUTHOR__,
     url='https://github.com/jupyter-xeus/xeus-python-shell',
     license='BSD 3-Clause',
     keywords='python ipython xeus-python',
     packages=find_packages(exclude=['test']),
     python_requires='>=3.6',
     install_requires=[
         'debugpy>=1.1.0,<2'
     ],
     extras_require={
         'ipython': ['ipython>=7.21,<9'],
-        'wasm': ['pyjs'],
+        'wasm': ['pyjs>=1.1.0,<2.0.0'],
     },
     platforms=['any'],
     classifiers=[
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

### Comparing `xeus-python-shell-0.5.0/xeus_python_shell/compiler.py` & `xeus-python-shell-0.6.0/xeus_python_shell/compiler.py`

 * *Files identical despite different names*

### Comparing `xeus-python-shell-0.5.0/xeus_python_shell/debugger.py` & `xeus-python-shell-0.6.0/xeus_python_shell/debugger.py`

 * *Files identical despite different names*

### Comparing `xeus-python-shell-0.5.0/xeus_python_shell/display.py` & `xeus-python-shell-0.6.0/xeus_python_shell/display.py`

 * *Files identical despite different names*

### Comparing `xeus-python-shell-0.5.0/xeus_python_shell/shell.py` & `xeus-python-shell-0.6.0/xeus_python_shell/shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 import sys
 import os
 
-# Emscripten platform needs multiple mocks to work
-if sys.platform == "emscripten":
-    from xeus_python_shell.lite_mocks import apply_mocks
-
-    apply_mocks()
-
 from IPython.core.interactiveshell import InteractiveShell
 from IPython.core.shellapp import InteractiveShellApp
 from IPython.core.application import BaseIPythonApplication
 from IPython.core import page, payloadpage
 from IPython.core.completer import provisionalcompleter, rectify_completions
 from IPython.core.history import HistoryManager
```

### Comparing `xeus-python-shell-0.5.0/xeus_python_shell.egg-info/PKG-INFO` & `xeus-python-shell-0.6.0/xeus_python_shell.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeus-python-shell
-Version: 0.5.0
+Version: 0.6.0
 Summary: The xeus-python core python logic.
 Home-page: https://github.com/jupyter-xeus/xeus-python-shell
 Author: QuantStack dev team
 Maintainer: QuantStack dev team
 License: BSD 3-Clause
 Keywords: python ipython xeus-python
 Platform: any
```

