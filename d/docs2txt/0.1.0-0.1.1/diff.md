# Comparing `tmp/docs2txt-0.1.0.tar.gz` & `tmp/docs2txt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docs2txt-0.1.0.tar", last modified: Sun Jul  9 22:39:41 2023, max compression
+gzip compressed data, was "docs2txt-0.1.1.tar", last modified: Sun Jul  9 22:48:38 2023, max compression
```

## Comparing `docs2txt-0.1.0.tar` & `docs2txt-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:39:41.807333 docs2txt-0.1.0/
--rw-r--r--   0 er         (501) staff       (20)      155 2023-07-09 22:35:52.000000 docs2txt-0.1.0/AUTHORS.rst
--rw-r--r--   0 er         (501) staff       (20)     3543 2023-07-09 22:35:52.000000 docs2txt-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 er         (501) staff       (20)       89 2023-07-09 22:35:52.000000 docs2txt-0.1.0/HISTORY.rst
--rw-r--r--   0 er         (501) staff       (20)     1064 2023-07-09 22:35:54.000000 docs2txt-0.1.0/LICENSE
--rw-r--r--   0 er         (501) staff       (20)      262 2023-07-09 22:35:52.000000 docs2txt-0.1.0/MANIFEST.in
--rw-r--r--   0 er         (501) staff       (20)     1925 2023-07-09 22:39:41.807620 docs2txt-0.1.0/PKG-INFO
--rw-r--r--   0 er         (501) staff       (20)      934 2023-07-09 22:35:52.000000 docs2txt-0.1.0/README.rst
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:39:41.793825 docs2txt-0.1.0/docs/
--rw-r--r--   0 er         (501) staff       (20)      609 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs/Makefile
--rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs/authors.rst
--rwxr-xr-x   0 er         (501) staff       (20)     4811 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs/conf.py
--rw-r--r--   0 er         (501) staff       (20)       33 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs/contributing.rst
--rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs/history.rst
--rw-r--r--   0 er         (501) staff       (20)      310 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs/index.rst
--rw-r--r--   0 er         (501) staff       (20)     1133 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs/installation.rst
--rw-r--r--   0 er         (501) staff       (20)      770 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs/make.bat
--rw-r--r--   0 er         (501) staff       (20)       27 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs/readme.rst
--rw-r--r--   0 er         (501) staff       (20)       76 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs/usage.rst
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:39:41.796076 docs2txt-0.1.0/docs2txt/
--rw-r--r--   0 er         (501) staff       (20)      130 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs2txt/__init__.py
--rw-r--r--   0 er         (501) staff       (20)      879 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs2txt/cli.py
--rw-r--r--   0 er         (501) staff       (20)     3471 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs2txt/docs_rs.py
--rw-r--r--   0 er         (501) staff       (20)      415 2023-07-09 22:35:52.000000 docs2txt-0.1.0/docs2txt/utils.py
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:39:41.805033 docs2txt-0.1.0/docs2txt.egg-info/
--rw-r--r--   0 er         (501) staff       (20)     1925 2023-07-09 22:39:41.000000 docs2txt-0.1.0/docs2txt.egg-info/PKG-INFO
--rw-r--r--   0 er         (501) staff       (20)      596 2023-07-09 22:39:41.000000 docs2txt-0.1.0/docs2txt.egg-info/SOURCES.txt
--rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 22:39:41.000000 docs2txt-0.1.0/docs2txt.egg-info/dependency_links.txt
--rw-r--r--   0 er         (501) staff       (20)       47 2023-07-09 22:39:41.000000 docs2txt-0.1.0/docs2txt.egg-info/entry_points.txt
--rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 21:28:14.000000 docs2txt-0.1.0/docs2txt.egg-info/not-zip-safe
--rw-r--r--   0 er         (501) staff       (20)       11 2023-07-09 22:39:41.000000 docs2txt-0.1.0/docs2txt.egg-info/requires.txt
--rw-r--r--   0 er         (501) staff       (20)        9 2023-07-09 22:39:41.000000 docs2txt-0.1.0/docs2txt.egg-info/top_level.txt
--rw-r--r--   0 er         (501) staff       (20)      380 2023-07-09 22:39:41.808898 docs2txt-0.1.0/setup.cfg
--rw-r--r--   0 er         (501) staff       (20)     1571 2023-07-09 22:37:57.000000 docs2txt-0.1.0/setup.py
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:39:41.806419 docs2txt-0.1.0/tests/
--rw-r--r--   0 er         (501) staff       (20)       38 2023-07-09 22:35:52.000000 docs2txt-0.1.0/tests/__init__.py
--rw-r--r--   0 er         (501) staff       (20)      859 2023-07-09 22:35:52.000000 docs2txt-0.1.0/tests/test_docs2txt.py
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:48:38.646919 docs2txt-0.1.1/
+-rw-r--r--   0 er         (501) staff       (20)      155 2023-07-09 22:35:52.000000 docs2txt-0.1.1/AUTHORS.rst
+-rw-r--r--   0 er         (501) staff       (20)     3543 2023-07-09 22:35:52.000000 docs2txt-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 er         (501) staff       (20)       89 2023-07-09 22:35:52.000000 docs2txt-0.1.1/HISTORY.rst
+-rw-r--r--   0 er         (501) staff       (20)     1064 2023-07-09 22:35:54.000000 docs2txt-0.1.1/LICENSE
+-rw-r--r--   0 er         (501) staff       (20)      262 2023-07-09 22:35:52.000000 docs2txt-0.1.1/MANIFEST.in
+-rw-r--r--   0 er         (501) staff       (20)     1925 2023-07-09 22:48:38.647148 docs2txt-0.1.1/PKG-INFO
+-rw-r--r--   0 er         (501) staff       (20)      934 2023-07-09 22:35:52.000000 docs2txt-0.1.1/README.rst
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:48:38.627032 docs2txt-0.1.1/docs/
+-rw-r--r--   0 er         (501) staff       (20)      609 2023-07-09 22:35:52.000000 docs2txt-0.1.1/docs/Makefile
+-rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.1/docs/authors.rst
+-rwxr-xr-x   0 er         (501) staff       (20)     4791 2023-07-09 22:45:01.000000 docs2txt-0.1.1/docs/conf.py
+-rw-r--r--   0 er         (501) staff       (20)       33 2023-07-09 22:35:52.000000 docs2txt-0.1.1/docs/contributing.rst
+-rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.1/docs/history.rst
+-rw-r--r--   0 er         (501) staff       (20)      310 2023-07-09 22:35:52.000000 docs2txt-0.1.1/docs/index.rst
+-rw-r--r--   0 er         (501) staff       (20)     1133 2023-07-09 22:35:52.000000 docs2txt-0.1.1/docs/installation.rst
+-rw-r--r--   0 er         (501) staff       (20)      770 2023-07-09 22:35:52.000000 docs2txt-0.1.1/docs/make.bat
+-rw-r--r--   0 er         (501) staff       (20)       27 2023-07-09 22:35:52.000000 docs2txt-0.1.1/docs/readme.rst
+-rw-r--r--   0 er         (501) staff       (20)       76 2023-07-09 22:35:52.000000 docs2txt-0.1.1/docs/usage.rst
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:48:38.629596 docs2txt-0.1.1/docs2txt/
+-rw-r--r--   0 er         (501) staff       (20)      130 2023-07-09 22:44:01.000000 docs2txt-0.1.1/docs2txt/__init__.py
+-rw-r--r--   0 er         (501) staff       (20)      879 2023-07-09 22:35:52.000000 docs2txt-0.1.1/docs2txt/__main__.py
+-rw-r--r--   0 er         (501) staff       (20)     3471 2023-07-09 22:35:52.000000 docs2txt-0.1.1/docs2txt/docs_rs.py
+-rw-r--r--   0 er         (501) staff       (20)      415 2023-07-09 22:35:52.000000 docs2txt-0.1.1/docs2txt/utils.py
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:48:38.645097 docs2txt-0.1.1/docs2txt.egg-info/
+-rw-r--r--   0 er         (501) staff       (20)     1925 2023-07-09 22:48:38.000000 docs2txt-0.1.1/docs2txt.egg-info/PKG-INFO
+-rw-r--r--   0 er         (501) staff       (20)      601 2023-07-09 22:48:38.000000 docs2txt-0.1.1/docs2txt.egg-info/SOURCES.txt
+-rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 22:48:38.000000 docs2txt-0.1.1/docs2txt.egg-info/dependency_links.txt
+-rw-r--r--   0 er         (501) staff       (20)       47 2023-07-09 22:48:38.000000 docs2txt-0.1.1/docs2txt.egg-info/entry_points.txt
+-rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 21:28:14.000000 docs2txt-0.1.1/docs2txt.egg-info/not-zip-safe
+-rw-r--r--   0 er         (501) staff       (20)       11 2023-07-09 22:48:38.000000 docs2txt-0.1.1/docs2txt.egg-info/requires.txt
+-rw-r--r--   0 er         (501) staff       (20)        9 2023-07-09 22:48:38.000000 docs2txt-0.1.1/docs2txt.egg-info/top_level.txt
+-rw-r--r--   0 er         (501) staff       (20)      380 2023-07-09 22:48:38.648209 docs2txt-0.1.1/setup.cfg
+-rw-r--r--   0 er         (501) staff       (20)     2064 2023-07-09 22:47:49.000000 docs2txt-0.1.1/setup.py
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:48:38.646381 docs2txt-0.1.1/tests/
+-rw-r--r--   0 er         (501) staff       (20)       38 2023-07-09 22:35:52.000000 docs2txt-0.1.1/tests/__init__.py
+-rw-r--r--   0 er         (501) staff       (20)      859 2023-07-09 22:35:52.000000 docs2txt-0.1.1/tests/test_docs2txt.py
```

### Comparing `docs2txt-0.1.0/CONTRIBUTING.rst` & `docs2txt-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.0/LICENSE` & `docs2txt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.0/PKG-INFO` & `docs2txt-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs2txt
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple program to download documentation from docs.rs and convert it into a plaintext file.
 Home-page: https://github.com/ehutzle/docs2txt
 Author: Eric Richard
 Author-email: ehutzle@gmail.com
 License: MIT license
 Keywords: docs2txt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `docs2txt-0.1.0/README.rst` & `docs2txt-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.0/docs/Makefile` & `docs2txt-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.0/docs/conf.py` & `docs2txt-0.1.1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 # source_suffix = ['.rst', '.md']
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = 'rs-docs-2-txt'
+project = 'docs2txt'
 copyright = "2023, Eric Richard"
 author = "Eric Richard"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
@@ -124,38 +124,38 @@
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
     (master_doc, 'docs2txt.tex',
-     'rs-docs-2-txt Documentation',
+     'docs2txt Documentation',
      'Eric Richard', 'manual'),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
     (master_doc, 'docs2txt',
-     'rs-docs-2-txt Documentation',
+     'docs2txt Documentation',
      [author], 1)
 ]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (master_doc, 'docs2txt',
-     'rs-docs-2-txt Documentation',
+     'docs2txt Documentation',
      author,
      'docs2txt',
      'One line description of project.',
      'Miscellaneous'),
 ]
```

### Comparing `docs2txt-0.1.0/docs/installation.rst` & `docs2txt-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.0/docs/make.bat` & `docs2txt-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.0/docs2txt/cli.py` & `docs2txt-0.1.1/docs2txt/__main__.py`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.0/docs2txt/docs_rs.py` & `docs2txt-0.1.1/docs2txt/docs_rs.py`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.0/docs2txt.egg-info/PKG-INFO` & `docs2txt-0.1.1/docs2txt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs2txt
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple program to download documentation from docs.rs and convert it into a plaintext file.
 Home-page: https://github.com/ehutzle/docs2txt
 Author: Eric Richard
 Author-email: ehutzle@gmail.com
 License: MIT license
 Keywords: docs2txt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `docs2txt-0.1.0/docs2txt.egg-info/SOURCES.txt` & `docs2txt-0.1.1/docs2txt.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 docs2txt/__init__.py
-docs2txt/cli.py
+docs2txt/__main__.py
 docs2txt/docs_rs.py
 docs2txt/utils.py
 docs2txt.egg-info/PKG-INFO
 docs2txt.egg-info/SOURCES.txt
 docs2txt.egg-info/dependency_links.txt
 docs2txt.egg-info/entry_points.txt
 docs2txt.egg-info/not-zip-safe
```

### Comparing `docs2txt-0.1.0/setup.py` & `docs2txt-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,31 @@
 #!/usr/bin/env python
 
 """The setup script."""
+import codecs
+import os
 
 from setuptools import setup, find_packages
 
+
+def read(rel_path):
+    here = os.path.abspath(os.path.dirname(__file__))
+    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
+        return fp.read()
+
+
+def get_version(rel_path):
+    for line in read(rel_path).splitlines():
+        if line.startswith('__version__'):
+            delim = '"' if '"' in line else "'"
+            return line.split(delim)[1]
+    else:
+        raise RuntimeError("Unable to find version string.")
+
+
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = ['Click>=7.0', ]
@@ -43,10 +61,10 @@
     include_package_data=True,
     keywords='docs2txt',
     name='docs2txt',
     packages=find_packages(include=['docs2txt', 'docs2txt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ehutzle/docs2txt',
-    version='0.1.0',
+    version=get_version("docs2txt/__init__.py"),
     zip_safe=False,
 )
```

### Comparing `docs2txt-0.1.0/tests/test_docs2txt.py` & `docs2txt-0.1.1/tests/test_docs2txt.py`

 * *Files identical despite different names*

