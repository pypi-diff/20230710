# Comparing `tmp/xcodeproj-1.1.0.tar.gz` & `tmp/xcodeproj-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcodeproj-1.1.0.tar", max compression
+gzip compressed data, was "xcodeproj-2.0.0.tar", max compression
```

## Comparing `xcodeproj-1.1.0.tar` & `xcodeproj-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1141 2023-03-22 05:31:26.588313 xcodeproj-1.1.0/LICENSE
--rw-r--r--   0        0        0     3638 2023-03-22 05:31:26.588614 xcodeproj-1.1.0/README.md
--rw-r--r--   0        0        0     1205 2023-04-24 05:12:35.593601 xcodeproj-1.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     9675 2023-04-24 02:42:41.641003 xcodeproj-1.1.0/xcodeproj/__init__.py
--rwxr-xr-x   0        0        0     3670 2023-03-22 05:31:26.599876 xcodeproj-1.1.0/xcodeproj/buildphases.py
--rwxr-xr-x   0        0        0      466 2023-03-22 05:31:26.600149 xcodeproj-1.1.0/xcodeproj/buildrules.py
--rwxr-xr-x   0        0        0     1082 2023-04-24 02:30:59.751221 xcodeproj-1.1.0/xcodeproj/files.py
--rwxr-xr-x   0        0        0     1470 2023-03-22 05:31:26.600583 xcodeproj-1.1.0/xcodeproj/other.py
--rwxr-xr-x   0        0        0     6908 2023-03-22 05:31:26.600841 xcodeproj-1.1.0/xcodeproj/pathobjects.py
--rwxr-xr-x   0        0        0     1783 2023-03-22 05:31:26.601078 xcodeproj-1.1.0/xcodeproj/pbxobject.py
--rwxr-xr-x   0        0        0     1888 2023-03-22 05:31:26.601477 xcodeproj-1.1.0/xcodeproj/pbxproject.py
--rwxr-xr-x   0        0        0    23926 2023-03-22 05:31:26.601951 xcodeproj-1.1.0/xcodeproj/schemes.py
--rwxr-xr-x   0        0        0     3602 2023-03-22 05:31:26.602239 xcodeproj-1.1.0/xcodeproj/targets.py
--rwxr-xr-x   0        0        0     2731 2023-03-22 08:37:07.901946 xcodeproj-1.1.0/xcodeproj/xcobjects.py
--rw-r--r--   0        0        0     4851 1970-01-01 00:00:00.000000 xcodeproj-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-07-10 08:35:44.634852 xcodeproj-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3638 2023-07-10 08:35:44.634852 xcodeproj-2.0.0/README.md
+-rw-r--r--   0        0        0     1205 2023-07-10 08:35:44.634852 xcodeproj-2.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0     9675 2023-07-10 08:35:44.638852 xcodeproj-2.0.0/xcodeproj/__init__.py
+-rwxr-xr-x   0        0        0     3670 2023-07-10 08:35:44.638852 xcodeproj-2.0.0/xcodeproj/buildphases.py
+-rwxr-xr-x   0        0        0      466 2023-07-10 08:35:44.638852 xcodeproj-2.0.0/xcodeproj/buildrules.py
+-rwxr-xr-x   0        0        0     1082 2023-07-10 08:35:44.638852 xcodeproj-2.0.0/xcodeproj/files.py
+-rwxr-xr-x   0        0        0     1470 2023-07-10 08:35:44.638852 xcodeproj-2.0.0/xcodeproj/other.py
+-rwxr-xr-x   0        0        0     6908 2023-07-10 08:35:44.638852 xcodeproj-2.0.0/xcodeproj/pathobjects.py
+-rwxr-xr-x   0        0        0     1783 2023-07-10 08:35:44.638852 xcodeproj-2.0.0/xcodeproj/pbxobject.py
+-rwxr-xr-x   0        0        0     1888 2023-07-10 08:35:44.638852 xcodeproj-2.0.0/xcodeproj/pbxproject.py
+-rwxr-xr-x   0        0        0    23926 2023-07-10 08:35:44.638852 xcodeproj-2.0.0/xcodeproj/schemes.py
+-rwxr-xr-x   0        0        0     3602 2023-07-10 08:35:44.638852 xcodeproj-2.0.0/xcodeproj/targets.py
+-rwxr-xr-x   0        0        0     2731 2023-07-10 08:35:44.638852 xcodeproj-2.0.0/xcodeproj/xcobjects.py
+-rw-r--r--   0        0        0     4601 1970-01-01 00:00:00.000000 xcodeproj-2.0.0/PKG-INFO
```

### Comparing `xcodeproj-1.1.0/LICENSE` & `xcodeproj-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.1.0/README.md` & `xcodeproj-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.1.0/pyproject.toml` & `xcodeproj-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcodeproj"
-version = "1.1.0"
+version = "2.0.0"
 description = "A utility for interacting with Xcode's xcodeproj bundle format."
 
 license = "MIT"
 
 authors = [
     "Dale Myers <dalemy@microsoft.com>"
 ]
@@ -35,15 +35,15 @@
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 mypy = "^1.2.0"
 pylint = "^2.17.2"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
-requests = "^2.28.2"
+requests = "^2.31.0"
 types-requests = "^2.28.11.17"
 
 [[tool.mypy.overrides]]
 module = [
     "deserialize"
 ]
 ignore_missing_imports = true
```

### Comparing `xcodeproj-1.1.0/xcodeproj/__init__.py` & `xcodeproj-2.0.0/xcodeproj/__init__.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.1.0/xcodeproj/buildphases.py` & `xcodeproj-2.0.0/xcodeproj/buildphases.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.1.0/xcodeproj/files.py` & `xcodeproj-2.0.0/xcodeproj/files.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.1.0/xcodeproj/other.py` & `xcodeproj-2.0.0/xcodeproj/other.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.1.0/xcodeproj/pathobjects.py` & `xcodeproj-2.0.0/xcodeproj/pathobjects.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.1.0/xcodeproj/pbxobject.py` & `xcodeproj-2.0.0/xcodeproj/pbxobject.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.1.0/xcodeproj/pbxproject.py` & `xcodeproj-2.0.0/xcodeproj/pbxproject.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.1.0/xcodeproj/schemes.py` & `xcodeproj-2.0.0/xcodeproj/schemes.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.1.0/xcodeproj/targets.py` & `xcodeproj-2.0.0/xcodeproj/targets.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.1.0/xcodeproj/xcobjects.py` & `xcodeproj-2.0.0/xcodeproj/xcobjects.py`

 * *Files identical despite different names*

### Comparing `xcodeproj-1.1.0/PKG-INFO` & `xcodeproj-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcodeproj
-Version: 1.1.0
+Version: 2.0.0
 Summary: A utility for interacting with Xcode's xcodeproj bundle format.
 Home-page: https://github.com/Microsoft/xcodeproj
 License: MIT
 Keywords: xcode,xcodeproj,pbxproj,apple
 Author: Dale Myers
 Author-email: dalemy@microsoft.com
 Requires-Python: >=3.8,<4.0
@@ -12,19 +12,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: deserialize (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/Microsoft/xcodeproj
 Description-Content-Type: text/markdown
```

