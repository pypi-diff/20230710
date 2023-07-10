# Comparing `tmp/rxctl-1.0.2.tar.gz` & `tmp/rxctl-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxctl-1.0.2.tar", max compression
+gzip compressed data, was "rxctl-1.0.3.tar", max compression
```

## Comparing `rxctl-1.0.2.tar` & `rxctl-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-06-11 13:17:52.848024 rxctl-1.0.2/LICENSE
--rw-r--r--   0        0        0     4795 2023-06-11 13:17:52.848024 rxctl-1.0.2/README.md
--rw-r--r--   0        0        0      590 2023-06-11 13:18:09.328276 rxctl-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-11 13:17:52.852024 rxctl-1.0.2/rxctl/__init__.py
--rw-r--r--   0        0        0       38 2023-06-11 13:18:09.328276 rxctl-1.0.2/rxctl/__version__.py
--rw-r--r--   0        0        0      262 2023-06-11 13:17:52.852024 rxctl-1.0.2/rxctl/bin/__init
--rwxr-xr-x   0        0        0      356 2023-06-11 13:17:52.852024 rxctl-1.0.2/rxctl/bin/__run
--rwxr-xr-x   0        0        0      626 2023-06-11 13:17:52.852024 rxctl-1.0.2/rxctl/bin/__wait
--rwxr-xr-x   0        0        0     3986 2023-06-11 13:17:52.852024 rxctl-1.0.2/rxctl/lib/ansible.sh
--rw-r--r--   0        0        0      428 2023-06-11 13:17:52.852024 rxctl-1.0.2/rxctl/lib/links.json
--rw-r--r--   0        0        0      703 2023-06-11 13:17:52.852024 rxctl-1.0.2/rxctl/lib/links.py
--rwxr-xr-x   0        0        0     3096 2023-06-11 13:17:52.852024 rxctl-1.0.2/rxctl/lib/log.py
--rw-r--r--   0        0        0    14879 2023-06-11 13:17:52.852024 rxctl-1.0.2/rxctl/lib/main.py
--rwxr-xr-x   0        0        0      439 2023-06-11 13:17:52.852024 rxctl-1.0.2/rxctl/lib/scp.sh
--rw-r--r--   0        0        0     2188 2023-06-11 13:17:52.852024 rxctl-1.0.2/rxctl/lib/utils.py
--rw-r--r--   0        0        0     5394 1970-01-01 00:00:00.000000 rxctl-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-10 10:40:17.345458 rxctl-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4795 2023-07-10 10:40:17.345458 rxctl-1.0.3/README.md
+-rw-r--r--   0        0        0      590 2023-07-10 10:40:38.825834 rxctl-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 10:40:17.349458 rxctl-1.0.3/rxctl/__init__.py
+-rw-r--r--   0        0        0       38 2023-07-10 10:40:38.829834 rxctl-1.0.3/rxctl/__version__.py
+-rw-r--r--   0        0        0      262 2023-07-10 10:40:17.349458 rxctl-1.0.3/rxctl/bin/__init
+-rwxr-xr-x   0        0        0      356 2023-07-10 10:40:17.349458 rxctl-1.0.3/rxctl/bin/__run
+-rwxr-xr-x   0        0        0      626 2023-07-10 10:40:17.349458 rxctl-1.0.3/rxctl/bin/__wait
+-rwxr-xr-x   0        0        0     3986 2023-07-10 10:40:17.349458 rxctl-1.0.3/rxctl/lib/ansible.sh
+-rw-r--r--   0        0        0      428 2023-07-10 10:40:17.349458 rxctl-1.0.3/rxctl/lib/links.json
+-rw-r--r--   0        0        0      703 2023-07-10 10:40:17.349458 rxctl-1.0.3/rxctl/lib/links.py
+-rwxr-xr-x   0        0        0     3096 2023-07-10 10:40:17.349458 rxctl-1.0.3/rxctl/lib/log.py
+-rw-r--r--   0        0        0    14879 2023-07-10 10:40:17.349458 rxctl-1.0.3/rxctl/lib/main.py
+-rwxr-xr-x   0        0        0      439 2023-07-10 10:40:17.349458 rxctl-1.0.3/rxctl/lib/scp.sh
+-rw-r--r--   0        0        0     2188 2023-07-10 10:40:17.349458 rxctl-1.0.3/rxctl/lib/utils.py
+-rw-r--r--   0        0        0     5394 1970-01-01 00:00:00.000000 rxctl-1.0.3/PKG-INFO
```

### Comparing `rxctl-1.0.2/LICENSE` & `rxctl-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rxctl-1.0.2/README.md` & `rxctl-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rxctl-1.0.2/pyproject.toml` & `rxctl-1.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rxctl"
-version = "1.0.2"
+version = "1.0.3"
 description = "Linux remote execution tool"
 authors = ["mihaiush <mihaiush@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/mihaiush/rxctl"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `rxctl-1.0.2/rxctl/bin/__wait` & `rxctl-1.0.3/rxctl/bin/__wait`

 * *Files identical despite different names*

### Comparing `rxctl-1.0.2/rxctl/lib/ansible.sh` & `rxctl-1.0.3/rxctl/lib/ansible.sh`

 * *Files identical despite different names*

### Comparing `rxctl-1.0.2/rxctl/lib/links.py` & `rxctl-1.0.3/rxctl/lib/links.py`

 * *Files identical despite different names*

### Comparing `rxctl-1.0.2/rxctl/lib/log.py` & `rxctl-1.0.3/rxctl/lib/log.py`

 * *Files identical despite different names*

### Comparing `rxctl-1.0.2/rxctl/lib/main.py` & `rxctl-1.0.3/rxctl/lib/main.py`

 * *Files identical despite different names*

### Comparing `rxctl-1.0.2/rxctl/lib/utils.py` & `rxctl-1.0.3/rxctl/lib/utils.py`

 * *Files identical despite different names*

### Comparing `rxctl-1.0.2/PKG-INFO` & `rxctl-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxctl
-Version: 1.0.2
+Version: 1.0.3
 Summary: Linux remote execution tool
 Home-page: https://github.com/mihaiush/rxctl
 Author: mihaiush
 Author-email: mihaiush@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

