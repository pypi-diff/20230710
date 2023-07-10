# Comparing `tmp/yplib-2.3.4.tar.gz` & `tmp/yplib-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.3.4.tar", last modified: Mon Jul 10 00:56:43 2023, max compression
+gzip compressed data, was "dist\yplib-2.3.5.tar", last modified: Mon Jul 10 01:03:33 2023, max compression
```

## Comparing `yplib-2.3.4.tar` & `yplib-2.3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 00:56:43.153315 yplib-2.3.4/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.4/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-10 00:56:43.152497 yplib-2.3.4/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 00:56:43.153315 yplib-2.3.4/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-10 00:56:21.000000 yplib-2.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 00:56:43.138952 yplib-2.3.4/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.4/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-07 00:30:37.000000 yplib-2.3.4/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.4/yplib/chart_html.py
--rw-rw-rw-   0        0        0      892 2023-07-07 00:36:13.000000 yplib-2.3.4/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.4/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.4/yplib/http_util.py
--rw-rw-rw-   0        0        0    31619 2023-07-10 00:55:20.000000 yplib-2.3.4/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.4/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.4/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.4/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.4/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-10 00:56:43.151884 yplib-2.3.4/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-10 00:56:42.000000 yplib-2.3.4/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-10 00:56:42.000000 yplib-2.3.4/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 00:56:42.000000 yplib-2.3.4/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 00:56:42.000000 yplib-2.3.4/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 01:03:33.982107 yplib-2.3.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.5/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-10 01:03:33.981652 yplib-2.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 01:03:33.982107 yplib-2.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-10 01:02:40.000000 yplib-2.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 01:03:33.978014 yplib-2.3.5/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.5/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-07 00:30:37.000000 yplib-2.3.5/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.5/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      892 2023-07-07 00:36:13.000000 yplib-2.3.5/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.5/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.5/yplib/http_util.py
+-rw-rw-rw-   0        0        0    32089 2023-07-10 01:02:03.000000 yplib-2.3.5/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.5/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.5/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.5/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.5/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-10 01:03:33.980571 yplib-2.3.5/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-10 01:03:33.000000 yplib-2.3.5/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-10 01:03:33.000000 yplib-2.3.5/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 01:03:33.000000 yplib-2.3.5/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 01:03:33.000000 yplib-2.3.5/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.3.4/LICENSE` & `yplib-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.3.4/setup.py` & `yplib-2.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.3.4",
+  version="2.3.5",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.3.4/yplib/__init__.py` & `yplib-2.3.5/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.4/yplib/chart.py` & `yplib-2.3.5/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.4/yplib/chart_html.py` & `yplib-2.3.5/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.4/yplib/db.py` & `yplib-2.3.5/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.4/yplib/file.py` & `yplib-2.3.5/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.4/yplib/http_util.py` & `yplib-2.3.5/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.4/yplib/index.py` & `yplib-2.3.5/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,21 @@
 # 将 log 数据, 写入到文件
 def to_print_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                   a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     lo = to_print(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
     to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'print', True, '.txt')
 
 
+# 将 log 数据, 写入到文件, 固定文件名称
+def to_print_txt(file_name, a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
+                 a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
+    lo = to_print(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
+    to_txt([lo], file_name, 'print', True, '.txt')
+
+
 # 将 log 数据, 写入到文件
 def to_log_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                 a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20='', time_prefix=True):
     lo = to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20, time_prefix=time_prefix)
     to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'log', True, '.log')
 
 
@@ -343,15 +350,15 @@
         s = json.dumps(data)
     else:
         s = str(data)
     return s
 
 
 # 匹配字符串
-# 可以参考 正则表达式的操作
+# 可以参考 正则表达式的操作, 可以使用 chatgpt 帮忙写出这段代码
 # pattern = r"CREATE TABLE (\w+)"
 # @see https://www.runoob.com/python3/python3-reg-expressions.html
 def match_str(pattern, str_a=''):
     match = re.search(pattern, str_a, re.I)
     if match:
         return match.group(1)
     else:
```

### Comparing `yplib-2.3.4/yplib/mail.py` & `yplib-2.3.5/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.4/yplib/mail_html.py` & `yplib-2.3.5/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.4/yplib/markdown.py` & `yplib-2.3.5/yplib/markdown.py`

 * *Files identical despite different names*

