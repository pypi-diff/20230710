# Comparing `tmp/puwifi-1.0.2.tar.gz` & `tmp/puwifi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puwifi-1.0.2.tar", last modified: Mon Jul 10 18:02:36 2023, max compression
+gzip compressed data, was "puwifi-1.0.3.tar", last modified: Mon Jul 10 18:09:43 2023, max compression
```

## Comparing `puwifi-1.0.2.tar` & `puwifi-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:02:36.755962 puwifi-1.0.2/
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-10 14:39:51.000000 puwifi-1.0.2/.gitattributes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:02:36.755962 puwifi-1.0.2/.github/
--rw-r--r--   0 root         (0) root         (0)      501 2023-07-10 14:39:51.000000 puwifi-1.0.2/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:02:36.755962 puwifi-1.0.2/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-07-10 14:39:51.000000 puwifi-1.0.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 root         (0) root         (0)      594 2023-07-10 14:39:51.000000 puwifi-1.0.2/.github/workflows/pylint.yml
--rw-r--r--   0 root         (0) root         (0)     3078 2023-07-10 17:52:26.000000 puwifi-1.0.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)    18172 2023-07-10 17:52:26.000000 puwifi-1.0.2/.pylintrc
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-10 14:39:51.000000 puwifi-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3793 2023-07-10 18:02:36.755962 puwifi-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3185 2023-07-10 18:00:00.000000 puwifi-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:02:36.755962 puwifi-1.0.2/puwifi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3793 2023-07-10 18:02:36.000000 puwifi-1.0.2/puwifi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-10 18:02:36.000000 puwifi-1.0.2/puwifi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 18:02:36.000000 puwifi-1.0.2/puwifi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-10 18:02:36.000000 puwifi-1.0.2/puwifi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-10 18:02:36.000000 puwifi-1.0.2/puwifi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-10 18:02:36.000000 puwifi-1.0.2/puwifi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9143 2023-07-10 17:52:26.000000 puwifi-1.0.2/puwifi.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-10 18:01:15.000000 puwifi-1.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-10 14:39:51.000000 puwifi-1.0.2/renovate.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 14:39:51.000000 puwifi-1.0.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 18:02:36.755962 puwifi-1.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:09:43.045961 puwifi-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-10 14:39:51.000000 puwifi-1.0.3/.gitattributes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:09:43.045961 puwifi-1.0.3/.github/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-07-10 14:39:51.000000 puwifi-1.0.3/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:09:43.045961 puwifi-1.0.3/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-07-10 14:39:51.000000 puwifi-1.0.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 root         (0) root         (0)      594 2023-07-10 14:39:51.000000 puwifi-1.0.3/.github/workflows/pylint.yml
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-07-10 17:52:26.000000 puwifi-1.0.3/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    18172 2023-07-10 17:52:26.000000 puwifi-1.0.3/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-10 14:39:51.000000 puwifi-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3867 2023-07-10 18:09:43.045961 puwifi-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-07-10 18:08:53.000000 puwifi-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:09:43.045961 puwifi-1.0.3/puwifi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3867 2023-07-10 18:09:43.000000 puwifi-1.0.3/puwifi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-10 18:09:43.000000 puwifi-1.0.3/puwifi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 18:09:43.000000 puwifi-1.0.3/puwifi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-10 18:09:43.000000 puwifi-1.0.3/puwifi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-10 18:09:43.000000 puwifi-1.0.3/puwifi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-10 18:09:43.000000 puwifi-1.0.3/puwifi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9143 2023-07-10 17:52:26.000000 puwifi-1.0.3/puwifi.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-10 18:09:35.000000 puwifi-1.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-10 14:39:51.000000 puwifi-1.0.3/renovate.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 14:39:51.000000 puwifi-1.0.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 18:09:43.045961 puwifi-1.0.3/setup.cfg
```

### Comparing `puwifi-1.0.2/.github/workflows/codeql-analysis.yml` & `puwifi-1.0.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.2/.github/workflows/pylint.yml` & `puwifi-1.0.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.2/.gitignore` & `puwifi-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.2/.pylintrc` & `puwifi-1.0.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.2/LICENSE` & `puwifi-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.2/PKG-INFO` & `puwifi-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: puwifi
-Version: 1.0.2
+Version: 1.0.3
 Summary: ⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever
 Author-email: SaicharanKandukuri <saicharankandukuri1x1@gmail.com>
 Project-URL: Homepage, https://github.com/SaicharanKandukuri/puwifi
 Project-URL: Bug Tracker, https://github.com/SaicharanKandukuri/puwifi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PU-wifi
-A python program written by that simulates puwifi authentication request process to keep you device connected to parul university wifi
+A python program that simulates [parul university](https://www.google.com/search?q=parul+university) wifi web authentication request process to keep you device connected to parul university wifi (with-a-loop)
 
 ![image](https://user-images.githubusercontent.com/68287637/146675073-7e1aebcc-056d-4351-b5aa-f7e2f57b1853.png)
 
 <!--
 ![image](https://user-images.githubusercontent.com/68287637/146674599-1568723d-6c70-49e8-8d71-1275ab3b169d.png)
 -->
```

### Comparing `puwifi-1.0.2/README.md` & `puwifi-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # PU-wifi
-A python program written by that simulates puwifi authentication request process to keep you device connected to parul university wifi
+A python program that simulates [parul university](https://www.google.com/search?q=parul+university) wifi web authentication request process to keep you device connected to parul university wifi (with-a-loop)
 
 ![image](https://user-images.githubusercontent.com/68287637/146675073-7e1aebcc-056d-4351-b5aa-f7e2f57b1853.png)
 
 <!--
 ![image](https://user-images.githubusercontent.com/68287637/146674599-1568723d-6c70-49e8-8d71-1275ab3b169d.png)
 -->
```

### Comparing `puwifi-1.0.2/puwifi.egg-info/PKG-INFO` & `puwifi-1.0.3/puwifi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: puwifi
-Version: 1.0.2
+Version: 1.0.3
 Summary: ⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever
 Author-email: SaicharanKandukuri <saicharankandukuri1x1@gmail.com>
 Project-URL: Homepage, https://github.com/SaicharanKandukuri/puwifi
 Project-URL: Bug Tracker, https://github.com/SaicharanKandukuri/puwifi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PU-wifi
-A python program written by that simulates puwifi authentication request process to keep you device connected to parul university wifi
+A python program that simulates [parul university](https://www.google.com/search?q=parul+university) wifi web authentication request process to keep you device connected to parul university wifi (with-a-loop)
 
 ![image](https://user-images.githubusercontent.com/68287637/146675073-7e1aebcc-056d-4351-b5aa-f7e2f57b1853.png)
 
 <!--
 ![image](https://user-images.githubusercontent.com/68287637/146674599-1568723d-6c70-49e8-8d71-1275ab3b169d.png)
 -->
```

### Comparing `puwifi-1.0.2/puwifi.py` & `puwifi-1.0.3/puwifi.py`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.2/pyproject.toml` & `puwifi-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="puwifi"
-version="1.0.2"
+version="1.0.3"
 
 authors = [
     { name="SaicharanKandukuri", email="saicharankandukuri1x1@gmail.com"}
 ]
 
 description = "⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever"
 readme = "README.md"
```

