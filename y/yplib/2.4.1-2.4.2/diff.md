# Comparing `tmp/yplib-2.4.1.tar.gz` & `tmp/yplib-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.4.1.tar", last modified: Mon Jul 10 08:24:06 2023, max compression
+gzip compressed data, was "dist\yplib-2.4.2.tar", last modified: Mon Jul 10 08:52:52 2023, max compression
```

## Comparing `yplib-2.4.1.tar` & `yplib-2.4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 08:24:05.998504 yplib-2.4.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.1/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-10 08:24:05.998029 yplib-2.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 08:24:05.998620 yplib-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-10 08:23:38.000000 yplib-2.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:24:05.995185 yplib-2.4.1/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.1/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.1/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.1/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.1/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.4.1/yplib/http_util.py
--rw-rw-rw-   0        0        0    32402 2023-07-10 08:23:31.000000 yplib-2.4.1/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.1/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.1/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.1/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.1/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:24:05.997060 yplib-2.4.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-10 08:24:05.000000 yplib-2.4.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-10 08:24:05.000000 yplib-2.4.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 08:24:05.000000 yplib-2.4.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 08:24:05.000000 yplib-2.4.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 08:52:52.302780 yplib-2.4.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.2/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-10 08:52:52.302220 yplib-2.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 08:52:52.302780 yplib-2.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-10 08:52:42.000000 yplib-2.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:52:52.298720 yplib-2.4.2/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.2/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.2/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.2/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.4.2/yplib/http_util.py
+-rw-rw-rw-   0        0        0    32901 2023-07-10 08:52:07.000000 yplib-2.4.2/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.2/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.2/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.2/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.2/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:52:52.301163 yplib-2.4.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-10 08:52:52.000000 yplib-2.4.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-10 08:52:52.000000 yplib-2.4.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 08:52:52.000000 yplib-2.4.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 08:52:52.000000 yplib-2.4.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.4.1/LICENSE` & `yplib-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.4.1/setup.py` & `yplib-2.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.4.1",
+  version="2.4.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.4.1/yplib/__init__.py` & `yplib-2.4.2/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.1/yplib/chart.py` & `yplib-2.4.2/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.1/yplib/chart_html.py` & `yplib-2.4.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.1/yplib/db.py` & `yplib-2.4.2/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.1/yplib/file.py` & `yplib-2.4.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.1/yplib/http_util.py` & `yplib-2.4.2/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.1/yplib/index.py` & `yplib-2.4.2/yplib/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,65 +76,97 @@
     lo = to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20, time_prefix=time_prefix)
     to_txt([lo], file_name, 'log', True, '.txt')
 
 
 # 将下划线命名转成驼峰命名
 # 例如 : user_id -> userId
 # 例如 : USER_ID -> userId
-def to_hump(s=''):
-    if s == '' or s is None:
+def to_hump_one(s):
+    if s is None or s == '':
         return s
-    s = s.lower()
+    s = str(s).lower()
     s1 = s.split('_')
     r = ""
     for w in s1:
         r += w.capitalize()
     return r[0].lower() + r[1:]
 
 
-def to_hump_more(a1='', a2='', a3='', a4='', a5=''):
-    if a1 == '':
-        return a1
-    elif a2 == '':
-        return to_hump(a1)
-    elif a3 == '':
-        return to_hump(a1), to_hump(a2)
-    elif a4 == '':
-        return to_hump(a1), to_hump(a2), to_hump(a3)
-    elif a5 == '':
-        return to_hump(a1), to_hump(a2), to_hump(a3), to_hump(a4)
-    return to_hump(a1), to_hump(a2), to_hump(a3), to_hump(a4), to_hump(a5)
+def to_hump(s):
+    if s is None or s == '':
+        return s
+    if isinstance(s, list) or isinstance(s, tuple) or isinstance(s, set):
+        rr = []
+        for ss in s:
+            rr.append(to_hump_one(ss))
+        return rr
+    return to_hump_one(s)
+
+
+def to_hump_more(a1, a2, a3, a4, a5):
+    l = [a1, a2, a3, a4, a5]
+    r = []
+    for a in l:
+        r.append(to_hump(a))
+    if not len(r):
+        return None
+    if len(r) == 1:
+        return r[0]
+    if len(r) == 2:
+        return r[0], r[1]
+    if len(r) == 3:
+        return r[0], r[1], r[2]
+    if len(r) == 4:
+        return r[0], r[1], r[2], r[3]
+    if len(r) == 5:
+        return r[0], r[1], r[2], r[3], r[4]
 
 
 # 将驼峰命名转成下划线命名
 # 例如 : userId -> user_id
-def to_underline(s=''):
+def to_underline_one(s):
     if s == '' or s is None:
         return s
     r = ''
-    for c in s:
+    for c in str(s):
         if c.isupper():
             r += '_' + c.lower()
         else:
             r += c
     return r
 
 
-def to_underline_more(a1='', a2='', a3='', a4='', a5=''):
-    if a1 == '':
-        return a1
-    elif a2 == '':
-        return to_underline(a1)
-    elif a3 == '':
-        return to_underline(a1), to_underline(a2)
-    elif a4 == '':
-        return to_underline(a1), to_underline(a2), to_underline(a3)
-    elif a5 == '':
-        return to_underline(a1), to_underline(a2), to_underline(a3), to_underline(a4)
-    return to_underline(a1), to_underline(a2), to_underline(a3), to_underline(a4), to_underline(a5)
+def to_underline(s):
+    if s == '' or s is None:
+        return s
+    if isinstance(s, list) or isinstance(s, tuple) or isinstance(s, set):
+        rr = []
+        for ss in s:
+            rr.append(to_underline_one(ss))
+        return rr
+    return to_underline_one(s)
+
+
+def to_underline_more(a1, a2, a3, a4, a5):
+    l = [a1, a2, a3, a4, a5]
+    r = []
+    for a in l:
+        r.append(to_underline(a))
+    if not len(r):
+        return None
+    if len(r) == 1:
+        return r[0]
+    if len(r) == 2:
+        return r[0], r[1]
+    if len(r) == 3:
+        return r[0], r[1], r[2]
+    if len(r) == 4:
+        return r[0], r[1], r[2], r[3]
+    if len(r) == 5:
+        return r[0], r[1], r[2], r[3], r[4]
 
 
 # 是否能用 json
 def can_use_json(data):
     if isinstance(data, dict) or isinstance(data, list) or isinstance(data, tuple) or isinstance(data, set):
         return True
     return False
```

### Comparing `yplib-2.4.1/yplib/mail.py` & `yplib-2.4.2/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.1/yplib/mail_html.py` & `yplib-2.4.2/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.1/yplib/markdown.py` & `yplib-2.4.2/yplib/markdown.py`

 * *Files identical despite different names*

