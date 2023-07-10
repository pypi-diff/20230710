# Comparing `tmp/npdtools-1.0a1.tar.gz` & `tmp/npdtools-1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npdtools-1.0a1.tar", last modified: Sun Jul  9 13:50:10 2023, max compression
+gzip compressed data, was "npdtools-1.0a2.tar", last modified: Mon Jul 10 16:28:15 2023, max compression
```

## Comparing `npdtools-1.0a1.tar` & `npdtools-1.0a2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-09 13:50:10.045077 npdtools-1.0a1/
--rw-r--r--   0 white     (1000) wjite     (1001)    16725 2021-06-06 10:07:23.000000 npdtools-1.0a1/LICENSE
--rw-r--r--   0 white     (1000) wjite     (1001)    11342 2023-07-09 13:50:10.045077 npdtools-1.0a1/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)    10788 2023-07-09 13:45:12.000000 npdtools-1.0a1/README.md
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-09 13:50:10.041743 npdtools-1.0a1/npdtools/
--rw-r--r--   0 white     (1000) wjite     (1001)       51 2023-07-09 12:34:14.000000 npdtools-1.0a1/npdtools/__init__.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-09 13:50:10.045077 npdtools-1.0a1/npdtools/errors/
--rw-r--r--   0 white     (1000) wjite     (1001)      494 2023-07-09 12:34:14.000000 npdtools-1.0a1/npdtools/errors/FNSError.py
--rw-r--r--   0 white     (1000) wjite     (1001)       46 2021-05-15 04:12:30.000000 npdtools-1.0a1/npdtools/errors/__init__.py
--rw-r--r--   0 white     (1000) wjite     (1001)      149 2023-07-09 12:44:17.000000 npdtools-1.0a1/npdtools/helpers.py
--rw-r--r--   0 white     (1000) wjite     (1001)      114 2023-07-09 08:05:30.000000 npdtools-1.0a1/npdtools/settings.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3627 2023-07-09 08:49:31.000000 npdtools-1.0a1/npdtools/token_manager.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-09 13:50:10.045077 npdtools-1.0a1/npdtools/types/
--rw-r--r--   0 white     (1000) wjite     (1001)      392 2023-07-09 12:34:39.000000 npdtools-1.0a1/npdtools/types/__init__.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1738 2023-07-09 12:33:56.000000 npdtools-1.0a1/npdtools/types/entity.py
--rw-r--r--   0 white     (1000) wjite     (1001)     4622 2023-07-09 12:34:39.000000 npdtools-1.0a1/npdtools/types/income.py
--rw-r--r--   0 white     (1000) wjite     (1001)     5346 2023-07-09 13:29:22.000000 npdtools-1.0a1/npdtools/types/invoice.py
--rw-r--r--   0 white     (1000) wjite     (1001)      560 2023-07-09 12:44:58.000000 npdtools-1.0a1/npdtools/types/service.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-09 13:50:10.045077 npdtools-1.0a1/npdtools.egg-info/
--rw-r--r--   0 white     (1000) wjite     (1001)    11342 2023-07-09 13:50:10.000000 npdtools-1.0a1/npdtools.egg-info/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)      458 2023-07-09 13:50:10.000000 npdtools-1.0a1/npdtools.egg-info/SOURCES.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        1 2023-07-09 13:50:10.000000 npdtools-1.0a1/npdtools.egg-info/dependency_links.txt
--rw-r--r--   0 white     (1000) wjite     (1001)       45 2023-07-09 13:50:10.000000 npdtools-1.0a1/npdtools.egg-info/requires.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        9 2023-07-09 13:50:10.000000 npdtools-1.0a1/npdtools.egg-info/top_level.txt
--rw-r--r--   0 white     (1000) wjite     (1001)       38 2023-07-09 13:50:10.045077 npdtools-1.0a1/setup.cfg
--rw-r--r--   0 white     (1000) wjite     (1001)      917 2023-07-09 13:48:43.000000 npdtools-1.0a1/setup.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-10 16:28:15.988816 npdtools-1.0a2/
+-rw-r--r--   0 white     (1000) wjite     (1001)    16725 2021-06-06 10:07:23.000000 npdtools-1.0a2/LICENSE
+-rw-r--r--   0 white     (1000) wjite     (1001)    11342 2023-07-10 16:28:15.988816 npdtools-1.0a2/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)    10788 2023-07-09 13:45:12.000000 npdtools-1.0a2/README.md
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-10 16:28:15.988816 npdtools-1.0a2/npdtools/
+-rw-r--r--   0 white     (1000) wjite     (1001)       51 2023-07-09 12:34:14.000000 npdtools-1.0a2/npdtools/__init__.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-10 16:28:15.988816 npdtools-1.0a2/npdtools/errors/
+-rw-r--r--   0 white     (1000) wjite     (1001)      494 2023-07-09 12:34:14.000000 npdtools-1.0a2/npdtools/errors/FNSError.py
+-rw-r--r--   0 white     (1000) wjite     (1001)       46 2021-05-15 04:12:30.000000 npdtools-1.0a2/npdtools/errors/__init__.py
+-rw-r--r--   0 white     (1000) wjite     (1001)      149 2023-07-09 12:44:17.000000 npdtools-1.0a2/npdtools/helpers.py
+-rw-r--r--   0 white     (1000) wjite     (1001)      114 2023-07-09 08:05:30.000000 npdtools-1.0a2/npdtools/settings.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3627 2023-07-09 08:49:31.000000 npdtools-1.0a2/npdtools/token_manager.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-10 16:28:15.988816 npdtools-1.0a2/npdtools/types/
+-rw-r--r--   0 white     (1000) wjite     (1001)      384 2023-07-10 16:11:46.000000 npdtools-1.0a2/npdtools/types/__init__.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     4045 2023-07-10 15:34:44.000000 npdtools-1.0a2/npdtools/types/entity.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     8565 2023-07-10 16:11:46.000000 npdtools-1.0a2/npdtools/types/income.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     9576 2023-07-10 16:11:46.000000 npdtools-1.0a2/npdtools/types/invoice.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1209 2023-07-10 16:11:42.000000 npdtools-1.0a2/npdtools/types/service.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-10 16:28:15.988816 npdtools-1.0a2/npdtools.egg-info/
+-rw-r--r--   0 white     (1000) wjite     (1001)    11342 2023-07-10 16:28:15.000000 npdtools-1.0a2/npdtools.egg-info/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)      458 2023-07-10 16:28:15.000000 npdtools-1.0a2/npdtools.egg-info/SOURCES.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        1 2023-07-10 16:28:15.000000 npdtools-1.0a2/npdtools.egg-info/dependency_links.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)       45 2023-07-10 16:28:15.000000 npdtools-1.0a2/npdtools.egg-info/requires.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        9 2023-07-10 16:28:15.000000 npdtools-1.0a2/npdtools.egg-info/top_level.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)       38 2023-07-10 16:28:15.988816 npdtools-1.0a2/setup.cfg
+-rw-r--r--   0 white     (1000) wjite     (1001)      917 2023-07-10 16:12:55.000000 npdtools-1.0a2/setup.py
```

### Comparing `npdtools-1.0a1/LICENSE` & `npdtools-1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `npdtools-1.0a1/PKG-INFO` & `npdtools-1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npdtools
-Version: 1.0a1
+Version: 1.0a2
 Summary: tool for work with FNS API
 Home-page: https://gitlab.com/whiteapfel/npdtools
 Author: WhiteApfel
 Author-email: white@pfel.ru
 License: MPL 2.0
 Project-URL: Документация, https://npd-tools.readthedocs.io/en/latest/
 Project-URL: Исходники, https://gitlab.com/whiteapfel/npdtools/
```

### Comparing `npdtools-1.0a1/README.md` & `npdtools-1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `npdtools-1.0a1/npdtools/token_manager.py` & `npdtools-1.0a2/npdtools/token_manager.py`

 * *Files identical despite different names*

### Comparing `npdtools-1.0a1/npdtools.egg-info/PKG-INFO` & `npdtools-1.0a2/npdtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npdtools
-Version: 1.0a1
+Version: 1.0a2
 Summary: tool for work with FNS API
 Home-page: https://gitlab.com/whiteapfel/npdtools
 Author: WhiteApfel
 Author-email: white@pfel.ru
 License: MPL 2.0
 Project-URL: Документация, https://npd-tools.readthedocs.io/en/latest/
 Project-URL: Исходники, https://gitlab.com/whiteapfel/npdtools/
```

### Comparing `npdtools-1.0a1/setup.py` & `npdtools-1.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(filename):
     with open(filename, encoding="utf-8") as file:
         return file.read()
 
 
 setup(
     name="npdtools",
-    version="1.0a1",
+    version="1.0a2",
     packages=["npdtools", "npdtools.types"],
     url="https://gitlab.com/whiteapfel/npdtools",
     license="MPL 2.0",
     author="WhiteApfel",
     author_email="white@pfel.ru",
     description="tool for work with FNS API",
     install_requires=["typing", "httpx", "python-dateutil", "pydantic>=2.0.2"],
```

