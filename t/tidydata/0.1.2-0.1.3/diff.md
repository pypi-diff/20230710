# Comparing `tmp/tidydata-0.1.2.tar.gz` & `tmp/tidydata-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidydata-0.1.2.tar", max compression
+gzip compressed data, was "tidydata-0.1.3.tar", max compression
```

## Comparing `tidydata-0.1.2.tar` & `tidydata-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      116 2023-06-21 13:25:39.956791 tidydata-0.1.2/README.md
--rw-r--r--   0        0        0      687 2023-07-09 14:28:14.510691 tidydata-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        2 2023-06-19 10:17:46.976922 tidydata-0.1.2/tidydata/__init__.py
--rw-r--r--   0        0        0       77 2023-06-19 10:17:46.976922 tidydata-0.1.2/tidydata/__main__.py
--rw-r--r--   0        0        0     1483 2023-06-30 09:11:54.490828 tidydata-0.1.2/tidydata/cli.py
--rw-r--r--   0        0        0    17287 2023-07-08 11:37:17.902116 tidydata-0.1.2/tidydata/config.py
--rw-r--r--   0        0        0    22749 2023-07-07 15:25:00.545473 tidydata-0.1.2/tidydata/core.py
--rw-r--r--   0        0        0     7218 2023-07-08 12:01:21.412965 tidydata-0.1.2/tidydata/variable.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 tidydata-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-21 13:25:39.956791 tidydata-0.1.3/README.md
+-rw-r--r--   0        0        0      687 2023-07-10 14:53:45.369564 tidydata-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        2 2023-06-19 10:17:46.976922 tidydata-0.1.3/tidydata/__init__.py
+-rw-r--r--   0        0        0       77 2023-06-19 10:17:46.976922 tidydata-0.1.3/tidydata/__main__.py
+-rw-r--r--   0        0        0     1483 2023-06-30 09:11:54.490828 tidydata-0.1.3/tidydata/cli.py
+-rw-r--r--   0        0        0    17287 2023-07-08 11:37:17.902116 tidydata-0.1.3/tidydata/config.py
+-rw-r--r--   0        0        0    22749 2023-07-07 15:25:00.545473 tidydata-0.1.3/tidydata/core.py
+-rw-r--r--   0        0        0     7288 2023-07-10 14:53:22.706110 tidydata-0.1.3/tidydata/variable.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 tidydata-0.1.3/PKG-INFO
```

### Comparing `tidydata-0.1.2/pyproject.toml` & `tidydata-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tidydata"
-version = "0.1.2"
+version = "0.1.3"
 description = "Data cleaner"
 authors = ["Kyrie He <kyrie1218@163.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
```

### Comparing `tidydata-0.1.2/tidydata/cli.py` & `tidydata-0.1.3/tidydata/cli.py`

 * *Files identical despite different names*

### Comparing `tidydata-0.1.2/tidydata/config.py` & `tidydata-0.1.3/tidydata/config.py`

 * *Files identical despite different names*

### Comparing `tidydata-0.1.2/tidydata/core.py` & `tidydata-0.1.3/tidydata/core.py`

 * *Files identical despite different names*

### Comparing `tidydata-0.1.2/tidydata/variable.py` & `tidydata-0.1.3/tidydata/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,12 +254,12 @@
 def reval(df: pd.DataFrame, exprs: List[str]):
     
     expr = '\n'.join(exprs)
     return df.eval(expr)
 
 
 
-def rassign(df: pd.DataFrame, exprs: Dict[str, Callable]):
-    
-    return df.assign(**exprs)
+def rassign(df: pd.DataFrame, exprs: Dict[str, str]):
+    lambda_exprs = {k: eval('lambda x: ' + v) for k, v in exprs.items()}
+    return df.assign(**lambda_exprs)
```

### Comparing `tidydata-0.1.2/PKG-INFO` & `tidydata-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidydata
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data cleaner
 Author: Kyrie He
 Author-email: kyrie1218@163.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
```

