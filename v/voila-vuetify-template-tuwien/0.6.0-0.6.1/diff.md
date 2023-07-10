# Comparing `tmp/voila-vuetify-template-tuwien-0.6.0.tar.gz` & `tmp/voila-vuetify-template-tuwien-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila-vuetify-template-tuwien-0.6.0.tar", last modified: Fri Jul  7 16:42:44 2023, max compression
+gzip compressed data, was "voila-vuetify-template-tuwien-0.6.1.tar", last modified: Mon Jul 10 10:20:55 2023, max compression
```

## Comparing `voila-vuetify-template-tuwien-0.6.0.tar` & `voila-vuetify-template-tuwien-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-07 16:42:44.766631 voila-vuetify-template-tuwien-0.6.0/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1545 2022-11-11 09:41:41.000000 voila-vuetify-template-tuwien-0.6.0/LICENSE
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       16 2022-11-11 09:41:41.000000 voila-vuetify-template-tuwien-0.6.0/MANIFEST.in
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      290 2023-07-07 16:42:44.766631 voila-vuetify-template-tuwien-0.6.0/PKG-INFO
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1574 2022-11-11 09:41:41.000000 voila-vuetify-template-tuwien-0.6.0/README.md
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      101 2023-07-07 16:42:44.766631 voila-vuetify-template-tuwien-0.6.0/setup.cfg
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3303 2023-07-07 16:42:13.000000 voila-vuetify-template-tuwien-0.6.0/setup.py
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-07 16:42:44.762632 voila-vuetify-template-tuwien-0.6.0/share/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-07 16:42:44.762632 voila-vuetify-template-tuwien-0.6.0/share/jupyter/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-07 16:42:44.762632 voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-07 16:42:44.762632 voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-07 16:42:44.762632 voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base-tuwien/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7797 2022-11-11 09:41:41.000000 voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1434 2022-11-11 09:41:41.000000 voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       25 2022-11-11 09:41:41.000000 voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base-tuwien/conf.json
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3179 2022-11-11 09:41:41.000000 voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7280 2022-11-11 09:41:41.000000 voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-07 16:42:44.762632 voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-default-tuwien/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     6381 2022-11-11 09:41:41.000000 voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       40 2023-07-07 16:17:38.000000 voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-default-tuwien/conf.json
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-07 16:42:44.762632 voila-vuetify-template-tuwien-0.6.0/share/jupyter/voila/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-07 16:42:44.762632 voila-vuetify-template-tuwien-0.6.0/share/jupyter/voila/templates/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-07 16:42:44.762632 voila-vuetify-template-tuwien-0.6.0/share/jupyter/voila/templates/vuetify-base/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1764 2023-07-07 16:16:44.000000 voila-vuetify-template-tuwien-0.6.0/share/jupyter/voila/templates/vuetify-base/index.html.j2
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-07 16:42:44.766631 voila-vuetify-template-tuwien-0.6.0/voila_vuetify_template_tuwien.egg-info/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      290 2023-07-07 16:42:44.000000 voila-vuetify-template-tuwien-0.6.0/voila_vuetify_template_tuwien.egg-info/PKG-INFO
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      821 2023-07-07 16:42:44.000000 voila-vuetify-template-tuwien-0.6.0/voila_vuetify_template_tuwien.egg-info/SOURCES.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        1 2023-07-07 16:42:44.000000 voila-vuetify-template-tuwien-0.6.0/voila_vuetify_template_tuwien.egg-info/dependency_links.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       18 2023-07-07 16:42:44.000000 voila-vuetify-template-tuwien-0.6.0/voila_vuetify_template_tuwien.egg-info/requires.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        6 2023-07-07 16:42:44.000000 voila-vuetify-template-tuwien-0.6.0/voila_vuetify_template_tuwien.egg-info/top_level.txt
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1545 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/LICENSE
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       16 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/MANIFEST.in
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      290 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/PKG-INFO
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1574 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/README.md
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      101 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/setup.cfg
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3303 2023-07-10 10:20:43.000000 voila-vuetify-template-tuwien-0.6.1/setup.py
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.350322 voila-vuetify-template-tuwien-0.6.1/share/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.350322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.350322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.350322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7797 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1434 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       25 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/conf.json
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3179 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7280 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     6381 2023-07-10 10:15:36.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       40 2023-07-10 10:18:15.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/conf.json
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.350322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/voila/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.350322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/voila/templates/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/share/jupyter/voila/templates/vuetify-base-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1764 2023-07-10 10:19:21.000000 voila-vuetify-template-tuwien-0.6.1/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-10 10:20:55.354322 voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      290 2023-07-10 10:20:55.000000 voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/PKG-INFO
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      828 2023-07-10 10:20:55.000000 voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/SOURCES.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        1 2023-07-10 10:20:55.000000 voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/dependency_links.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       18 2023-07-10 10:20:55.000000 voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/requires.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        6 2023-07-10 10:20:55.000000 voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/top_level.txt
```

### Comparing `voila-vuetify-template-tuwien-0.6.0/LICENSE` & `voila-vuetify-template-tuwien-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.0/README.md` & `voila-vuetify-template-tuwien-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.0/setup.py` & `voila-vuetify-template-tuwien-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 for (dirpath, dirnames, filenames) in os.walk('share/jupyter/'):
     if filenames:
         data_files.append((dirpath, [os.path.join(dirpath, filename) for filename in filenames]))
 
 
 setup(
     name='voila-vuetify-template-tuwien',
-    version="0.6.0",
+    version="0.6.1",
     description="A vuetify template for Voila",
     data_files=data_files,
     install_requires=['voila>=0.2.0,<0.5'],
     include_package_data=True,
     url='https://gitlab.tuwien.ac.at/hpc/datalab/jupyter/voila/voila-vuetify-tu-wien-template',
     keywords=[
         'ipython',
```

### Comparing `voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js` & `voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html` & `voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2` & `voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js` & `voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html` & `voila-vuetify-template-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.0/share/jupyter/voila/templates/vuetify-base/index.html.j2` & `voila-vuetify-template-tuwien-0.6.1/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.0/voila_vuetify_template_tuwien.egg-info/SOURCES.txt` & `voila-vuetify-template-tuwien-0.6.1/voila_vuetify_template_tuwien.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js
 share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html
 share/jupyter/nbconvert/templates/vuetify-base-tuwien/conf.json
 share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2
 share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js
 share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html
 share/jupyter/nbconvert/templates/vuetify-default-tuwien/conf.json
-share/jupyter/voila/templates/vuetify-base/index.html.j2
+share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2
 voila_vuetify_template_tuwien.egg-info/PKG-INFO
 voila_vuetify_template_tuwien.egg-info/SOURCES.txt
 voila_vuetify_template_tuwien.egg-info/dependency_links.txt
 voila_vuetify_template_tuwien.egg-info/requires.txt
 voila_vuetify_template_tuwien.egg-info/top_level.txt
```

