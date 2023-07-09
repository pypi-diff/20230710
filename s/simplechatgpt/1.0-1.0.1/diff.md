# Comparing `tmp/simplechatgpt-1.0.tar.gz` & `tmp/simplechatgpt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplechatgpt-1.0.tar", max compression
+gzip compressed data, was "simplechatgpt-1.0.1.tar", max compression
```

## Comparing `simplechatgpt-1.0.tar` & `simplechatgpt-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-07-08 21:50:06.936780 simplechatgpt-1.0/LICENSE.txt
--rw-r--r--   0        0        0     1411 2023-07-08 21:49:49.437647 simplechatgpt-1.0/README.md
--rw-r--r--   0        0        0      358 2023-07-08 21:50:47.778614 simplechatgpt-1.0/pyproject.toml
--rw-r--r--   0        0        0       35 2023-07-08 20:55:04.933164 simplechatgpt-1.0/simplechatgpt/__init__.py
--rw-r--r--   0        0        0     1948 2023-07-08 21:50:58.612601 simplechatgpt-1.0/simplechatgpt/chat.py
--rw-r--r--   0        0        0     1882 1970-01-01 00:00:00.000000 simplechatgpt-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-08 21:50:06.936780 simplechatgpt-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1411 2023-07-08 21:49:49.437647 simplechatgpt-1.0.1/README.md
+-rw-r--r--   0        0        0      437 2023-07-09 22:32:48.150346 simplechatgpt-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-07-08 20:55:04.933164 simplechatgpt-1.0.1/simplechatgpt/__init__.py
+-rw-r--r--   0        0        0     1948 2023-07-08 21:50:58.612601 simplechatgpt-1.0.1/simplechatgpt/chat.py
+-rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 simplechatgpt-1.0.1/PKG-INFO
```

### Comparing `simplechatgpt-1.0/LICENSE.txt` & `simplechatgpt-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simplechatgpt-1.0/README.md` & `simplechatgpt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `simplechatgpt-1.0/simplechatgpt/chat.py` & `simplechatgpt-1.0.1/simplechatgpt/chat.py`

 * *Files identical despite different names*

### Comparing `simplechatgpt-1.0/PKG-INFO` & `simplechatgpt-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: simplechatgpt
-Version: 1.0
+Version: 1.0.1
 Summary: An extremely simple interface to ChatGPT
+Home-page: https://github.com/Thomas-McKanna/simplechatgpt
+License: MIT
 Author: Thomas McKanna
 Author-email: thomasmckanna@proton.me
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dependency (>=0.0.3,<0.0.4)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Description-Content-Type: text/markdown
```

