# Comparing `tmp/optibar-1.0.1.tar.gz` & `tmp/optibar-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optibar-1.0.1.tar", last modified: Mon Jul 10 17:17:36 2023, max compression
+gzip compressed data, was "optibar-1.0.2.tar", last modified: Mon Jul 10 19:01:13 2023, max compression
```

## Comparing `optibar-1.0.1.tar` & `optibar-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 17:17:36.945004 optibar-1.0.1/
--rw-rw-rw-   0        0        0      779 2023-07-10 17:17:36.935172 optibar-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-10 17:17:36.925151 optibar-1.0.1/optibar/
--rw-rw-rw-   0        0        0     8340 2023-07-10 17:16:14.000000 optibar-1.0.1/optibar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 17:17:36.935172 optibar-1.0.1/optibar.egg-info/
--rw-rw-rw-   0        0        0      779 2023-07-10 17:17:36.000000 optibar-1.0.1/optibar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-07-10 17:17:36.000000 optibar-1.0.1/optibar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 17:17:36.000000 optibar-1.0.1/optibar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-10 17:17:36.000000 optibar-1.0.1/optibar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 17:17:36.945004 optibar-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1056 2023-07-10 17:17:11.000000 optibar-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 19:01:13.781730 optibar-1.0.2/
+-rw-rw-rw-   0        0        0      809 2023-07-10 19:01:13.780731 optibar-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-10 19:01:13.761575 optibar-1.0.2/optibar/
+-rw-rw-rw-   0        0        0     9102 2023-07-10 18:30:07.000000 optibar-1.0.2/optibar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 19:01:13.779732 optibar-1.0.2/optibar.egg-info/
+-rw-rw-rw-   0        0        0      809 2023-07-10 19:01:13.000000 optibar-1.0.2/optibar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-07-10 19:01:13.000000 optibar-1.0.2/optibar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 19:01:13.000000 optibar-1.0.2/optibar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-10 19:01:13.000000 optibar-1.0.2/optibar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 19:01:13.782731 optibar-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2023-07-10 18:36:23.000000 optibar-1.0.2/setup.py
```

### Comparing `optibar-1.0.1/PKG-INFO` & `optibar-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: optibar
-Version: 1.0.1
+Version: 1.0.2
 Summary: Make Advanced And Customizable ProgressBar
 Author: VenzTechnolo
 Author-email: venztechnolo@gmail.com
-Keywords: python,progress,progressbar,bar,python3
+Keywords: python,progress,progressbar,fast,bar,python3
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 
-OptiBar 1.0.1
+OptiBar 1.0.2
 
 Make Advanced And Customizable ProgressBar
 Fast, Optimized And Professonial
 Hello, welcome, the optibar module is very fast and allows
 you to customize to some extent to create an advanced bar,
 this website will teach you how you can create an advanced bar
 with this module, of course this module for now Made for
 pip users only,
 
-Bugs Fixed ! In New Version
+Bugs Fixed & Refreshed Again To Make It Is Quicker !
```

### Comparing `optibar-1.0.1/optibar/__init__.py` & `optibar-1.0.2/optibar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
                     a += " "
                 print ("\r  "+self.pmsg + "                                                                                " + a)
             else :
                 if self.st == 0 :
                     print (f"{self.details}\n{val_}{clm.Fore.RESET} {int (z * 2.5)}% / 100% - {self.value}{self.vn} / {self.max_value}{self.vn}{clm.Fore.RESET}",end="")
                     self.st = 1
                 elif self.st == 1 :
-                    print (f"\r{val_}{clm.Fore.RESET} {int (z * 2.5)}% / 100% - {self.value}{self.vn} / {self.max_value}{self.vn}{clm.Fore.RESET}",end="")
+                    print (f"\r{val_}{clm.Fore.RESET} {int (z * 2.5)}% / 100% - {self.value}{self.vn} / {self.max_value}{self.vn}{clm.Fore.RESET}                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          ",end="")
         else :
             if self.u == 0 :
                 self.u = 1
                 if self.e_mode == "error" :
                     print (f"\n{clm.Back.RED}{clm.Fore.WHITE} "+self.emsg+f" {clm.Back.RESET}{clm.Fore.RESET}")
                 elif self.e_mode == "bug" :
                     print (f"\n{clm.Back.YELLOW}{clm.Fore.WHITE} "+self.emsg+f" {clm.Back.RESET}{clm.Fore.RESET}")
```

### Comparing `optibar-1.0.1/optibar.egg-info/PKG-INFO` & `optibar-1.0.2/optibar.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: optibar
-Version: 1.0.1
+Version: 1.0.2
 Summary: Make Advanced And Customizable ProgressBar
 Author: VenzTechnolo
 Author-email: venztechnolo@gmail.com
-Keywords: python,progress,progressbar,bar,python3
+Keywords: python,progress,progressbar,fast,bar,python3
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 
-OptiBar 1.0.1
+OptiBar 1.0.2
 
 Make Advanced And Customizable ProgressBar
 Fast, Optimized And Professonial
 Hello, welcome, the optibar module is very fast and allows
 you to customize to some extent to create an advanced bar,
 this website will teach you how you can create an advanced bar
 with this module, of course this module for now Made for
 pip users only,
 
-Bugs Fixed ! In New Version
+Bugs Fixed & Refreshed Again To Make It Is Quicker !
```

### Comparing `optibar-1.0.1/setup.py` & `optibar-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'Make Advanced And Customizable ProgressBar'
-ld = """OptiBar 1.0.1\n
+ld = """OptiBar 1.0.2\n
 Make Advanced And Customizable ProgressBar
 Fast, Optimized And Professonial
 Hello, welcome, the optibar module is very fast and allows
 you to customize to some extent to create an advanced bar,
 this website will teach you how you can create an advanced bar
 with this module, of course this module for now Made for
 pip users only,\n
-Bugs Fixed ! In New Version"""
+Bugs Fixed & Refreshed Again To Make It Is Quicker !"""
 setup (
     name="optibar",
     version=VERSION,
     author="VenzTechnolo",
     author_email="venztechnolo@gmail.com",
     description=DESCRIPTION,
     long_description=ld,
     packages=find_packages(),
     py_modules=["colorama"],
-    keywords=["python", "progress", "progressbar", "bar", "python3"],
+    keywords=["python", "progress", "progressbar", "fast", "bar", "python3"],
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Development Status :: 4 - Beta"
     ]
 )
```

