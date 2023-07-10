# Comparing `tmp/yplib-2.3.3.tar.gz` & `tmp/yplib-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.3.3.tar", last modified: Fri Jul  7 01:02:48 2023, max compression
+gzip compressed data, was "dist\yplib-2.3.4.tar", last modified: Mon Jul 10 00:56:43 2023, max compression
```

## Comparing `yplib-2.3.3.tar` & `yplib-2.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 01:02:48.923077 yplib-2.3.3/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.3/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-07 01:02:48.922958 yplib-2.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 01:02:48.923483 yplib-2.3.3/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-07 01:01:47.000000 yplib-2.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 01:02:48.919192 yplib-2.3.3/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.3/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-07 00:30:37.000000 yplib-2.3.3/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.3/yplib/chart_html.py
--rw-rw-rw-   0        0        0      892 2023-07-07 00:36:13.000000 yplib-2.3.3/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.3/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.3/yplib/http_util.py
--rw-rw-rw-   0        0        0    30937 2023-07-07 00:55:03.000000 yplib-2.3.3/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.3/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.3/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.3/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.3/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-07 01:02:48.921989 yplib-2.3.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-07 01:02:48.000000 yplib-2.3.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-07 01:02:48.000000 yplib-2.3.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 01:02:48.000000 yplib-2.3.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 01:02:48.000000 yplib-2.3.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 00:56:43.153315 yplib-2.3.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.4/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-10 00:56:43.152497 yplib-2.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 00:56:43.153315 yplib-2.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-10 00:56:21.000000 yplib-2.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 00:56:43.138952 yplib-2.3.4/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-07 00:30:37.000000 yplib-2.3.4/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.4/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      892 2023-07-07 00:36:13.000000 yplib-2.3.4/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.4/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.4/yplib/http_util.py
+-rw-rw-rw-   0        0        0    31619 2023-07-10 00:55:20.000000 yplib-2.3.4/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.4/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.4/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.4/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.4/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-10 00:56:43.151884 yplib-2.3.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-10 00:56:42.000000 yplib-2.3.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-10 00:56:42.000000 yplib-2.3.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 00:56:42.000000 yplib-2.3.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 00:56:42.000000 yplib-2.3.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.3.3/LICENSE` & `yplib-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.3.3/setup.py` & `yplib-2.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.3.3",
+  version="2.3.4",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.3.3/yplib/__init__.py` & `yplib-2.3.4/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.3/yplib/chart.py` & `yplib-2.3.4/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.3/yplib/chart_html.py` & `yplib-2.3.4/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.3/yplib/db.py` & `yplib-2.3.4/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.3/yplib/file.py` & `yplib-2.3.4/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.3/yplib/http_util.py` & `yplib-2.3.4/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.3/yplib/index.py` & `yplib-2.3.4/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,25 +206,29 @@
 def to_int(s):
     if isinstance(s, int):
         return s
     if s is None or s == '':
         return 0
     if isinstance(s, float):
         return int(s)
-    s = ''.join(filter(lambda ch: ch in '0123456789', str(s)))
+    s = re.sub(r'\D', "", str(s))
+    # s = ''.join(filter(lambda ch: ch in '0123456789', str(s)))
+    # @see https://www.runoob.com/python3/python3-reg-expressions.html
     return 0 if s == '' else int(s)
 
 
 # 去掉 str 中的 非数字字符, 然后, 再转化为 float
 def to_float(s):
     if isinstance(s, float):
         return s
     if s is None or s == '':
         return 0.0
-    s = ''.join(filter(lambda ch: ch in '0123456789.', str(s)))
+    # s = ''.join(filter(lambda ch: ch in '0123456789.', str(s)))
+    # @see https://www.runoob.com/python3/python3-reg-expressions.html
+    s = re.sub('[^0-9.]', '', str(s))
     return 0.0 if s == '' else float(s)
 
 
 # 将字符串 s 转化成 datetime
 def to_datetime(s=None, r_str=False):
     if s is None or s == '':
         return str(datetime.today()) if r_str else datetime.today()
@@ -338,14 +342,31 @@
     if can_use_json(data):
         s = json.dumps(data)
     else:
         s = str(data)
     return s
 
 
+# 匹配字符串
+# 可以参考 正则表达式的操作
+# pattern = r"CREATE TABLE (\w+)"
+# @see https://www.runoob.com/python3/python3-reg-expressions.html
+def match_str(pattern, str_a=''):
+    match = re.search(pattern, str_a, re.I)
+    if match:
+        return match.group(1)
+    else:
+        return None
+
+
+# # 示例用法
+# # 输出：t_admin
+# print(match_str(r'create TABLE (\w+)', 'CREATE TABLE t_admin (id bigint(20) NOT NULL'))
+
+
 # 根据json的key排序,用于签名
 # 按照 key 排序, 按照 key=value 然后再 & 连接, 如果数据中有 list, 使用 , 连接 list 中的数据, 然后拼接成 str 返回
 # sep       : 分隔符 , 默认 &
 # join      : 连接符 , 默认 =
 # join_list : list 数据 连接符 , 默认 ,
 def sort_by_json_key(data_obj, sep='&', join='=', join_list=','):
     if isinstance(data_obj, list) or isinstance(data_obj, tuple) or isinstance(data_obj, set):
```

### Comparing `yplib-2.3.3/yplib/mail.py` & `yplib-2.3.4/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.3/yplib/mail_html.py` & `yplib-2.3.4/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.3/yplib/markdown.py` & `yplib-2.3.4/yplib/markdown.py`

 * *Files identical despite different names*

