# Comparing `tmp/dknovautils-0.1.8.tar.gz` & `tmp/dknovautils-0.1.9.tar.gz`

## Comparing `dknovautils-0.1.8.tar` & `dknovautils-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0      563 2020-02-02 00:00:00.000000 dknovautils-0.1.8/.gitignore
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 dknovautils-0.1.8/LICENSE
--rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 dknovautils-0.1.8/README.md
--rwxr-xr-x   0        0        0      578 2020-02-02 00:00:00.000000 dknovautils-0.1.8/pyproject.toml
--rwxr-xr-x   0        0        0     2059 2020-02-02 00:00:00.000000 dknovautils-0.1.8/test_a.py
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 dknovautils-0.1.8/test_b01.py
--rwxr-xr-x   0        0        0      145 2020-02-02 00:00:00.000000 dknovautils-0.1.8/test_c.py
--rwxr-xr-x   0        0        0     1184 2020-02-02 00:00:00.000000 dknovautils-0.1.8/upload.sh
--rwxr-xr-x   0        0        0      880 2020-02-02 00:00:00.000000 dknovautils-0.1.8/dknovautils.egg-info/PKG-INFO
--rwxr-xr-x   0        0        0      407 2020-02-02 00:00:00.000000 dknovautils-0.1.8/dknovautils.egg-info/SOURCES.txt
--rwxr-xr-x   0        0        0        1 2020-02-02 00:00:00.000000 dknovautils-0.1.8/dknovautils.egg-info/dependency_links.txt
--rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 dknovautils-0.1.8/dknovautils.egg-info/requires.txt
--rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 dknovautils-0.1.8/dknovautils.egg-info/top_level.txt
--rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/__init__.py
--rwxr-xr-x   0        0        0     2523 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/commons.py
--rwxr-xr-x   0        0        0      711 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/dk_imports.py
--rwxr-xr-x   0        0        0     8679 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/dkat.py
--rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/dkfiles.py
--rwxr-xr-x   0        0        0     1153 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/dkipy.py
--rwxr-xr-x   0        0        0      501 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/example.py
--rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/myadd.py
--rwxr-xr-x   0        0        0      160 2020-02-02 00:00:00.000000 dknovautils-0.1.8/src/dknovautils/mysubtract.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 dknovautils-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0     2059 2020-02-02 00:00:00.000000 dknovautils-0.1.9/test_a.py
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 dknovautils-0.1.9/test_b01.py
+-rwxr-xr-x   0        0        0      145 2020-02-02 00:00:00.000000 dknovautils-0.1.9/test_c.py
+-rwxr-xr-x   0        0        0     1202 2020-02-02 00:00:00.000000 dknovautils-0.1.9/upload.sh
+-rwxr-xr-x   0        0        0      880 2020-02-02 00:00:00.000000 dknovautils-0.1.9/dknovautils.egg-info/PKG-INFO
+-rwxr-xr-x   0        0        0      407 2020-02-02 00:00:00.000000 dknovautils-0.1.9/dknovautils.egg-info/SOURCES.txt
+-rwxr-xr-x   0        0        0        1 2020-02-02 00:00:00.000000 dknovautils-0.1.9/dknovautils.egg-info/dependency_links.txt
+-rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 dknovautils-0.1.9/dknovautils.egg-info/requires.txt
+-rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 dknovautils-0.1.9/dknovautils.egg-info/top_level.txt
+-rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 dknovautils-0.1.9/src/dknovautils/__init__.py
+-rwxr-xr-x   0        0        0     2523 2020-02-02 00:00:00.000000 dknovautils-0.1.9/src/dknovautils/commons.py
+-rwxr-xr-x   0        0        0      711 2020-02-02 00:00:00.000000 dknovautils-0.1.9/src/dknovautils/dk_imports.py
+-rwxr-xr-x   0        0        0     8679 2020-02-02 00:00:00.000000 dknovautils-0.1.9/src/dknovautils/dkat.py
+-rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 dknovautils-0.1.9/src/dknovautils/dkfiles.py
+-rwxr-xr-x   0        0        0     1153 2020-02-02 00:00:00.000000 dknovautils-0.1.9/src/dknovautils/dkipy.py
+-rwxr-xr-x   0        0        0      501 2020-02-02 00:00:00.000000 dknovautils-0.1.9/src/dknovautils/example.py
+-rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 dknovautils-0.1.9/src/dknovautils/myadd.py
+-rwxr-xr-x   0        0        0      160 2020-02-02 00:00:00.000000 dknovautils-0.1.9/src/dknovautils/mysubtract.py
+-rwxr-xr-x   0        0        0      563 2020-02-02 00:00:00.000000 dknovautils-0.1.9/.gitignore
+-rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 dknovautils-0.1.9/LICENSE
+-rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 dknovautils-0.1.9/README.md
+-rwxr-xr-x   0        0        0      578 2020-02-02 00:00:00.000000 dknovautils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 dknovautils-0.1.9/PKG-INFO
```

### Comparing `dknovautils-0.1.8/.gitignore` & `dknovautils-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.8/LICENSE` & `dknovautils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.8/pyproject.toml` & `dknovautils-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "dknovautils"
-version = '0.1.8'
+version = '0.1.9'
 authors = [
   { name="dknova", email="dikisite@outlook.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dknovautils-0.1.8/test_a.py` & `dknovautils-0.1.9/test_a.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.8/upload.sh` & `dknovautils-0.1.9/upload.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-AppVer="0.1.8"
+AppVer="0.1.9"
 
 # sed -i "s/^DkAppVer.*/DkAppVer = '$AppVer'/" ./setup.py
 
 sed -i "s/^DkAppVer.*/DkAppVer = '$AppVer'/" ./src/dknovautils/dk_imports.py
 sed -i "s/^DkAppVer.*/DkAppVer = '$AppVer'/" ./src/dknovautils/dkat.py
 
 sed -i "s/^version =.*/version = '$AppVer'/" ./pyproject.toml
@@ -20,14 +20,16 @@
 
 
 #        输入用户名 密码 即可完成上传。
 
 
 :<<EOF
 
+在wsl2中执行
+
 会自动修改 setup.py 中的版本号。运行脚本完成上传。 在wsl中运行。
 
 访问该网址进行注册：https://pypi.org/account/register/
 pip账号 dknova dikisite@outlook.com pwd:zh
 
 
 What is a Circular Import?
```

### Comparing `dknovautils-0.1.8/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.1.9/dknovautils.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.8/src/dknovautils/commons.py` & `dknovautils-0.1.9/src/dknovautils/commons.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.8/src/dknovautils/dk_imports.py` & `dknovautils-0.1.9/src/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.8/src/dknovautils/dkat.py` & `dknovautils-0.1.9/src/dknovautils/dkat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from typing import Any
 import dknovautils
 from dknovautils.commons import *
 
 
-DkAppVer = '0.1.8'
+DkAppVer = '0.1.9'
 
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
```

### Comparing `dknovautils-0.1.8/src/dknovautils/dkipy.py` & `dknovautils-0.1.9/src/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.8/PKG-INFO` & `dknovautils-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.1.8
+Version: 0.1.9
 Summary: A small example package
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: dknova <dikisite@outlook.com>
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Learning python
```

