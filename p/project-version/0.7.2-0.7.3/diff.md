# Comparing `tmp/project-version-0.7.2.tar.gz` & `tmp/project-version-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project-version-0.7.2.tar", last modified: Sat Jan 29 16:33:49 2022, max compression
+gzip compressed data, was "project-version-0.7.3.tar", last modified: Mon Jul 10 18:05:14 2023, max compression
```

## Comparing `project-version-0.7.2.tar` & `project-version-0.7.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-29 16:33:49.824038 project-version-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-29 16:33:31.000000 project-version-0.7.2/.project-version
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-01-29 16:33:31.000000 project-version-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-01-29 16:33:31.000000 project-version-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    24810 2022-01-29 16:33:49.824038 project-version-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    23928 2022-01-29 16:33:31.000000 project-version-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-29 16:33:49.820038 project-version-0.7.2/project_version/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-29 16:33:31.000000 project-version-0.7.2/project_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4515 2022-01-29 16:33:31.000000 project-version-0.7.2/project_version/abstarct.py
--rw-r--r--   0 runner    (1001) docker     (121)     5926 2022-01-29 16:33:31.000000 project-version-0.7.2/project_version/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-01-29 16:33:31.000000 project-version-0.7.2/project_version/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-01-29 16:33:31.000000 project-version-0.7.2/project_version/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-01-29 16:33:31.000000 project-version-0.7.2/project_version/help.py
--rw-r--r--   0 runner    (1001) docker     (121)     5141 2022-01-29 16:33:31.000000 project-version-0.7.2/project_version/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-01-29 16:33:31.000000 project-version-0.7.2/project_version/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-29 16:33:49.820038 project-version-0.7.2/project_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    24810 2022-01-29 16:33:49.000000 project-version-0.7.2/project_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-01-29 16:33:49.000000 project-version-0.7.2/project_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-29 16:33:49.000000 project-version-0.7.2/project_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-01-29 16:33:49.000000 project-version-0.7.2/project_version.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-29 16:33:49.000000 project-version-0.7.2/project_version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-01-29 16:33:49.000000 project-version-0.7.2/project_version.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-29 16:33:49.824038 project-version-0.7.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-01-29 16:33:31.000000 project-version-0.7.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-01-29 16:33:31.000000 project-version-0.7.2/requirements/ops.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-29 16:33:31.000000 project-version-0.7.2/requirements/project.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-01-29 16:33:31.000000 project-version-0.7.2/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-01-29 16:33:49.824038 project-version-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1994 2022-01-29 16:33:31.000000 project-version-0.7.2/setup.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-10 18:05:14.493921 project-version-0.7.3/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        6 2023-07-10 18:04:43.000000 project-version-0.7.3/.project-version
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2023-07-10 18:03:48.000000 project-version-0.7.3/LICENSE
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       75 2023-07-10 18:03:48.000000 project-version-0.7.3/MANIFEST.in
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    24773 2023-07-10 18:05:14.493998 project-version-0.7.3/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    23928 2023-07-10 18:03:48.000000 project-version-0.7.3/README.md
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-10 18:05:14.492679 project-version-0.7.3/project_version/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-10 18:03:48.000000 project-version-0.7.3/project_version/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     4515 2023-07-10 18:03:48.000000 project-version-0.7.3/project_version/abstarct.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     5926 2023-07-10 18:03:48.000000 project-version-0.7.3/project_version/commands.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      169 2023-07-10 18:03:48.000000 project-version-0.7.3/project_version/constants.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      420 2023-07-10 18:03:48.000000 project-version-0.7.3/project_version/entrypoint.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      522 2023-07-10 18:03:48.000000 project-version-0.7.3/project_version/help.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     5141 2023-07-10 18:03:48.000000 project-version-0.7.3/project_version/services.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1113 2023-07-10 18:03:48.000000 project-version-0.7.3/project_version/utils.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-10 18:05:14.493422 project-version-0.7.3/project_version.egg-info/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    24773 2023-07-10 18:05:14.000000 project-version-0.7.3/project_version.egg-info/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      611 2023-07-10 18:05:14.000000 project-version-0.7.3/project_version.egg-info/SOURCES.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-10 18:05:14.000000 project-version-0.7.3/project_version.egg-info/dependency_links.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       67 2023-07-10 18:05:14.000000 project-version-0.7.3/project_version.egg-info/entry_points.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       30 2023-07-10 18:05:14.000000 project-version-0.7.3/project_version.egg-info/requires.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       16 2023-07-10 18:05:14.000000 project-version-0.7.3/project_version.egg-info/top_level.txt
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-10 18:05:14.493823 project-version-0.7.3/requirements/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      442 2023-07-10 18:03:48.000000 project-version-0.7.3/requirements/dev.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       69 2023-07-10 18:03:48.000000 project-version-0.7.3/requirements/ops.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       30 2023-07-10 18:04:35.000000 project-version-0.7.3/requirements/project.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       46 2023-07-10 18:03:48.000000 project-version-0.7.3/requirements/tests.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      604 2023-07-10 18:05:14.494229 project-version-0.7.3/setup.cfg
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1994 2023-07-10 18:03:48.000000 project-version-0.7.3/setup.py
```

### Comparing `project-version-0.7.2/LICENSE` & `project-version-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `project-version-0.7.2/PKG-INFO` & `project-version-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: project-version
-Version: 0.7.2
+Version: 0.7.3
 Summary: Explicit, strict and automatic project version management based on semantic versioning.
 Home-page: https://github.com/dmytrostriletskyi/project-version
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -569,9 +567,7 @@
 ```
 
 If you are new for the contribution, please read:
 
 * About pull requests — https://help.github.com/en/articles/about-pull-requests
 * Create a pull request — https://help.github.com/en/articles/creating-a-pull-request-from-a-fork
 * The beginners guide to contributing — https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/
-
-
```

### Comparing `project-version-0.7.2/README.md` & `project-version-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `project-version-0.7.2/project_version/abstarct.py` & `project-version-0.7.3/project_version/abstarct.py`

 * *Files identical despite different names*

### Comparing `project-version-0.7.2/project_version/commands.py` & `project-version-0.7.3/project_version/commands.py`

 * *Files identical despite different names*

### Comparing `project-version-0.7.2/project_version/help.py` & `project-version-0.7.3/project_version/help.py`

 * *Files identical despite different names*

### Comparing `project-version-0.7.2/project_version/services.py` & `project-version-0.7.3/project_version/services.py`

 * *Files identical despite different names*

### Comparing `project-version-0.7.2/project_version/utils.py` & `project-version-0.7.3/project_version/utils.py`

 * *Files identical despite different names*

### Comparing `project-version-0.7.2/project_version.egg-info/PKG-INFO` & `project-version-0.7.3/project_version.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: project-version
-Version: 0.7.2
+Version: 0.7.3
 Summary: Explicit, strict and automatic project version management based on semantic versioning.
 Home-page: https://github.com/dmytrostriletskyi/project-version
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -569,9 +567,7 @@
 ```
 
 If you are new for the contribution, please read:
 
 * About pull requests — https://help.github.com/en/articles/about-pull-requests
 * Create a pull request — https://help.github.com/en/articles/creating-a-pull-request-from-a-fork
 * The beginners guide to contributing — https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/
-
-
```

### Comparing `project-version-0.7.2/project_version.egg-info/SOURCES.txt` & `project-version-0.7.3/project_version.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `project-version-0.7.2/setup.cfg` & `project-version-0.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `project-version-0.7.2/setup.py` & `project-version-0.7.3/setup.py`

 * *Files identical despite different names*

