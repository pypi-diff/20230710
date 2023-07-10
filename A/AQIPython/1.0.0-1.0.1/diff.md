# Comparing `tmp/AQIPython-1.0.0.tar.gz` & `tmp/AQIPython-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AQIPython-1.0.0.tar", last modified: Mon Jul 10 19:44:49 2023, max compression
+gzip compressed data, was "dist/AQIPython-1.0.1.tar", last modified: Mon Jul 10 21:01:45 2023, max compression
```

## Comparing `AQIPython-1.0.0.tar` & `AQIPython-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 spritan   (1000) spritan   (1000)        0 2023-07-10 19:44:49.000000 AQIPython-1.0.0/
-drwxrwxrwx   0 spritan   (1000) spritan   (1000)        0 2023-07-10 19:44:49.000000 AQIPython-1.0.0/AQIPython/
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)       35 2023-07-10 16:21:49.000000 AQIPython-1.0.0/AQIPython/__init__.py
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)     1241 2023-07-10 19:34:25.000000 AQIPython-1.0.0/AQIPython/aqi_Calc.py
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)     3754 2023-07-10 19:11:58.000000 AQIPython-1.0.0/AQIPython/breakPoints.py
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)     1855 2023-07-10 19:11:16.000000 AQIPython-1.0.0/AQIPython/errorCustom.py
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)      651 2023-07-10 18:18:12.000000 AQIPython-1.0.0/AQIPython/unitOperations.py
-drwxrwxrwx   0 spritan   (1000) spritan   (1000)        0 2023-07-10 19:44:49.000000 AQIPython-1.0.0/AQIPython.egg-info/
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)     2931 2023-07-10 19:44:48.000000 AQIPython-1.0.0/AQIPython.egg-info/PKG-INFO
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)      324 2023-07-10 19:44:48.000000 AQIPython-1.0.0/AQIPython.egg-info/SOURCES.txt
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)        1 2023-07-10 19:44:48.000000 AQIPython-1.0.0/AQIPython.egg-info/dependency_links.txt
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)       20 2023-07-10 19:44:48.000000 AQIPython-1.0.0/AQIPython.egg-info/requires.txt
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)       10 2023-07-10 19:44:48.000000 AQIPython-1.0.0/AQIPython.egg-info/top_level.txt
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)     1100 2023-07-10 15:29:20.000000 AQIPython-1.0.0/LICENSE
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)       25 2023-07-10 15:29:20.000000 AQIPython-1.0.0/MANIFEST.in
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)     2931 2023-07-10 19:44:49.000000 AQIPython-1.0.0/PKG-INFO
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)     2429 2023-07-10 19:43:06.000000 AQIPython-1.0.0/README.md
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)       38 2023-07-10 19:44:49.000000 AQIPython-1.0.0/setup.cfg
--rwxrwxrwx   0 spritan   (1000) spritan   (1000)      877 2023-07-10 19:12:23.000000 AQIPython-1.0.0/setup.py
+drwxrwxrwx   0 spritan   (1000) spritan   (1000)        0 2023-07-10 21:01:45.000000 AQIPython-1.0.1/
+drwxrwxrwx   0 spritan   (1000) spritan   (1000)        0 2023-07-10 21:01:45.000000 AQIPython-1.0.1/AQIPython/
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)       35 2023-07-10 16:21:49.000000 AQIPython-1.0.1/AQIPython/__init__.py
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)     1241 2023-07-10 19:34:25.000000 AQIPython-1.0.1/AQIPython/aqi_Calc.py
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)     3754 2023-07-10 19:11:58.000000 AQIPython-1.0.1/AQIPython/breakPoints.py
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)     1855 2023-07-10 19:11:16.000000 AQIPython-1.0.1/AQIPython/errorCustom.py
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)      651 2023-07-10 18:18:12.000000 AQIPython-1.0.1/AQIPython/unitOperations.py
+drwxrwxrwx   0 spritan   (1000) spritan   (1000)        0 2023-07-10 21:01:45.000000 AQIPython-1.0.1/AQIPython.egg-info/
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)     2979 2023-07-10 21:01:45.000000 AQIPython-1.0.1/AQIPython.egg-info/PKG-INFO
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)      324 2023-07-10 21:01:45.000000 AQIPython-1.0.1/AQIPython.egg-info/SOURCES.txt
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)        1 2023-07-10 21:01:45.000000 AQIPython-1.0.1/AQIPython.egg-info/dependency_links.txt
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)       20 2023-07-10 21:01:45.000000 AQIPython-1.0.1/AQIPython.egg-info/requires.txt
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)       10 2023-07-10 21:01:45.000000 AQIPython-1.0.1/AQIPython.egg-info/top_level.txt
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)     1100 2023-07-10 15:29:20.000000 AQIPython-1.0.1/LICENSE
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)       25 2023-07-10 15:29:20.000000 AQIPython-1.0.1/MANIFEST.in
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)     2979 2023-07-10 21:01:45.000000 AQIPython-1.0.1/PKG-INFO
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)     2429 2023-07-10 19:43:06.000000 AQIPython-1.0.1/README.md
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)       38 2023-07-10 21:01:45.000000 AQIPython-1.0.1/setup.cfg
+-rwxrwxrwx   0 spritan   (1000) spritan   (1000)      943 2023-07-10 21:00:07.000000 AQIPython-1.0.1/setup.py
```

### Comparing `AQIPython-1.0.0/AQIPython/aqi_Calc.py` & `AQIPython-1.0.1/AQIPython/aqi_Calc.py`

 * *Files identical despite different names*

### Comparing `AQIPython-1.0.0/AQIPython/breakPoints.py` & `AQIPython-1.0.1/AQIPython/breakPoints.py`

 * *Files identical despite different names*

### Comparing `AQIPython-1.0.0/AQIPython/errorCustom.py` & `AQIPython-1.0.1/AQIPython/errorCustom.py`

 * *Files identical despite different names*

### Comparing `AQIPython-1.0.0/AQIPython/unitOperations.py` & `AQIPython-1.0.1/AQIPython/unitOperations.py`

 * *Files identical despite different names*

### Comparing `AQIPython-1.0.0/AQIPython.egg-info/PKG-INFO` & `AQIPython-1.0.1/AQIPython.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: AQIPython
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Multistandard python AQI calculator library 
 Home-page: https://github.com/Spritan/AQIPython
 Author: Spritan
 Author-email: proypabsab@gmail.com
 License: MIT
+Keywords: AQI,Air Quality,Sensors,IOT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Healthcare Industry
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # AQIPython
```

### Comparing `AQIPython-1.0.0/LICENSE` & `AQIPython-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AQIPython-1.0.0/PKG-INFO` & `AQIPython-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: AQIPython
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Multistandard python AQI calculator library 
 Home-page: https://github.com/Spritan/AQIPython
 Author: Spritan
 Author-email: proypabsab@gmail.com
 License: MIT
+Keywords: AQI,Air Quality,Sensors,IOT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Healthcare Industry
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # AQIPython
```

### Comparing `AQIPython-1.0.0/README.md` & `AQIPython-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `AQIPython-1.0.0/setup.py` & `AQIPython-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import find_packages, setup
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="AQIPython",
-    version="1.0.0",
+    version="1.0.1",
     description="A Multistandard python AQI calculator library ",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Spritan/AQIPython",
     author="Spritan",
     author_email="proypabsab@gmail.com",
     license="MIT",
+    keywords = ["AQI", "Air Quality", "Sensors","IOT"],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Education',
+        'Intended Audience :: Healthcare Industry',
         "Programming Language :: Python",
         "Operating System :: OS Independent",
     ],
     # install_requires=["bson >= 0.5.10"],
     extras_require={
         "dev": ["twine>=4.0.2"],
     },
```

