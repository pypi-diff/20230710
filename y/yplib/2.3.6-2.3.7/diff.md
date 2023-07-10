# Comparing `tmp/yplib-2.3.6.tar.gz` & `tmp/yplib-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.3.6.tar", last modified: Mon Jul 10 01:59:53 2023, max compression
+gzip compressed data, was "dist\yplib-2.3.7.tar", last modified: Mon Jul 10 03:20:24 2023, max compression
```

## Comparing `yplib-2.3.6.tar` & `yplib-2.3.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 01:59:53.531352 yplib-2.3.6/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.6/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-10 01:59:53.530609 yplib-2.3.6/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 01:59:53.531426 yplib-2.3.6/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-10 01:59:40.000000 yplib-2.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 01:59:53.525761 yplib-2.3.6/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.6/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-07 00:30:37.000000 yplib-2.3.6/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.6/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1285 2023-07-10 01:59:01.000000 yplib-2.3.6/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.6/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.6/yplib/http_util.py
--rw-rw-rw-   0        0        0    32089 2023-07-10 01:02:03.000000 yplib-2.3.6/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.6/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.6/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.6/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.6/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-10 01:59:53.529818 yplib-2.3.6/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-10 01:59:53.000000 yplib-2.3.6/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-10 01:59:53.000000 yplib-2.3.6/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 01:59:53.000000 yplib-2.3.6/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 01:59:53.000000 yplib-2.3.6/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 03:20:24.145800 yplib-2.3.7/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.7/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-10 03:20:24.145800 yplib-2.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 03:20:24.145800 yplib-2.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-10 03:20:08.000000 yplib-2.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 03:20:24.134987 yplib-2.3.7/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.7/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-07 00:30:37.000000 yplib-2.3.7/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.7/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1285 2023-07-10 01:59:01.000000 yplib-2.3.7/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.7/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.7/yplib/http_util.py
+-rw-rw-rw-   0        0        0    32177 2023-07-10 03:17:28.000000 yplib-2.3.7/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.7/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.7/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.7/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.7/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-10 03:20:24.144902 yplib-2.3.7/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-10 03:20:23.000000 yplib-2.3.7/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-10 03:20:23.000000 yplib-2.3.7/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 03:20:23.000000 yplib-2.3.7/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 03:20:23.000000 yplib-2.3.7/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.3.6/LICENSE` & `yplib-2.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.3.6/setup.py` & `yplib-2.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.3.6",
+  version="2.3.7",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.3.6/yplib/__init__.py` & `yplib-2.3.7/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.6/yplib/chart.py` & `yplib-2.3.7/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.6/yplib/chart_html.py` & `yplib-2.3.7/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.6/yplib/db.py` & `yplib-2.3.7/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.6/yplib/file.py` & `yplib-2.3.7/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.6/yplib/http_util.py` & `yplib-2.3.7/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.6/yplib/index.py` & `yplib-2.3.7/yplib/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,20 +141,19 @@
             p_n = sep.join(f_n[0:i])
             if not os.path.exists(p_n):
                 os.mkdir(p_n)
 
 
 # 获得文件名称
 # 按照  name_天小时分钟_秒毫秒随机数 的规则来生成
-def get_file_name(file_name, suffix='.txt'):
-    [day, hour, minute, second, ss] = datetime.today().strftime('%d_%H_%M_%S_%f').split('_')
-    return str(file_name) \
-        + '_' + day + hour + minute \
-        + '_' + second + ss[0] + random_int_str(1) \
-        + suffix
+def get_file_name(file_name, suffix='.txt', is_date=False):
+    # %Y-%m-%d %H:%M:%S
+    [year, month, day, hour, minute, second, ss] = datetime.today().strftime('%Y_%m_%d_%H_%M_%S_%f').split('_')
+    s = year + month + day + '_' + hour + minute if is_date else hour + minute
+    return str(file_name) + '_' + s + '_' + second + ss[0] + random_int_str(1) + suffix
 
 
 # 文件是否存在
 def file_is_empty(file_name=None):
     return file_name is None or file_name == '' or not os.path.exists(file_name)
```

### Comparing `yplib-2.3.6/yplib/mail.py` & `yplib-2.3.7/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.6/yplib/mail_html.py` & `yplib-2.3.7/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.6/yplib/markdown.py` & `yplib-2.3.7/yplib/markdown.py`

 * *Files identical despite different names*

