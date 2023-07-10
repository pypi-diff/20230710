# Comparing `tmp/DefyDatabase-10.0.0a4.dev202307071900.tar.gz` & `tmp/DefyDatabase-10.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DefyDatabase-10.0.0a4.dev202307071900.tar", last modified: Fri Jul  7 10:55:25 2023, max compression
+gzip compressed data, was "DefyDatabase-10.0.0b1.tar", last modified: Mon Jul 10 04:14:25 2023, max compression
```

## Comparing `DefyDatabase-10.0.0a4.dev202307071900.tar` & `DefyDatabase-10.0.0b1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 10:55:25.921162 DefyDatabase-10.0.0a4.dev202307071900/
-drwxrwxrwx   0        0        0        0 2023-07-07 10:55:25.919170 DefyDatabase-10.0.0a4.dev202307071900/DefyDatabase.egg-info/
--rw-rw-rw-   0        0        0      567 2023-07-07 10:55:25.000000 DefyDatabase-10.0.0a4.dev202307071900/DefyDatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-07-07 10:55:25.000000 DefyDatabase-10.0.0a4.dev202307071900/DefyDatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 10:55:25.000000 DefyDatabase-10.0.0a4.dev202307071900/DefyDatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 10:55:25.000000 DefyDatabase-10.0.0a4.dev202307071900/DefyDatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      567 2023-07-07 10:55:25.919677 DefyDatabase-10.0.0a4.dev202307071900/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a4.dev202307071900/README.md
--rw-rw-rw-   0        0        0     2578 2023-07-07 10:54:48.000000 DefyDatabase-10.0.0a4.dev202307071900/defydb.py
--rw-rw-rw-   0        0        0       42 2023-07-07 10:55:25.921162 DefyDatabase-10.0.0a4.dev202307071900/setup.cfg
--rw-rw-rw-   0        0        0      985 2023-07-07 10:54:16.000000 DefyDatabase-10.0.0a4.dev202307071900/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 04:14:25.227723 DefyDatabase-10.0.0b1/
+drwxrwxrwx   0        0        0        0 2023-07-10 04:14:25.225634 DefyDatabase-10.0.0b1/DefyDatabase.egg-info/
+-rw-rw-rw-   0        0        0      550 2023-07-10 04:14:25.000000 DefyDatabase-10.0.0b1/DefyDatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-07-10 04:14:25.000000 DefyDatabase-10.0.0b1/DefyDatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 04:14:25.000000 DefyDatabase-10.0.0b1/DefyDatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 04:14:25.000000 DefyDatabase-10.0.0b1/DefyDatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      550 2023-07-10 04:14:25.227723 DefyDatabase-10.0.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0b1/README.md
+-rw-rw-rw-   0        0        0     5413 2023-07-10 04:00:19.000000 DefyDatabase-10.0.0b1/defydb.py
+-rw-rw-rw-   0        0        0       42 2023-07-10 04:14:25.227723 DefyDatabase-10.0.0b1/setup.cfg
+-rw-rw-rw-   0        0        0      664 2023-07-10 04:06:09.000000 DefyDatabase-10.0.0b1/setup.py
```

### Comparing `DefyDatabase-10.0.0a4.dev202307071900/DefyDatabase.egg-info/PKG-INFO` & `DefyDatabase-10.0.0b1/DefyDatabase.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: DefyDatabase
-Version: 10.0.0a4.dev202307071900
+Version: 10.0.0b1
 Summary: Database for personal data based on SQLite
 Author: Defymen
 Author-email: vmuonline@126.com
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `DefyDatabase-10.0.0a4.dev202307071900/PKG-INFO` & `DefyDatabase-10.0.0b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: DefyDatabase
-Version: 10.0.0a4.dev202307071900
+Version: 10.0.0b1
 Summary: Database for personal data based on SQLite
 Author: Defymen
 Author-email: vmuonline@126.com
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `DefyDatabase-10.0.0a4.dev202307071900/setup.py` & `DefyDatabase-10.0.0b1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,23 +9,14 @@
     author="Defymen",
     author_email="vmuonline@126.com",
     description="Database for personal data based on SQLite",
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=['defydb'],
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
 )
-six_classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Programming Language :: Python :: 2",
-    "Programming Language :: Python :: 3",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Topic :: Software Development :: Libraries",
-    "Topic :: Utilities",
-]
```

