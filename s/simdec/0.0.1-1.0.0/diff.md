# Comparing `tmp/simdec-0.0.1.tar.gz` & `tmp/simdec-1.0.0.tar.gz`

## Comparing `simdec-0.0.1.tar` & `simdec-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,14 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 simdec-0.0.1/.DS_Store
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 simdec-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 simdec-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 simdec-0.0.1/src/simdec/.DS_Store
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 simdec-0.0.1/src/simdec/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 simdec-0.0.1/README.md
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 simdec-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 simdec-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 simdec-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5698 2020-02-02 00:00:00.000000 simdec-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 simdec-1.0.0/Makefile
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 simdec-1.0.0/app.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 simdec-1.0.0/src/simdec/__init__.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 simdec-1.0.0/src/simdec/decomposition.py
+-rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 simdec-1.0.0/src/simdec/significance.py
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 simdec-1.0.0/src/simdec/visualization.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 simdec-1.0.0/src/simdec/workflow.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 simdec-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 simdec-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 simdec-1.0.0/README.md
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 simdec-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 simdec-1.0.0/PKG-INFO
```

### Comparing `simdec-0.0.1/pyproject.toml` & `simdec-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,84 @@
 [build-system]
 requires = ["hatchling>=1.14.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simdec"
-version = "0.0.1"
+version = "1.0.0"
 description = "Sensitivity analysis using simulation decomposition"
 readme = "README.md"
 requires-python = ">=3.9"
+license = "BSD-3-Clause"
 authors = [
-  { name = "Pamphile Roy" },
+    { name = "Pamphile Roy" },
 ]
 maintainers = [
-  { name = "simdec contributors" },
+    { name = "simdec contributors" },
 ]
 classifiers = [
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Intended Audience :: End Users/Desktop",
-  "Intended Audience :: Developers",
-  "Intended Audience :: Science/Research",
-  "Operating System :: OS Independent",
+    "Intended Audience :: End Users/Desktop",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: BSD License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
-  "numpy",
-  "pandas",
+    "numpy",
+    "pandas",
+    "SALib",
+    "seaborn",
+    "typer[all]",
+    "panel",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
 ]
 
 doc = [
     "sphinx",
-    "pydata-sphinx-theme"
+    "pydata-sphinx-theme",
+    "accessible-pygments",
+    "numpydoc",
 ]
 
 dev = [
-    "simdec[test]",
-    "simdec[doc]",
+    "simdec[doc,test]",
     "pre-commit",
     "hatch",
 ]
 
+[project.scripts]
+simdec = "simdec.workflow:app"
+
 [project.urls]
-Documentation = "https://simdec.readthedocs.io"
-"Source code" = "https://github.com/Simulation-Decomposition/simdec-python"
+homepage = "https://www.simdec.fi/"
+documentation = "https://simdec.readthedocs.io"
+source = "https://github.com/Simulation-Decomposition/simdec-python"
+
+[tool.hatch]
+build.targets.sdist.exclude = [
+  ".github",
+  "docs",
+  "tests",
+  "*.rst",
+  "*.yml",
+  ".*",
+]
 
 [tool.pytest.ini_options]
 addopts = "--durations 10"
 testpaths = [
     "tests",
 ]
+
+[tool.ruff.per-file-ignores]
+"**/__init__.py" = ["F403", "F405"]
```

