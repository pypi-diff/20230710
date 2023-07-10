# Comparing `tmp/yplib-2.4.0.tar.gz` & `tmp/yplib-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.4.0.tar", last modified: Mon Jul 10 08:22:00 2023, max compression
+gzip compressed data, was "dist\yplib-2.4.1.tar", last modified: Mon Jul 10 08:24:06 2023, max compression
```

## Comparing `yplib-2.4.0.tar` & `yplib-2.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 08:22:00.087624 yplib-2.4.0/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.0/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-10 08:22:00.087441 yplib-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 08:22:00.088165 yplib-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-10 08:21:42.000000 yplib-2.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:22:00.083597 yplib-2.4.0/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.0/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.0/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.0/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.0/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.0/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.4.0/yplib/http_util.py
--rw-rw-rw-   0        0        0    32402 2023-07-10 08:21:25.000000 yplib-2.4.0/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.0/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.0/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.0/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.0/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:22:00.086735 yplib-2.4.0/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-10 08:22:00.000000 yplib-2.4.0/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-10 08:22:00.000000 yplib-2.4.0/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 08:22:00.000000 yplib-2.4.0/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 08:22:00.000000 yplib-2.4.0/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 08:24:05.998504 yplib-2.4.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.1/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-10 08:24:05.998029 yplib-2.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 08:24:05.998620 yplib-2.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-10 08:23:38.000000 yplib-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:24:05.995185 yplib-2.4.1/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.1/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.1/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.1/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.1/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.1/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.4.1/yplib/http_util.py
+-rw-rw-rw-   0        0        0    32402 2023-07-10 08:23:31.000000 yplib-2.4.1/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.1/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.1/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.1/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.1/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:24:05.997060 yplib-2.4.1/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-10 08:24:05.000000 yplib-2.4.1/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-10 08:24:05.000000 yplib-2.4.1/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 08:24:05.000000 yplib-2.4.1/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 08:24:05.000000 yplib-2.4.1/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.4.0/LICENSE` & `yplib-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.4.0/setup.py` & `yplib-2.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.4.0",
+  version="2.4.1",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.4.0/yplib/__init__.py` & `yplib-2.4.1/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.0/yplib/chart.py` & `yplib-2.4.1/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.0/yplib/chart_html.py` & `yplib-2.4.1/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.0/yplib/db.py` & `yplib-2.4.1/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.0/yplib/file.py` & `yplib-2.4.1/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.0/yplib/http_util.py` & `yplib-2.4.1/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.0/yplib/index.py` & `yplib-2.4.1/yplib/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import xlrd
 import xlwt
 
 
 # 是否是 windows 系统
 def is_win():
-    return platform.system().lower() == "windows"
+    return platform.system().lower() == 'windows'
 
 
 # 是否是 linux 系统, 不是 windows , 就是 linux 系统
 def is_linux():
     return not is_win()
```

### Comparing `yplib-2.4.0/yplib/mail.py` & `yplib-2.4.1/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.0/yplib/mail_html.py` & `yplib-2.4.1/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.0/yplib/markdown.py` & `yplib-2.4.1/yplib/markdown.py`

 * *Files identical despite different names*

