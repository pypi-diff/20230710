# Comparing `tmp/gfort2py-2.1.0.tar.gz` & `tmp/gfort2py-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfort2py-2.1.0.tar", last modified: Sun Jul  2 17:50:38 2023, max compression
+gzip compressed data, was "gfort2py-2.2.0.tar", last modified: Mon Jul 10 14:32:35 2023, max compression
```

## Comparing `gfort2py-2.1.0.tar` & `gfort2py-2.2.0.tar`

### file list

```diff
@@ -1,90 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.263303 gfort2py-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.251303 gfort2py-2.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.251303 gfort2py-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.github/workflows/ci-mac.yml
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.github/workflows/ci-old.yml
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.github/workflows/coveralls.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-02 17:50:22.000000 gfort2py-2.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-07-02 17:50:22.000000 gfort2py-2.1.0/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-02 17:50:22.000000 gfort2py-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-07-02 17:50:38.263303 gfort2py-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-07-02 17:50:22.000000 gfort2py-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-02 17:50:22.000000 gfort2py-2.1.0/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.251303 gfort2py-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.251303 gfort2py-2.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/source/fortranabi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/source/mod_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/source/testsuite.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.255303 gfort2py-2.1.0/gfort2py/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fArrays.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fDT.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fProc.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fProcPtr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fScalars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fStrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fUnary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fVar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fVar_t.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/gfort2py.py
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/module_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.259303 gfort2py-2.1.0/gfort2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-07-02 17:50:38.000000 gfort2py-2.1.0/gfort2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-02 17:50:38.000000 gfort2py-2.1.0/gfort2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:50:38.000000 gfort2py-2.1.0/gfort2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:50:38.000000 gfort2py-2.1.0/gfort2py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-02 17:50:38.000000 gfort2py-2.1.0/gfort2py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-02 17:50:38.000000 gfort2py-2.1.0/gfort2py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-02 17:50:22.000000 gfort2py-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-02 17:50:22.000000 gfort2py-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 17:50:22.000000 gfort2py-2.1.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-02 17:50:38.263303 gfort2py-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 17:50:22.000000 gfort2py-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.263303 gfort2py-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/basic.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/basic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/common.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/complex.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/complex_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/dt.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/dt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/dummy_arrays.f90
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/dummy_arrays_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/elemental.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/explicit_arrays.f90
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/explicit_arrays_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/interface.f90
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/namelist.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/oo.f90
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/oo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/pdt.f90
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/pdt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/pointers.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/pointers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/proc_ptrs.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/proc_ptrs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/strings.f90
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/strings_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/submodule.f90
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/template._f90
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/test_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:32:35.336711 gfort2py-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:32:35.328710 gfort2py-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:32:35.332710 gfort2py-2.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-10 14:32:18.000000 gfort2py-2.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-10 14:32:18.000000 gfort2py-2.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-10 14:32:18.000000 gfort2py-2.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:32:35.332710 gfort2py-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-10 14:32:18.000000 gfort2py-2.2.0/.github/workflows/ci-mac.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-10 14:32:18.000000 gfort2py-2.2.0/.github/workflows/ci-old.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-10 14:32:18.000000 gfort2py-2.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-10 14:32:18.000000 gfort2py-2.2.0/.github/workflows/coveralls.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-10 14:32:18.000000 gfort2py-2.2.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-10 14:32:18.000000 gfort2py-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-10 14:32:18.000000 gfort2py-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-10 14:32:18.000000 gfort2py-2.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-10 14:32:18.000000 gfort2py-2.2.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-10 14:32:18.000000 gfort2py-2.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-07-10 14:32:18.000000 gfort2py-2.2.0/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 14:32:18.000000 gfort2py-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-07-10 14:32:35.336711 gfort2py-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-07-10 14:32:18.000000 gfort2py-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-10 14:32:18.000000 gfort2py-2.2.0/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:32:35.332710 gfort2py-2.2.0/gfort2py/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/fArrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/fDT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/fParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/fProc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/fProcPtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/fScalars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/fStrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/fUnary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/fVar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/fVar_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/gfort2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23305 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/module_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-10 14:32:18.000000 gfort2py-2.2.0/gfort2py/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:32:35.332710 gfort2py-2.2.0/gfort2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-07-10 14:32:35.000000 gfort2py-2.2.0/gfort2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-10 14:32:35.000000 gfort2py-2.2.0/gfort2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:32:35.000000 gfort2py-2.2.0/gfort2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:32:35.000000 gfort2py-2.2.0/gfort2py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-10 14:32:35.000000 gfort2py-2.2.0/gfort2py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 14:32:35.000000 gfort2py-2.2.0/gfort2py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-10 14:32:18.000000 gfort2py-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 14:32:18.000000 gfort2py-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 14:32:18.000000 gfort2py-2.2.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-10 14:32:35.336711 gfort2py-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:32:18.000000 gfort2py-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:32:35.336711 gfort2py-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/basic.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/basic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/common.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/complex.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/complex_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/dt.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/dt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/dummy_arrays.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/dummy_arrays_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/elemental.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/explicit_arrays.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/explicit_arrays_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/interface.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/kinds_check.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/namelist.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/oo.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/oo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/pdt.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/pdt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/pointers.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/pointers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/proc_ptrs.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/proc_ptrs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/strings.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/strings_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/submodule.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/t_params_modules.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/t_params_modules_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/t_vars_modules.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/t_vars_modules_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/template._f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:32:35.336711 gfort2py-2.2.0/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/templates/module_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/templates/module_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/templates/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tests/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-10 14:32:18.000000 gfort2py-2.2.0/tox.ini
```

### Comparing `gfort2py-2.1.0/.github/dependabot.yml` & `gfort2py-2.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/.github/workflows/ci-mac.yml` & `gfort2py-2.2.0/.github/workflows/ci-mac.yml`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/.github/workflows/ci-old.yml` & `gfort2py-2.2.0/.github/workflows/ci-old.yml`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/.github/workflows/ci.yml` & `gfort2py-2.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/.github/workflows/coveralls.yml` & `gfort2py-2.2.0/.github/workflows/coveralls.yml`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/.github/workflows/pypi.yml` & `gfort2py-2.2.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/.gitignore` & `gfort2py-2.2.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 *.c
 *.s
 tests/tester
 tests/*.f90.*
 tests/*.gz.*
 tests/*.gz
 *.smod
+tests/kinds
 
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 dist/
```

### Comparing `gfort2py-2.1.0/CODE_OF_CONDUCT.md` & `gfort2py-2.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/COPYING.txt` & `gfort2py-2.2.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/PKG-INFO` & `gfort2py-2.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: gfort2py
-Version: 2.1.0
-Summary: "Python bindings for Fortran"
-Home-page: https://github.com/rjfarmer/gfort2py
-Author: Robert Farmer
-Author-email: robert.j.farmer37@gmail.com
-License: GPLv2+
-Platform: unix
-Platform: linux
-Platform: osx
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Code Generators
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: dev
-License-File: COPYING.txt
-
 [![Continuous Integration](https://github.com/rjfarmer/gfort2py/actions/workflows/ci.yml/badge.svg)](https://github.com/rjfarmer/gfort2py/actions/workflows/ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/rjfarmer/gfort2py/badge.svg?branch=main)](https://coveralls.io/github/rjfarmer/gfort2py?branch=main)
 [![PyPI version](https://badge.fury.io/py/gfort2py.svg)](https://badge.fury.io/py/gfort2py)
 [![DOI](https://zenodo.org/badge/72889348.svg)](https://zenodo.org/badge/latestdoi/72889348)
 [![Python versions](https://img.shields.io/pypi/pyversions/gfort2py.svg)](https://img.shields.io/pypi/pyversions/gfort2py.svg)
 
 
@@ -62,35 +37,34 @@
 ## Using
 ### Fortran side
 Your Fortran code must be inside a module and then compiled as a shared library.
 
 On linux: 
 ````bash
 gfortran -fPIC -shared -c file.f90
-gfortran -fPIC -shared -o libfile file.f90
+gfortran -fPIC -shared -o libfile.so file.f90
 ````
 
 On MacOS: 
 ````bash
 gfortran -dynamiclib -c file.f90
-gfortran -dynamiclib -o libfile file.f90
+gfortran -dynamiclib -o libfile.dylib file.f90
 ````
 
 On Windows:
 ````bash
 gfortran -shared -c file.f90
 gfortran -shared -o libfile.dll file.f90
 ````
 
 If your code comes as program that does everything, then just turn the program into a function call inside a module,
 then create a new file with your program that uses the module and calls the function you just made.
 
 If the shared library needs other
-shared libraries you will need to set LD_LIBRARY_PATH environment variable, and it is also recommended is to run chrpath on the 
-shared libraries so you can access them from anywhere.
+shared libraries you will need to set LD_LIBRARY_PATH environment variable, and it is also recommended to run chrpath on the shared libraries so you can access them from anywhere.
 
 ### Python side
 ````python
 
 import gfort2py as gf
 
 SHARED_LIB_NAME=f'./test_mod.{gf.lib_ext()}' # Handle whether on Linux or Mac
@@ -105,15 +79,15 @@
 ### Functions
 ````python
 y = x.func_name(a,b,c)
 ````
 
 Will call the Fortran function with variables ``a,b,c`` and returns the result in ``y``.
 
-``y`` will be  named tuple which contains (result, args). Where result is a python object for the return value (0 if a subroutine) and where args is a dict containing all arguments passed to the procedure (both those with intent (in) which will be unchanged and intent(inout/out) which may have changed).
+``y`` will be  named tuple which contains (result, args). Where ``result`` is a python object for the return value (0 if a subroutine) and where args is a dict containing all arguments passed to the procedure (both those with intent (in) which will be unchanged and intent(inout/out) which may have changed).
 
 
 ### Variables
 
 ````python
 x.some_var = 1
 ````
@@ -331,15 +305,15 @@
 x.func_ptr = x.func_arg # With the function itself
 ```` -->
 
 ## Accessing module file data
 
 For those wanting to explore the module file format, there is a routine ``mod_info`` available from the top-level ``gfort2py`` module:
 
-````
+````python
 module = gf.mod_info('file.mod')
 ````
 
 That will parse the mod file and convert it into an intermediate format inside ``module``.
 
 Variables or procedures can be looked up via the item interface (I also recommend using pprint for easier viewing):
 
@@ -357,10 +331,92 @@
 
 For those wanting to get more involved, adding Fortran examples to the test suite of currently untested or unsupported features would be helpful. Bonus points if you also provide a Python test case (that can be marked ``@pytest.mark.skip`` if it does not work) that demonstrates the proposed interface to the new Fortran feature. Features with test cases will move higher in the order of things I add to the code.
 
 See [how to write a test case](tests/README.md) for details on how to write test cases.
 
 For those wanting to go further and add the new feature themselves open a bug report and we can chat about what needs doing.
 
+## Debugging
+
+For those wanting to dig further into ``gfort2py``.
+
+Assuming that you loaded things as:
+
+````python
+x = gf.fFort(SO, MOD)
+````
+
+You can find out the available Fortran variables/procedures module information with:
+
+````python
+var = x._module['variable_name']
+````
+
+### Variables
+
+For variables you can create a ``fVar`` (the object that handles converting too and from Python to Fortran) with:
+
+````python
+fvar = gf.fVar.fVar(var,x._module)
+````
+
+Note that at this point the ``fvar`` has no idea where to look for the variable. If you want to access its value in a module then
+
+````python
+fvar.in_dll(x._lib)
+print(fvar.value)
+````
+
+and you can then set the value (after calling ``in_dll``) with:
+
+````python
+fvar.value = value
+````
+
+### Procedures
+
+For a procedure you can do:
+
+````python
+proc = x._module['procedure_name']
+````
+
+and its Fortran object is:
+
+````python
+fproc = gf.fProc.fProc(x._lib,proc,x._module)
+````
+
+Calling the procedure is then:
+
+````python
+fproc(*args,**kwargs)
+````
+
+To access the arguments of a procedure then:
+
+````python
+args = [x._module[i.ref] for i in proc.args().symbol]
+````
+
+The return value of a function is accessed via:
+
+````python
+return_arg = x._module[proc.return_arg()]
+````
+
+### Derived types
+
+To access a derived type (the type definition not an instance of the type)
 
+````python
+dt_type = x._module['Derived_name']
+````
 
+Note the capitalization, derived types start with a capital.
 
+Similar to a variable, to access an instance of a derived type variable its:
+
+````python
+dt_var = x._module['dt_variable_name']
+dt_fvar = gf.fVar.fVar(dt_var,x._module)
+````
```

### Comparing `gfort2py-2.1.0/README.md` & `gfort2py-2.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: gfort2py
+Version: 2.2.0
+Summary: "Python bindings for Fortran"
+Home-page: https://github.com/rjfarmer/gfort2py
+Author: Robert Farmer
+Author-email: robert.j.farmer37@gmail.com
+License: GPLv2+
+Platform: unix
+Platform: linux
+Platform: osx
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Code Generators
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: dev
+License-File: COPYING.txt
+
 [![Continuous Integration](https://github.com/rjfarmer/gfort2py/actions/workflows/ci.yml/badge.svg)](https://github.com/rjfarmer/gfort2py/actions/workflows/ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/rjfarmer/gfort2py/badge.svg?branch=main)](https://coveralls.io/github/rjfarmer/gfort2py?branch=main)
 [![PyPI version](https://badge.fury.io/py/gfort2py.svg)](https://badge.fury.io/py/gfort2py)
 [![DOI](https://zenodo.org/badge/72889348.svg)](https://zenodo.org/badge/latestdoi/72889348)
 [![Python versions](https://img.shields.io/pypi/pyversions/gfort2py.svg)](https://img.shields.io/pypi/pyversions/gfort2py.svg)
 
 
@@ -37,35 +62,34 @@
 ## Using
 ### Fortran side
 Your Fortran code must be inside a module and then compiled as a shared library.
 
 On linux: 
 ````bash
 gfortran -fPIC -shared -c file.f90
-gfortran -fPIC -shared -o libfile file.f90
+gfortran -fPIC -shared -o libfile.so file.f90
 ````
 
 On MacOS: 
 ````bash
 gfortran -dynamiclib -c file.f90
-gfortran -dynamiclib -o libfile file.f90
+gfortran -dynamiclib -o libfile.dylib file.f90
 ````
 
 On Windows:
 ````bash
 gfortran -shared -c file.f90
 gfortran -shared -o libfile.dll file.f90
 ````
 
 If your code comes as program that does everything, then just turn the program into a function call inside a module,
 then create a new file with your program that uses the module and calls the function you just made.
 
 If the shared library needs other
-shared libraries you will need to set LD_LIBRARY_PATH environment variable, and it is also recommended is to run chrpath on the 
-shared libraries so you can access them from anywhere.
+shared libraries you will need to set LD_LIBRARY_PATH environment variable, and it is also recommended to run chrpath on the shared libraries so you can access them from anywhere.
 
 ### Python side
 ````python
 
 import gfort2py as gf
 
 SHARED_LIB_NAME=f'./test_mod.{gf.lib_ext()}' # Handle whether on Linux or Mac
@@ -80,15 +104,15 @@
 ### Functions
 ````python
 y = x.func_name(a,b,c)
 ````
 
 Will call the Fortran function with variables ``a,b,c`` and returns the result in ``y``.
 
-``y`` will be  named tuple which contains (result, args). Where result is a python object for the return value (0 if a subroutine) and where args is a dict containing all arguments passed to the procedure (both those with intent (in) which will be unchanged and intent(inout/out) which may have changed).
+``y`` will be  named tuple which contains (result, args). Where ``result`` is a python object for the return value (0 if a subroutine) and where args is a dict containing all arguments passed to the procedure (both those with intent (in) which will be unchanged and intent(inout/out) which may have changed).
 
 
 ### Variables
 
 ````python
 x.some_var = 1
 ````
@@ -306,15 +330,15 @@
 x.func_ptr = x.func_arg # With the function itself
 ```` -->
 
 ## Accessing module file data
 
 For those wanting to explore the module file format, there is a routine ``mod_info`` available from the top-level ``gfort2py`` module:
 
-````
+````python
 module = gf.mod_info('file.mod')
 ````
 
 That will parse the mod file and convert it into an intermediate format inside ``module``.
 
 Variables or procedures can be looked up via the item interface (I also recommend using pprint for easier viewing):
 
@@ -332,10 +356,92 @@
 
 For those wanting to get more involved, adding Fortran examples to the test suite of currently untested or unsupported features would be helpful. Bonus points if you also provide a Python test case (that can be marked ``@pytest.mark.skip`` if it does not work) that demonstrates the proposed interface to the new Fortran feature. Features with test cases will move higher in the order of things I add to the code.
 
 See [how to write a test case](tests/README.md) for details on how to write test cases.
 
 For those wanting to go further and add the new feature themselves open a bug report and we can chat about what needs doing.
 
+## Debugging
+
+For those wanting to dig further into ``gfort2py``.
+
+Assuming that you loaded things as:
+
+````python
+x = gf.fFort(SO, MOD)
+````
+
+You can find out the available Fortran variables/procedures module information with:
+
+````python
+var = x._module['variable_name']
+````
+
+### Variables
+
+For variables you can create a ``fVar`` (the object that handles converting too and from Python to Fortran) with:
+
+````python
+fvar = gf.fVar.fVar(var,x._module)
+````
+
+Note that at this point the ``fvar`` has no idea where to look for the variable. If you want to access its value in a module then
+
+````python
+fvar.in_dll(x._lib)
+print(fvar.value)
+````
+
+and you can then set the value (after calling ``in_dll``) with:
+
+````python
+fvar.value = value
+````
+
+### Procedures
+
+For a procedure you can do:
+
+````python
+proc = x._module['procedure_name']
+````
+
+and its Fortran object is:
+
+````python
+fproc = gf.fProc.fProc(x._lib,proc,x._module)
+````
+
+Calling the procedure is then:
+
+````python
+fproc(*args,**kwargs)
+````
+
+To access the arguments of a procedure then:
+
+````python
+args = [x._module[i.ref] for i in proc.args().symbol]
+````
+
+The return value of a function is accessed via:
+
+````python
+return_arg = x._module[proc.return_arg()]
+````
+
+### Derived types
+
+To access a derived type (the type definition not an instance of the type)
 
+````python
+dt_type = x._module['Derived_name']
+````
 
+Note the capitalization, derived types start with a capital.
 
+Similar to a variable, to access an instance of a derived type variable its:
+
+````python
+dt_var = x._module['dt_variable_name']
+dt_fvar = gf.fVar.fVar(dt_var,x._module)
+````
```

### Comparing `gfort2py-2.1.0/gfort2py/fArrays.py` & `gfort2py-2.2.0/gfort2py/fArrays.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,20 @@
         print(f"span {self.cvalue.span}")
         print(f"dims {self.ndim}")
         for i in range(self.ndim):
             print(f"\t lbound {self.cvalue.dims[i].lbound}")
             print(f"\t ubound {self.cvalue.dims[i].ubound}")
             print(f"\t stride {self.cvalue.dims[i].stride}")
 
+    def _make_empty(self):
+        dtype = self.obj.dtype()
+        shape = self.obj.shape()
+
+        return np.zeros(shape, dtype=dtype, order="F")
+
 
 class fAssumedSize(fArray_t):
     def ctype(self):
         return self._ctype_base * np.prod(self._value.shape)
 
     def from_param(self, value):
         self._value = self._array_check(value)
```

### Comparing `gfort2py-2.1.0/gfort2py/fDT.py` & `gfort2py-2.2.0/gfort2py/fDT.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/gfort2py/fProc.py` & `gfort2py-2.2.0/gfort2py/fProc.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import select
 import collections
 import functools
 from dataclasses import dataclass
 
 from .fVar import fVar
 from .fVar_t import fVar_t
+from .utils import resolve_other_args
 
 _TEST_FLAG = os.environ.get("_GFORT2PY_TEST_FLAG") is not None
 
 
 @dataclass
 class variable:
     value: "typing.Any"
@@ -68,44 +69,45 @@
         return self.obj.head.module
 
     @property
     def name(self):
         return self.obj.name
 
     def __call__(self, *args, **kwargs):
-        self._set_return()
-
         func_args = self._convert_args(*args, **kwargs)
 
         with _captureStdOut() as cs:
             if func_args is not None:
                 res = self._func(*func_args)
             else:
                 res = self._func()
 
         return self._convert_result(res, func_args)
 
-    def _set_return(self):
+    def _set_return(self, other_args):
         if self.obj.is_subroutine():
             self._func.restype = None  # Subroutine
         else:
-            if (
-                self.return_var.obj.is_char()
-            ):  # Returning a character is done as a character + len at start of arg list
+            self.return_var.obj = resolve_other_args(self.return_var.obj, other_args)
+
+            if self.return_var.obj.is_returned_as_arg():
                 self._func.restype = None
             else:
                 self._func.restype = self.return_var.ctype()
 
     def args_start(self):
         res = []
         if self.obj.is_function():
             if self.return_var.obj.is_char():
                 l = self.return_var.len()
                 res.append(self.return_var.from_param(" " * l))
                 res.append(self.return_var.ctype_len())
+            elif self.return_var.obj.is_always_explicit() and self.obj.is_array():
+                empty_array = self.return_var._make_empty()
+                res.append(ctypes.pointer(self.return_var.from_param(empty_array)))
 
         return res
 
     def args_check(self, *args, **kwargs):
         count = 0
         arguments = []
         # Build list of inputs
@@ -141,30 +143,37 @@
             args.append(a)
             if e is not None:
                 args_end.append(e)
 
         return args, args_end
 
     def _convert_args(self, *args, **kwargs):
-        args_start = self.args_start()
-
         self.input_args = self.args_check(*args, **kwargs)
 
+        # Set this now after arsg_check as we need to be able to
+        # resolve runtime arguments
+        self._set_return(self.input_args)
+        args_start = self.args_start()
+
         args_mid, args_end = self.args_convert(self.input_args)
 
         return args_start + args_mid + args_end
 
     def _convert_result(self, result, args):
         res = {}
 
         if self.obj.is_function():
-            if self.return_var.obj.is_char():
-                result = args[0]
-                _ = args.pop(0)
-                _ = args.pop(0)  # Twice to pop first and second value
+            if self.return_var.obj.is_returned_as_arg():
+                if self.return_var.obj.is_char():
+                    result = args[0]
+                    _ = args.pop(0)
+                    _ = args.pop(0)  # Twice to pop first and second value
+                elif self.return_var.obj.is_always_explicit() and self.obj.is_array():
+                    result = self.return_var.value
+                    _ = args.pop(0)
 
         if len(self.obj.args()):
             for var in self.input_args:
                 if var.fvar.unpack:
                     try:
                         x = ptr_unpack(var.fvar.value)
                     except AttributeError:  # unset optional arguments
```

### Comparing `gfort2py-2.1.0/gfort2py/fScalars.py` & `gfort2py-2.2.0/gfort2py/fScalars.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/gfort2py/fStrings.py` & `gfort2py-2.2.0/gfort2py/fStrings.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/gfort2py/fUnary.py` & `gfort2py-2.2.0/gfort2py/fUnary.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/gfort2py/fVar.py` & `gfort2py-2.2.0/gfort2py/fVar.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,20 @@
                     raise TypeError(
                         "Unknown type of character array not currently supported"
                     )
             elif obj.is_explicit():
                 return fExplicitArr(obj, *args, **kwargs)
             elif obj.is_assumed_size():
                 return fAssumedSize(obj, *args, **kwargs)
-            elif obj.is_assumed_shape() or obj.is_allocatable() or obj.is_pointer():
+            elif (
+                obj.is_assumed_shape()
+                or obj.is_allocatable()
+                or obj.is_pointer()
+                or obj.is_always_explicit()
+            ):
                 return fAssumedShape(obj, *args, **kwargs)
             else:
                 raise TypeError("Unknown array type")
         else:
             if obj.is_char():
                 if obj.is_allocatable():
                     return fAllocStr(obj, *args, **kwargs)
```

### Comparing `gfort2py-2.1.0/gfort2py/fVar_t.py` & `gfort2py-2.2.0/gfort2py/fVar_t.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,14 +82,18 @@
                 end = self.ctype_len(value)
 
         return self.Args(start, arg, end)
 
 
 def ctype_map(type, kind):
     if type == "INTEGER":
+        if kind == 1:
+            return ctypes.c_int8
+        elif kind == 2:
+            return ctypes.c_int16
         if kind == 4:
             return ctypes.c_int32
         elif kind == 8:
             return ctypes.c_int64
         else:
             raise TypeError("Integer type of kind={kind} not supported")
     elif type == "REAL":
```

### Comparing `gfort2py-2.1.0/gfort2py/gfort2py.py` & `gfort2py-2.2.0/gfort2py/gfort2py.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/gfort2py/module_parse.py` & `gfort2py-2.2.0/gfort2py/module_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # SPDX-License-Identifier: GPL-2.0+
 
+# https://github.com/gcc-mirror/gcc/blob/master/gcc/fortran/module.cc
 from pyparsing import OneOrMore, nestedExpr
 from dataclasses import dataclass
 import numpy as np
 import gzip
 import sys
 
 import pprint
@@ -78,27 +79,44 @@
         return self._item_name.keys()
 
 
 #################################
 
 
 @dataclass
-class c_item:
-    name: str
-    id: int
-    saved_flag: bool
-    _unknown: int
-    _unknown2: str
+class symbol_ref:
+    ref: int = -1
 
     def __post_init__(self):
-        self.name = string_clean(self.name)
-        self.id = int(self.id)
-        self.saved_flag = int(self.saved_flag)
-        self._unknown = int(self._unknown)
-        self._unknown2 = string_clean(self._unknown2)
+        self.ref = int(self.ref)
+
+
+#################################
+
+
+@dataclass(init=False)
+class c_item:
+    name: str = ""
+    common_link: symbol_ref = -1
+    saved_flag: bool = False
+    thread_private: bool = False
+    omp_device_type: bool = False
+    is_bind_c: bool = False
+    binding_label: str = ""
+
+    def __init__(self, *args):
+        self.name = string_clean(args[0])
+        self.common_link = symbol_ref(args[1])
+        self.saved_flag = bin(int(args[2]))[-1] == "1"
+        self.thread_private = bin(int(args[2]))[-2] == "1"
+        self.omp_device_type = bin(int(args[2]))[-3] == "1"
+        self.is_bind_c = args[3] == 1
+        self.binding_label = string_clean(args[4])
+
+        self.raw = args
 
 
 #################################
 
 
 @dataclass(init=False)
 class generics:
@@ -109,14 +127,16 @@
     def __init__(self, *args):
         self.name = string_clean(args[0])
         self.module = string_clean(args[1])
         self.id = []
         for i in args[2:]:
             self.id.append(int(i))
 
+        self.raw = args
+
 
 #################################
 
 
 def hextofloat(s, double=False):
     # Given hex like parameter '0.12decde@9' returns 5065465344.0
     man, exp = s.split("@")
@@ -153,28 +173,32 @@
             raise NotAnArrayError("Not an array")
 
     def dtype(self):
         t = self.type()
         k = int(self.kind())
 
         if t == "INTEGER" or t == "LOGICAL":
-            if k == 4:
+            if k == 1:
+                return "i1"
+            elif k == 2:
+                return "i2"
+            elif k == 4:
                 return "i4"
             elif k == 8:
                 return "i8"
         elif t == "REAL":
             if k == 4:
                 return "f4"
             elif k == 8:
                 return "f8"
         elif t == "COMPLEX":
             if k == 4:
-                return "c4"
+                return np.csingle
             elif k == 8:
-                return "c8"
+                return np.cdouble
         elif t == "CHARACTER":
             return f"S{self.strlen.value}"
 
         raise NotImplementedError(f"Object of type {t} and kind {k} not supported yet")
 
     def type(self):
         return self.sym.ts.type
@@ -226,26 +250,29 @@
 
     def is_function(self):
         return self.sym.sym_ref.ref != 0
 
     def is_array(self):
         return "DIMENSION" in self.sym.attr.attributes
 
-    def is_always_explicit(self):
-        return "ALWAYS_EXPLICIT" in self.sym.attr.attributes
-
     def is_dummy(self):
         return "DUMMY" in self.sym.attr.attributes
 
     def is_allocatable(self):
         return "ALLOCATABLE" in self.sym.attr.attributes
 
+    def is_return(self):
+        return "RESULT" in self.sym.attr.attributes
+
     def needs_array_desc(self):
         return self.is_dummy() or self.is_allocatable() or self.is_always_explicit()
 
+    def is_always_explicit(self):
+        return "ALWAYS_EXPLICIT" in self.sym.attr.attributes
+
     def not_a_pointer(self):
         return (
             self.needs_array_desc()
             and self.is_array()
             and not self.is_assumed_shape()
             and not self.is_assumed_size()
         )
@@ -258,14 +285,19 @@
 
     def is_assumed_size(self):
         return self.sym.array_spec.array_type == "ASSUMED_SIZE"
 
     def is_assumed_shape(self):
         return self.sym.array_spec.array_type == "ASSUMED_SHAPE"
 
+    def is_returned_as_arg(self):
+        return (self.is_always_explicit() and self.is_return() and self.is_array()) or (
+            self.is_char()
+        )
+
     def is_deferred_len(self):
         # Only needed for things that need an extra function argument for their length
         if self.is_char():
             try:
                 return self.sym.ts.charlen.value == -1
             except AttributeError:
                 return True
@@ -276,14 +308,17 @@
 
     def is_derived(self):
         return self.sym.ts.type == "DERIVED"
 
     def is_pdt_def(self):
         return "PDT_TEMPLATE" in self.sym.attr.attributes
 
+    def in_common_block(self):
+        return "IN_CMMMON" in self.sym.attr.attributes
+
     @property
     def strlen(self):
         if self.is_char() and not self.is_deferred_len():
             return self.sym.ts.charlen
         raise AttributeError("Not a deferred length type")
 
     @property
@@ -346,14 +381,15 @@
         self.intent = string_clean(args[1])
         self.proc = string_clean(args[2])
         self.if_source = string_clean(args[3])
         self.save = string_clean(args[4])
         self.ext_attr = int(args[5])
         self.extension = int(args[6])
         self.attributes = set([string_clean(i) for i in args[7:]])
+        self.raw = args
 
 
 @dataclass
 class namespace:
     ref: int = -1
 
     def __post_init__(self):
@@ -377,31 +413,25 @@
 
     @property
     def mn_name(self):
         if self.module:
             return f"__{self.module}_MOD_{self.name}"
 
 
-@dataclass
-class symbol_ref:
-    ref: int = -1
-
-    def __post_init__(self):
-        self.ref = int(self.ref)
-
-
 @dataclass(init=False)
 class formal_arglist:
     symbol: t.List[symbol_ref] = None
 
     def __init__(self, *args):
         self.symbol = []
         for i in args:
             self.symbol.append(symbol_ref(i))
 
+        self.raw = args
+
     def __len__(self):
         return len(self.symbol)
 
     def __iter__(self):
         return iter(self.symbol)
 
 
@@ -426,36 +456,39 @@
         self.ppc = args[0][1][4]
         self.pass_arg = string_clean(args[0][1][5])
         self.pass_arg_num = symbol_ref(args[0][1][6])
 
         # TODO: Handle is_generic
         self.proc_ref = symbol_ref(args[0][1][7][0])
 
+        self.raw = args
+        self.kwargs = kwargs
+
 
 @dataclass(init=False)
 class derived_ns:
     unknown1: str = None
     proc: t.List[typebound_proc] = None
 
     def __init__(self, *args, **kwargs):
+        self.raw = args
+        self.kwargs = kwargs
+
         if not len(args):
             return
         self.unknown1 = args[0]
         self.proc = []
         for i in args[1]:
             self.proc.append(typebound_proc(i))
 
 
 @dataclass(init=False)
 class actual_arglist:
-    args: None
-    kwargs: None
-
     def __init__(self, *args, **kwargs):
-        self.args = args
+        self.raw = args
         self.kwargs = kwargs
 
 
 @dataclass(init=False)
 class typespec:
     type: str = ""
     kind: int = -1  # If class symbol_ref else kind
@@ -465,15 +498,15 @@
     is_iso_c: int = -1
     type2: str = ""  # Repeat of type
     charlen: int = -1  # If character
     deferred_cl: bool = False  # if character and deferred length
     args = None
 
     def __init__(self, *args):
-        self.args = args
+        self.raw = args
         self.type = args[0]
         if self.type == "CLASS" or self.type == "DERIVED":
             self.class_ref = symbol_ref(args[1])
         else:
             self.kind = int(args[1])
 
         if len(args[2]):
@@ -505,32 +538,28 @@
     rank: int = -1
     _value: t.Any = None
     _resolved_value: t.Any = None  # value may by a symbol_ref, so this is the value after resolving the reference
     arglist: actual_arglist = None  # PDT's?
     charlen: int = -1
     unary_op: str = ""
     unary_args: t.Any = None
-    _unknown: t.Any = None
 
     def __init__(self, *args):
+        self.raw = args
         self._resolved_value = None
         if not len(args):
             return
         self.exp_type = args[0]
         self.ts = typespec(*args[1])
         self.rank = int(args[2])
 
         if self.exp_type == "OP":
             self._value = None
             self.unary_op = args[3]
             self.unary_args = [expression(*args[4]), expression(*args[5])]
-            try:
-                self._unknown = args[6]  # What is this for?
-            except IndexError:
-                pass
         elif self.exp_type == "FUNCTION":
             self._value = symbol_ref(args[3])
         elif self.exp_type == "CONSTANT":
             if self.ts.type == "REAL":
                 self._value = hextofloat(string_clean(args[3]), self.ts.kind == 8)
             elif self.ts.type == "INTEGER":
                 self._value = int(string_clean(args[3]))
@@ -561,14 +590,19 @@
         elif self.exp_type == "COMPCALL":
             raise NotImplementedError(args)
         elif self.exp_type == "PPC":
             raise NotImplementedError(args)
         else:
             raise AttributeError(f"Can't match {self.exp_type}")
 
+        try:
+            self.arglist = actual_arglist(*args[6])
+        except IndexError:
+            self.arglist = []
+
     @property
     def value(self):
         if self._resolved_value is not None:
             return self._resolved_value
         else:
             return self._value
 
@@ -582,14 +616,15 @@
     rank: int = -1
     corank: int = -1
     array_type: str = ""
     lower: t.List[expression] = None
     upper: t.List[expression] = None
 
     def __init__(self, *args):
+        self.raw = args
         if not len(args):
             return
 
         self.rank = int(args[0])
         self.corank = int(args[1])
         self.array_type = args[2]
         self.lower = []
@@ -634,14 +669,15 @@
     actual_arg: actual_arglist = None
     attr: attribute = None
     access: str = ""
     initializer: expression = None
     proc_ptr: typebound_proc = None
 
     def __init__(self, *args):
+        self.raw = args
         args = list(args)
 
         self.id = int(args[0])
         self.name = string_clean(args[1])
         self.ts = typespec(*args[2])
         self.array_spec = arrayspec(*args[3])
         if len(args[4]):
@@ -668,39 +704,42 @@
     comp: t.List[component] = None
 
     def __init__(self, *args):
         self.comp = []
         for i in args:
             self.comp.append(component(*i))
 
+        self.raw = args
+
     def __len__(self):
         return len(self.comp)
 
     def __iter__(self):
         return iter(self.comp)
 
 
 @dataclass(init=False)
 class namelist:
     sym_ref: t.List[symbol_ref] = None
 
     def __init__(self, *args):
+        self.raw = args
         self.sym_ref = []
         if len(args):
             for i in args:
                 self.sym_ref.append(symbol_ref(i))
 
 
 @dataclass(init=False)
 class simd_dec:
     args: None
     kwargs: None
 
     def __init__(self, *args, **kwargs):
-        self.args = args
+        self.raw = args
         self.kwargs = kwargs
 
 
 @dataclass(init=False)
 class data:
     attr: attribute
     comp: components = None
@@ -718,14 +757,15 @@
     nml: namelist = None
     intrinsic: int = -1
     intrinsic_symbol: int = -1
     hash: int = -1
     simd: simd_dec = None
 
     def __init__(self, *args):
+        self.raw = args
         args = list(
             args
         )  # Do it this was as there are optional terms we may need to pop
         self.attr = attribute(*args[0])
         self.comp = components(*args[1])
 
         if isinstance(args[2], str):
@@ -819,15 +859,15 @@
 
         return result
 
     def proc_common(self, data):
         result = {}
         for i in data:
             d = c_item(*i)
-            result[d.id] = d
+            result[d.name] = d
         return result
 
     def proc_generics(self, data):
         result = {}
         for i in data:
             d = generics(*i)
             result[d.name] = d
```

### Comparing `gfort2py-2.1.0/gfort2py/utils.py` & `gfort2py-2.2.0/gfort2py/utils.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/gfort2py.egg-info/PKG-INFO` & `gfort2py-2.2.0/gfort2py.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfort2py
-Version: 2.1.0
+Version: 2.2.0
 Summary: "Python bindings for Fortran"
 Home-page: https://github.com/rjfarmer/gfort2py
 Author: Robert Farmer
 Author-email: robert.j.farmer37@gmail.com
 License: GPLv2+
 Platform: unix
 Platform: linux
@@ -62,35 +62,34 @@
 ## Using
 ### Fortran side
 Your Fortran code must be inside a module and then compiled as a shared library.
 
 On linux: 
 ````bash
 gfortran -fPIC -shared -c file.f90
-gfortran -fPIC -shared -o libfile file.f90
+gfortran -fPIC -shared -o libfile.so file.f90
 ````
 
 On MacOS: 
 ````bash
 gfortran -dynamiclib -c file.f90
-gfortran -dynamiclib -o libfile file.f90
+gfortran -dynamiclib -o libfile.dylib file.f90
 ````
 
 On Windows:
 ````bash
 gfortran -shared -c file.f90
 gfortran -shared -o libfile.dll file.f90
 ````
 
 If your code comes as program that does everything, then just turn the program into a function call inside a module,
 then create a new file with your program that uses the module and calls the function you just made.
 
 If the shared library needs other
-shared libraries you will need to set LD_LIBRARY_PATH environment variable, and it is also recommended is to run chrpath on the 
-shared libraries so you can access them from anywhere.
+shared libraries you will need to set LD_LIBRARY_PATH environment variable, and it is also recommended to run chrpath on the shared libraries so you can access them from anywhere.
 
 ### Python side
 ````python
 
 import gfort2py as gf
 
 SHARED_LIB_NAME=f'./test_mod.{gf.lib_ext()}' # Handle whether on Linux or Mac
@@ -105,15 +104,15 @@
 ### Functions
 ````python
 y = x.func_name(a,b,c)
 ````
 
 Will call the Fortran function with variables ``a,b,c`` and returns the result in ``y``.
 
-``y`` will be  named tuple which contains (result, args). Where result is a python object for the return value (0 if a subroutine) and where args is a dict containing all arguments passed to the procedure (both those with intent (in) which will be unchanged and intent(inout/out) which may have changed).
+``y`` will be  named tuple which contains (result, args). Where ``result`` is a python object for the return value (0 if a subroutine) and where args is a dict containing all arguments passed to the procedure (both those with intent (in) which will be unchanged and intent(inout/out) which may have changed).
 
 
 ### Variables
 
 ````python
 x.some_var = 1
 ````
@@ -331,15 +330,15 @@
 x.func_ptr = x.func_arg # With the function itself
 ```` -->
 
 ## Accessing module file data
 
 For those wanting to explore the module file format, there is a routine ``mod_info`` available from the top-level ``gfort2py`` module:
 
-````
+````python
 module = gf.mod_info('file.mod')
 ````
 
 That will parse the mod file and convert it into an intermediate format inside ``module``.
 
 Variables or procedures can be looked up via the item interface (I also recommend using pprint for easier viewing):
 
@@ -357,10 +356,92 @@
 
 For those wanting to get more involved, adding Fortran examples to the test suite of currently untested or unsupported features would be helpful. Bonus points if you also provide a Python test case (that can be marked ``@pytest.mark.skip`` if it does not work) that demonstrates the proposed interface to the new Fortran feature. Features with test cases will move higher in the order of things I add to the code.
 
 See [how to write a test case](tests/README.md) for details on how to write test cases.
 
 For those wanting to go further and add the new feature themselves open a bug report and we can chat about what needs doing.
 
+## Debugging
+
+For those wanting to dig further into ``gfort2py``.
+
+Assuming that you loaded things as:
+
+````python
+x = gf.fFort(SO, MOD)
+````
+
+You can find out the available Fortran variables/procedures module information with:
+
+````python
+var = x._module['variable_name']
+````
+
+### Variables
+
+For variables you can create a ``fVar`` (the object that handles converting too and from Python to Fortran) with:
 
+````python
+fvar = gf.fVar.fVar(var,x._module)
+````
+
+Note that at this point the ``fvar`` has no idea where to look for the variable. If you want to access its value in a module then
+
+````python
+fvar.in_dll(x._lib)
+print(fvar.value)
+````
+
+and you can then set the value (after calling ``in_dll``) with:
 
+````python
+fvar.value = value
+````
+
+### Procedures
 
+For a procedure you can do:
+
+````python
+proc = x._module['procedure_name']
+````
+
+and its Fortran object is:
+
+````python
+fproc = gf.fProc.fProc(x._lib,proc,x._module)
+````
+
+Calling the procedure is then:
+
+````python
+fproc(*args,**kwargs)
+````
+
+To access the arguments of a procedure then:
+
+````python
+args = [x._module[i.ref] for i in proc.args().symbol]
+````
+
+The return value of a function is accessed via:
+
+````python
+return_arg = x._module[proc.return_arg()]
+````
+
+### Derived types
+
+To access a derived type (the type definition not an instance of the type)
+
+````python
+dt_type = x._module['Derived_name']
+````
+
+Note the capitalization, derived types start with a capital.
+
+Similar to a variable, to access an instance of a derived type variable its:
+
+````python
+dt_var = x._module['dt_variable_name']
+dt_fvar = gf.fVar.fVar(dt_var,x._module)
+````
```

### Comparing `gfort2py-2.1.0/gfort2py.egg-info/SOURCES.txt` & `gfort2py-2.2.0/gfort2py.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -10,27 +10,21 @@
 pyproject.toml
 requirements.txt
 requirements_dev.txt
 setup.cfg
 setup.py
 tox.ini
 .github/dependabot.yml
+.github/ISSUE_TEMPLATE/bug_report.md
+.github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/ci-mac.yml
 .github/workflows/ci-old.yml
 .github/workflows/ci.yml
 .github/workflows/coveralls.yml
 .github/workflows/pypi.yml
-docs/Makefile
-docs/make.bat
-docs/source/conf.py
-docs/source/fortranabi.rst
-docs/source/index.rst
-docs/source/mod_files.rst
-docs/source/testsuite.rst
-docs/source/usage.rst
 gfort2py/__init__.py
 gfort2py/fArrays.py
 gfort2py/fDT.py
 gfort2py/fParameters.py
 gfort2py/fProc.py
 gfort2py/fProcPtr.py
 gfort2py/fScalars.py
@@ -50,32 +44,41 @@
 gfort2py.egg-info/top_level.txt
 tests/Makefile
 tests/README.md
 tests/__init__.py
 tests/basic.f90
 tests/basic_test.py
 tests/common.f90
+tests/common.py
 tests/complex.f90
 tests/complex_test.py
 tests/conftest.py
 tests/dt.f90
 tests/dt_test.py
 tests/dummy_arrays.f90
 tests/dummy_arrays_test.py
 tests/elemental.f90
 tests/explicit_arrays.f90
 tests/explicit_arrays_test.py
 tests/interface.f90
+tests/kinds_check.f90
 tests/namelist.f90
 tests/oo.f90
 tests/oo_test.py
 tests/pdt.f90
 tests/pdt_test.py
 tests/pointers.f90
 tests/pointers_test.py
 tests/proc_ptrs.f90
 tests/proc_ptrs_test.py
 tests/strings.f90
 tests/strings_test.py
 tests/submodule.f90
+tests/t_params_modules.f90
+tests/t_params_modules_test.py
+tests/t_vars_modules.f90
+tests/t_vars_modules_test.py
 tests/template._f90
-tests/test_template.py
+tests/test_template.py
+tests/templates/module_params.py
+tests/templates/module_variables.py
+tests/templates/utils.py
```

### Comparing `gfort2py-2.1.0/setup.cfg` & `gfort2py-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/tests/Makefile` & `gfort2py-2.2.0/tests/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 .PHONY = all clean
 
 FC = gfortran
 
-OPTIONS=-ggdb -fdump-tree-all -D_FORTIFY_SOURCE=2 -fstack-clash-protection -fstack-protector-all -fstack-protector
+OPTIONS=-ggdb -fdump-tree-original -D_FORTIFY_SOURCE=2 -ffree-line-length-none  -ffree-form -fstack-clash-protection -fstack-protector-all -fstack-protector
 
 SRCS = $(wildcard *.f90)
 MODS =  $(wildcard *.mod)
 
 GZ = $(patsubst %.mod,%.gz,$(MODS))
 
 UNAME_S := $(shell uname -s)
@@ -25,20 +25,31 @@
    LIB_SUFFIX = dylib
    LIBS = $(patsubst %.f90,%.dylib,$(SRCS))
 else
 $(error Unknown OS)
 endif
 
 
-all: $(LIBS) $(GZ)
+all: $(LIBS) $(GZ) kinds
 
 
 %.$(LIB_SUFFIX): %.f90
 	$(FC) $(OPTIONS) $(LIB_FLAGS) -o  $@ $<
 
 %.gz: %.mod
 	@cp $< $@
 	@gunzip -f $@ -c > $@.extract
 	@rm $@
 
+%.o : %.mod
+
+%.mod : %.o
+	@true
+
+%.o : %.f90
+	$(FC) $(OPTIONS) $(LIB_FLAGS) -o  $@ $<
+
+kinds: kinds_check.o
+	$(FC) -o kinds kinds_check.f90
+
 clean:
 	-rm -f *.o *.mod *.gz *.pyc *.f90.*.* *.$(LIB_SUFFIX) *.original *.extract *.smod *.fpy
```

### Comparing `gfort2py-2.1.0/tests/README.md` & `gfort2py-2.2.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `gfort2py-2.1.0/tests/basic.f90` & `gfort2py-2.2.0/tests/basic.f90`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	use basic2
 
 	implicit none
 	
 	     ! Parameters
 		integer, parameter :: dp = selected_real_kind(p=15)
 		integer, parameter :: qp = selected_real_kind(p=30)
-		integer, parameter :: lp = selected_int_kind(8)
+		integer, parameter :: lp = selected_int_kind(16)
 		
 		integer, parameter      :: const_int=1
 		integer, parameter      :: const_int_p1=const_int+1
 		integer(lp), parameter  :: const_int_lp=1_lp
 
 		logical,parameter :: const_logical_true=.true.
 		logical,parameter :: const_logical_false=.false.
```

### Comparing `gfort2py-2.1.0/tests/basic_test.py` & `gfort2py-2.2.0/tests/basic_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: GPL-2.0+
 
 import os, sys
 import ctypes
+from pprint import pprint
 
 os.environ["_GFORT2PY_TEST_FLAG"] = "1"
 
 import numpy as np
 import gfort2py as gf
 
 import pytest
@@ -16,18 +17,35 @@
 x = gf.fFort(SO, MOD)
 
 
 class TestBasicMethods:
     def assertEqual(self, x, y):
         assert x == y
 
+    def test_version(self):
+        assert gf.__version__
+
+    def test_mod_info(self):
+        assert len(gf.mod_info(MOD).keys())
+
+    def test_doc(self):
+        assert x.__doc__ == f"MODULE={MOD}"
+
+    def test_str(self):
+        assert str(x) == MOD
+
     def test_mising_var(self):
         with pytest.raises(AttributeError) as cm:
             a = x.invalid_var
 
+    def test_lookups(self):
+        assert len(x.keys())
+        assert "a_int" in x
+        assert len(dir(x))
+
     def test_a_int(self):
         v = 1
         x.a_int = v
         self.assertEqual(x.a_int, v)
 
     def test_a_int_str(self):
         with pytest.raises(TypeError) as cm:
@@ -72,14 +90,19 @@
     def test_sub_alter_mod(self):
         y = x.sub_alter_mod()
         self.assertEqual(x.a_int, 99)
         self.assertEqual(x.a_int_lp, 99)
         self.assertEqual(x.a_real, 99.0)
         self.assertEqual(x.a_real_dp, 99.0)
 
+    def test_int_lp(self):
+        x.a_int_lp = 5
+        assert x.a_int_lp == 5
+        assert x.a_int_lp_set == 6
+
     @pytest.mark.skip("Skipping due to quad support")
     def test_sub_alter_mod_qp(self):
         y = x.sub_alter_mod()
         self.assertEqual(x.a_real_qp, 99.0)
 
     def test_func_int_in(self):
         v = 5
```

### Comparing `gfort2py-2.1.0/tests/common.f90` & `gfort2py-2.2.0/tests/common.f90`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	use iso_fortran_env, only: output_unit, real128
 	
 	implicit none
 	
 	! Parameters
 	integer, parameter :: dp = selected_real_kind(p=15)
 	integer, parameter :: qp = selected_real_kind(p=30)
-	integer, parameter :: lp = selected_int_kind(8)
+	integer, parameter :: lp = selected_int_kind(16)
 	
 	
 	integer :: x_int, y_int, z_int
 	common  x_int, y_int, z_int
 	
 	integer :: x_int1, y_int1, z_int1
 	common  /com_mod/ x_int1, y_int1, z_int1
```

### Comparing `gfort2py-2.1.0/tests/complex.f90` & `gfort2py-2.2.0/tests/complex.f90`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 	implicit none
 	
 		! Parameters
 		integer, parameter :: dp = selected_real_kind(p=15)
 		integer, parameter :: qp = selected_real_kind(p=30)
-		integer, parameter :: lp = selected_int_kind(8)
+		integer, parameter :: lp = selected_int_kind(16)
 		
 		
 		complex, parameter         :: const_cmplx=(1.0,1.0)
 		complex(dp), parameter  :: const_cmplx_dp=(1.0_dp,1.0_dp)
 		complex(qp), parameter  :: const_cmplx_qp=(1.0_qp,1.0_qp)
```

### Comparing `gfort2py-2.1.0/tests/complex_test.py` & `gfort2py-2.2.0/tests/complex_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: GPL-2.0+
 
 import os, sys
 import ctypes
+from pprint import pprint
 
 os.environ["_GFORT2PY_TEST_FLAG"] = "1"
 
 import numpy as np
 import gfort2py as gf
 
 import pytest
```

### Comparing `gfort2py-2.1.0/tests/dt.f90` & `gfort2py-2.2.0/tests/dt.f90`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     use iso_fortran_env, only: output_unit, real128
     
     implicit none
     
     ! Parameters
     integer, parameter :: dp = selected_real_kind(p=15)
     integer, parameter :: qp = selected_real_kind(p=30)
-    integer, parameter :: lp = selected_int_kind(8)
+    integer, parameter :: lp = selected_int_kind(16)
     
     
     TYPE s_struct_basic
         integer           :: a_int
         integer(lp)       :: a_int_lp
         real              :: a_real
         real(dp)          :: a_real_dp
```

### Comparing `gfort2py-2.1.0/tests/dt_test.py` & `gfort2py-2.2.0/tests/dt_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: GPL-2.0+
 
 import os, sys
 import ctypes
+from pprint import pprint
 
 os.environ["_GFORT2PY_TEST_FLAG"] = "1"
 
 import numpy as np
 import gfort2py as gf
 
 import pytest
@@ -87,30 +88,30 @@
         self.assertEqual(x.f_struct["a_int"], 5)
         self.assertEqual(x.f_struct["a_int_lp"], 6)
         self.assertEqual(x.f_struct["a_real"], 7.0)
         self.assertEqual(x.f_struct["a_real_dp"], 8.0)
         self.assertEqual(x.f_struct["a_str"], "9999999999")
 
         v = np.array([9, 10, 11, 12, 13], dtype="int32")
-        np.testing.assert_array_equal(x.f_struct["b_int_exp_1d"], v)
+        assert np.array_equal(x.f_struct["b_int_exp_1d"], v)
 
         v = np.array([9, 10, 11, 12, 13], dtype="int32")
-        np.testing.assert_array_equal(x.e_int_target_1d, v)
+        assert np.array_equal(x.e_int_target_1d, v)
 
     def test_func_set_f_struct_array_alloc(self):
         y = x.func_set_f_struct()
 
         v = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10], dtype="int32")
-        np.testing.assert_array_equal(x.f_struct["c_int_alloc_1d"], v)
+        assert np.array_equal(x.f_struct["c_int_alloc_1d"], v)
 
     def test_func_set_f_struct_array_ptr(self):
         y = x.func_set_f_struct()
 
         v = np.array([9, 10, 11, 12, 13], dtype="int32")
-        np.testing.assert_array_equal(x.f_struct["d_int_point_1d"], v)
+        assert np.array_equal(x.f_struct["d_int_point_1d"], v)
 
     # @pytest.mark.skip
     def test_recur_dt(self):  # Skip for now
         with pytest.raises(NotImplementedError) as cm:
             x.r_recur["a_int"] = 9
             self.assertEqual(x.r_recur["a_int"], 9)
             x.r_recur["s_recur"]["a_int"] = 9
@@ -152,20 +153,16 @@
         y = x.sub_struct_exp_1d({})
 
         s = y.args["x"]
 
         self.assertEqual(s[0]["a_int"], 5)
         self.assertEqual(s[1]["a_int"], 9)
 
-        np.testing.assert_array_equal(
-            s[0]["b_int_exp_1d"], np.array([66, 66, 66, 66, 66])
-        )
-        np.testing.assert_array_equal(
-            s[1]["b_int_exp_1d"], np.array([77, 77, 77, 77, 77])
-        )
+        assert np.array_equal(s[0]["b_int_exp_1d"], np.array([66, 66, 66, 66, 66]))
+        assert np.array_equal(s[1]["b_int_exp_1d"], np.array([77, 77, 77, 77, 77]))
 
     def test_fvar_as_arg(self, capfd):
         y = x.f_struct_simple
         y["x"] = 99
         y["y"] = 98
 
         z = x.sub_f_simple_in(y)
```

### Comparing `gfort2py-2.1.0/tests/dummy_arrays.f90` & `gfort2py-2.2.0/tests/dummy_arrays.f90`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	use iso_fortran_env, only: output_unit, real128
 	
 	implicit none
 	
 	! Parameters
 	integer, parameter :: dp = selected_real_kind(p=15)
 	integer, parameter :: qp = selected_real_kind(p=30)
-	integer, parameter :: lp = selected_int_kind(8)
+	integer, parameter :: lp = selected_int_kind(16)
 	
 	integer, allocatable, dimension(:) :: c_int_alloc_1d
 	integer, allocatable, dimension(:,:) :: c_int_alloc_2d
 	integer, allocatable, dimension(:,:,:) :: c_int_alloc_3d
 	integer, allocatable, dimension(:,:,:,:) :: c_int_alloc_4d
 	integer, allocatable, dimension(:,:,:,:,:) :: c_int_alloc_5d
```

### Comparing `gfort2py-2.1.0/tests/dummy_arrays_test.py` & `gfort2py-2.2.0/tests/dummy_arrays_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: GPL-2.0+
 
 import os, sys
 import ctypes
+from pprint import pprint
 
 os.environ["_GFORT2PY_TEST_FLAG"] = "1"
 
 import numpy as np
 import gfort2py as gf
 
 import pytest
@@ -35,255 +36,255 @@
         self.assertEqual(np.sum(x.c_int_alloc_1d), 5)
 
     def test_c_int_alloc_1d(self):
         y = x.sub_alloc_int_1d_cleanup()
         y = x.sub_alloc_int_1d_arrs()
         v = np.zeros([5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_int_alloc_1d, v)
+        assert np.array_equal(x.c_int_alloc_1d, v)
 
     def test_c_int_alloc_2d(self):
         y = x.sub_alloc_int_1d_cleanup()
         y = x.sub_alloc_int_1d_arrs()
         v = np.zeros([5, 5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_int_alloc_2d, v)
+        assert np.array_equal(x.c_int_alloc_2d, v)
 
     def test_c_int_alloc_3d(self):
         y = x.sub_alloc_int_1d_cleanup()
         y = x.sub_alloc_int_1d_arrs()
         v = np.zeros([5, 5, 5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_int_alloc_3d, v)
+        assert np.array_equal(x.c_int_alloc_3d, v)
 
     def test_c_int_alloc_4d(self):
         y = x.sub_alloc_int_1d_cleanup()
         y = x.sub_alloc_int_1d_arrs()
         v = np.zeros([5, 5, 5, 5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_int_alloc_4d, v)
+        assert np.array_equal(x.c_int_alloc_4d, v)
 
     def test_c_int_alloc_5d(self):
         y = x.sub_alloc_int_1d_cleanup()
         y = x.sub_alloc_int_1d_arrs()
         v = np.zeros([5, 5, 5, 5, 5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_int_alloc_5d, v)
+        assert np.array_equal(x.c_int_alloc_5d, v)
 
     def test_c_int_alloc_1d_set(self):
         y = x.sub_alloc_int_1d_cleanup()
         y = x.sub_alloc_int_1d_arrs()
         v = np.zeros([5])
         v[:] = 5
         x.c_int_alloc_1d = v
-        np.testing.assert_array_equal(x.c_int_alloc_1d, v)
+        assert np.array_equal(x.c_int_alloc_1d, v)
         self.assertEqual(np.sum(x.c_int_alloc_1d), 25)
 
     def test_c_int_alloc_2d_set(self):
         y = x.sub_alloc_int_1d_cleanup()
         y = x.sub_alloc_int_1d_arrs()
         v = np.zeros([5, 5])
         v[:] = 5
         x.c_int_alloc_2d = v
-        np.testing.assert_array_equal(x.c_int_alloc_2d, v)
+        assert np.array_equal(x.c_int_alloc_2d, v)
 
     def test_c_int_alloc_3d_set(self):
         y = x.sub_alloc_int_1d_cleanup()
         y = x.sub_alloc_int_1d_arrs()
         v = np.zeros([5, 5, 5])
         v[:] = 5
         x.c_int_alloc_3d = v
-        np.testing.assert_array_equal(x.c_int_alloc_3d, v)
+        assert np.array_equal(x.c_int_alloc_3d, v)
 
     def test_c_int_alloc_4d_set(self):
         y = x.sub_alloc_int_1d_cleanup()
         y = x.sub_alloc_int_1d_arrs()
         v = np.zeros([5, 5, 5, 5])
         v[:] = 5
         x.c_int_alloc_4d = v
-        np.testing.assert_array_equal(x.c_int_alloc_4d, v)
+        assert np.array_equal(x.c_int_alloc_4d, v)
 
     @pytest.mark.skip
     def test_c_int_alloc_5d_set(self):
         y = x.sub_alloc_int_1d_cleanup()
         y = x.sub_alloc_int_1d_arrs()
         v = np.zeros([5, 5, 5, 5, 5])
         v[:] = 5
         x.c_int_alloc_5d = v
-        np.testing.assert_array_equal(x.c_int_alloc_5d, v)
+        assert np.array_equal(x.c_int_alloc_5d, v)
 
     @pytest.mark.skip
     def test_c_int_alloc_1d_large(self):
         # Can have issues exiting when using large (>255) arrays
         y = x.sub_alloc_int_1d_cleanup()
         y = x.sub_alloc_int_1d_arrs()
         v = np.zeros([256], dtype="int32")
         v[:] = 5
         x.c_int_alloc_1d = v
-        np.testing.assert_array_equal(x.c_int_alloc_1d, v)
+        assert np.array_equal(x.c_int_alloc_1d, v)
 
     def test_c_real_alloc_1d(self):
         y = x.sub_alloc_real_1d_cleanup()
         y = x.sub_alloc_real_1d_arrs()
         v = np.zeros([5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_real_alloc_1d, v)
+        assert np.array_equal(x.c_real_alloc_1d, v)
 
     def test_c_real_alloc_2d(self):
         y = x.sub_alloc_real_1d_cleanup()
         y = x.sub_alloc_real_1d_arrs()
         v = np.zeros([5, 5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_real_alloc_2d, v)
+        assert np.array_equal(x.c_real_alloc_2d, v)
 
     def test_c_real_alloc_3d(self):
         y = x.sub_alloc_real_1d_cleanup()
         y = x.sub_alloc_real_1d_arrs()
         v = np.zeros([5, 5, 5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_real_alloc_3d, v)
+        assert np.array_equal(x.c_real_alloc_3d, v)
 
     def test_c_real_alloc_4d(self):
         y = x.sub_alloc_real_1d_cleanup()
         y = x.sub_alloc_real_1d_arrs()
         v = np.zeros([5, 5, 5, 5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_real_alloc_4d, v)
+        assert np.array_equal(x.c_real_alloc_4d, v)
 
     def test_c_real_alloc_5d(self):
         y = x.sub_alloc_real_1d_cleanup()
         y = x.sub_alloc_real_1d_arrs()
         v = np.zeros([5, 5, 5, 5, 5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_real_alloc_5d, v)
+        assert np.array_equal(x.c_real_alloc_5d, v)
 
     def test_c_real_dp_alloc_1d_set(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5])
         v[:] = 2.0
         x.c_real_dp_alloc_1d = v
-        np.testing.assert_array_equal(x.c_real_dp_alloc_1d, v)
+        assert np.array_equal(x.c_real_dp_alloc_1d, v)
 
     def test_c_real_dp_alloc_2d_set(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5, 5])
         v[:] = 2.0
         x.c_real_dp_alloc_2d = v
-        np.testing.assert_array_equal(x.c_real_dp_alloc_2d, v)
+        assert np.array_equal(x.c_real_dp_alloc_2d, v)
 
     def test_c_real_dp_alloc_3d_set(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5, 5, 5])
         v[:] = 2.0
         x.c_real_dp_alloc_3d = v
-        np.testing.assert_array_equal(x.c_real_dp_alloc_3d, v)
+        assert np.array_equal(x.c_real_dp_alloc_3d, v)
 
     def test_c_real_dp_alloc_4d_set(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5, 5, 5, 5])
         v[:] = 2.0
         x.c_real_dp_alloc_4d = v
-        np.testing.assert_array_equal(x.c_real_dp_alloc_4d, v)
+        assert np.array_equal(x.c_real_dp_alloc_4d, v)
 
     @pytest.mark.skip
     def test_c_real_dp_alloc_5d_set(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5, 5, 5, 5, 5])
         v[:] = 2.0
         x.c_real_dp_alloc_5d = v
-        np.testing.assert_array_equal(x.c_real_dp_alloc_5d, v)
+        assert np.array_equal(x.c_real_dp_alloc_5d, v)
 
     def test_c_real_dp_alloc_1d(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_real_dp_alloc_1d, v)
+        assert np.array_equal(x.c_real_dp_alloc_1d, v)
 
     def test_c_real_dp_alloc_2d(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5, 5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_real_dp_alloc_2d, v)
+        assert np.array_equal(x.c_real_dp_alloc_2d, v)
 
     def test_c_real_dp_alloc_3d(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5, 5, 5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_real_dp_alloc_3d, v)
+        assert np.array_equal(x.c_real_dp_alloc_3d, v)
 
     def test_c_real_dp_alloc_4d(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5, 5, 5, 5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_real_dp_alloc_4d, v)
+        assert np.array_equal(x.c_real_dp_alloc_4d, v)
 
     def test_c_real_dp_alloc_5d(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5, 5, 5, 5, 5])
         v[:] = 1
-        np.testing.assert_array_equal(x.c_real_dp_alloc_5d, v)
+        assert np.array_equal(x.c_real_dp_alloc_5d, v)
 
     def test_c_real_dp_alloc_1d_set(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5])
         v[:] = 2.0
         x.c_real_dp_alloc_1d = v
-        np.testing.assert_array_equal(x.c_real_dp_alloc_1d, v)
+        assert np.array_equal(x.c_real_dp_alloc_1d, v)
 
     def test_c_real_dp_alloc_2d_set(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5, 5])
         v[:] = 2.0
         x.c_real_dp_alloc_2d = v
-        np.testing.assert_array_equal(x.c_real_dp_alloc_2d, v)
+        assert np.array_equal(x.c_real_dp_alloc_2d, v)
 
     def test_c_real_dp_alloc_3d_set(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5, 5, 5])
         v[:] = 2.0
         x.c_real_dp_alloc_3d = v
-        np.testing.assert_array_equal(x.c_real_dp_alloc_3d, v)
+        assert np.array_equal(x.c_real_dp_alloc_3d, v)
 
     @pytest.mark.skip
     def test_c_real_dp_alloc_4d_set(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5, 5, 5, 5])
         v[:] = 2.0
         x.c_real_dp_alloc_4d = v
-        np.testing.assert_array_equal(x.c_real_dp_alloc_4d, v)
+        assert np.array_equal(x.c_real_dp_alloc_4d, v)
 
     @pytest.mark.skip
     def test_c_real_dp_alloc_5d_set(self):
         y = x.sub_alloc_real_dp_1d_cleanup()
         y = x.sub_alloc_real_dp_1d_arrs()
         v = np.zeros([5, 5, 5, 5, 5])
         v[:] = 2.0
         x.c_real_dp_alloc_5d = v
-        np.testing.assert_array_equal(x.c_real_dp_alloc_5d, v)
+        assert np.array_equal(x.c_real_dp_alloc_5d, v)
 
     def test_func_assumed_shape_arr_1d(self):
         v = np.zeros([5], dtype="int32")
         v[0] = 2.0
         y = x.func_assumed_shape_arr_1d(v)
         self.assertEqual(y.result, True)
-        np.testing.assert_array_equal(y.args["x"], np.array([9, 9, 9, 9, 9]))
+        assert np.array_equal(y.args["x"], np.array([9, 9, 9, 9, 9]))
 
     def test_func_assumed_shape_arr_2d(self):
         v = np.zeros([5, 5], dtype="int32")
         v[1, 0] = 2.0
         y = x.func_assumed_shape_arr_2d(v)
         self.assertEqual(y.result, True)
 
@@ -323,15 +324,15 @@
         y = x.func_assumed_size_arr_real_dp_1d(v)
         self.assertEqual(y.result, True)
 
     def test_sub_alloc_arr_1d(self):
         y = x.sub_alloc_arr_1d(None)
         vTest = np.zeros(10)
         vTest[:] = 10
-        np.testing.assert_array_equal(y.args["x"], vTest)
+        assert np.array_equal(y.args["x"], vTest)
 
     def test_logical_arr(self):
         xarr = np.zeros(10)
         x2arr = np.zeros(10)
         x2arr[:] = False
         xarr[:] = True
 
@@ -342,49 +343,49 @@
 
     def test_sub_arr_assumed_rank_int_1d(self, capfd):
         v = np.arange(10, 15)
         o = " ".join([str(i) for i in v.flatten(order="F")])
 
         y = x.sub_arr_assumed_rank_int_1d(v)
         out, err = capfd.readouterr()
-        np.testing.assert_array_equal(y.args["zzz"], np.array([100] * 5))
+        assert np.array_equal(y.args["zzz"], np.array([100] * 5))
 
     def test_sub_arr_assumed_rank_real_1d(self, capfd):
         v = np.arange(10.0, 15.0)
         o = " ".join([str(i) for i in v.flatten(order="F")])
 
         y = x.sub_arr_assumed_rank_real_1d(v)
         out, err = capfd.readouterr()
-        np.testing.assert_array_equal(y.args["zzz"], np.array([100.0] * 5))
+        assert np.array_equal(y.args["zzz"], np.array([100.0] * 5))
 
     def test_sub_arr_assumed_rank_dp_1d(self, capfd):
         v = np.arange(10.0, 15.0)
         o = " ".join([str(i) for i in v.flatten(order="F")])
 
         y = x.sub_arr_assumed_rank_dp_1d(v)
         out, err = capfd.readouterr()
-        np.testing.assert_array_equal(y.args["zzz"], np.array([100.0] * 5))
+        assert np.array_equal(y.args["zzz"], np.array([100.0] * 5))
 
     @pytest.mark.skip
     def test_sub_check_alloc_int_2d(self):
         arr_test = np.zeros((3, 4), dtype=np.int32, order="F")
         y = x.sub_check_alloc_int_2d(None)
         y2 = x.sub_check_alloc_int_2d(arr_test)
-        np.testing.assert_array_equal(y.args["x"], y2.args["x"])
+        assert np.array_equal(y.args["x"], y2.args["x"])
 
         z = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]])
 
-        np.testing.assert_array_equal(y.args["x"], z)
+        assert np.array_equal(y.args["x"], z)
 
     @pytest.mark.skip
     def test_sub_check_alloc_int_3d(self):
         arr_test = np.zeros((3, 4, 5), dtype=np.int32, order="F")
         y = x.sub_check_alloc_int_3d(None)
         y2 = x.sub_check_alloc_int_3d(arr_test)
-        np.testing.assert_array_equal(y.args["x"], y2.args["x"])
+        assert np.array_equal(y.args["x"], y2.args["x"])
 
         z = np.array(
             [
                 [
                     [1, 2, 3, 4, 5],
                     [5, 6, 7, 8, 9],
                     [9, 10, 11, 12, 13],
@@ -401,8 +402,8 @@
                     [13, 14, 15, 16, 17],
                     [17, 18, 19, 20, 21],
                     [21, 22, 23, 24, 25],
                 ],
             ]
         )
 
-        np.testing.assert_array_equal(y.args["x"], z)
+        assert np.array_equal(y.args["x"], z)
```

### Comparing `gfort2py-2.1.0/tests/elemental.f90` & `gfort2py-2.2.0/tests/elemental.f90`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	use iso_fortran_env, only: output_unit, real128
 	
 	implicit none
 	
 	! Parameters
 	integer, parameter :: dp = selected_real_kind(p=15)
 	integer, parameter :: qp = selected_real_kind(p=30)
-	integer, parameter :: lp = selected_int_kind(8)
+	integer, parameter :: lp = selected_int_kind(16)
 	
 	
 	contains
 
 
 	elemental integer function ele_func_1(x)
 		integer,intent(in) :: x
```

### Comparing `gfort2py-2.1.0/tests/explicit_arrays.f90` & `gfort2py-2.2.0/tests/explicit_arrays.f90`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	use iso_fortran_env, only: output_unit, real128
 	
 	implicit none
 	
 	! Parameters
 	integer, parameter :: dp = selected_real_kind(p=15)
 	integer, parameter :: qp = selected_real_kind(p=30)
-	integer, parameter :: lp = selected_int_kind(8)
+	integer, parameter :: lp = selected_int_kind(16)
 	
 	
 	integer,parameter,dimension(10) :: const_int_arr=(/1,2,3,4,5,6,7,8,9,0/)
 	real,parameter,dimension(10) :: const_real_arr=(/1.0,2.0,3.0,4.0,5.0,6.0,7.0,8.0,9.0,0.0/)
 	real(dp),parameter,dimension(10) :: const_real_dp_arr=(/1_dp,2_dp,3_dp,4_dp,5_dp,6_dp,7_dp,8_dp,9_dp,0_dp/)
 	logical, parameter, dimension(5) :: const_logical_arr=(/.true.,.false.,.true.,.false.,.true./)
 
@@ -163,14 +163,26 @@
 		integer :: i
 		
 		do i=1,(N*2)+1
 			x(i) = i
 		end do
 		
 	end subroutine func_mesh_exp3
+
+
+	subroutine func_mesh_exp4(x,N) 
+		integer, intent(in) :: N
+		integer :: x((N+3)*2+1)
+		integer :: i
+		
+		do i=1,(N+3)*2+1
+			x(i) = i
+		end do
+		
+	end subroutine func_mesh_exp4
 	
 	
 	subroutine check_exp_2d_2m3(arr, success)
 		! Github issues #19
 		integer, dimension(2,3) :: arr
 		logical :: success
 		
@@ -198,10 +210,36 @@
 !			write(*,*) arr(i,:)
 !		end do
 		
 		arr(1,NT) = 5
 
 	end subroutine check_exp_2d_2m3_nt	
 	
-	
+
+
+	function func_return_1d_int_arr() result(x)
+		integer,dimension(5) :: x
+
+		x = (/1,2,3,4,5/)
+
+	end function func_return_1d_int_arr
+
+	function func_return_1d_int_arr_n(n) result(x)
+		integer, intent(in) :: n
+		integer,dimension(n) :: x
+		integer :: i
+
+		do i=1,n
+			x(i) = i
+		end do
+
+	end function func_return_1d_int_arr_n
+
+
+	function func_return_2d_int_arr() result(x)
+		integer,dimension(3,2) :: x
+
+		x = reshape((/1,2,3,4,5,6/), shape(x))
+
+	end function func_return_2d_int_arr
 
 end module explicit_arrays
```

### Comparing `gfort2py-2.1.0/tests/explicit_arrays_test.py` & `gfort2py-2.2.0/tests/explicit_arrays_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: GPL-2.0+
 
 import os, sys
 import ctypes
+from pprint import pprint
 
 os.environ["_GFORT2PY_TEST_FLAG"] = "1"
 
 import numpy as np
 import gfort2py as gf
 
 import pytest
@@ -21,54 +22,54 @@
         assert x == y
 
     def test_const_int_arr_error(self):
         with pytest.raises(AttributeError) as cm:
             x.const_int_arr = "abc"
 
     def test_const_int_arr(self):
-        np.testing.assert_array_equal(
+        assert np.array_equal(
             x.const_int_arr, np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 0], dtype="int32")
         )
 
     def test_const_real_arr(self):
-        np.testing.assert_array_equal(
+        assert np.array_equal(
             x.const_real_arr,
             np.array([1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 9.0, 0.0], dtype="float"),
         )
 
     def test_const_dp_arr(self):
-        np.testing.assert_array_equal(
+        assert np.array_equal(
             x.const_real_dp_arr,
             np.array([1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 9.0, 0.0], dtype="float"),
         )
 
     def test_b_int_exp_1d(self):
         v = np.random.randint(0, 100, size=(5))
         x.b_int_exp_1d = v
-        np.testing.assert_array_equal(x.b_int_exp_1d, v)
+        assert np.array_equal(x.b_int_exp_1d, v)
 
     def test_b_int_exp_2d(self):
         v = np.asfortranarray(np.random.randint(0, 100, size=(5, 5)), dtype="int32")
         x.b_int_exp_2d = v
-        np.testing.assert_array_equal(x.b_int_exp_2d, v)
+        assert np.array_equal(x.b_int_exp_2d, v)
 
     def test_b_int_exp_3d(self):
         v = np.random.randint(0, 100, size=(5, 5, 5))
         x.b_int_exp_3d = v
-        np.testing.assert_array_equal(x.b_int_exp_3d, v)
+        assert np.array_equal(x.b_int_exp_3d, v)
 
     def test_b_int_exp_4d(self):
         v = np.random.randint(0, 100, size=(5, 5, 5, 5))
         x.b_int_exp_4d = v
-        np.testing.assert_array_equal(x.b_int_exp_4d, v)
+        assert np.array_equal(x.b_int_exp_4d, v)
 
     def test_b_int_exp_5d(self):
         v = np.random.randint(0, 100, size=(5, 5, 5, 5, 5))
         x.b_int_exp_5d = v
-        np.testing.assert_array_equal(x.b_int_exp_5d, v)
+        assert np.array_equal(x.b_int_exp_5d, v)
 
     def test_b_real_exp_1d(self):
         v = np.random.random(size=(5))
         x.b_real_exp_1d = v
         np.testing.assert_allclose(x.b_real_exp_1d, v)
 
     def test_b_real_exp_2d(self):
@@ -234,15 +235,15 @@
 
     def test_sub_exp_inout(self, capfd):
         v = np.array([1, 2, 3, 4, 5])
 
         y = x.sub_exp_inout(v)
         out, err = capfd.readouterr()
 
-        np.testing.assert_array_equal(y.args["x"], 2 * v)
+        assert np.array_equal(y.args["x"], 2 * v)
 
     def test_sub_arr_exp_p(self, capfd):
         v = np.arange(0, 5)
         o = " ".join([str(i) for i in v.flatten(order="F")])
 
         y = x.sub_exp_array_int_1d(v)
         out, err = capfd.readouterr()
@@ -251,32 +252,37 @@
     def test_logical_arr_multi(self):
         xarr = np.zeros(5)
         xarr[:] = True
 
         y = x.func_logical_multi(1.0, 2.0, xarr, 3.0, 4.0)
         self.assertEqual(y.result, True)
 
-    @pytest.mark.skip
     def test_mesh_exp(self):
         # Github issue #13
         i = 5
         y = x.func_mesh_exp(i)
-        np.all(y.result == np.arrange(0, i + 1 + 1))
+        np.array_equal(y.result, np.arange(0, i + 1 + 1))
 
     def test_mesh_exp2(self):
         i = 5
         z = np.zeros(i + 1)
         y = x.func_mesh_exp2(z, i)
-        assert np.all(y.args["x"] == np.arange(1, i + 1 + 1))
+        assert np.array_equal(y.args["x"], np.arange(1, i + 1 + 1))
 
     def test_mesh_exp3(self):
         i = 5
         z = np.zeros((i * 2) + 1)
         y = x.func_mesh_exp3(z, i)
-        assert np.all(y.args["x"] == np.arange(1, (i * 2) + 1 + 1))
+        assert np.array_equal(y.args["x"], np.arange(1, (i * 2) + 1 + 1))
+
+    def test_mesh_exp4(self):
+        i = 5
+        z = np.zeros(((i + 3) * 2) + 1)
+        y = x.func_mesh_exp4(z, i)
+        assert np.array_equal(y.args["x"], np.arange(1, ((i + 3) * 2) + 1 + 1))
 
     def test_check_exp_2d_2m3(self):
         # Github issue #19
         arr_test = np.zeros((3, 4), dtype=int, order="F")
 
         arr_test[0, 1] = 1
         arr_test[1, 0] = 2
@@ -285,14 +291,27 @@
 
         y = x.check_exp_2d_2m3_nt(arr_test, 4, 0)
 
         self.assertEqual(y.args["success"], True)
 
         arr_test[0, 3] = 5
 
-        np.testing.assert_array_equal(y.args["arr"], arr_test)
+        assert np.array_equal(y.args["arr"], arr_test)
 
     def test_logical_param_array(self):
-        assert np.all(
-            x.const_logical_arr
-            == np.array([True, False, True, False, True], dtype=bool)
+        assert np.array_equal(
+            x.const_logical_arr, np.array([True, False, True, False, True], dtype=bool)
+        )
+
+    def test_func_return_1d_int_arr(self):
+        res = x.func_return_1d_int_arr()
+        assert np.array_equal(res.result, np.array([1, 2, 3, 4, 5]))
+
+    def test_func_return_1d_int_arr_n(self):
+        res = x.func_return_1d_int_arr_n(5)
+        assert np.array_equal(res.result, np.array([1, 2, 3, 4, 5]))
+
+    def test_func_return_2d_int_arr(self):
+        res = x.func_return_2d_int_arr()
+        assert np.array_equal(
+            res.result, np.array([1, 2, 3, 4, 5, 6]).reshape(3, 2, order="F")
         )
```

### Comparing `gfort2py-2.1.0/tests/interface.f90` & `gfort2py-2.2.0/tests/interface.f90`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	use iso_fortran_env, only: output_unit, real128
 	
 	implicit none
 	
 	! Parameters
 	integer, parameter :: dp = selected_real_kind(p=15)
 	integer, parameter :: qp = selected_real_kind(p=30)
-	integer, parameter :: lp = selected_int_kind(8)
+	integer, parameter :: lp = selected_int_kind(16)
 	
 	
 	interface convert
 		module procedure convert_int
 		module procedure convert_real
 		module procedure convert_real_dp
 		module procedure convert_str
```

### Comparing `gfort2py-2.1.0/tests/oo.f90` & `gfort2py-2.2.0/tests/oo.f90`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     use iso_fortran_env, only: output_unit, real128
     
     implicit none
     
     ! Parameters
     integer, parameter :: dp = selected_real_kind(p=15)
     integer, parameter :: qp = selected_real_kind(p=30)
-    integer, parameter :: lp = selected_int_kind(8)
+    integer, parameter :: lp = selected_int_kind(16)
     
     
     TYPE s_proc
         integer :: a_int
         
         contains
```

### Comparing `gfort2py-2.1.0/tests/pdt.f90` & `gfort2py-2.2.0/tests/pdt.f90`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 	
 	implicit none
 	
 	! Parameters
 	integer, parameter :: sp = selected_real_kind(p=8)
 	integer, parameter :: dp = selected_real_kind(p=15)
 	integer, parameter :: qp = selected_real_kind(p=30)
-	integer, parameter :: lp = selected_int_kind(8)
+	integer, parameter :: lp = selected_int_kind(16)
 	
 	
 	type pdt_def(k,a)
 		integer, kind :: k = sp 
 		integer, len :: a
 		real(k) :: array(a,a)
```

### Comparing `gfort2py-2.1.0/tests/pointers.f90` & `gfort2py-2.2.0/tests/pointers.f90`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	use iso_fortran_env, only: output_unit, real128
 	
 	implicit none
 	
 	! Parameters
 	integer, parameter :: dp = selected_real_kind(p=15)
 	integer, parameter :: qp = selected_real_kind(p=30)
-	integer, parameter :: lp = selected_int_kind(8)
+	integer, parameter :: lp = selected_int_kind(16)
 	
 	integer,pointer            :: a_int_point => null()
 	integer(lp),pointer        :: a_int_lp_point => null()
 	real,pointer               :: a_real_point => null()
 	real(dp),pointer           :: a_real_dp_point => null()
 	real(qp),pointer           :: a_real_qp_point => null()
 	character(len=10),pointer  :: a_str_point => null()
```

### Comparing `gfort2py-2.1.0/tests/pointers_test.py` & `gfort2py-2.2.0/tests/pointers_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: GPL-2.0+
 
 import os, sys
 import ctypes
+from pprint import pprint
 
 os.environ["_GFORT2PY_TEST_FLAG"] = "1"
 
 import numpy as np
 import gfort2py as gf
 
 import pytest
```

### Comparing `gfort2py-2.1.0/tests/proc_ptrs.f90` & `gfort2py-2.2.0/tests/proc_ptrs.f90`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     use iso_fortran_env, only: output_unit, real128
     
     implicit none
     
     ! Parameters
     integer, parameter :: dp = selected_real_kind(p=15)
     integer, parameter :: qp = selected_real_kind(p=30)
-    integer, parameter :: lp = selected_int_kind(8)
+    integer, parameter :: lp = selected_int_kind(16)
     
           
     procedure(func_func_run), pointer:: p_func_func_run_ptr => NULL()
     procedure(func_func_run), pointer:: p_func_func_run_ptr2 => func_func_run
     
     procedure(func_func_run_dp), pointer:: p_func_func_run_dp_ptr => NULL()
```

### Comparing `gfort2py-2.1.0/tests/proc_ptrs_test.py` & `gfort2py-2.2.0/tests/proc_ptrs_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: GPL-2.0+
 
 import os, sys
 import ctypes
+from pprint import pprint
 
 os.environ["_GFORT2PY_TEST_FLAG"] = "1"
 
 import numpy as np
 import gfort2py as gf
 
 import pytest
```

### Comparing `gfort2py-2.1.0/tests/strings.f90` & `gfort2py-2.2.0/tests/strings.f90`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	use iso_fortran_env, only: output_unit, real128
 	
 	implicit none
 	
 	! Parameters
 	integer, parameter :: dp = selected_real_kind(p=15)
 	integer, parameter :: qp = selected_real_kind(p=30)
-	integer, parameter :: lp = selected_int_kind(8)
+	integer, parameter :: lp = selected_int_kind(16)
 	
 	
 	character(len=10),parameter :: const_str='1234567890'
 	
 	character(len=10) :: a_str
 	character(len=10) :: a_str_set='abcdefghjk'
 	character(:), allocatable :: str_alloc
@@ -347,8 +347,14 @@
 		x%a_str2 = 'asdfghjkl;zx'
 
 		x% a_int = 99
 
 	end subroutine set_str_array_dt_out
 
 
+	subroutine set_chr_star_star(x)
+		character*(*), intent(out) :: x
+		x = "abcdefghijkl"
+	end subroutine set_chr_star_star
+
+
 end module strings
```

### Comparing `gfort2py-2.1.0/tests/strings_test.py` & `gfort2py-2.2.0/tests/strings_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: GPL-2.0+
 
 import os, sys
 import ctypes
+from pprint import pprint
 
 os.environ["_GFORT2PY_TEST_FLAG"] = "1"
 
 import numpy as np
 import gfort2py as gf
 
 import pytest
@@ -280,7 +281,11 @@
 
     def test_set_str_array_dt_out(self):
         res = x.set_str_array_dt_out({})
 
         assert res.args["x"]["a_str1"] == "qwertyuiop[]"
         assert res.args["x"]["a_str2"] == "asdfghjkl;zx"
         assert res.args["x"]["a_int"] == 99
+
+    def test_set_chr_star_star(self):
+        res = x.set_chr_star_star("            ")
+        assert res.args["x"] == "abcdefghijkl"
```

### Comparing `gfort2py-2.1.0/tests/submodule.f90` & `gfort2py-2.2.0/tests/submodule.f90`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	use iso_fortran_env, only: output_unit, real128
 	
 	implicit none
 	
 	! Parameters
 	integer, parameter :: dp = selected_real_kind(p=15)
 	integer, parameter :: qp = selected_real_kind(p=30)
-	integer, parameter :: lp = selected_int_kind(8)
+	integer, parameter :: lp = selected_int_kind(16)
 	
 	
 	interface 
 		module function func_smod(x,y) result(z)
 			real(dp), intent(in) :: x,y
 			real(dp) :: z
 		end function func_smod
```

