# Comparing `tmp/finqual-0.1.96.tar.gz` & `tmp/finqual-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finqual-0.1.96.tar", last modified: Sun Jul  9 21:10:50 2023, max compression
+gzip compressed data, was "finqual-0.2.0.tar", last modified: Sun Jul  9 23:40:40 2023, max compression
```

## Comparing `finqual-0.1.96.tar` & `finqual-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 21:10:50.236621 finqual-0.1.96/
--rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-0.1.96/LICENSE.txt
--rw-rw-rw-   0        0        0     2491 2023-07-09 21:10:50.235621 finqual-0.1.96/PKG-INFO
--rw-rw-rw-   0        0        0     1968 2023-07-09 19:52:56.000000 finqual-0.1.96/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 21:10:50.225102 finqual-0.1.96/finqual/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-0.1.96/finqual/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 21:10:50.234619 finqual-0.1.96/finqual/data/
--rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-0.1.96/finqual/data/sec_sic.csv
--rw-rw-rw-   0        0        0   120333 2023-07-09 21:10:07.000000 finqual-0.1.96/finqual/finqual.py
-drwxrwxrwx   0        0        0        0 2023-07-09 21:10:50.234619 finqual-0.1.96/finqual.egg-info/
--rw-rw-rw-   0        0        0     2491 2023-07-09 21:10:50.000000 finqual-0.1.96/finqual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-09 21:10:50.000000 finqual-0.1.96/finqual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 21:10:50.000000 finqual-0.1.96/finqual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-09 21:10:50.000000 finqual-0.1.96/finqual.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 21:10:50.236621 finqual-0.1.96/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-07-09 21:10:12.000000 finqual-0.1.96/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:40:40.012618 finqual-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4966 2023-07-09 23:40:40.012618 finqual-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4444 2023-07-09 23:39:19.000000 finqual-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 23:40:39.992825 finqual-0.2.0/finqual/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-0.2.0/finqual/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:40:40.011617 finqual-0.2.0/finqual/data/
+-rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-0.2.0/finqual/data/sec_sic.csv
+-rw-rw-rw-   0        0        0   120333 2023-07-09 21:10:07.000000 finqual-0.2.0/finqual/finqual.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:40:39.992825 finqual-0.2.0/finqual.egg-info/
+-rw-rw-rw-   0        0        0     4966 2023-07-09 23:40:39.000000 finqual-0.2.0/finqual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-09 23:40:39.000000 finqual-0.2.0/finqual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 23:40:39.000000 finqual-0.2.0/finqual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-09 23:40:39.000000 finqual-0.2.0/finqual.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 23:40:40.012618 finqual-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      832 2023-07-09 23:34:31.000000 finqual-0.2.0/setup.py
```

### Comparing `finqual-0.1.96/LICENSE.txt` & `finqual-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finqual-0.1.96/finqual/data/sec_sic.csv` & `finqual-0.2.0/finqual/data/sec_sic.csv`

 * *Files identical despite different names*

### Comparing `finqual-0.1.96/finqual/finqual.py` & `finqual-0.2.0/finqual/finqual.py`

 * *Files identical despite different names*

### Comparing `finqual-0.1.96/setup.py` & `finqual-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 
 with open('README.md', 'r') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='finqual',
-    version='0.1.96',
+    version='0.2.0',
     description='A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.',
     author='Myztika',
     packages=['finqual'],
     package_dir = {'finqual':"finqual"},
     package_data={'finqual': ['data/*.csv']},
     long_description=long_description,
     long_description_content_type='text/markdown',
```

