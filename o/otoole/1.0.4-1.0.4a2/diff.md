# Comparing `tmp/otoole-1.0.4.tar.gz` & `tmp/otoole-1.0.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otoole-1.0.4.tar", last modified: Mon Jul 10 09:04:09 2023, max compression
+gzip compressed data, was "otoole-1.0.4a2.tar", last modified: Mon Jul 10 09:02:19 2023, max compression
```

## Comparing `otoole-1.0.4.tar` & `otoole-1.0.4a2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.994553 otoole-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-10 09:03:57.000000 otoole-1.0.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.958553 otoole-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.962553 otoole-1.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-10 09:03:57.000000 otoole-1.0.4/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-10 09:03:57.000000 otoole-1.0.4/.github/ISSUE_TEMPLATE/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-10 09:03:57.000000 otoole-1.0.4/.github/ISSUE_TEMPLATE/feature.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 09:03:57.000000 otoole-1.0.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.962553 otoole-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-10 09:03:57.000000 otoole-1.0.4/.github/workflows/citation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-10 09:03:57.000000 otoole-1.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-10 09:03:57.000000 otoole-1.0.4/.github/workflows/python.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-10 09:03:57.000000 otoole-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-10 09:03:57.000000 otoole-1.0.4/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-10 09:03:57.000000 otoole-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-10 09:03:57.000000 otoole-1.0.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-10 09:03:57.000000 otoole-1.0.4/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-10 09:03:57.000000 otoole-1.0.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-10 09:03:57.000000 otoole-1.0.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-10 09:03:57.000000 otoole-1.0.4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-10 09:03:57.000000 otoole-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-10 09:04:08.994553 otoole-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-10 09:03:57.000000 otoole-1.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.966553 otoole-1.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.974553 otoole-1.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)   135029 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/_static/OSeMOSYS.png
--rw-r--r--   0 runner    (1001) docker     (123)    61672 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/_static/osemosys_dataflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/_static/otoole_figures.drawio
--rw-r--r--   0 runner    (1001) docker     (123)   178856 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/_static/overview.png
--rw-r--r--   0 runner    (1001) docker     (123)   168226 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/_static/overview_v2.png
--rw-r--r--   0 runner    (1001) docker     (123)    95949 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/_static/simplicity_res.png
--rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/_static/validataion_model.png
--rw-r--r--   0 runner    (1001) docker     (123)   217753 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/_static/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/functionality.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-10 09:03:57.000000 otoole-1.0.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-10 09:03:57.000000 otoole-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-10 09:03:57.000000 otoole-1.0.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.974553 otoole-1.0.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-10 09:03:57.000000 otoole-1.0.4/scripts/prepare_cbc.sh
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-10 09:03:57.000000 otoole-1.0.4/scripts/prepare_cbc_short.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-10 09:04:08.994553 otoole-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-10 09:03:57.000000 otoole-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.950553 otoole-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.978553 otoole-1.0.4/src/otoole/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18758 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.982553 otoole-1.0.4/src/otoole/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10703 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/preprocess/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/preprocess/longify_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/preprocess/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/preprocess/validate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/read_strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.982553 otoole-1.0.4/src/otoole/results/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32615 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/results/result_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/results/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/validate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.986553 otoole-1.0.4/src/otoole/visualise/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/visualise/res.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-07-10 09:03:57.000000 otoole-1.0.4/src/otoole/write_strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.982553 otoole-1.0.4/src/otoole.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-10 09:04:08.000000 otoole-1.0.4/src/otoole.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-10 09:04:08.000000 otoole-1.0.4/src/otoole.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:04:08.000000 otoole-1.0.4/src/otoole.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 09:04:08.000000 otoole-1.0.4/src/otoole.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:04:08.000000 otoole-1.0.4/src/otoole.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-10 09:04:08.000000 otoole-1.0.4/src/otoole.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 09:04:08.000000 otoole-1.0.4/src/otoole.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.990553 otoole-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.990553 otoole-1.0.4/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)   130205 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/fixtures/combined_inputs.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    10703 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/fixtures/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/fixtures/config_r.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.994553 otoole-1.0.4/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/fixtures/data/AccumulatedAnnualDemand.csv
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/fixtures/data/AvailabilityFactor.csv
--rw-r--r--   0 runner    (1001) docker     (123)    44422 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/fixtures/simplicity-v0.2.1.zip
--rw-r--r--   0 runner    (1001) docker     (123)    43735 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/fixtures/simplicity.txt
--rw-r--r--   0 runner    (1001) docker     (123)    75398 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/fixtures/simplicity.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:04:08.994553 otoole-1.0.4/tests/results/
--rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/results/test_results_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/test_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    41641 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/test_read_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/test_validate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/test_visualise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-07-10 09:03:57.000000 otoole-1.0.4/tests/test_write_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-10 09:03:57.000000 otoole-1.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.814081 otoole-1.0.4a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-10 09:02:03.000000 otoole-1.0.4a2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.794081 otoole-1.0.4a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.794081 otoole-1.0.4a2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-10 09:02:03.000000 otoole-1.0.4a2/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-10 09:02:03.000000 otoole-1.0.4a2/.github/ISSUE_TEMPLATE/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-10 09:02:03.000000 otoole-1.0.4a2/.github/ISSUE_TEMPLATE/feature.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 09:02:03.000000 otoole-1.0.4a2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.794081 otoole-1.0.4a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-10 09:02:03.000000 otoole-1.0.4a2/.github/workflows/citation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-10 09:02:03.000000 otoole-1.0.4a2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-10 09:02:03.000000 otoole-1.0.4a2/.github/workflows/python.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-10 09:02:03.000000 otoole-1.0.4a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-10 09:02:03.000000 otoole-1.0.4a2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-10 09:02:03.000000 otoole-1.0.4a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-10 09:02:03.000000 otoole-1.0.4a2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-10 09:02:03.000000 otoole-1.0.4a2/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-10 09:02:03.000000 otoole-1.0.4a2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-10 09:02:03.000000 otoole-1.0.4a2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-10 09:02:03.000000 otoole-1.0.4a2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-10 09:02:03.000000 otoole-1.0.4a2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-10 09:02:19.814081 otoole-1.0.4a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-10 09:02:03.000000 otoole-1.0.4a2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.798081 otoole-1.0.4a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.802080 otoole-1.0.4a2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   135029 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/_static/OSeMOSYS.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61672 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/_static/osemosys_dataflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/_static/otoole_figures.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)   178856 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/_static/overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)   168226 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/_static/overview_v2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    95949 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/_static/simplicity_res.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/_static/validataion_model.png
+-rw-r--r--   0 runner    (1001) docker     (123)   217753 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/_static/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/functionality.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-10 09:02:03.000000 otoole-1.0.4a2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-10 09:02:03.000000 otoole-1.0.4a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-10 09:02:03.000000 otoole-1.0.4a2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.802080 otoole-1.0.4a2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-10 09:02:03.000000 otoole-1.0.4a2/scripts/prepare_cbc.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-10 09:02:03.000000 otoole-1.0.4a2/scripts/prepare_cbc_short.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-10 09:02:19.814081 otoole-1.0.4a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-10 09:02:03.000000 otoole-1.0.4a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.790081 otoole-1.0.4a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.806080 otoole-1.0.4a2/src/otoole/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18758 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.806080 otoole-1.0.4a2/src/otoole/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10703 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/preprocess/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/preprocess/longify_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/preprocess/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/preprocess/validate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/read_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.806080 otoole-1.0.4a2/src/otoole/results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32615 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/results/result_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/results/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/validate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.810080 otoole-1.0.4a2/src/otoole/visualise/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/visualise/res.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-07-10 09:02:03.000000 otoole-1.0.4a2/src/otoole/write_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.806080 otoole-1.0.4a2/src/otoole.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-10 09:02:19.000000 otoole-1.0.4a2/src/otoole.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-10 09:02:19.000000 otoole-1.0.4a2/src/otoole.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:02:19.000000 otoole-1.0.4a2/src/otoole.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 09:02:19.000000 otoole-1.0.4a2/src/otoole.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:02:19.000000 otoole-1.0.4a2/src/otoole.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-10 09:02:19.000000 otoole-1.0.4a2/src/otoole.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 09:02:19.000000 otoole-1.0.4a2/src/otoole.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.810080 otoole-1.0.4a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.814081 otoole-1.0.4a2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)   130205 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/fixtures/combined_inputs.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    10703 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/fixtures/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/fixtures/config_r.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.814081 otoole-1.0.4a2/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/fixtures/data/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/fixtures/data/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    44422 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/fixtures/simplicity-v0.2.1.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    43735 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/fixtures/simplicity.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    75398 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/fixtures/simplicity.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:02:19.814081 otoole-1.0.4a2/tests/results/
+-rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/results/test_results_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41641 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/test_read_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/test_validate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/test_visualise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tests/test_write_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-10 09:02:03.000000 otoole-1.0.4a2/tox.ini
```

### Comparing `otoole-1.0.4/.coveragerc` & `otoole-1.0.4a2/.coveragerc`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/.github/ISSUE_TEMPLATE/bug_report.yaml` & `otoole-1.0.4a2/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/.github/ISSUE_TEMPLATE/docs.yaml` & `otoole-1.0.4a2/.github/ISSUE_TEMPLATE/docs.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/.github/ISSUE_TEMPLATE/feature.yaml` & `otoole-1.0.4a2/.github/ISSUE_TEMPLATE/feature.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/.github/workflows/python-publish.yml` & `otoole-1.0.4a2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/.github/workflows/python.yaml` & `otoole-1.0.4a2/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/.gitignore` & `otoole-1.0.4a2/.gitignore`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/.pre-commit-config.yaml` & `otoole-1.0.4a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/.zenodo.json` & `otoole-1.0.4a2/.zenodo.json`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/CHANGELOG.rst` & `otoole-1.0.4a2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/CITATION.cff` & `otoole-1.0.4a2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/LICENSE.txt` & `otoole-1.0.4a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/PKG-INFO` & `otoole-1.0.4a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoole
-Version: 1.0.4
+Version: 1.0.4a2
 Summary: A Python toolkit to support use of OSeMOSYS
 Home-page: https://github.com/OSeMOSYS/otoole
 Author: Will Usher
 Author-email: wusher@kth.se
 License: MIT
 Project-URL: Documentation, https://otoole.readthedocs.io/en/latest/?badge=latest
 Platform: any
```

### Comparing `otoole-1.0.4/README.rst` & `otoole-1.0.4a2/README.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/Makefile` & `otoole-1.0.4a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/_static/OSeMOSYS.png` & `otoole-1.0.4a2/docs/_static/OSeMOSYS.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/_static/logo.png` & `otoole-1.0.4a2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/_static/osemosys_dataflow.png` & `otoole-1.0.4a2/docs/_static/osemosys_dataflow.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/_static/otoole_figures.drawio` & `otoole-1.0.4a2/docs/_static/otoole_figures.drawio`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/_static/overview.png` & `otoole-1.0.4a2/docs/_static/overview.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/_static/overview_v2.png` & `otoole-1.0.4a2/docs/_static/overview_v2.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/_static/simplicity_res.png` & `otoole-1.0.4a2/docs/_static/simplicity_res.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/_static/validataion_model.png` & `otoole-1.0.4a2/docs/_static/validataion_model.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/_static/workflow.png` & `otoole-1.0.4a2/docs/_static/workflow.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/conf.py` & `otoole-1.0.4a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/contributing.rst` & `otoole-1.0.4a2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/data.rst` & `otoole-1.0.4a2/docs/data.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/examples.rst` & `otoole-1.0.4a2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/functionality.rst` & `otoole-1.0.4a2/docs/functionality.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/index.rst` & `otoole-1.0.4a2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/docs/install.rst` & `otoole-1.0.4a2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/scripts/prepare_cbc.sh` & `otoole-1.0.4a2/scripts/prepare_cbc.sh`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/scripts/prepare_cbc_short.sh` & `otoole-1.0.4a2/scripts/prepare_cbc_short.sh`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/setup.cfg` & `otoole-1.0.4a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/setup.py` & `otoole-1.0.4a2/setup.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/__init__.py` & `otoole-1.0.4a2/src/otoole/__init__.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/cli.py` & `otoole-1.0.4a2/src/otoole/cli.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/exceptions.py` & `otoole-1.0.4a2/src/otoole/exceptions.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/input.py` & `otoole-1.0.4a2/src/otoole/input.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/preprocess/config.yaml` & `otoole-1.0.4a2/src/otoole/preprocess/config.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/preprocess/longify_data.py` & `otoole-1.0.4a2/src/otoole/preprocess/longify_data.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/preprocess/setup.py` & `otoole-1.0.4a2/src/otoole/preprocess/setup.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/preprocess/validate_config.py` & `otoole-1.0.4a2/src/otoole/preprocess/validate_config.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/read_strategies.py` & `otoole-1.0.4a2/src/otoole/read_strategies.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/results/result_package.py` & `otoole-1.0.4a2/src/otoole/results/result_package.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/results/results.py` & `otoole-1.0.4a2/src/otoole/results/results.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/utils.py` & `otoole-1.0.4a2/src/otoole/utils.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/validate.py` & `otoole-1.0.4a2/src/otoole/validate.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/validate.yaml` & `otoole-1.0.4a2/src/otoole/validate.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/visualise/res.py` & `otoole-1.0.4a2/src/otoole/visualise/res.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole/write_strategies.py` & `otoole-1.0.4a2/src/otoole/write_strategies.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/src/otoole.egg-info/PKG-INFO` & `otoole-1.0.4a2/src/otoole.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoole
-Version: 1.0.4
+Version: 1.0.4a2
 Summary: A Python toolkit to support use of OSeMOSYS
 Home-page: https://github.com/OSeMOSYS/otoole
 Author: Will Usher
 Author-email: wusher@kth.se
 License: MIT
 Project-URL: Documentation, https://otoole.readthedocs.io/en/latest/?badge=latest
 Platform: any
```

### Comparing `otoole-1.0.4/src/otoole.egg-info/SOURCES.txt` & `otoole-1.0.4a2/src/otoole.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/conftest.py` & `otoole-1.0.4a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/fixtures/combined_inputs.xlsx` & `otoole-1.0.4a2/tests/fixtures/combined_inputs.xlsx`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/fixtures/config.yaml` & `otoole-1.0.4a2/tests/fixtures/config.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/fixtures/config_r.yaml` & `otoole-1.0.4a2/tests/fixtures/config_r.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/fixtures/simplicity-v0.2.1.zip` & `otoole-1.0.4a2/tests/fixtures/simplicity-v0.2.1.zip`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/fixtures/simplicity.txt` & `otoole-1.0.4a2/tests/fixtures/simplicity.txt`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/fixtures/simplicity.xlsx` & `otoole-1.0.4a2/tests/fixtures/simplicity.xlsx`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/results/test_results_package.py` & `otoole-1.0.4a2/tests/results/test_results_package.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/test_cli.py` & `otoole-1.0.4a2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/test_convert.py` & `otoole-1.0.4a2/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/test_input.py` & `otoole-1.0.4a2/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/test_read_strategies.py` & `otoole-1.0.4a2/tests/test_read_strategies.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/test_setup.py` & `otoole-1.0.4a2/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/test_utils.py` & `otoole-1.0.4a2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/test_validate.py` & `otoole-1.0.4a2/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/test_validate_config.py` & `otoole-1.0.4a2/tests/test_validate_config.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tests/test_write_strategies.py` & `otoole-1.0.4a2/tests/test_write_strategies.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.4/tox.ini` & `otoole-1.0.4a2/tox.ini`

 * *Files identical despite different names*

