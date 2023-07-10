# Comparing `tmp/waterfly-10.7.2023.tar.gz` & `tmp/waterfly-8.7.2023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waterfly-10.7.2023.tar", last modified: Mon Jul 10 19:13:15 2023, max compression
+gzip compressed data, was "waterfly-8.7.2023.tar", last modified: Sat Jul  8 18:40:09 2023, max compression
```

## Comparing `waterfly-10.7.2023.tar` & `waterfly-8.7.2023.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 19:13:15.820457 waterfly-10.7.2023/
--rw-rw-rw-   0        0        0     1899 2023-07-10 19:13:15.804838 waterfly-10.7.2023/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-10 19:13:15.820457 waterfly-10.7.2023/setup.cfg
--rw-rw-rw-   0        0        0     2163 2023-07-10 19:10:00.000000 waterfly-10.7.2023/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 19:13:15.773595 waterfly-10.7.2023/waterfly/
--rw-rw-rw-   0        0        0    21124 2023-07-10 19:07:12.000000 waterfly-10.7.2023/waterfly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 19:13:15.804838 waterfly-10.7.2023/waterfly.egg-info/
--rw-rw-rw-   0        0        0     1899 2023-07-10 19:13:15.000000 waterfly-10.7.2023/waterfly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-07-10 19:13:15.000000 waterfly-10.7.2023/waterfly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 19:13:15.000000 waterfly-10.7.2023/waterfly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-10 19:13:15.000000 waterfly-10.7.2023/waterfly.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 19:13:15.000000 waterfly-10.7.2023/waterfly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.640290 waterfly-8.7.2023/
+-rw-rw-rw-   0        0        0     1822 2023-07-08 18:40:09.640290 waterfly-8.7.2023/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-08 18:40:09.640290 waterfly-8.7.2023/setup.cfg
+-rw-rw-rw-   0        0        0     2173 2023-07-08 18:34:35.000000 waterfly-8.7.2023/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.593429 waterfly-8.7.2023/waterfly/
+-rw-rw-rw-   0        0        0     7887 2023-07-08 17:40:07.000000 waterfly-8.7.2023/waterfly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.640290 waterfly-8.7.2023/waterfly.egg-info/
+-rw-rw-rw-   0        0        0     1822 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/top_level.txt
```

### Comparing `waterfly-10.7.2023/PKG-INFO` & `waterfly-8.7.2023/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: waterfly
-Version: 10.7.2023
-Summary: Waterfly is a powerful new AI tool to create Firefly URLs, process images, and draw on images.
+Version: 8.7.2023
+Summary: Waterfly is a powerful new AI tool
 Author: Igor_Shapovalov_Andrejovich
 Author-email: igor.shapovalov.andrejovich@gmail.com
 
 
 
 Hi here!
 
@@ -20,15 +20,15 @@
 with an aspect ratio that is ideal for desktop backgrounds
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
 
 Already have the image you need? Edit it!
 
 The code that will remove the background:
-edit.backdrop('image.img', 'backdrop.img')
+edit.backdrop('image.img')
 You can add a vignette like this:
 edit.vignette('image.img', level)
 Turn the image into a cartoon:
 edit.cartoon('image.img')
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
```

### Comparing `waterfly-10.7.2023/setup.py` & `waterfly-8.7.2023/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
     name='waterfly',
-    version='10.7.2023',
+    version='8.7.2023',
     install_requires=[
         'googletrans>=3.1.0a0',
         'opencv-python',
-        'rembg',
-        'requests',
-        'pyautogui'
+        'rembg'
     ],
-    description='Waterfly is a powerful new AI tool to create Firefly URLs, process images, and draw on images.',
+    description='''Waterfly is a powerful new AI tool
+that reserves as partly an unofficial client for Adobe Firefly,
+to create Firefly URLs, process images, and draw on images.''',
     long_description='''
 
 Hi here!
 
 Create URLs for images and text styles, for example:
 create.image('Chocolate tree', ['hyper_realistic', 'cool_colors', 'studio_light'], 'portrait')
 Create a great photo of a chocolate tree for your Instagram stories with very realistic graphics,
@@ -26,15 +26,15 @@
 with an aspect ratio that is ideal for desktop backgrounds
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
 
 Already have the image you need? Edit it!
 
 The code that will remove the background:
-edit.backdrop('image.img', 'backdrop.img')
+edit.backdrop('image.img')
 You can add a vignette like this:
 edit.vignette('image.img', level)
 Turn the image into a cartoon:
 edit.cartoon('image.img')
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
```

### Comparing `waterfly-10.7.2023/waterfly.egg-info/PKG-INFO` & `waterfly-8.7.2023/waterfly.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: waterfly
-Version: 10.7.2023
-Summary: Waterfly is a powerful new AI tool to create Firefly URLs, process images, and draw on images.
+Version: 8.7.2023
+Summary: Waterfly is a powerful new AI tool
 Author: Igor_Shapovalov_Andrejovich
 Author-email: igor.shapovalov.andrejovich@gmail.com
 
 
 
 Hi here!
 
@@ -20,15 +20,15 @@
 with an aspect ratio that is ideal for desktop backgrounds
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
 
 Already have the image you need? Edit it!
 
 The code that will remove the background:
-edit.backdrop('image.img', 'backdrop.img')
+edit.backdrop('image.img')
 You can add a vignette like this:
 edit.vignette('image.img', level)
 Turn the image into a cartoon:
 edit.cartoon('image.img')
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
```

