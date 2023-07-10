# Comparing `tmp/yet_another_wizz_cli-1.2.1.tar.gz` & `tmp/yet_another_wizz_cli-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet_another_wizz_cli-1.2.1.tar", last modified: Mon Jul 10 12:57:44 2023, max compression
+gzip compressed data, was "yet_another_wizz_cli-1.2.2.tar", last modified: Mon Jul 10 19:31:40 2023, max compression
```

## Comparing `yet_another_wizz_cli-1.2.1.tar` & `yet_another_wizz_cli-1.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:57:44.478753 yet_another_wizz_cli-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-07-10 12:57:44.478753 yet_another_wizz_cli-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 12:57:44.478753 yet_another_wizz_cli-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:57:44.474753 yet_another_wizz_cli-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:57:44.478753 yet_another_wizz_cli-1.2.1/src/yaw_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:57:44.478753 yet_another_wizz_cli-1.2.1/src/yaw_cli/commandline/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/commandline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/commandline/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/commandline/subcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/commandline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:57:44.478753 yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/default_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/directories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-07-10 12:57:33.000000 yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:57:44.478753 yet_another_wizz_cli-1.2.1/src/yet_another_wizz_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-07-10 12:57:44.000000 yet_another_wizz_cli-1.2.1/src/yet_another_wizz_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-10 12:57:44.000000 yet_another_wizz_cli-1.2.1/src/yet_another_wizz_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:57:44.000000 yet_another_wizz_cli-1.2.1/src/yet_another_wizz_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 12:57:44.000000 yet_another_wizz_cli-1.2.1/src/yet_another_wizz_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-10 12:57:44.000000 yet_another_wizz_cli-1.2.1/src/yet_another_wizz_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 12:57:44.000000 yet_another_wizz_cli-1.2.1/src/yet_another_wizz_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:40.782389 yet_another_wizz_cli-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-10 19:31:40.782389 yet_another_wizz_cli-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:31:40.782389 yet_another_wizz_cli-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:40.778390 yet_another_wizz_cli-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:40.778390 yet_another_wizz_cli-1.2.2/src/yaw_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:40.778390 yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:40.778390 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/default_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16003 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:40.778390 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-10 19:31:40.000000 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-10 19:31:40.000000 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:31:40.000000 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 19:31:40.000000 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-10 19:31:40.000000 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 19:31:40.000000 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/top_level.txt
```

### Comparing `yet_another_wizz_cli-1.2.1/LICENSE` & `yet_another_wizz_cli-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.1/PKG-INFO` & `yet_another_wizz_cli-1.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yet_another_wizz_cli
-Version: 1.2.1
+Version: 1.2.2
 Summary: Command line client for yet_another_wizz.
 Home-page: https://github.com/jlvdb/yet_another_wizz_cli.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
@@ -16,16 +16,16 @@
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 yet_another_wizz_cli
 ====================
 
-.. image:: https://badge.fury.io/py/yet-another-wizz-cli.svg
-    :target: https://badge.fury.io/py/yet-another-wizz-cli
+.. image:: https://img.shields.io/pypi/v/yet_another_wizz_cli?logo=pypi&logoColor=blue
+    :target: https://pypi.org/project/yet_another_wizz_cli/
 .. image:: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz_cli/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz_cli
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
@@ -107,20 +107,34 @@
 support throughout the development of this software.
 
 
 Change log
 ==========
 
 
+Version 1.2.2
+-------------
+
+Added simple unit tests that run a randommised setup.
+
+.. rubric:: Bug fixes
+
+- Fixed the install dependency, which was pointing to ``yet_another_wizz``
+  instead of the section in the client setup.
+- Fixed formatting errors in the default configuration file: The task sections
+  were missing ":" if they were followed by a mapping of default arguments, the
+  filepath entry in the randoms sections was not indented correctly.
+
+
 Version 1.2.1
 -------------
 
 .. rubric:: Bug fixes
 
-Corrected the incorrectly named dependency for ``yet_another_wizz``.
+- Corrected the incorrectly named dependency for ``yet_another_wizz``.
 
 
 Version 1.2
 -----------
 
 Initial release as separate package. Previously the package was bundled with
 ``yet_another_wizz`` itself.
```

### Comparing `yet_another_wizz_cli-1.2.1/README.rst` & `yet_another_wizz_cli-1.2.2/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 yet_another_wizz_cli
 ====================
 
-.. image:: https://badge.fury.io/py/yet-another-wizz-cli.svg
-    :target: https://badge.fury.io/py/yet-another-wizz-cli
+.. image:: https://img.shields.io/pypi/v/yet_another_wizz_cli?logo=pypi&logoColor=blue
+    :target: https://pypi.org/project/yet_another_wizz_cli/
 .. image:: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz_cli/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz_cli
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
@@ -88,20 +88,34 @@
 support throughout the development of this software.
 
 
 Change log
 ==========
 
 
+Version 1.2.2
+-------------
+
+Added simple unit tests that run a randommised setup.
+
+.. rubric:: Bug fixes
+
+- Fixed the install dependency, which was pointing to ``yet_another_wizz``
+  instead of the section in the client setup.
+- Fixed formatting errors in the default configuration file: The task sections
+  were missing ":" if they were followed by a mapping of default arguments, the
+  filepath entry in the randoms sections was not indented correctly.
+
+
 Version 1.2.1
 -------------
 
 .. rubric:: Bug fixes
 
-Corrected the incorrectly named dependency for ``yet_another_wizz``.
+- Corrected the incorrectly named dependency for ``yet_another_wizz``.
 
 
 Version 1.2
 -----------
 
 Initial release as separate package. Previously the package was bundled with
 ``yet_another_wizz`` itself.
```

### Comparing `yet_another_wizz_cli-1.2.1/pyproject.toml` & `yet_another_wizz_cli-1.2.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 requires-python = ">=3.8"
 dependencies = [
     "numpy",
     "pandas",
     "pyyaml",
     "matplotlib",
-    "yet-another-wizz>=2.5.1",
+    "yet-another-wizz>=2.5.2",
 ]
 
 [project.scripts]
 yaw_cli = "yaw_cli:Commandline.main"
 
 [project.optional-dependencies]
 plot = ["matplotlib"]
@@ -39,29 +39,33 @@
 ]
 test = [
     "coverage",
     "pytest",
     "pytest-cov",
 ]
 dev = [
-    "yet_another_wizz[style]",
-    "yet_another_wizz[test]",
+    "yet_another_wizz_cli[style]",
+    "yet_another_wizz_cli[test]",
     "ipykernel",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "yaw_cli.__version__"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.pytest.ini_options]
-minversion = "6.0"
-addopts = "-ra -q"
-testpaths = ["tests"]
+testpaths = [
+    "tests",
+]
+addopts = [
+    "--cov=yaw_cli",
+    "--cov-report=xml",
+]
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 include = ".pyi?$"
 exclude = """
```

### Comparing `yet_another_wizz_cli-1.2.1/src/yaw_cli/commandline/main.py` & `yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/main.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.1/src/yaw_cli/commandline/subcommands.py` & `yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/subcommands.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.1/src/yaw_cli/commandline/utils.py` & `yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/utils.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/__init__.py` & `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/data.py` & `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/data.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/default_setup.py` & `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/default_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 setup_default += format_line(
     "data:", "data catalog file and column names", indents=level
 )
 level += 1
 setup_default += format_line(
     "filepath:",
     "either a single file path (no tomographic bins) or a mapping of integer bin index to file path (as shown below)",
-    indents=2,
+    indents=level,
 )
 setup_default += format_line("1: ...", "bin 1", indents=level + 1)
 setup_default += format_line("2: ...", "bin 2", indents=level + 1)
 setup_default += format_line("ra: ra", "right ascension in degrees", indents=level)
 setup_default += format_line("dec: dec", "declination in degrees", indents=level)
 setup_default += format_line(
     "redshift: z",
@@ -204,10 +204,13 @@
 )
 setup_default += f"{COMM_SEP}  - cross\n{COMM_SEP}  - zcc\n"
 setup_default += wrap_comment(
     "to get a basic cluster redshift estimate or with the optional parameters listed below (all values optional, defaults listed)."
 )
 setup_default += "tasks:\n"
 for task in tasks.Task.all_tasks():
-    setup_default += format_line(task.get_name(), task.get_help(), indents=DASH)
+    name = task.get_name()
+    if task.get_n_par() > 0:
+        name += ":"
+    setup_default += format_line(name, task.get_help(), indents=DASH)
     setup_default += make_doc(task, indent=2, indicate_opt=False)
 setup_default = setup_default.strip("\n")
```

### Comparing `yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/directories.py` & `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/directories.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/logger.py` & `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/logger.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/merge.py` & `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     # merge and check scales
     common = set.intersection(*scale_sets)
     if len(common) == 0:
         MergeError("found no common scales")
     extra = set.union(*scale_sets) - common
     if len(extra) > 0:
-        logger.warn(f"ignoring unmatched scales: {', '.join(extra)}")
+        logger.warning(f"ignoring unmatched scales: {', '.join(extra)}")
 
     # merge binning
     if merge_binning:
         bins = np.unique(np.concatenate(bins))
         bin_config = ManualBinningConfig(bins)
         if bin_config.zbin_num != n_bins:
             raise MergeError("cannot concatenate bins contiguously")
@@ -103,15 +103,15 @@
     for project in projects:
         bin_sets.append(project.get_bin_indices())
     common = set.intersection(*bin_sets)
     if len(common) == 0:
         MergeError("found no common bins")
     extra = set.union(*bin_sets) - common
     if len(extra) > 0:
-        logger.warn(f"ignoring uncommon bins: {', '.join(str(b) for b in extra)}")
+        logger.warning(f"ignoring uncommon bins: {', '.join(str(b) for b in extra)}")
     return common
 
 
 def merge_state_attr(
     states: Iterable[ProjectState], attr: str, require: bool = False
 ) -> bool:
     attr_states = [getattr(state, attr) for state in states]
@@ -123,35 +123,35 @@
 
 def get_merged_state(projects: Sequence[YawDirectory]) -> ProjectState:
     states = [project.get_state() for project in projects]
     try:
         has_w_ss = merge_state_attr(states, "has_w_ss", require=True)
     except MergeError:
         has_w_ss = False
-        logger.warn("ignoring uncommon reference autocorrelation functions")
+        logger.warning("ignoring uncommon reference autocorrelation functions")
     try:
         has_w_pp = merge_state_attr(states, "has_w_pp", require=True)
     except MergeError:
         has_w_pp = False
-        logger.warn("ignoring uncommon unknown autocorrelation functions")
+        logger.warning("ignoring uncommon unknown autocorrelation functions")
     try:
         has_w_sp = merge_state_attr(states, "has_w_sp", require=True)
     except MergeError:
         has_w_sp = False
-        logger.warn("ignoring uncommon crosscorrelation functions")
+        logger.warning("ignoring uncommon crosscorrelation functions")
     try:
         has_nz_true = merge_state_attr(states, "has_nz_true", require=True)
     except MergeError:
         has_nz_true = False
-        logger.warn("ignoring uncommon true redshift distributions")
+        logger.warning("ignoring uncommon true redshift distributions")
     try:
         has_nz_ref = merge_state_attr(states, "has_nz_ref", require=True)
     except MergeError:
         has_nz_ref = False
-        logger.warn("ignoring uncommon reference sample redshift distributions")
+        logger.warning("ignoring uncommon reference sample redshift distributions")
     return ProjectState(
         has_w_ss=has_w_ss,
         has_w_pp=has_w_pp,
         has_w_sp=has_w_sp,
         has_nz_true=has_nz_true,
         has_nz_ref=has_nz_ref,
     )
```

### Comparing `yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/plot.py` & `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/plot.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/processing.py` & `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         return self.project.get_state()
 
     def _warn_patches(self):
         LIM = 512
         msg = f"a large number of patches (>{LIM}) may degrade the performance"
         if not self._warned_patches:
             if self.project.inputs.get_n_patches() > LIM:
-                logger.warn(msg)
+                logger.warning(msg)
                 self._warned_patches = True
 
     def set_bin_idx(self, idx: int) -> None:
         if idx not in self.project.get_bin_indices():
             raise IndexError(f"bin with index {idx} not configured in setup")
         self._bin_idx = idx
         # reset internally referenced correlation functions
@@ -195,15 +195,15 @@
             denom_info.append(get_info(unk_data))
 
         info = f"{get_info(cross_data)} / sqrt({' '.join(denom_info)})"
         for scale in self.project.iter_scales():
             key = (scale, tag)
             est_dir = self.project.get_estimate_dir(scale, tag, create=True)
             path = est_dir.get_cross(self.get_bin_idx())
-            nz_data = RedshiftData.from_correlation_data(
+            nz_data = RedshiftData.from_corrdata(
                 cross_data[key], ref_data[key], unk_data[key], info=info
             )
             nz_data.to_files(path)
 
     def plot(self):
         plot_dir = self.project.estimate_path
         try:
@@ -238,15 +238,15 @@
             title="Unknown autocorrelation",
             name="auto_unknown.png",
         )
         plotted |= plot_wrapper(
             method=plotter.nz, title="Redshift estimate", name="nz_estimate.png"
         )
         if not plotted:
-            logger.warn("there was no data to plot")
+            logger.warning("there was no data to plot")
 
 
 class DataProcessor(PostProcessor):
     def __init__(self, project: ProjectDirectory) -> None:
         super().__init__(project)
         # warning state flags
         self._warned_patches = False
@@ -311,15 +311,15 @@
             for cat in cats:
                 if cat is not None:
                     break
             else:
                 raise MissingCatalogError("no catalogs loaded")
             self._linkage = PatchLinkage.from_setup(self.config, cat)
             if self._linkage.density > 0.3 and not self._warned_linkage:
-                logger.warn(
+                logger.warning(
                     "linkage density > 0.3, either patches overlap "
                     "significantly or are small compared to scales"
                 )
                 self._warned_linkage = True
 
     def run_auto_ref(self, *, compute_rr: bool) -> _Tcf:
         if self._ref_rand is None:
```

### Comparing `yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/project.py` & `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/project.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.1/src/yaw_cli/pipeline/tasks.py` & `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,18 @@
 
     def to_dict(self) -> dict[str, Any]:
         # return only non-default values
         defaults = self.get_defaults()
         return {k: v for k, v in asdict(self).items() if v != defaults[k]}
 
     @classmethod
+    def get_n_par(cls) -> int:
+        return len(fields(cls))
+
+    @classmethod
     def get_parnames(cls) -> list[str]:
         return [par.name for par in fields(cls)]
 
     @classmethod
     def get_defaults(cls) -> dict[str, Any]:
         return {par.name: par.default for par in fields(cls)}
 
@@ -595,15 +599,15 @@
                             )
                             zcc_processed = True
 
                 if do_true:
                     engine.write_nz_true()
 
         if do_zcc and not zcc_processed:
-            logger.warn("task 'zcc': there were no pair counts to process")
+            logger.warning("task 'zcc': there were no pair counts to process")
 
         if drop_cache:
             engine.drop_cache()
 
         if plot:
             print_yaw_message("plotting data")
             engine.plot()
```

### Comparing `yet_another_wizz_cli-1.2.1/src/yet_another_wizz_cli.egg-info/PKG-INFO` & `yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yet-another-wizz-cli
-Version: 1.2.1
+Version: 1.2.2
 Summary: Command line client for yet_another_wizz.
 Home-page: https://github.com/jlvdb/yet_another_wizz_cli.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
@@ -16,16 +16,16 @@
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 yet_another_wizz_cli
 ====================
 
-.. image:: https://badge.fury.io/py/yet-another-wizz-cli.svg
-    :target: https://badge.fury.io/py/yet-another-wizz-cli
+.. image:: https://img.shields.io/pypi/v/yet_another_wizz_cli?logo=pypi&logoColor=blue
+    :target: https://pypi.org/project/yet_another_wizz_cli/
 .. image:: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz_cli/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz_cli
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
@@ -107,20 +107,34 @@
 support throughout the development of this software.
 
 
 Change log
 ==========
 
 
+Version 1.2.2
+-------------
+
+Added simple unit tests that run a randommised setup.
+
+.. rubric:: Bug fixes
+
+- Fixed the install dependency, which was pointing to ``yet_another_wizz``
+  instead of the section in the client setup.
+- Fixed formatting errors in the default configuration file: The task sections
+  were missing ":" if they were followed by a mapping of default arguments, the
+  filepath entry in the randoms sections was not indented correctly.
+
+
 Version 1.2.1
 -------------
 
 .. rubric:: Bug fixes
 
-Corrected the incorrectly named dependency for ``yet_another_wizz``.
+- Corrected the incorrectly named dependency for ``yet_another_wizz``.
 
 
 Version 1.2
 -----------
 
 Initial release as separate package. Previously the package was bundled with
 ``yet_another_wizz`` itself.
```

### Comparing `yet_another_wizz_cli-1.2.1/src/yet_another_wizz_cli.egg-info/SOURCES.txt` & `yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

