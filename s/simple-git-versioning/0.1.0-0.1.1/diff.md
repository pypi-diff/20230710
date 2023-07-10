# Comparing `tmp/simple-git-versioning-0.1.0.tar.gz` & `tmp/simple-git-versioning-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-git-versioning-0.1.0.tar", last modified: Mon Jul 10 20:02:26 2023, max compression
+gzip compressed data, was "simple-git-versioning-0.1.1.tar", last modified: Mon Jul 10 20:13:01 2023, max compression
```

## Comparing `simple-git-versioning-0.1.0.tar` & `simple-git-versioning-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:02:26.741561 simple-git-versioning-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5175 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3840 2023-07-10 20:02:26.741561 simple-git-versioning-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/Pipfile
--rw-rw-rw-   0 root         (0) root         (0)    46710 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/Pipfile.lock
--rw-rw-rw-   0 root         (0) root         (0)     2974 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1640 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 20:02:26.741561 simple-git-versioning-0.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:02:26.738561 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3840 2023-07-10 20:02:26.000000 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      681 2023-07-10 20:02:26.000000 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 20:02:26.000000 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      204 2023-07-10 20:02:26.000000 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 20:02:26.000000 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-10 20:02:26.000000 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:02:26.738561 simple-git-versioning-0.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:02:26.739561 simple-git-versioning-0.1.0/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)     7368 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/unit/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    10566 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/unit/test_pep440.py
--rw-rw-rw-   0 root         (0) root         (0)    14420 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/unit/test_project.py
--rw-rw-rw-   0 root         (0) root         (0)     3196 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/unit/test_semver2.py
--rw-rw-rw-   0 root         (0) root         (0)     3248 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/unit/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:02:26.740561 simple-git-versioning-0.1.0/versioning/
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/versioning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14854 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/versioning/pep440.py
--rw-rw-rw-   0 root         (0) root         (0)     7746 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/versioning/project.py
--rw-rw-rw-   0 root         (0) root         (0)     8643 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/versioning/semver2.py
--rw-rw-rw-   0 root         (0) root         (0)     2040 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/versioning/setuptools.py
--rw-rw-rw-   0 root         (0) root         (0)     1146 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/versioning/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:13:01.875044 simple-git-versioning-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5175 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3840 2023-07-10 20:13:01.875044 simple-git-versioning-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)    46710 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/Pipfile.lock
+-rw-rw-rw-   0 root         (0) root         (0)     2974 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 20:13:01.875044 simple-git-versioning-0.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:13:01.871378 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3840 2023-07-10 20:13:01.000000 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-10 20:13:01.000000 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 20:13:01.000000 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-10 20:13:01.000000 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 20:13:01.000000 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-10 20:13:01.000000 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:13:01.871378 simple-git-versioning-0.1.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:13:01.872294 simple-git-versioning-0.1.1/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)     7368 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/unit/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    10566 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/unit/test_pep440.py
+-rw-rw-rw-   0 root         (0) root         (0)    14420 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/unit/test_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     3196 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/unit/test_semver2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3248 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/unit/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:13:01.874128 simple-git-versioning-0.1.1/versioning/
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/versioning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14854 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/versioning/pep440.py
+-rw-rw-rw-   0 root         (0) root         (0)     7746 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/versioning/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     8643 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/versioning/semver2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/versioning/setuptools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/versioning/version.py
```

### Comparing `simple-git-versioning-0.1.0/.gitlab-ci.yml` & `simple-git-versioning-0.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/.pre-commit-config.yaml` & `simple-git-versioning-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/LICENSE` & `simple-git-versioning-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/PKG-INFO` & `simple-git-versioning-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-git-versioning
-Version: 0.1.0
+Version: 0.1.1
 Summary: Thinly scoped and opinionated tool that computes a version number from git tags and trailers
 Author-email: Quentin Bouget <ypsah@devyard.org>
 License: MIT
 Project-URL: homepage, https://gitlab.com/ypsah/simple-git-versioning
 Project-URL: repository, https://gitlab.com/ypsah/simple-git-versioning
 Keywords: versioning,git,git-trailers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `simple-git-versioning-0.1.0/Pipfile.lock` & `simple-git-versioning-0.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/README.md` & `simple-git-versioning-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/pyproject.toml` & `simple-git-versioning-0.1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -18,34 +18,36 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.11",
 ]
 readme = "README.md"
-version = "0.1.0"
-dynamic = ["dependencies"]
+dynamic = ["dependencies", "version"]
 
 [project.urls]
 homepage = "https://gitlab.com/ypsah/simple-git-versioning"
 repository = "https://gitlab.com/ypsah/simple-git-versioning"
 
 [project.scripts]
 pep440 = "versioning.pep440:main"
 semver2 = "versioning.semver2:main"
 
 [project.entry-points."setuptools.finalize_distribution_options"]
 simple-git-versioning = "versioning.setuptools:finalize_distribution_options"
 
 [build-system]
-requires = ["setuptools>=63", "setuptools-scm", "setuptools-pipfile"]
+requires = ["setuptools>=63", "setuptools-scm", "setuptools-pipfile", "simple-git-versioning>=0.1.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools-pipfile]
 
+[tool.simple-git-versioning]
+setuptools = "pep440"
+
 [tool.black]
 line-length = 120
 target-version = ['py311']
 # enrole in feature-preview
 preview = true
 
 [tool.isort]
```

### Comparing `simple-git-versioning-0.1.0/simple_git_versioning.egg-info/PKG-INFO` & `simple-git-versioning-0.1.1/simple_git_versioning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-git-versioning
-Version: 0.1.0
+Version: 0.1.1
 Summary: Thinly scoped and opinionated tool that computes a version number from git tags and trailers
 Author-email: Quentin Bouget <ypsah@devyard.org>
 License: MIT
 Project-URL: homepage, https://gitlab.com/ypsah/simple-git-versioning
 Project-URL: repository, https://gitlab.com/ypsah/simple-git-versioning
 Keywords: versioning,git,git-trailers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `simple-git-versioning-0.1.0/simple_git_versioning.egg-info/SOURCES.txt` & `simple-git-versioning-0.1.1/simple_git_versioning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/tests/unit/__init__.py` & `simple-git-versioning-0.1.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/tests/unit/test_cli.py` & `simple-git-versioning-0.1.1/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/tests/unit/test_pep440.py` & `simple-git-versioning-0.1.1/tests/unit/test_pep440.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/tests/unit/test_project.py` & `simple-git-versioning-0.1.1/tests/unit/test_project.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/tests/unit/test_semver2.py` & `simple-git-versioning-0.1.1/tests/unit/test_semver2.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/tests/unit/test_version.py` & `simple-git-versioning-0.1.1/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/versioning/__init__.py` & `simple-git-versioning-0.1.1/versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/versioning/pep440.py` & `simple-git-versioning-0.1.1/versioning/pep440.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/versioning/project.py` & `simple-git-versioning-0.1.1/versioning/project.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/versioning/semver2.py` & `simple-git-versioning-0.1.1/versioning/semver2.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/versioning/setuptools.py` & `simple-git-versioning-0.1.1/versioning/setuptools.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.0/versioning/version.py` & `simple-git-versioning-0.1.1/versioning/version.py`

 * *Files identical despite different names*

