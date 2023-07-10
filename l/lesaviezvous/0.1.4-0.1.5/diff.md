# Comparing `tmp/lesaviezvous-0.1.4.tar.gz` & `tmp/lesaviezvous-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lesaviezvous-0.1.4.tar", last modified: Mon Jul 10 17:00:45 2023, max compression
+gzip compressed data, was "lesaviezvous-0.1.5.tar", last modified: Mon Jul 10 17:27:33 2023, max compression
```

## Comparing `lesaviezvous-0.1.4.tar` & `lesaviezvous-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:00:45.300675 lesaviezvous-0.1.4/
--rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.1.4/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     2997 2023-07-10 17:00:45.300675 lesaviezvous-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1103 2023-07-10 16:59:17.000000 lesaviezvous-0.1.4/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:00:45.300675 lesaviezvous-0.1.4/lesaviezvous/
--rw-r--r--   0 runner    (1000) runner    (1000)      214 2023-07-10 06:39:24.000000 lesaviezvous-0.1.4/lesaviezvous/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      243 2023-07-10 16:45:22.000000 lesaviezvous-0.1.4/lesaviezvous/lesaviezvous.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:00:45.300675 lesaviezvous-0.1.4/lesaviezvous.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2997 2023-07-10 17:00:44.000000 lesaviezvous-0.1.4/lesaviezvous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      274 2023-07-10 17:00:44.000000 lesaviezvous-0.1.4/lesaviezvous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 17:00:44.000000 lesaviezvous-0.1.4/lesaviezvous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-10 17:00:44.000000 lesaviezvous-0.1.4/lesaviezvous.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 17:00:44.000000 lesaviezvous-0.1.4/lesaviezvous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      499 2023-07-10 16:44:12.000000 lesaviezvous-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 17:00:45.300675 lesaviezvous-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      777 2023-07-10 17:00:04.000000 lesaviezvous-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:27:33.845835 lesaviezvous-0.1.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1339 2023-07-10 17:27:33.845835 lesaviezvous-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      501 2023-07-10 17:27:03.000000 lesaviezvous-0.1.5/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:27:33.841835 lesaviezvous-0.1.5/lesaviezvous/
+-rw-r--r--   0 runner    (1000) runner    (1000)      214 2023-07-10 06:39:24.000000 lesaviezvous-0.1.5/lesaviezvous/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    79468 2023-07-10 17:20:29.000000 lesaviezvous-0.1.5/lesaviezvous/dp.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       96 2023-07-10 17:25:18.000000 lesaviezvous-0.1.5/lesaviezvous/lesaviezvous.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:27:33.845835 lesaviezvous-0.1.5/lesaviezvous.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1339 2023-07-10 17:27:33.000000 lesaviezvous-0.1.5/lesaviezvous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      258 2023-07-10 17:27:33.000000 lesaviezvous-0.1.5/lesaviezvous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 17:27:33.000000 lesaviezvous-0.1.5/lesaviezvous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 17:27:33.000000 lesaviezvous-0.1.5/lesaviezvous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      499 2023-07-10 16:44:12.000000 lesaviezvous-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 17:27:33.845835 lesaviezvous-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      769 2023-07-10 17:23:32.000000 lesaviezvous-0.1.5/setup.py
```

### Comparing `lesaviezvous-0.1.4/LICENSE` & `lesaviezvous-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.1.4/setup.py` & `lesaviezvous-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from setuptools import setup, find_packages
 from readme_renderer.markdown import render
 
 long_description = ""
 with open('README.md', encoding='utf-8') as file:
-  long_description = file.read()
+    long_description = file.read()
 
 setup(
-  name = "lesaviezvous",
-  version = "0.1.4",
-  author="Coding Team",
-  author_email="codingteam@telegmail.com",
-  license='MIT',
-  description='Un package Python pour obtenir des informations intéressantes du monde.',
-  long_description=render(long_description),
-  long_description_content_type="text/markdown",
-  url="https://github.com/codingtuto/lesaviezvouspkg/",
-  packages=find_packages(exclude=["testing"]),
-  install_requires=[
-    'requests'
-  ],
-  python_requires='>=3.7',
-  classifiers=[
-    "Programming Language :: Python :: 3",
-    "Topic :: Utilities"
-  ],
-)
+    name="lesaviezvous",
+    version="0.1.5",
+    author="Coding Team",
+    author_email="codingteam@telegmail.com",
+    license='MIT',
+    description='Un package Python pour obtenir des informations intéressantes du monde.',
+    long_description=render(long_description),
+    long_description_content_type="text/markdown",
+    url="https://github.com/codingtuto/lesaviezvouspkg/",
+    packages=find_packages(exclude=["testing"]),
+    python_requires='>=3.7',
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Topic :: Utilities"
+    ],
+)
```

