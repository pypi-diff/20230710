# Comparing `tmp/diz-0.0.5.tar.gz` & `tmp/diz-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diz-0.0.5.tar", last modified: Mon Jul 10 03:57:35 2023, max compression
+gzip compressed data, was "diz-0.0.7.tar", last modified: Mon Jul 10 04:17:13 2023, max compression
```

## Comparing `diz-0.0.5.tar` & `diz-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:57:35.545819 diz-0.0.5/
--rw-r--r--   0 mj         (501) staff       (20)      213 2023-07-10 03:57:35.545702 diz-0.0.5/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)       63 2023-07-10 03:31:32.000000 diz-0.0.5/README.md
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:57:35.543021 diz-0.0.5/diz/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-10 03:55:54.000000 diz-0.0.5/diz/__init__.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:57:35.543972 diz-0.0.5/diz/commands/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-0.0.5/diz/commands/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)     2108 2023-07-10 03:54:31.000000 diz-0.0.5/diz/commands/setup.py
--rw-r--r--   0 mj         (501) staff       (20)      772 2023-07-10 03:56:40.000000 diz-0.0.5/diz/main.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:57:35.545418 diz-0.0.5/diz/utils/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-0.0.5/diz/utils/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-0.0.5/diz/utils/dir.py
--rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-0.0.5/diz/utils/download.py
--rw-r--r--   0 mj         (501) staff       (20)      762 2023-07-10 03:53:40.000000 diz-0.0.5/diz/utils/pip.py
--rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-0.0.5/diz/utils/validators.py
--rw-r--r--   0 mj         (501) staff       (20)      311 2023-07-10 03:53:40.000000 diz-0.0.5/diz/utils/yaml.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:57:35.543734 diz-0.0.5/diz.egg-info/
--rw-r--r--   0 mj         (501) staff       (20)      213 2023-07-10 03:57:35.000000 diz-0.0.5/diz.egg-info/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)      377 2023-07-10 03:57:35.000000 diz-0.0.5/diz.egg-info/SOURCES.txt
--rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 03:57:35.000000 diz-0.0.5/diz.egg-info/dependency_links.txt
--rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 03:57:35.000000 diz-0.0.5/diz.egg-info/entry_points.txt
--rw-r--r--   0 mj         (501) staff       (20)       98 2023-07-10 03:57:35.000000 diz-0.0.5/diz.egg-info/requires.txt
--rw-r--r--   0 mj         (501) staff       (20)        4 2023-07-10 03:57:35.000000 diz-0.0.5/diz.egg-info/top_level.txt
--rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 03:57:35.545857 diz-0.0.5/setup.cfg
--rw-r--r--   0 mj         (501) staff       (20)      649 2023-07-10 03:57:25.000000 diz-0.0.5/setup.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 04:17:13.074743 diz-0.0.7/
+-rw-r--r--   0 mj         (501) staff       (20)      213 2023-07-10 04:17:13.074635 diz-0.0.7/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)       63 2023-07-10 03:31:32.000000 diz-0.0.7/README.md
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 04:17:13.072886 diz-0.0.7/diz/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-10 03:55:54.000000 diz-0.0.7/diz/__init__.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 04:17:13.073802 diz-0.0.7/diz/commands/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-0.0.7/diz/commands/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)     2108 2023-07-10 03:54:31.000000 diz-0.0.7/diz/commands/setup.py
+-rw-r--r--   0 mj         (501) staff       (20)      772 2023-07-10 03:56:40.000000 diz-0.0.7/diz/main.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 04:17:13.074478 diz-0.0.7/diz/utils/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-0.0.7/diz/utils/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-0.0.7/diz/utils/dir.py
+-rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-0.0.7/diz/utils/download.py
+-rw-r--r--   0 mj         (501) staff       (20)      762 2023-07-10 04:14:00.000000 diz-0.0.7/diz/utils/pip.py
+-rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-0.0.7/diz/utils/validators.py
+-rw-r--r--   0 mj         (501) staff       (20)      308 2023-07-10 04:14:09.000000 diz-0.0.7/diz/utils/yaml.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 04:17:13.073592 diz-0.0.7/diz.egg-info/
+-rw-r--r--   0 mj         (501) staff       (20)      213 2023-07-10 04:17:13.000000 diz-0.0.7/diz.egg-info/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)      377 2023-07-10 04:17:13.000000 diz-0.0.7/diz.egg-info/SOURCES.txt
+-rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 04:17:13.000000 diz-0.0.7/diz.egg-info/dependency_links.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 04:17:13.000000 diz-0.0.7/diz.egg-info/entry_points.txt
+-rw-r--r--   0 mj         (501) staff       (20)       98 2023-07-10 04:17:13.000000 diz-0.0.7/diz.egg-info/requires.txt
+-rw-r--r--   0 mj         (501) staff       (20)        4 2023-07-10 04:17:13.000000 diz-0.0.7/diz.egg-info/top_level.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 04:17:13.074787 diz-0.0.7/setup.cfg
+-rw-r--r--   0 mj         (501) staff       (20)      649 2023-07-10 04:16:24.000000 diz-0.0.7/setup.py
```

### Comparing `diz-0.0.5/diz/commands/setup.py` & `diz-0.0.7/diz/commands/setup.py`

 * *Files identical despite different names*

### Comparing `diz-0.0.5/diz/main.py` & `diz-0.0.7/diz/main.py`

 * *Files identical despite different names*

### Comparing `diz-0.0.5/diz/utils/pip.py` & `diz-0.0.7/diz/utils/pip.py`

 * *Files identical despite different names*

### Comparing `diz-0.0.5/setup.py` & `diz-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='diz',
-    version='0.0.5',
+    version='0.0.7',
     author='mjason',
     description='用来构建大模型环境的工具',
     long_description=readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'GitPython>=3.1.31',
```

