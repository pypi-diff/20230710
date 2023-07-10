# Comparing `tmp/diz-0.0.8.tar.gz` & `tmp/diz-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diz-0.0.8.tar", last modified: Mon Jul 10 07:30:00 2023, max compression
+gzip compressed data, was "diz-0.0.9.tar", last modified: Mon Jul 10 07:32:12 2023, max compression
```

## Comparing `diz-0.0.8.tar` & `diz-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:30:00.327637 diz-0.0.8/
--rw-r--r--   0 mj         (501) staff       (20)     1368 2023-07-10 07:30:00.327514 diz-0.0.8/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)     1218 2023-07-10 07:28:47.000000 diz-0.0.8/README.md
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:30:00.324674 diz-0.0.8/diz/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-10 03:55:54.000000 diz-0.0.8/diz/__init__.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:30:00.325826 diz-0.0.8/diz/commands/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-0.0.8/diz/commands/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)      480 2023-07-10 07:28:31.000000 diz-0.0.8/diz/commands/install.py
--rw-r--r--   0 mj         (501) staff       (20)     2108 2023-07-10 03:54:31.000000 diz-0.0.8/diz/commands/setup.py
--rw-r--r--   0 mj         (501) staff       (20)      870 2023-07-10 07:08:04.000000 diz-0.0.8/diz/commands/shell.py
--rw-r--r--   0 mj         (501) staff       (20)     1572 2023-07-10 07:26:28.000000 diz-0.0.8/diz/main.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:30:00.327211 diz-0.0.8/diz/utils/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-0.0.8/diz/utils/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-0.0.8/diz/utils/dir.py
--rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-0.0.8/diz/utils/download.py
--rw-r--r--   0 mj         (501) staff       (20)      762 2023-07-10 04:14:00.000000 diz-0.0.8/diz/utils/pip.py
--rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-0.0.8/diz/utils/validators.py
--rw-r--r--   0 mj         (501) staff       (20)      308 2023-07-10 04:14:09.000000 diz-0.0.8/diz/utils/yaml.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:30:00.325317 diz-0.0.8/diz.egg-info/
--rw-r--r--   0 mj         (501) staff       (20)     1368 2023-07-10 07:30:00.000000 diz-0.0.8/diz.egg-info/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)      423 2023-07-10 07:30:00.000000 diz-0.0.8/diz.egg-info/SOURCES.txt
--rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 07:30:00.000000 diz-0.0.8/diz.egg-info/dependency_links.txt
--rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 07:30:00.000000 diz-0.0.8/diz.egg-info/entry_points.txt
--rw-r--r--   0 mj         (501) staff       (20)      129 2023-07-10 07:30:00.000000 diz-0.0.8/diz.egg-info/requires.txt
--rw-r--r--   0 mj         (501) staff       (20)        4 2023-07-10 07:30:00.000000 diz-0.0.8/diz.egg-info/top_level.txt
--rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 07:30:00.327679 diz-0.0.8/setup.cfg
--rw-r--r--   0 mj         (501) staff       (20)      703 2023-07-10 07:29:17.000000 diz-0.0.8/setup.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:32:12.650825 diz-0.0.9/
+-rw-r--r--   0 mj         (501) staff       (20)     1368 2023-07-10 07:32:12.650706 diz-0.0.9/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)     1218 2023-07-10 07:28:47.000000 diz-0.0.9/README.md
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:32:12.648302 diz-0.0.9/diz/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-10 03:55:54.000000 diz-0.0.9/diz/__init__.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:32:12.649803 diz-0.0.9/diz/commands/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-0.0.9/diz/commands/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)      480 2023-07-10 07:28:31.000000 diz-0.0.9/diz/commands/install.py
+-rw-r--r--   0 mj         (501) staff       (20)     2146 2023-07-10 07:31:06.000000 diz-0.0.9/diz/commands/setup.py
+-rw-r--r--   0 mj         (501) staff       (20)      870 2023-07-10 07:08:04.000000 diz-0.0.9/diz/commands/shell.py
+-rw-r--r--   0 mj         (501) staff       (20)     1572 2023-07-10 07:26:28.000000 diz-0.0.9/diz/main.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:32:12.650530 diz-0.0.9/diz/utils/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-0.0.9/diz/utils/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-0.0.9/diz/utils/dir.py
+-rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-0.0.9/diz/utils/download.py
+-rw-r--r--   0 mj         (501) staff       (20)      762 2023-07-10 04:14:00.000000 diz-0.0.9/diz/utils/pip.py
+-rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-0.0.9/diz/utils/validators.py
+-rw-r--r--   0 mj         (501) staff       (20)      308 2023-07-10 04:14:09.000000 diz-0.0.9/diz/utils/yaml.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:32:12.649191 diz-0.0.9/diz.egg-info/
+-rw-r--r--   0 mj         (501) staff       (20)     1368 2023-07-10 07:32:12.000000 diz-0.0.9/diz.egg-info/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)      423 2023-07-10 07:32:12.000000 diz-0.0.9/diz.egg-info/SOURCES.txt
+-rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 07:32:12.000000 diz-0.0.9/diz.egg-info/dependency_links.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 07:32:12.000000 diz-0.0.9/diz.egg-info/entry_points.txt
+-rw-r--r--   0 mj         (501) staff       (20)      129 2023-07-10 07:32:12.000000 diz-0.0.9/diz.egg-info/requires.txt
+-rw-r--r--   0 mj         (501) staff       (20)        4 2023-07-10 07:32:12.000000 diz-0.0.9/diz.egg-info/top_level.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 07:32:12.650864 diz-0.0.9/setup.cfg
+-rw-r--r--   0 mj         (501) staff       (20)      703 2023-07-10 07:31:57.000000 diz-0.0.9/setup.py
```

### Comparing `diz-0.0.8/PKG-INFO` & `diz-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diz
-Version: 0.0.8
+Version: 0.0.9
 Summary: 用来构建大模型环境的工具
 Author: mjason
 Description-Content-Type: text/markdown
 
 # diz
 
 目前开源的大模型项目普遍来说都有如下问题：
```

### Comparing `diz-0.0.8/README.md` & `diz-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `diz-0.0.8/diz/commands/setup.py` & `diz-0.0.9/diz/commands/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,14 +52,15 @@
             os.system(f"cd {self.path} && python -m venv venv")
             print("创建虚拟环境完成！")
 
     def install_deps(self):
         venv_path = self.get_dir("venv")
         for dep in self.config['deps']:
             pip.install(dep, venv_path)
+        pip.install("diz", venv_path)
 
     def run(self):
         self.create_dir("code")
         self.create_dir("model")
         self.clone_code()
         self.download_model_from_huggingface()
         self.create_venv()
```

### Comparing `diz-0.0.8/diz/commands/shell.py` & `diz-0.0.9/diz/commands/shell.py`

 * *Files identical despite different names*

### Comparing `diz-0.0.8/diz/main.py` & `diz-0.0.9/diz/main.py`

 * *Files identical despite different names*

### Comparing `diz-0.0.8/diz/utils/pip.py` & `diz-0.0.9/diz/utils/pip.py`

 * *Files identical despite different names*

### Comparing `diz-0.0.8/diz.egg-info/PKG-INFO` & `diz-0.0.9/diz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diz
-Version: 0.0.8
+Version: 0.0.9
 Summary: 用来构建大模型环境的工具
 Author: mjason
 Description-Content-Type: text/markdown
 
 # diz
 
 目前开源的大模型项目普遍来说都有如下问题：
```

### Comparing `diz-0.0.8/setup.py` & `diz-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='diz',
-    version='0.0.8',
+    version='0.0.9',
     author='mjason',
     description='用来构建大模型环境的工具',
     long_description=readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'GitPython>=3.1.31',
```

