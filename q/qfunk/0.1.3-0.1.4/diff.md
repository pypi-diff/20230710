# Comparing `tmp/qfunk-0.1.3.tar.gz` & `tmp/qfunk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfunk-0.1.3.tar", last modified: Fri Jul  7 13:31:18 2023, max compression
+gzip compressed data, was "qfunk-0.1.4.tar", last modified: Mon Jul 10 13:06:13 2023, max compression
```

## Comparing `qfunk-0.1.3.tar` & `qfunk-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-07 13:31:18.585781 qfunk-0.1.3/
--rwxrwxrwx   0 joshua    (1000) joshua    (1000)     1086 2021-09-12 18:34:10.000000 qfunk-0.1.3/LICENSE.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      556 2023-07-07 13:31:18.585781 qfunk-0.1.3/PKG-INFO
--rwxrwxrwx   0 joshua    (1000) joshua    (1000)     5267 2021-10-12 10:57:54.000000 qfunk-0.1.3/README.md
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-07 13:31:18.585781 qfunk-0.1.3/qfunk/
--rwxrwxrwx   0 joshua    (1000) joshua    (1000)        0 2020-12-21 12:08:47.000000 qfunk-0.1.3/qfunk/__init__.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    14942 2022-09-19 12:31:27.000000 qfunk-0.1.3/qfunk/decompose.py
--rwxrwxrwx   0 joshua    (1000) joshua    (1000)     6401 2023-07-06 14:45:16.000000 qfunk-0.1.3/qfunk/generator.py
--rwxrwxrwx   0 joshua    (1000) joshua    (1000)    27590 2022-01-14 22:51:51.000000 qfunk-0.1.3/qfunk/opensys.py
--rwxrwxrwx   0 joshua    (1000) joshua    (1000)    16393 2023-07-07 13:08:44.000000 qfunk-0.1.3/qfunk/qoptic.py
--rwxrwxrwx   0 joshua    (1000) joshua    (1000)     2291 2022-01-21 18:56:08.000000 qfunk-0.1.3/qfunk/testbench.py
--rwxrwxrwx   0 joshua    (1000) joshua    (1000)    10134 2022-11-07 10:07:09.000000 qfunk-0.1.3/qfunk/utility.py
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-07 13:31:18.585781 qfunk-0.1.3/qfunk.egg-info/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      556 2023-07-07 13:31:18.000000 qfunk-0.1.3/qfunk.egg-info/PKG-INFO
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      281 2023-07-07 13:31:18.000000 qfunk-0.1.3/qfunk.egg-info/SOURCES.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)        1 2023-07-07 13:31:18.000000 qfunk-0.1.3/qfunk.egg-info/dependency_links.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)        6 2023-07-07 13:31:18.000000 qfunk-0.1.3/qfunk.egg-info/top_level.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       79 2023-07-07 13:31:18.585781 qfunk-0.1.3/setup.cfg
--rwxrwxrwx   0 joshua    (1000) joshua    (1000)      760 2023-07-07 13:31:16.000000 qfunk-0.1.3/setup.py
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-10 13:06:13.040631 qfunk-0.1.4/
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)     1086 2021-09-12 18:34:10.000000 qfunk-0.1.4/LICENSE.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      556 2023-07-10 13:06:13.040631 qfunk-0.1.4/PKG-INFO
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)     5267 2021-10-12 10:57:54.000000 qfunk-0.1.4/README.md
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-10 13:06:13.036631 qfunk-0.1.4/qfunk/
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)        0 2020-12-21 12:08:47.000000 qfunk-0.1.4/qfunk/__init__.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    14942 2022-09-19 12:31:27.000000 qfunk-0.1.4/qfunk/decompose.py
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)     6401 2023-07-10 12:19:46.000000 qfunk-0.1.4/qfunk/generator.py
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)    27590 2022-01-14 22:51:51.000000 qfunk-0.1.4/qfunk/opensys.py
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)    16391 2023-07-07 14:15:45.000000 qfunk-0.1.4/qfunk/qoptic.py
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)     2291 2022-01-21 18:56:08.000000 qfunk-0.1.4/qfunk/testbench.py
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)    17059 2023-07-10 12:55:53.000000 qfunk-0.1.4/qfunk/utility.py
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-10 13:06:13.040631 qfunk-0.1.4/qfunk.egg-info/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      556 2023-07-10 13:06:12.000000 qfunk-0.1.4/qfunk.egg-info/PKG-INFO
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      281 2023-07-10 13:06:12.000000 qfunk-0.1.4/qfunk.egg-info/SOURCES.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)        1 2023-07-10 13:06:12.000000 qfunk-0.1.4/qfunk.egg-info/dependency_links.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)        6 2023-07-10 13:06:12.000000 qfunk-0.1.4/qfunk.egg-info/top_level.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)       79 2023-07-10 13:06:13.040631 qfunk-0.1.4/setup.cfg
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)      760 2023-07-10 13:05:15.000000 qfunk-0.1.4/setup.py
```

### Comparing `qfunk-0.1.3/LICENSE.txt` & `qfunk-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qfunk-0.1.3/PKG-INFO` & `qfunk-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: qfunk
-Version: 0.1.3
+Version: 0.1.4
 Summary: quantum information library
 Home-page: https://github.com/simonsupercool/qfunk
-Download-URL: https://github.com/simonsupercool/qfunk/archive/refs/tags/v0.1.3.tar.gz
+Download-URL: https://github.com/simonsupercool/qfunk/archive/refs/tags/v0.1.4.tar.gz
 Author: Simon Milz, Joshua Morris
 Author-email: Simon.Milz@oeaw.ac.at, joshua.morris@univie.ac.at
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `qfunk-0.1.3/README.md` & `qfunk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `qfunk-0.1.3/qfunk/decompose.py` & `qfunk-0.1.4/qfunk/decompose.py`

 * *Files identical despite different names*

### Comparing `qfunk-0.1.3/qfunk/generator.py` & `qfunk-0.1.4/qfunk/generator.py`

 * *Files identical despite different names*

### Comparing `qfunk-0.1.3/qfunk/opensys.py` & `qfunk-0.1.4/qfunk/opensys.py`

 * *Files identical despite different names*

### Comparing `qfunk-0.1.3/qfunk/qoptic.py` & `qfunk-0.1.4/qfunk/qoptic.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
      # reverse ordering to match fock state order
      P = P[::-1,::-1]
 
 
      # ensure normalisation property holds
      for k in range(row_num):
-          P[k,:] /= np.sqrt(np.sum(P[k,:]))
+          P[k,:] /= np.sqrt(P[k,:].sum())
 
      return P
 
 
 
 def number_states(m_num,p_num):
     """
```

### Comparing `qfunk-0.1.3/qfunk/testbench.py` & `qfunk-0.1.4/qfunk/testbench.py`

 * *Files identical despite different names*

### Comparing `qfunk-0.1.3/qfunk.egg-info/PKG-INFO` & `qfunk-0.1.4/qfunk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: qfunk
-Version: 0.1.3
+Version: 0.1.4
 Summary: quantum information library
 Home-page: https://github.com/simonsupercool/qfunk
-Download-URL: https://github.com/simonsupercool/qfunk/archive/refs/tags/v0.1.3.tar.gz
+Download-URL: https://github.com/simonsupercool/qfunk/archive/refs/tags/v0.1.4.tar.gz
 Author: Simon Milz, Joshua Morris
 Author-email: Simon.Milz@oeaw.ac.at, joshua.morris@univie.ac.at
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `qfunk-0.1.3/setup.py` & `qfunk-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qfunk",
-    version="0.1.3",
+    version="0.1.4",
     author="Simon Milz, Joshua Morris",
     author_email="Simon.Milz@oeaw.ac.at, joshua.morris@univie.ac.at",
     description="quantum information library",
     long_description_content_type="text/markdown",
     url="https://github.com/simonsupercool/qfunk",
-    download_url = "https://github.com/simonsupercool/qfunk/archive/refs/tags/v0.1.3.tar.gz",
+    download_url = "https://github.com/simonsupercool/qfunk/archive/refs/tags/v0.1.4.tar.gz",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.5',
```

