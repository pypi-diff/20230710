# Comparing `tmp/diz-0.0.2.tar.gz` & `tmp/diz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diz-0.0.2.tar", last modified: Mon Jul 10 03:33:56 2023, max compression
+gzip compressed data, was "diz-0.0.3.tar", last modified: Mon Jul 10 03:38:07 2023, max compression
```

## Comparing `diz-0.0.2.tar` & `diz-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:33:56.182610 diz-0.0.2/
--rw-r--r--   0 mj         (501) staff       (20)      173 2023-07-10 03:33:56.182429 diz-0.0.2/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)       63 2023-07-10 03:31:32.000000 diz-0.0.2/README.md
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:33:56.179496 diz-0.0.2/commands/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-0.0.2/commands/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)     2067 2023-07-09 15:14:17.000000 diz-0.0.2/commands/setup.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:33:56.180443 diz-0.0.2/diz.egg-info/
--rw-r--r--   0 mj         (501) staff       (20)      173 2023-07-10 03:33:56.000000 diz-0.0.2/diz.egg-info/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)      317 2023-07-10 03:33:56.000000 diz-0.0.2/diz.egg-info/SOURCES.txt
--rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 03:33:56.000000 diz-0.0.2/diz.egg-info/dependency_links.txt
--rw-r--r--   0 mj         (501) staff       (20)       37 2023-07-10 03:33:56.000000 diz-0.0.2/diz.egg-info/entry_points.txt
--rw-r--r--   0 mj         (501) staff       (20)       98 2023-07-10 03:33:56.000000 diz-0.0.2/diz.egg-info/requires.txt
--rw-r--r--   0 mj         (501) staff       (20)       15 2023-07-10 03:33:56.000000 diz-0.0.2/diz.egg-info/top_level.txt
--rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 03:33:56.182687 diz-0.0.2/setup.cfg
--rw-r--r--   0 mj         (501) staff       (20)      597 2023-07-10 03:33:34.000000 diz-0.0.2/setup.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:33:56.181975 diz-0.0.2/utils/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-0.0.2/utils/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-0.0.2/utils/dir.py
--rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-0.0.2/utils/download.py
--rw-r--r--   0 mj         (501) staff       (20)      758 2023-07-09 15:11:55.000000 diz-0.0.2/utils/pip.py
--rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-0.0.2/utils/validators.py
--rw-r--r--   0 mj         (501) staff       (20)      313 2023-07-09 14:46:10.000000 diz-0.0.2/utils/yaml.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:38:07.878291 diz-0.0.3/
+-rw-r--r--   0 mj         (501) staff       (20)      213 2023-07-10 03:38:07.878179 diz-0.0.3/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)       63 2023-07-10 03:31:32.000000 diz-0.0.3/README.md
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:38:07.876667 diz-0.0.3/commands/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-0.0.3/commands/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)     2067 2023-07-09 15:14:17.000000 diz-0.0.3/commands/setup.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:38:07.877387 diz-0.0.3/diz.egg-info/
+-rw-r--r--   0 mj         (501) staff       (20)      213 2023-07-10 03:38:07.000000 diz-0.0.3/diz.egg-info/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)      317 2023-07-10 03:38:07.000000 diz-0.0.3/diz.egg-info/SOURCES.txt
+-rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 03:38:07.000000 diz-0.0.3/diz.egg-info/dependency_links.txt
+-rw-r--r--   0 mj         (501) staff       (20)       33 2023-07-10 03:38:07.000000 diz-0.0.3/diz.egg-info/entry_points.txt
+-rw-r--r--   0 mj         (501) staff       (20)       98 2023-07-10 03:38:07.000000 diz-0.0.3/diz.egg-info/requires.txt
+-rw-r--r--   0 mj         (501) staff       (20)       15 2023-07-10 03:38:07.000000 diz-0.0.3/diz.egg-info/top_level.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 03:38:07.878336 diz-0.0.3/setup.cfg
+-rw-r--r--   0 mj         (501) staff       (20)      644 2023-07-10 03:37:58.000000 diz-0.0.3/setup.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:38:07.878002 diz-0.0.3/utils/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-0.0.3/utils/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-0.0.3/utils/dir.py
+-rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-0.0.3/utils/download.py
+-rw-r--r--   0 mj         (501) staff       (20)      758 2023-07-09 15:11:55.000000 diz-0.0.3/utils/pip.py
+-rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-0.0.3/utils/validators.py
+-rw-r--r--   0 mj         (501) staff       (20)      313 2023-07-09 14:46:10.000000 diz-0.0.3/utils/yaml.py
```

### Comparing `diz-0.0.2/commands/setup.py` & `diz-0.0.3/commands/setup.py`

 * *Files identical despite different names*

### Comparing `diz-0.0.2/setup.py` & `diz-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='diz',
-    version='0.0.2',
+    version='0.0.3',
     author='mjason',
     description='用来构建大模型环境的工具',
     long_description=readme(),
+    long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'GitPython>=3.1.31',
         'huggingface-hub>=0.16.4',
         'PyYAML>=6.0',
         'requests>=2.31.0',
         'toolz>=0.12.0',
         'typer>=0.9.0'
     ],
     entry_points={
         'console_scripts': [
-            'diz = diz.main:app'
+            'diz = main:app'
         ]
     }
 )
```

### Comparing `diz-0.0.2/utils/pip.py` & `diz-0.0.3/utils/pip.py`

 * *Files identical despite different names*

