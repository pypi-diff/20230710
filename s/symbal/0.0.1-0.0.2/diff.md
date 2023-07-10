# Comparing `tmp/symbal-0.0.1.tar.gz` & `tmp/symbal-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbal-0.0.1.tar", last modified: Mon Jul 10 15:53:59 2023, max compression
+gzip compressed data, was "symbal-0.0.2.tar", last modified: Mon Jul 10 15:56:23 2023, max compression
```

## Comparing `symbal-0.0.1.tar` & `symbal-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 15:53:59.211540 symbal-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      663 2023-07-10 15:53:59.210959 symbal-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.1/README.md
--rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 15:53:59.211540 symbal-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-07-09 21:31:44.000000 symbal-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:53:59.203978 symbal-0.0.1/symbal/
--rw-rw-rw-   0        0        0      303 2023-07-09 21:58:25.000000 symbal-0.0.1/symbal/__init__.py
--rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.1/symbal/penalties.py
--rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.1/symbal/test_function.py
--rw-rw-rw-   0        0        0     2135 2023-07-09 21:47:00.000000 symbal-0.0.1/symbal/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:53:59.208965 symbal-0.0.1/symbal.egg-info/
--rw-rw-rw-   0        0        0      663 2023-07-10 15:53:59.000000 symbal-0.0.1/symbal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-07-10 15:53:59.000000 symbal-0.0.1/symbal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 15:53:59.000000 symbal-0.0.1/symbal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-10 15:53:59.000000 symbal-0.0.1/symbal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 15:56:23.225362 symbal-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      666 2023-07-10 15:56:23.224364 symbal-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.2/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 15:56:23.225362 symbal-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-07-10 15:56:14.000000 symbal-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 15:56:23.217383 symbal-0.0.2/symbal/
+-rw-rw-rw-   0        0        0      303 2023-07-10 15:56:14.000000 symbal-0.0.2/symbal/__init__.py
+-rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.2/symbal/penalties.py
+-rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.2/symbal/test_function.py
+-rw-rw-rw-   0        0        0     2135 2023-07-09 21:47:00.000000 symbal-0.0.2/symbal/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 15:56:23.223366 symbal-0.0.2/symbal.egg-info/
+-rw-rw-rw-   0        0        0      666 2023-07-10 15:56:23.000000 symbal-0.0.2/symbal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-07-10 15:56:23.000000 symbal-0.0.2/symbal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 15:56:23.000000 symbal-0.0.2/symbal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 15:56:23.000000 symbal-0.0.2/symbal.egg-info/top_level.txt
```

### Comparing `symbal-0.0.1/LICENSE` & `symbal-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `symbal-0.0.1/setup.py` & `symbal-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='symbal',
-    version='0.0.1',
+    version='0.0.2',
     author='Alex Summers',
     author_email='ajs0201@auburn.edu',
-    description='A small Python wrapper for Quantum Espresso - still in development',
+    description='A Python package for batch adaptive sampling with symbolic regression',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ajsummers/symbal',
     project_urls={
         'Issues': 'https://github.com/ajsummers/symbal/issues'
     },
     classifiers=[
```

### Comparing `symbal-0.0.1/symbal/test_function.py` & `symbal-0.0.2/symbal/test_function.py`

 * *Files identical despite different names*

### Comparing `symbal-0.0.1/symbal/utils.py` & `symbal-0.0.2/symbal/utils.py`

 * *Files identical despite different names*

