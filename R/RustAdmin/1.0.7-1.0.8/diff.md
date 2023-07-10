# Comparing `tmp/RustAdmin-1.0.7.tar.gz` & `tmp/RustAdmin-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RustAdmin-1.0.7.tar", last modified: Sat Jul  8 20:27:33 2023, max compression
+gzip compressed data, was "RustAdmin-1.0.8.tar", last modified: Mon Jul 10 20:50:53 2023, max compression
```

## Comparing `RustAdmin-1.0.7.tar` & `RustAdmin-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 20:27:33.083735 RustAdmin-1.0.7/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      478 2023-07-08 20:27:33.083735 RustAdmin-1.0.7/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 20:27:33.079735 RustAdmin-1.0.7/RustAdmin.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      478 2023-07-08 20:27:32.000000 RustAdmin-1.0.7/RustAdmin.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      208 2023-07-08 20:27:32.000000 RustAdmin-1.0.7/RustAdmin.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-08 20:27:32.000000 RustAdmin-1.0.7/RustAdmin.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-07-08 20:27:32.000000 RustAdmin-1.0.7/RustAdmin.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-07-08 20:27:32.000000 RustAdmin-1.0.7/RustAdmin.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 20:27:33.083735 RustAdmin-1.0.7/admin/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-07-08 20:26:41.000000 RustAdmin-1.0.7/admin/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14449 2023-07-08 19:55:04.000000 RustAdmin-1.0.7/admin/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-08 20:27:33.083735 RustAdmin-1.0.7/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      643 2023-07-08 20:27:12.000000 RustAdmin-1.0.7/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 20:50:53.574926 RustAdmin-1.0.8/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      478 2023-07-10 20:50:53.574926 RustAdmin-1.0.8/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 20:50:53.574926 RustAdmin-1.0.8/RustAdmin.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      478 2023-07-10 20:50:53.000000 RustAdmin-1.0.8/RustAdmin.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      208 2023-07-10 20:50:53.000000 RustAdmin-1.0.8/RustAdmin.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 20:50:53.000000 RustAdmin-1.0.8/RustAdmin.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-07-10 20:50:53.000000 RustAdmin-1.0.8/RustAdmin.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-07-10 20:50:53.000000 RustAdmin-1.0.8/RustAdmin.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 20:50:53.574926 RustAdmin-1.0.8/admin/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-07-08 20:26:41.000000 RustAdmin-1.0.8/admin/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14445 2023-07-10 20:49:06.000000 RustAdmin-1.0.8/admin/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-10 20:50:53.574926 RustAdmin-1.0.8/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      643 2023-07-10 20:50:26.000000 RustAdmin-1.0.8/setup.py
```

### Comparing `RustAdmin-1.0.7/admin/main.py` & `RustAdmin-1.0.8/admin/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     app_dir = os.path.join(project_dir, "app")
     os.makedirs(app_dir)
 
     errors_dir = os.path.join(app_dir, "errors")
     os.makedirs(errors_dir)
 
-    templates_dir = os.path.join(app_dir, "templates")
+    templates_dir = os.path.join(app_dir, "views")
     os.makedirs(templates_dir)
 
     public_dir = os.path.join(app_dir, "public")
     os.makedirs(public_dir)
 
     with open(os.path.join(project_dir, "manage.py"), "w") as f:
         f.write(''' # Add your manage code here:
```

### Comparing `RustAdmin-1.0.7/setup.py` & `RustAdmin-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RustAdmin',
-    version='1.0.7',
+    version='1.0.8',
     author='Pawan Kumar',
     author_email='control@vvfin.in',
     include_package_data=True,
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
```

