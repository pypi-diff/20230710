# Comparing `tmp/diz-0.0.4.tar.gz` & `tmp/diz-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diz-0.0.4.tar", last modified: Mon Jul 10 03:44:16 2023, max compression
+gzip compressed data, was "diz-0.0.5.tar", last modified: Mon Jul 10 03:57:35 2023, max compression
```

## Comparing `diz-0.0.4.tar` & `diz-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:44:16.007757 diz-0.0.4/
--rw-r--r--   0 mj         (501) staff       (20)      213 2023-07-10 03:44:16.007641 diz-0.0.4/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)       63 2023-07-10 03:31:32.000000 diz-0.0.4/README.md
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:44:16.006198 diz-0.0.4/commands/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-0.0.4/commands/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)     2067 2023-07-09 15:14:17.000000 diz-0.0.4/commands/setup.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:44:16.006865 diz-0.0.4/diz.egg-info/
--rw-r--r--   0 mj         (501) staff       (20)      213 2023-07-10 03:44:15.000000 diz-0.0.4/diz.egg-info/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)      317 2023-07-10 03:44:15.000000 diz-0.0.4/diz.egg-info/SOURCES.txt
--rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 03:44:15.000000 diz-0.0.4/diz.egg-info/dependency_links.txt
--rw-r--r--   0 mj         (501) staff       (20)       37 2023-07-10 03:44:15.000000 diz-0.0.4/diz.egg-info/entry_points.txt
--rw-r--r--   0 mj         (501) staff       (20)       98 2023-07-10 03:44:15.000000 diz-0.0.4/diz.egg-info/requires.txt
--rw-r--r--   0 mj         (501) staff       (20)       15 2023-07-10 03:44:15.000000 diz-0.0.4/diz.egg-info/top_level.txt
--rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 03:44:16.007800 diz-0.0.4/setup.cfg
--rw-r--r--   0 mj         (501) staff       (20)      648 2023-07-10 03:41:56.000000 diz-0.0.4/setup.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:44:16.007472 diz-0.0.4/utils/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-0.0.4/utils/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-0.0.4/utils/dir.py
--rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-0.0.4/utils/download.py
--rw-r--r--   0 mj         (501) staff       (20)      758 2023-07-09 15:11:55.000000 diz-0.0.4/utils/pip.py
--rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-0.0.4/utils/validators.py
--rw-r--r--   0 mj         (501) staff       (20)      313 2023-07-09 14:46:10.000000 diz-0.0.4/utils/yaml.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:57:35.545819 diz-0.0.5/
+-rw-r--r--   0 mj         (501) staff       (20)      213 2023-07-10 03:57:35.545702 diz-0.0.5/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)       63 2023-07-10 03:31:32.000000 diz-0.0.5/README.md
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:57:35.543021 diz-0.0.5/diz/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-10 03:55:54.000000 diz-0.0.5/diz/__init__.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:57:35.543972 diz-0.0.5/diz/commands/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-0.0.5/diz/commands/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)     2108 2023-07-10 03:54:31.000000 diz-0.0.5/diz/commands/setup.py
+-rw-r--r--   0 mj         (501) staff       (20)      772 2023-07-10 03:56:40.000000 diz-0.0.5/diz/main.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:57:35.545418 diz-0.0.5/diz/utils/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-0.0.5/diz/utils/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-0.0.5/diz/utils/dir.py
+-rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-0.0.5/diz/utils/download.py
+-rw-r--r--   0 mj         (501) staff       (20)      762 2023-07-10 03:53:40.000000 diz-0.0.5/diz/utils/pip.py
+-rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-0.0.5/diz/utils/validators.py
+-rw-r--r--   0 mj         (501) staff       (20)      311 2023-07-10 03:53:40.000000 diz-0.0.5/diz/utils/yaml.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:57:35.543734 diz-0.0.5/diz.egg-info/
+-rw-r--r--   0 mj         (501) staff       (20)      213 2023-07-10 03:57:35.000000 diz-0.0.5/diz.egg-info/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)      377 2023-07-10 03:57:35.000000 diz-0.0.5/diz.egg-info/SOURCES.txt
+-rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 03:57:35.000000 diz-0.0.5/diz.egg-info/dependency_links.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 03:57:35.000000 diz-0.0.5/diz.egg-info/entry_points.txt
+-rw-r--r--   0 mj         (501) staff       (20)       98 2023-07-10 03:57:35.000000 diz-0.0.5/diz.egg-info/requires.txt
+-rw-r--r--   0 mj         (501) staff       (20)        4 2023-07-10 03:57:35.000000 diz-0.0.5/diz.egg-info/top_level.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 03:57:35.545857 diz-0.0.5/setup.cfg
+-rw-r--r--   0 mj         (501) staff       (20)      649 2023-07-10 03:57:25.000000 diz-0.0.5/setup.py
```

### Comparing `diz-0.0.4/commands/setup.py` & `diz-0.0.5/diz/commands/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os.path
 import git
-import utils.dir
-from utils import download, yaml, pip
+import diz.utils.dir
+from diz.utils import pip
+from diz.utils import download, yaml
 from toolz import pipe
 
 
 class SetupCommand:
     def __init__(self, pkg: str, path: str):
         self.pkg = pkg
         self.path = path
@@ -29,29 +30,29 @@
             path,
             lambda p: os.path.join(self.install_path, p),
             os.path.expanduser,
         )
         return target_path
 
     def clone_code(self):
-        if utils.dir.is_empty(self.create_dir("code", False)):
+        if diz.utils.dir.is_empty(self.create_dir("code", False)):
             git.Repo.clone_from(self.config['code_repo'], self.create_dir("code", False))
             print("下载完成！")
         else:
             print("已经下载过了，无需下载。")
 
     def download_model_from_huggingface(self):
-        if utils.dir.is_empty(self.create_dir("model", False)):
+        if diz.utils.dir.is_empty(self.create_dir("model", False)):
             download.save_huggingface_model(self.config['huggingface'], self.create_dir("model", False))
             print("下载完成！")
         else:
             print("已经下载过了，无需下载。")
 
     def create_venv(self):
-        if utils.dir.is_empty(self.create_dir("venv", False)):
+        if diz.utils.dir.is_empty(self.create_dir("venv", False)):
             os.system(f"cd {self.path} && python -m venv venv")
             print("创建虚拟环境完成！")
 
     def install_deps(self):
         venv_path = self.get_dir("venv")
         for dep in self.config['deps']:
             pip.install(dep, venv_path)
```

### Comparing `diz-0.0.4/setup.py` & `diz-0.0.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='diz',
-    version='0.0.4',
+    version='0.0.5',
     author='mjason',
     description='用来构建大模型环境的工具',
     long_description=readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'GitPython>=3.1.31',
@@ -20,11 +20,11 @@
         'PyYAML>=6.0',
         'requests>=2.31.0',
         'toolz>=0.12.0',
         'typer>=0.9.0'
     ],
     entry_points={
         'console_scripts': [
-            'diz = diz.main:app'
+            'diz = diz.main:main'
         ]
     }
 )
```

### Comparing `diz-0.0.4/utils/pip.py` & `diz-0.0.5/diz/utils/pip.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import subprocess
 import requests
-from utils import validators
+from diz.utils import validators
 import os
 import tempfile
 
 
 def run_command_in_venv(command, venv_path):
     activate_script = f"{venv_path}/bin/activate"
     cmd = f"source {activate_script} && {command}"
```

