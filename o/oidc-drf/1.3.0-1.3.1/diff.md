# Comparing `tmp/oidc_drf-1.3.0.tar.gz` & `tmp/oidc_drf-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_drf-1.3.0.tar", last modified: Mon Jul 10 09:32:16 2023, max compression
+gzip compressed data, was "oidc_drf-1.3.1.tar", last modified: Mon Jul 10 10:53:10 2023, max compression
```

## Comparing `oidc_drf-1.3.0.tar` & `oidc_drf-1.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 09:32:16.661878 oidc_drf-1.3.0/
--rw-r--r--   0 hmogbl     (501) staff       (20)     7299 2023-07-10 09:32:16.661740 oidc_drf-1.3.0/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)     6480 2023-07-06 10:57:47.000000 oidc_drf-1.3.0/README.md
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 09:32:16.660562 oidc_drf-1.3.0/oidc_drf/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.3.0/oidc_drf/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-05 17:40:53.000000 oidc_drf-1.3.0/oidc_drf/admin.py
--rw-r--r--   0 hmogbl     (501) staff       (20)    16022 2023-07-06 10:55:49.000000 oidc_drf-1.3.0/oidc_drf/backends.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     4767 2023-07-06 08:46:10.000000 oidc_drf-1.3.0/oidc_drf/drf.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 09:32:16.661546 oidc_drf-1.3.0/oidc_drf/migrations/
--rw-r--r--   0 hmogbl     (501) staff       (20)      737 2023-07-10 09:25:40.000000 oidc_drf-1.3.0/oidc_drf/migrations/0001_initial.py
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.3.0/oidc_drf/migrations/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      277 2023-07-06 10:54:59.000000 oidc_drf-1.3.0/oidc_drf/models.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.3.0/oidc_drf/urls.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     2759 2023-07-06 05:52:37.000000 oidc_drf-1.3.0/oidc_drf/utils.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     8348 2023-07-06 10:55:47.000000 oidc_drf-1.3.0/oidc_drf/views.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 09:32:16.661191 oidc_drf-1.3.0/oidc_drf.egg-info/
--rw-r--r--   0 hmogbl     (501) staff       (20)     7299 2023-07-10 09:32:16.000000 oidc_drf-1.3.0/oidc_drf.egg-info/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)      393 2023-07-10 09:32:16.000000 oidc_drf-1.3.0/oidc_drf.egg-info/SOURCES.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-10 09:32:16.000000 oidc_drf-1.3.0/oidc_drf.egg-info/dependency_links.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-10 09:32:16.000000 oidc_drf-1.3.0/oidc_drf.egg-info/requires.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-10 09:32:16.000000 oidc_drf-1.3.0/oidc_drf.egg-info/top_level.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-10 09:32:16.661915 oidc_drf-1.3.0/setup.cfg
--rw-r--r--   0 hmogbl     (501) staff       (20)     1197 2023-07-10 09:27:55.000000 oidc_drf-1.3.0/setup.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 10:53:10.521790 oidc_drf-1.3.1/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     7299 2023-07-10 10:53:10.521657 oidc_drf-1.3.1/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)     6480 2023-07-06 10:57:47.000000 oidc_drf-1.3.1/README.md
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 10:53:10.520199 oidc_drf-1.3.1/oidc_drf/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.3.1/oidc_drf/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      797 2023-07-10 10:52:57.000000 oidc_drf-1.3.1/oidc_drf/admin.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)    16022 2023-07-06 10:55:49.000000 oidc_drf-1.3.1/oidc_drf/backends.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4767 2023-07-06 08:46:10.000000 oidc_drf-1.3.1/oidc_drf/drf.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 10:53:10.521493 oidc_drf-1.3.1/oidc_drf/migrations/
+-rw-r--r--   0 hmogbl     (501) staff       (20)      737 2023-07-10 09:25:40.000000 oidc_drf-1.3.1/oidc_drf/migrations/0001_initial.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.3.1/oidc_drf/migrations/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      277 2023-07-06 10:54:59.000000 oidc_drf-1.3.1/oidc_drf/models.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.3.1/oidc_drf/urls.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     2759 2023-07-06 05:52:37.000000 oidc_drf-1.3.1/oidc_drf/utils.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     8348 2023-07-06 10:55:47.000000 oidc_drf-1.3.1/oidc_drf/views.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-10 10:53:10.521053 oidc_drf-1.3.1/oidc_drf.egg-info/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     7299 2023-07-10 10:53:10.000000 oidc_drf-1.3.1/oidc_drf.egg-info/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)      393 2023-07-10 10:53:10.000000 oidc_drf-1.3.1/oidc_drf.egg-info/SOURCES.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-10 10:53:10.000000 oidc_drf-1.3.1/oidc_drf.egg-info/dependency_links.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-10 10:53:10.000000 oidc_drf-1.3.1/oidc_drf.egg-info/requires.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-10 10:53:10.000000 oidc_drf-1.3.1/oidc_drf.egg-info/top_level.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-10 10:53:10.521834 oidc_drf-1.3.1/setup.cfg
+-rw-r--r--   0 hmogbl     (501) staff       (20)     1197 2023-07-10 10:53:05.000000 oidc_drf-1.3.1/setup.py
```

### Comparing `oidc_drf-1.3.0/PKG-INFO` & `oidc_drf-1.3.1/oidc_drf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oidc_drf
-Version: 1.3.0
+Name: oidc-drf
+Version: 1.3.1
 Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.3.0/README.md` & `oidc_drf-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.3.0/oidc_drf/admin.py` & `oidc_drf-1.3.1/oidc_drf/admin.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 
 class OIDCExtraDataAdmin(admin.ModelAdmin):
     list_display = ['user', 'formatted_oidc_data']
     readonly_fields = ('formatted_oidc_data',)
     exclude = ('data',)  # Exclude the original oidc_data field
 
     def formatted_oidc_data(self, obj):
-        oidc_data = json.loads(obj.data)
-        formatted_data = json.dumps(oidc_data, indent=4)
-        return formatted_data
+        if obj.data:
+            oidc_data = json.loads(obj.data)
+            formatted_data = json.dumps(oidc_data, indent=4)
+            return formatted_data
+        return ""
 
     formatted_oidc_data.short_description = 'OIDC Data'
 
 
+    list_display = ['user', 'formatted_oidc_data']
+    readonly_fields = ('formatted_oidc_data',)
+    exclude = ('data',)  # Exclude the original oidc_data field
+    
+
 admin.site.register(OIDCExtraData, OIDCExtraDataAdmin)
```

### Comparing `oidc_drf-1.3.0/oidc_drf/backends.py` & `oidc_drf-1.3.1/oidc_drf/backends.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.3.0/oidc_drf/drf.py` & `oidc_drf-1.3.1/oidc_drf/drf.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.3.0/oidc_drf/migrations/0001_initial.py` & `oidc_drf-1.3.1/oidc_drf/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.3.0/oidc_drf/utils.py` & `oidc_drf-1.3.1/oidc_drf/utils.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.3.0/oidc_drf/views.py` & `oidc_drf-1.3.1/oidc_drf/views.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.3.0/oidc_drf.egg-info/PKG-INFO` & `oidc_drf-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oidc-drf
-Version: 1.3.0
+Name: oidc_drf
+Version: 1.3.1
 Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.3.0/setup.py` & `oidc_drf-1.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='oidc_drf',
-    version='1.3.0',
+    version='1.3.1',
     author='Hamad Almogbl',
     author_email='hamad.almogbl@gmail.com',
     description='Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/halmogbl/oidc_drf',
     packages=find_packages(),
```

