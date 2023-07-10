# Comparing `tmp/audmath-1.2.1.tar.gz` & `tmp/audmath-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audmath-1.2.1.tar", last modified: Tue Feb  7 11:00:10 2023, max compression
+gzip compressed data, was "audmath-1.3.0.tar", last modified: Mon Jul 10 10:40:45 2023, max compression
```

## Comparing `audmath-1.2.1.tar` & `audmath-1.3.0.tar`

### file list

```diff
@@ -1,51 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:00:10.605175 audmath-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:00:10.601175 audmath-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:00:10.601175 audmath-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-07 10:59:55.000000 audmath-1.2.1/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-02-07 10:59:55.000000 audmath-1.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-02-07 10:59:55.000000 audmath-1.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-07 10:59:55.000000 audmath-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-07 10:59:55.000000 audmath-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-02-07 10:59:55.000000 audmath-1.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-02-07 10:59:55.000000 audmath-1.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-02-07 10:59:55.000000 audmath-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-02-07 11:00:10.605175 audmath-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-02-07 10:59:55.000000 audmath-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:00:10.601175 audmath-1.2.1/audmath/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-07 10:59:55.000000 audmath-1.2.1/audmath/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:00:10.601175 audmath-1.2.1/audmath/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 10:59:55.000000 audmath-1.2.1/audmath/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22463 2023-02-07 10:59:55.000000 audmath-1.2.1/audmath/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-07 10:59:55.000000 audmath-1.2.1/audmath/core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-07 10:59:55.000000 audmath-1.2.1/audmath/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:00:10.601175 audmath-1.2.1/audmath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-02-07 11:00:10.000000 audmath-1.2.1/audmath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-02-07 11:00:10.000000 audmath-1.2.1/audmath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 11:00:10.000000 audmath-1.2.1/audmath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-07 11:00:10.000000 audmath-1.2.1/audmath.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-07 11:00:10.000000 audmath-1.2.1/audmath.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:00:10.601175 audmath-1.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:00:10.601175 audmath-1.2.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:00:10.601175 audmath-1.2.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-07 10:59:55.000000 audmath-1.2.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-07 10:59:55.000000 audmath-1.2.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-07 10:59:55.000000 audmath-1.2.1/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:00:10.605175 audmath-1.2.1/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-07 10:59:55.000000 audmath-1.2.1/docs/api-src/audmath.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-07 10:59:55.000000 audmath-1.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-02-07 10:59:55.000000 audmath-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-07 10:59:55.000000 audmath-1.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-07 10:59:55.000000 audmath-1.2.1/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-02-07 10:59:55.000000 audmath-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-07 10:59:55.000000 audmath-1.2.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-07 10:59:55.000000 audmath-1.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-07 10:59:55.000000 audmath-1.2.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:00:10.605175 audmath-1.2.1/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-07 10:59:55.000000 audmath-1.2.1/misc/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-07 10:59:55.000000 audmath-1.2.1/misc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-07 10:59:55.000000 audmath-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-02-07 11:00:10.605175 audmath-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-07 10:59:55.000000 audmath-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:00:10.605175 audmath-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-07 10:59:55.000000 audmath-1.2.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22132 2023-02-07 10:59:55.000000 audmath-1.2.1/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:45.233165 audmath-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-10 10:40:24.000000 audmath-1.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:45.225164 audmath-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:45.229164 audmath-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-10 10:40:24.000000 audmath-1.3.0/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-10 10:40:24.000000 audmath-1.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-10 10:40:24.000000 audmath-1.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-10 10:40:24.000000 audmath-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-10 10:40:24.000000 audmath-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-10 10:40:24.000000 audmath-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-10 10:40:24.000000 audmath-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-10 10:40:24.000000 audmath-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-10 10:40:45.233165 audmath-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-10 10:40:24.000000 audmath-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:45.229164 audmath-1.3.0/audmath/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-10 10:40:24.000000 audmath-1.3.0/audmath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:45.229164 audmath-1.3.0/audmath/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:24.000000 audmath-1.3.0/audmath/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22903 2023-07-10 10:40:24.000000 audmath-1.3.0/audmath/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-10 10:40:24.000000 audmath-1.3.0/audmath/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-10 10:40:24.000000 audmath-1.3.0/audmath/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:45.229164 audmath-1.3.0/audmath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-10 10:40:45.000000 audmath-1.3.0/audmath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-10 10:40:45.000000 audmath-1.3.0/audmath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:40:45.000000 audmath-1.3.0/audmath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 10:40:45.000000 audmath-1.3.0/audmath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 10:40:45.000000 audmath-1.3.0/audmath.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:45.233165 audmath-1.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:45.229164 audmath-1.3.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:45.233165 audmath-1.3.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 10:40:24.000000 audmath-1.3.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-10 10:40:24.000000 audmath-1.3.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-10 10:40:24.000000 audmath-1.3.0/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:45.233165 audmath-1.3.0/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-10 10:40:24.000000 audmath-1.3.0/docs/api-src/audmath.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 10:40:24.000000 audmath-1.3.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-10 10:40:24.000000 audmath-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 10:40:24.000000 audmath-1.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 10:40:24.000000 audmath-1.3.0/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-10 10:40:24.000000 audmath-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-10 10:40:24.000000 audmath-1.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-10 10:40:24.000000 audmath-1.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 10:40:24.000000 audmath-1.3.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:45.233165 audmath-1.3.0/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-10 10:40:24.000000 audmath-1.3.0/misc/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 10:40:24.000000 audmath-1.3.0/misc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-10 10:40:24.000000 audmath-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 10:40:24.000000 audmath-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:40:45.233165 audmath-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:45.233165 audmath-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-10 10:40:24.000000 audmath-1.3.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-10 10:40:24.000000 audmath-1.3.0/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-07-10 10:40:24.000000 audmath-1.3.0/tests/test_duration_in_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-10 10:40:24.000000 audmath-1.3.0/tests/test_inverse_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-10 10:40:24.000000 audmath-1.3.0/tests/test_inverse_normal_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-10 10:40:24.000000 audmath-1.3.0/tests/test_rms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-10 10:40:24.000000 audmath-1.3.0/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-10 10:40:24.000000 audmath-1.3.0/tests/test_window.py
```

### Comparing `audmath-1.2.1/.github/workflows/publish.yml` & `audmath-1.3.0/.github/workflows/publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -24,26 +24,26 @@
       uses: actions/setup-node@v3
       with:
         node-version: '16.0'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install setuptools wheel twine
+        pip install build twine virtualenv
 
     # PyPI package
     - name: Build and publish
       env:
         TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
         TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
       run: |
-        python setup.py sdist bdist_wheel
+        python -m build
         python -m twine upload dist/*
 
-    # Docuemntation
+    # Documentation
     - name: Install doc dependencies
       run: |
         pip install -r requirements.txt
         pip install -r docs/requirements.txt
 
     - name: Build documentation
       run: |
```

### Comparing `audmath-1.2.1/.github/workflows/test.yml` & `audmath-1.3.0/.github/workflows/test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,14 @@
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ ubuntu-20.04, windows-latest, macOS-latest]
         python-version: ['3.8']
         include:
           - os: ubuntu-latest
-            python-version: '3.7'
-          - os: ubuntu-latest
             python-version: '3.9'
           - os: ubuntu-latest
             python-version: '3.10'
           - os: ubuntu-latest
             python-version: '3.11'
 
     steps:
```

### Comparing `audmath-1.2.1/CHANGELOG.rst` & `audmath-1.3.0/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,43 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.3.0 (2023/07/10)
+--------------------------
+
+* Added: ``audmath.samples()``
+* Removed: support for Python 3.7
+
+
+Version 1.2.1 (2022/02/07)
+--------------------------
+
+* Added: support for
+  ``None``,
+  ``''``,
+  ``'None'``,
+  ``'NaN'``,
+  ``'NaT'``,
+  ``np.NaN``,
+  ``pd.NA``,
+  ``pd.NaT``
+  to represent ``NaN``
+  in ``audmath.duration_in_seconds()``
+* Added: support for ``'Inf'``, ``'-Inf'``, ``np.inf``, ``-np.inf``
+  to represent ``Inf``, ``-Inf``
+  in ``audmath.duration_in_seconds()``
+* Fixed: sign support in string values
+  (``'-1 ms'``, ``'+s'``)
+  in ``audmath.duration_in_seconds()``
+
+
 Version 1.2.0 (2022/02/01)
 --------------------------
 
 * Added: ``audmath.duration_in_seconds()``
   to convert any duration value to seconds
```

### Comparing `audmath-1.2.1/CONTRIBUTING.rst` & `audmath-1.3.0/CONTRIBUTING.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Contributing
 ============
 
 Everyone is invited to contribute to this project.
 Feel free to create a `pull request`_ .
-If you find errors, omissions, inconsistencies or other things
-that need improvement, please create an issue_.
+If you find errors,
+omissions,
+inconsistencies,
+or other things
+that need improvement,
+please create an issue_.
 
 .. _issue: https://github.com/audeering/audmath/issues/new/
 .. _pull request: https://github.com/audeering/audmath/compare/
 
 
 Development Installation
 ------------------------
 
 Instead of pip-installing the latest release from PyPI_,
 you should get the newest development version from Github_::
 
    git clone https://github.com/audeering/audmath/
    cd audmath
-   # Create virutal environment for this project
+   # Create virtual environment for this project
    # e.g.
    # virtualenv --python="python3"  $HOME/.envs/audmath
    # source $HOME/.envs/audmath/bin/activate
    pip install -r requirements.txt
 
 
 This way,
@@ -33,41 +37,47 @@
 .. _Github: https://github.com/audeering/audmath/
 
 
 Coding Convention
 -----------------
 
 We follow the PEP8_ convention for Python code
-and check for correct syntax with flake8_.
-Exceptions are defined under the ``[flake8]`` section
-in :file:`setup.cfg`.
+and check for correct syntax with ruff_.
+In addition,
+we check for common spelling errors with codespell_.
+Both tools and possible exceptions
+are defined in :file:`pyproject.toml`.
 
 The checks are executed in the CI using `pre-commit`_.
 You can enable those checks locally by executing::
 
     pip install pre-commit  # consider system wide installation
     pre-commit install
     pre-commit run --all-files
 
-Afterwards flake8_ is executed
+Afterwards ruff_ and codespell_ are executed
 every time you create a commit.
 
-You can also install flake8_
+You can also install ruff_ and codespell_
 and call it directly::
 
-    pip install flake8  # consider system wide installation
-    flake8
+    pip install ruff codespell  # consider system wide installation
+    ruff check .
+    codespell
 
 It can be restricted to specific folders::
 
-    flake8 audfoo/ tests/
+    ruff check audfoo/ tests/
+    codespell audfoo/ tests/
 
+
+.. _codespell: https://github.com/codespell-project/codespell/
 .. _PEP8: http://www.python.org/dev/peps/pep-0008/
-.. _flake8: https://flake8.pycqa.org/en/latest/index.html
 .. _pre-commit: https://pre-commit.com
+.. _ruff: https://beta.ruff.rs
 
 
 Building the Documentation
 --------------------------
 
 If you make changes to the documentation,
 you can re-create the HTML pages using Sphinx_.
@@ -82,30 +92,30 @@
 The generated files will be available
 in the directory :file:`build/sphinx/html/`.
 
 It is also possible to automatically check if all links are still valid::
 
    python -m sphinx docs/ build/sphinx/html -b linkcheck
 
-.. _Sphinx: http://sphinx-doc.org/
+.. _Sphinx: http://sphinx-doc.org
 
 
 Running the Tests
 -----------------
 
 You'll need pytest_ for that.
 It can be installed with::
 
    pip install -r tests/requirements.txt
 
 To execute the tests, simply run::
 
    python -m pytest
 
-.. _pytest: https://pytest.org/
+.. _pytest: https://pytest.org
 
 
 Creating a New Release
 ----------------------
 
 New releases are made using the following steps:
```

### Comparing `audmath-1.2.1/LICENSE` & `audmath-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audmath-1.2.1/README.rst` & `audmath-1.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 .. _installation: https://audeering.github.io/audmath/installation.html
 .. _usage: https://audeering.github.io/audmath/usage.html
 
 .. badges images and links:
 .. |tests| image:: https://github.com/audeering/audmath/workflows/Test/badge.svg
     :target: https://github.com/audeering/audmath/actions?query=workflow%3ATest
     :alt: Test status
-.. |coverage| image:: https://codecov.io/gh/audeering/audmath/branch/master/graph/badge.svg?token=JFyZlt0Nqk
+.. |coverage| image:: https://codecov.io/gh/audeering/audmath/branch/main/graph/badge.svg?token=JFyZlt0Nqk
     :target: https://codecov.io/gh/audeering/audmath
     :alt: code coverage
 .. |docs| image:: https://img.shields.io/pypi/v/audmath?label=docs
     :target: https://audeering.github.io/audmath/
     :alt: audmath's documentation
 .. |license| image:: https://img.shields.io/badge/license-MIT-green.svg
-    :target: https://github.com/audeering/audmath/blob/master/LICENSE
+    :target: https://github.com/audeering/audmath/blob/main/LICENSE
     :alt: audmath's MIT license
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/audmath.svg
     :target: https://pypi.org/project/audmath/
     :alt: audmath's supported Python versions
```

### Comparing `audmath-1.2.1/audmath/core/api.py` & `audmath-1.3.0/audmath/core/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import collections
-import typing
 import re
+import typing
 
 import numpy as np
 
 from audmath.core.utils import polyval
 
 
 VALUE_UNIT_PATTERN = re.compile(
@@ -485,113 +485,112 @@
 
     # Return if no other values are left
     if non_valid.sum() == len(x):
         return np.float64(x)
 
     switch_sign[non_valid] = 0
 
-    # Constants to avoid recalculation
-    ROOT_2PI = np.sqrt(2 * np.pi)
-    EXP_NEG2 = np.exp(-2)
+    # Pre-calculate to avoid recalculation
+    exp_neg2 = np.exp(-2)
 
     # Approximation for 0 <= |y - 0.5| <= 3/8
-    P0 = [
+    p0 = [
         -5.99633501014107895267E1,
         9.80010754185999661536E1,
         -5.66762857469070293439E1,
         1.39312609387279679503E1,
         -1.23916583867381258016E0,
     ]
-    Q0 = [
+    q0 = [
         1.0,
         1.95448858338141759834E0,
         4.67627912898881538453E0,
         8.63602421390890590575E1,
         -2.25462687854119370527E2,
         2.00260212380060660359E2,
         -8.20372256168333339912E1,
         1.59056225126211695515E1,
         -1.18331621121330003142E0,
     ]
 
     # Approximation for interval z = sqrt(-2 log y ) between 2 and 8,
     # i.e. y between exp(-2) = .135 and exp(-32) = 1.27e-14
-    P1 = [
+    p1 = [
         4.05544892305962419923E0,
         3.15251094599893866154E1,
         5.71628192246421288162E1,
         4.40805073893200834700E1,
         1.46849561928858024014E1,
         2.18663306850790267539E0,
         -1.40256079171354495875E-1,
         -3.50424626827848203418E-2,
         -8.57456785154685413611E-4,
     ]
 
-    Q1 = [
+    q1 = [
         1.0,
         1.57799883256466749731E1,
         4.53907635128879210584E1,
         4.13172038254672030440E1,
         1.50425385692907503408E1,
         2.50464946208309415979E0,
         -1.42182922854787788574E-1,
         -3.80806407691578277194E-2,
         -9.33259480895457427372E-4,
     ]
 
     # Approximation for interval z = sqrt(-2 log y ) between 8 and 64,
     # i.e. y between exp(-32) = 1.27e-14 and exp(-2048) = 3.67e-890
-    P2 = [
+    p2 = [
         3.23774891776946035970E0,
         6.91522889068984211695E0,
         3.93881025292474443415E0,
         1.33303460815807542389E0,
         2.01485389549179081538E-1,
         1.23716634817820021358E-2,
         3.01581553508235416007E-4,
         2.65806974686737550832E-6,
         6.23974539184983293730E-9,
     ]
 
-    Q2 = [
+    q2 = [
         1.0,
         6.02427039364742014255E0,
         3.67983563856160859403E0,
         1.37702099489081330271E0,
         2.16236993594496635890E-1,
         1.34204006088543189037E-2,
         3.28014464682127739104E-4,
         2.89247864745380683936E-6,
         6.79019408009981274425E-9,
     ]
 
-    idx1 = y > (1 - EXP_NEG2)  # y > 0.864...
+    idx1 = y > (1 - exp_neg2)  # y > 0.864...
     idx = np.where(non_valid, False, idx1)
     y[idx] = 1.0 - y[idx]
     switch_sign[idx] = 0
 
     # Case where we don't need high precision
-    idx2 = y > EXP_NEG2  # y > 0.135...
+    idx2 = y > exp_neg2  # y > 0.135...
     idx = np.where(non_valid, False, idx2)
     y[idx] = y[idx] - 0.5
     y2 = y[idx] ** 2
-    x[idx] = y[idx] + y[idx] * (y2 * polyval(y2, P0) / polyval(y2, Q0))
-    x[idx] = x[idx] * ROOT_2PI
+    x[idx] = y[idx] + y[idx] * (y2 * polyval(y2, p0) / polyval(y2, q0))
+    x[idx] = x[idx] * np.sqrt(2 * np.pi)
     switch_sign[idx] = 0
 
     idx3 = ~idx2
     idx = np.where(non_valid, False, idx3)
     x[idx] = np.sqrt(-2.0 * np.log(y[idx]))
     x0 = x[idx] - np.log(x[idx]) / x[idx]
     z = 1.0 / x[idx]
     x1 = np.where(
         x[idx] < 8.0,  # y > exp(-32) = 1.2664165549e-14
-        z * polyval(z, P1) / polyval(z, Q1),
-        z * polyval(z, P2) / polyval(z, Q2),
+        z * polyval(z, p1) / polyval(z, q1),
+        z * polyval(z, p2) / polyval(z, q2),
     )
     x[idx] = x0 - x1
 
     x = np.where(switch_sign == 1, -1 * x, x)
 
     return np.float64(x)
 
@@ -648,14 +647,40 @@
     """
     x = np.array(x)
     if x.size == 0:
         return np.float64(0.0)
     return np.sqrt(np.mean(np.square(x), axis=axis, keepdims=keepdims))
 
 
+def samples(
+        duration: float,
+        sampling_rate: int,
+) -> int:
+    r"""Duration in samples.
+
+    The duration is evenly rounded,
+    after converted to samples.
+
+    Args:
+        duration: duration in s
+        sampling_rate: sampling rate in Hz
+
+    Returns:
+        duration in number of samples
+
+    Examples:
+        >>> samples(0.5, 10)
+        5
+        >>> samples(0.55, 10)
+        6
+
+    """
+    return round(duration * sampling_rate)
+
+
 def window(
         samples: int,
         shape: str = 'tukey',
         half: str = None,
 ) -> np.ndarray:
     r"""Return a window.
```

### Comparing `audmath-1.2.1/docs/_templates/autosummary/class.rst` & `audmath-1.3.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audmath-1.2.1/docs/conf.py` & `audmath-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audmath-1.2.1/docs/index.rst` & `audmath-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audmath-1.2.1/misc/benchmark.py` & `audmath-1.3.0/misc/benchmark.py`

 * *Files identical despite different names*

