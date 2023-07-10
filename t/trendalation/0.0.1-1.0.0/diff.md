# Comparing `tmp/trendalation-0.0.1.tar.gz` & `tmp/trendalation-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trendalation-0.0.1.tar", last modified: Fri Jul  7 00:48:56 2023, max compression
+gzip compressed data, was "trendalation-1.0.0.tar", last modified: Mon Jul 10 01:47:35 2023, max compression
```

## Comparing `trendalation-0.0.1.tar` & `trendalation-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-07 00:48:56.698835 trendalation-0.0.1/
--rw-r--r--   0 raghavsaboo   (501) staff       (20)     1084 2023-07-07 00:41:12.000000 trendalation-0.0.1/LICENSE.rst
--rw-r--r--   0 raghavsaboo   (501) staff       (20)        0 2023-07-02 18:27:10.000000 trendalation-0.0.1/MANIFEST.in
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      542 2023-07-07 00:48:56.698898 trendalation-0.0.1/PKG-INFO
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      685 2023-07-07 00:38:17.000000 trendalation-0.0.1/README.md
--rw-r--r--   0 raghavsaboo   (501) staff       (20)        0 2023-07-02 18:27:10.000000 trendalation-0.0.1/pyproject.toml
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      107 2023-07-07 00:48:56.699201 trendalation-0.0.1/setup.cfg
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      707 2023-07-07 00:48:01.000000 trendalation-0.0.1/setup.py
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-07 00:48:56.697010 trendalation-0.0.1/src/
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-07 00:48:56.698680 trendalation-0.0.1/src/trendalation.egg-info/
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      542 2023-07-07 00:48:56.000000 trendalation-0.0.1/src/trendalation.egg-info/PKG-INFO
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      266 2023-07-07 00:48:56.000000 trendalation-0.0.1/src/trendalation.egg-info/SOURCES.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-07 00:48:56.000000 trendalation-0.0.1/src/trendalation.egg-info/dependency_links.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)       25 2023-07-07 00:48:56.000000 trendalation-0.0.1/src/trendalation.egg-info/requires.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-07 00:48:56.000000 trendalation-0.0.1/src/trendalation.egg-info/top_level.txt
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-10 01:47:35.677561 trendalation-1.0.0/
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)     1084 2023-07-08 16:44:54.000000 trendalation-1.0.0/LICENSE.rst
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      556 2023-07-10 01:47:35.677626 trendalation-1.0.0/PKG-INFO
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      872 2023-07-08 16:44:54.000000 trendalation-1.0.0/README.md
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)       93 2023-07-08 17:30:19.000000 trendalation-1.0.0/pyproject.toml
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      107 2023-07-10 01:47:35.677850 trendalation-1.0.0/setup.cfg
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      787 2023-07-10 01:47:24.000000 trendalation-1.0.0/setup.py
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-10 01:47:35.675118 trendalation-1.0.0/src/
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-10 01:47:35.676574 trendalation-1.0.0/src/trendalation/
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      118 2023-07-10 01:46:20.000000 trendalation-1.0.0/src/trendalation/__init__.py
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)     5885 2023-07-10 01:30:01.000000 trendalation-1.0.0/src/trendalation/classification.py
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)     1479 2023-07-10 01:30:01.000000 trendalation-1.0.0/src/trendalation/metrics.py
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)       22 2023-07-10 01:37:36.000000 trendalation-1.0.0/src/trendalation/version.py
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-10 01:47:35.677410 trendalation-1.0.0/src/trendalation.egg-info/
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      556 2023-07-10 01:47:35.000000 trendalation-1.0.0/src/trendalation.egg-info/PKG-INFO
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      374 2023-07-10 01:47:35.000000 trendalation-1.0.0/src/trendalation.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-10 01:47:35.000000 trendalation-1.0.0/src/trendalation.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)       25 2023-07-10 01:47:35.000000 trendalation-1.0.0/src/trendalation.egg-info/requires.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)       13 2023-07-10 01:47:35.000000 trendalation-1.0.0/src/trendalation.egg-info/top_level.txt
```

### Comparing `trendalation-0.0.1/LICENSE.rst` & `trendalation-1.0.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `trendalation-0.0.1/PKG-INFO` & `trendalation-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 Metadata-Version: 2.1
 Name: trendalation
-Version: 0.0.1
-Summary: UNKNOWN
+Version: 1.0.0
 Home-page: https://github.com/kartikeysinha/trendalation
-Author: Raghav Saboo, Kartikey Sinha
+Author: ['Raghav Saboo', 'Kartikey Sinha']
 Author-email: raghs2000@gmail.com
 License: MIT
-Keywords: anomaly detection
-Platform: UNKNOWN
+Keywords: anomaly detection,procrustes,time-series,trends
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
 License-File: LICENSE.rst
-
-UNKNOWN
-
```

### Comparing `trendalation-0.0.1/README.md` & `trendalation-1.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 SciPy (>= 1.11.1)
 
 ### Using pip
 
 The easiest way to install trendalation is using pip:
 `pip install trendalation`
 
-### Build from source
-
 ## Documentation
 
 ## Help and Support
 
-## Citation
+In order to report bugfixes and new feature requests, simply create a new issue on the repository.
+The issues will be reviewed by the authors on a regular basis & you're welcome to work on any open issues.
+
+## Contribution
 
-If you use scikit-learn in a scientific publication, we would appreciate citations:
-```insert link for citation instructions```
+This project is a community effort, and everyone is welcome to contribute.
+Feel free to work on any open issues and setup PRs.
```

### Comparing `trendalation-0.0.1/setup.py` & `trendalation-1.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='trendalation',
-    version='0.0.1',
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
+    python_requires=">=3.8",
+    version='1.0.0',
     license='MIT',
-    author="Raghav Saboo, Kartikey Sinha",
+    author=['Raghav Saboo', 'Kartikey Sinha'],
     author_email='raghs2000@gmail.com',
-    packages=find_packages('src'),
-    package_dir={'': 'src'},
     url='https://github.com/kartikeysinha/trendalation',
-    keywords='anomaly detection',
+    keywords=['anomaly detection', 'procrustes', 'time-series', 'trends'],
     install_requires=[
         'numpy',
         'scikit-learn',
         'scipy'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `trendalation-0.0.1/src/trendalation.egg-info/PKG-INFO` & `trendalation-1.0.0/src/trendalation.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 Metadata-Version: 2.1
 Name: trendalation
-Version: 0.0.1
-Summary: UNKNOWN
+Version: 1.0.0
 Home-page: https://github.com/kartikeysinha/trendalation
-Author: Raghav Saboo, Kartikey Sinha
+Author: ['Raghav Saboo', 'Kartikey Sinha']
 Author-email: raghs2000@gmail.com
 License: MIT
-Keywords: anomaly detection
-Platform: UNKNOWN
+Keywords: anomaly detection,procrustes,time-series,trends
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
 License-File: LICENSE.rst
-
-UNKNOWN
-
```

