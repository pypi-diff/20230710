# Comparing `tmp/inet-nm-0.0.5.tar.gz` & `tmp/inet-nm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inet-nm-0.0.5.tar", last modified: Mon Jun 12 15:27:18 2023, max compression
+gzip compressed data, was "inet-nm-0.0.6.tar", last modified: Mon Jul 10 10:27:27 2023, max compression
```

## Comparing `inet-nm-0.0.5.tar` & `inet-nm-0.0.6.tar`

### file list

```diff
@@ -1,65 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.473480 inet-nm-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-12 15:26:36.000000 inet-nm-0.0.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.453480 inet-nm-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.461480 inet-nm-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-12 15:26:36.000000 inet-nm-0.0.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-12 15:26:36.000000 inet-nm-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-12 15:26:36.000000 inet-nm-0.0.5/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-12 15:26:36.000000 inet-nm-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 15:26:36.000000 inet-nm-0.0.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 15:26:36.000000 inet-nm-0.0.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-12 15:26:36.000000 inet-nm-0.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-06-12 15:26:36.000000 inet-nm-0.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-12 15:26:36.000000 inet-nm-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-12 15:27:18.473480 inet-nm-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-06-12 15:26:36.000000 inet-nm-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.465480 inet-nm-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.465480 inet-nm-0.0.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-12 15:26:36.000000 inet-nm-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 15:26:36.000000 inet-nm-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-12 15:27:18.473480 inet-nm-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-12 15:26:36.000000 inet-nm-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.453480 inet-nm-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.469480 inet-nm-0.0.5/src/inet_nm/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/commissioner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/locking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/runner_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/runner_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/update_os_board_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.469480 inet-nm-0.0.5/src/inet_nm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.473480 inet-nm-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_comissioner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_locking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_runner_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.473934 inet-nm-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-10 10:26:50.000000 inet-nm-0.0.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.465934 inet-nm-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.469934 inet-nm-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-10 10:26:50.000000 inet-nm-0.0.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-10 10:26:50.000000 inet-nm-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-10 10:26:50.000000 inet-nm-0.0.6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-10 10:26:50.000000 inet-nm-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-10 10:26:50.000000 inet-nm-0.0.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 10:26:50.000000 inet-nm-0.0.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-10 10:26:50.000000 inet-nm-0.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-07-10 10:26:50.000000 inet-nm-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-10 10:26:50.000000 inet-nm-0.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-07-10 10:27:27.477934 inet-nm-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-07-10 10:26:50.000000 inet-nm-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.469934 inet-nm-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.469934 inet-nm-0.0.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/cli-example.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-10 10:26:50.000000 inet-nm-0.0.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-10 10:26:50.000000 inet-nm-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 10:26:50.000000 inet-nm-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-10 10:27:27.477934 inet-nm-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-10 10:26:50.000000 inet-nm-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.469934 inet-nm-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.473934 inet-nm-0.0.6/src/inet_nm/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_commission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_tmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_tty_from_uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_update_commissioned.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/cli_update_from_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/commissioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/locking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/runner_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-10 10:26:50.000000 inet-nm-0.0.6/src/inet_nm/runner_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.473934 inet-nm-0.0.6/src/inet_nm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 10:27:27.000000 inet-nm-0.0.6/src/inet_nm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:27.473934 inet-nm-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_comissioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_example_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_locking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_runner_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tests/test_runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-10 10:26:50.000000 inet-nm-0.0.6/tox.ini
```

### Comparing `inet-nm-0.0.5/.coveragerc` & `inet-nm-0.0.6/.coveragerc`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # .coveragerc to control coverage.py
 [run]
 branch = True
 source = inet_nm
+parallel = True
 # omit = bad_file.py
 
 [paths]
 source =
     src/
     */site-packages/
```

### Comparing `inet-nm-0.0.5/.github/workflows/ci.yml` & `inet-nm-0.0.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/.gitignore` & `inet-nm-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/.pre-commit-config.yaml` & `inet-nm-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/.readthedocs.yml` & `inet-nm-0.0.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/CHANGELOG.md` & `inet-nm-0.0.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/CONTRIBUTING.md` & `inet-nm-0.0.6/CONTRIBUTING.md`

 * *Files 20% similar despite different names*

```diff
@@ -105,14 +105,35 @@
    pip install pre-commit
    pre-commit install
    ```
 
    `inet-nm` comes with a lot of hooks configured to automatically help the
    developer to check the code being written.
 
+### Follow the design decisions
+
+#### Naming of CLI modules
+The provided design decision seems to be well-defined and clear. However, I have a couple of suggestions to improve it:
+
+- It would be useful to explain the background context more explicitly, especially if this document is for people not deeply involved in Python coverage or CLI development. For example, clarify what "coverage" is in this context and why it's important.
+- "use only `-` where `_` for the console script name" is somewhat unclear. It would be better to explicitly state the rules for name conversion.
+- The sentence "This allows the automated test to not only use include the console script..." is grammatically incorrect and confusing.
+
+Here's an example of a more detailed, and possibly clearer, design decision:
+
+#### Naming of CLI modules
+
+Coverage testing is a vital aspect of our development cycle, providing insights about which parts of our codebase are exercised during a test run. To support this, Python's `coverage` tool requires the modules to be invoked with a `main` function, since `coverage -m <MODULE>` is supported but specifying a function is not.
+
+In light of this requirement, we propose a naming standard for modules and console scripts. For each console script, we will have a corresponding Python module named `cli_<NAME>.py`. This module will include a `main` function, enabling it to be invoked by the `coverage` tool.
+
+Additionally, we'll define the console scripts in `setup.cfg` with the format `inet-nm-<NAME>`. This name is derived from the module name, but replaces underscores (`_`) with hyphens (`-`). The rationale for this is compatibility with naming standards in command line utilities.
+
+Adhering to this standard allows our automated tests to include the console script execution in the coverage report. Furthermore, it facilitates the generation of usage documentation by establishing a consistent naming pattern for console scripts and their corresponding modules.
+
 ### Implement your changes
 
 1. Create a branch to hold your changes:
 
    ```
    git checkout -b my-feature
    ```
```

### Comparing `inet-nm-0.0.5/LICENSE.txt` & `inet-nm-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/PKG-INFO` & `inet-nm-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inet-nm
-Version: 0.0.5
+Version: 0.0.6
 Summary: cli application for managing nodes
 Home-page: https://github.com/inetrg/inet-nm
 Author: Kevin Weiss
 Author-email: weiss.kevin604@gmail.com
 License: MIT
 Project-URL: Documentation, https://inet-nm.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/inetrg/inet-nm
@@ -82,15 +82,17 @@
 
 ## Usage
 
 Below is the usage for each of the command-line applications included in inet_nm:
 
 ### inet-nm-update-from-os
 
-This command is used to cache a list of boards and features.
+This command is used to cache a list of boards and features. The
+default commands are compatible with [RIOT OS](https://www.riot-os.org/) but
+can be overridden for other systems.
 
 ```
 $ inet-nm-update-from-os -h
 usage: inet-nm-update-from-os [-h] [-c CONFIG] [-i BOARD_INFO] [-f BOARD_FEATURES] [-n BOARD_ENV_VAR] basedir
 
 Cache a list of boards
 
@@ -185,14 +187,16 @@
 ```
 $ inet-nm-tty-from-uid -h
 usage: inet-nm-tty-from-uid [-h] [-c CONFIG] uid
 ```
 
 ## Example Workflow
 
+Up-to-date examples are available at [`docs/cli-example.md`](docs/cli-example.md).
+
 1. First update the boards list in the cache to allow for autocomplete and
 features.
 ```
 $ inet-nm-update-from-os RIOT/examples/hello-world/
 Getting features_provided for acd52832
 Getting features_provided for adafruit-clue
 ...
@@ -279,56 +283,7 @@
 
 ## License
 
 This project is licensed under the terms of the MIT license. See the LICENSE file.
 
 ---
 For any questions or contributions, please refer to the issues tab or the contributing guide.
-
-## Roadmap
-
-- Add optional power control
-    - Check if power control available for which boards
-    - Turn all ports on by default whenever checking connection
-    - Turn all unused off commissioned nodes by default once the action is complete
-    - flags to prevent power options
-    - Generic command to turn on all ports or specific nodes
-    - Caching usb locations
-- cleanup exception handling
-  - Removing lock if they have been removed before...
-```
-$ inet-nm-tmux -a
-duplicate session: default
-[exited]
-Traceback (most recent call last):
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_cli.py", line 91, in nm_tmux
-    runner.run()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 123, in run
-    self.release()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 85, in release
-    lock.release()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/filelock.py", line 89, in release
-    os.unlink(self.file_name)
-FileNotFoundError: [Errno 2] No such file or directory: '/tmp/inet_nm/locks/e8d68aaf8b4119ca21db0849a8339568.lock'
-
-During handling of the above exception, another exception occurred:
-
-Traceback (most recent call last):
-  File "/home/weiss/wd/inet-nm/.venv/bin/inet-nm-tmux", line 33, in <module>
-    sys.exit(load_entry_point('inet-nm', 'console_scripts', 'inet-nm-tmux')())
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_cli.py", line 91, in nm_tmux
-    runner.run()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 130, in __exit__
-    self.release()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 85, in release
-    lock.release()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/filelock.py", line 88, in release
-    os.close(self.fd)
-OSError: [Errno 9] Bad file descriptor
-```
-- remove all or one board
-- allow user boards that will not get overwritten
-- Nice readme with some gifs of usage
-- Add a CLI way and example get the port live based off UID to handle reconnecting within tmux session
-- Improve getting started
-- Add a session or exec timeout that will abort if the call takes too long
-- Add tests that go through the cli
```

### Comparing `inet-nm-0.0.5/README.md` & `inet-nm-0.0.6/src/inet_nm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: inet-nm
+Version: 0.0.6
+Summary: cli application for managing nodes
+Home-page: https://github.com/inetrg/inet-nm
+Author: Kevin Weiss
+Author-email: weiss.kevin604@gmail.com
+License: MIT
+Project-URL: Documentation, https://inet-nm.readthedocs.io/en/stable/
+Project-URL: Source, https://github.com/inetrg/inet-nm
+Project-URL: Changelog, https://github.com/inetrg/inet-nm/blob/master/CHANGELOG.md
+Project-URL: Tracker, https://github.com/inetrg/inet-nm/issues
+Project-URL: Download, https://pypi.org/project/inet-nm/#files
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: testing
+Provides-Extra: all
+License-File: LICENSE.txt
+
 [![CI Tests](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml/badge.svg)](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml)
 [![ReadTheDocs](https://readthedocs.org/projects/inet-nm/badge/?version=latest)](https://inet-nm.readthedocs.io/en/stable/)
 [![PyPI-Server](https://img.shields.io/pypi/v/inet-nm.svg)](https://pypi.org/project/inet-nm/)
 [![Monthly Downloads](https://pepy.tech/badge/inet-nm/month)](https://pepy.tech/project/inet-nm)
 
 # inet_nm - INET Node Manager
 
@@ -60,15 +82,17 @@
 
 ## Usage
 
 Below is the usage for each of the command-line applications included in inet_nm:
 
 ### inet-nm-update-from-os
 
-This command is used to cache a list of boards and features.
+This command is used to cache a list of boards and features. The
+default commands are compatible with [RIOT OS](https://www.riot-os.org/) but
+can be overridden for other systems.
 
 ```
 $ inet-nm-update-from-os -h
 usage: inet-nm-update-from-os [-h] [-c CONFIG] [-i BOARD_INFO] [-f BOARD_FEATURES] [-n BOARD_ENV_VAR] basedir
 
 Cache a list of boards
 
@@ -163,14 +187,16 @@
 ```
 $ inet-nm-tty-from-uid -h
 usage: inet-nm-tty-from-uid [-h] [-c CONFIG] uid
 ```
 
 ## Example Workflow
 
+Up-to-date examples are available at [`docs/cli-example.md`](docs/cli-example.md).
+
 1. First update the boards list in the cache to allow for autocomplete and
 features.
 ```
 $ inet-nm-update-from-os RIOT/examples/hello-world/
 Getting features_provided for acd52832
 Getting features_provided for adafruit-clue
 ...
@@ -257,56 +283,7 @@
 
 ## License
 
 This project is licensed under the terms of the MIT license. See the LICENSE file.
 
 ---
 For any questions or contributions, please refer to the issues tab or the contributing guide.
-
-## Roadmap
-
-- Add optional power control
-    - Check if power control available for which boards
-    - Turn all ports on by default whenever checking connection
-    - Turn all unused off commissioned nodes by default once the action is complete
-    - flags to prevent power options
-    - Generic command to turn on all ports or specific nodes
-    - Caching usb locations
-- cleanup exception handling
-  - Removing lock if they have been removed before...
-```
-$ inet-nm-tmux -a
-duplicate session: default
-[exited]
-Traceback (most recent call last):
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_cli.py", line 91, in nm_tmux
-    runner.run()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 123, in run
-    self.release()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 85, in release
-    lock.release()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/filelock.py", line 89, in release
-    os.unlink(self.file_name)
-FileNotFoundError: [Errno 2] No such file or directory: '/tmp/inet_nm/locks/e8d68aaf8b4119ca21db0849a8339568.lock'
-
-During handling of the above exception, another exception occurred:
-
-Traceback (most recent call last):
-  File "/home/weiss/wd/inet-nm/.venv/bin/inet-nm-tmux", line 33, in <module>
-    sys.exit(load_entry_point('inet-nm', 'console_scripts', 'inet-nm-tmux')())
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_cli.py", line 91, in nm_tmux
-    runner.run()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 130, in __exit__
-    self.release()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 85, in release
-    lock.release()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/filelock.py", line 88, in release
-    os.close(self.fd)
-OSError: [Errno 9] Bad file descriptor
-```
-- remove all or one board
-- allow user boards that will not get overwritten
-- Nice readme with some gifs of usage
-- Add a CLI way and example get the port live based off UID to handle reconnecting within tmux session
-- Improve getting started
-- Add a session or exec timeout that will abort if the call takes too long
-- Add tests that go through the cli
```

### Comparing `inet-nm-0.0.5/docs/Makefile` & `inet-nm-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/docs/conf.py` & `inet-nm-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/docs/index.md` & `inet-nm-0.0.6/docs/index.md`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 ## Contents
 
 ```{toctree}
 :maxdepth: 2
 
 Overview <readme>
+Examples <cli-example>
 Contributions & Help <contributing>
 License <license>
 Authors <authors>
 Changelog <changelog>
 Module Reference <api/modules>
 ```
```

### Comparing `inet-nm-0.0.5/setup.cfg` & `inet-nm-0.0.6/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -34,39 +34,43 @@
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 testing = 
 	setuptools
+	pexpect
 	pytest
 	pytest-cov
+	flaky
 all = 
 	inquirer
 
 [options.entry_points]
 console_scripts = 
-	inet-nm-tmux = inet_nm.runner_cli:nm_tmux
-	inet-nm-exec = inet_nm.runner_cli:nm_exec
-	inet-nm-check = inet_nm.check:cli_count_board_inventory
-	inet-nm-commission = inet_nm.commissioner:commission
-	inet-nm-tty-from-uid = inet_nm.commissioner:cli_tty_from_uid
-	inet-nm-update-commissioned = inet_nm.commissioner:update_commissioned
-	inet-nm-free = inet_nm.locking:cli_release_all_locks
-	inet-nm-update-from-os = inet_nm.update_os_board_list:cli_update_boards_from_os
+	inet-nm-tmux = inet_nm.cli_tmux:main
+	inet-nm-exec = inet_nm.cli_exec:main
+	inet-nm-check = inet_nm.cli_check:main
+	inet-nm-commission = inet_nm.cli_commission:main
+	inet-nm-tty-from-uid = inet_nm.cli_tty_from_uid:main
+	inet-nm-update-commissioned = inet_nm.cli_update_commissioned:main
+	inet-nm-free = inet_nm.cli_free:main
+	inet-nm-update-from-os = inet_nm.cli_update_from_os:main
 
 [tool:pytest]
 addopts = 
 	--cov inet_nm --cov-report term-missing
 	--verbose
 norecursedirs = 
 	dist
 	build
 	.tox
 testpaths = tests
+markers = 
+	slow: mark tests as slow (deselect with '-m "not slow"')
 
 [devpi:upload]
 no_vcs = 1
 formats = bdist_wheel
 
 [flake8]
 max_line_length = 88
```

### Comparing `inet-nm-0.0.5/setup.py` & `inet-nm-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/src/inet_nm/_helpers.py` & `inet-nm-0.0.6/src/inet_nm/_helpers.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/src/inet_nm/check.py` & `inet-nm-0.0.6/src/inet_nm/check.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 This module contains functions for checking the state of the boards.
 
 This is meant for evaluating inventory.
 """
 import argparse
-import json
 from typing import Dict, List
 
 import pyudev
 
 import inet_nm.config as cfg
 from inet_nm.data_types import NmNode
 from inet_nm.locking import get_locked_uids
@@ -332,29 +331,7 @@
     Returns:
         A list of all features.
     """
     features = []
     for node in nodes:
         features.extend(node.features_provided)
     return sorted(list(set(features)))
-
-
-def cli_count_board_inventory():
-    """CLI entrypoint for counting the inventory of boards."""
-    parser = argparse.ArgumentParser(description="Check the state of the boards")
-    cfg.config_arg(parser)
-    check_args(parser)
-    parser.add_argument(
-        "--show-features", action="store_true", help="Shows all features for all boards"
-    )
-    args = parser.parse_args()
-    kwargs = vars(args)
-    show_features = kwargs.pop("show_features")
-
-    nodes = get_filtered_nodes(**kwargs)
-
-    if show_features:
-        info = all_features_from_nodes(nodes)
-    else:
-        info = nodes_to_boards(nodes)
-    out = json.dumps(info, indent=2, sort_keys=True)
-    print(out)
```

### Comparing `inet-nm-0.0.5/src/inet_nm/config.py` & `inet-nm-0.0.6/src/inet_nm/config.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/src/inet_nm/data_types.py` & `inet-nm-0.0.6/src/inet_nm/data_types.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/src/inet_nm/filelock.py` & `inet-nm-0.0.6/src/inet_nm/filelock.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/src/inet_nm/locking.py` & `inet-nm-0.0.6/src/inet_nm/locking.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """This module contains functions for locking nodes."""
 import os
 import tempfile
 from pathlib import Path
 from typing import List
 
-from inet_nm._helpers import nm_print
 from inet_nm.data_types import NmNode
 
 
 def locks_dir() -> Path:
     """
     Get the directory for lock files.
 
@@ -47,14 +46,7 @@
     return locks_dir() / f"{node.uid}.lock"
 
 
 def release_all_locks():
     """Release all locks by deleting all lock files."""
     for lock_file in locks_dir().glob("*"):
         lock_file.unlink()
-
-
-def cli_release_all_locks():
-    """Release all locks by deleting all lock files and print the process."""
-    for lock_file in locks_dir().glob("*"):
-        nm_print(f"Removing lock file {lock_file}")
-        lock_file.unlink()
```

### Comparing `inet-nm-0.0.5/src/inet_nm/runner_apps.py` & `inet-nm-0.0.6/src/inet_nm/runner_apps.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/src/inet_nm/runner_base.py` & `inet-nm-0.0.6/src/inet_nm/runner_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 An operation is defined by a method `func` which is to be implemented
 in the subclass.
 """
 from threading import Thread
 from typing import Dict, List
 
 import inet_nm.locking as lk
+from inet_nm._helpers import nm_print
 from inet_nm.commissioner import TtyNotPresent, get_tty_from_nm_node
 from inet_nm.data_types import NmNode, NodeEnv
 from inet_nm.filelock import FileLock
 
 
 class NmNodesRunner:
     """
@@ -78,15 +79,18 @@
         for lock in self.locks:
             lock.acquire(timeout=timeout or self.default_timeout)
         self._acquired = True
 
     def release(self):
         """Release all acquired file locks."""
         for lock in self.locks:
-            lock.release()
+            try:
+                lock.release()
+            except FileNotFoundError:
+                nm_print(f"File {lock.file_name} already unlocked.")
         self._acquired = False
 
     def run(self):
         """
         Run operations on all nodes.
 
         This method spawns a new thread for each node and runs the
@@ -123,9 +127,10 @@
         self.release()
 
     def __enter__(self):
         self.acquire()
         return self
 
     def __exit__(self, type, value, traceback):
-        self.release()
-        self._acquired = False
+        if self._acquired:
+            self.release()
+            self._acquired = False
```

### Comparing `inet-nm-0.0.5/src/inet_nm/runner_cli.py` & `inet-nm-0.0.6/src/inet_nm/cli_tmux.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,31 @@
 import argparse
 import signal
 import subprocess
 import sys
 
-import inet_nm.check as check
+import inet_nm.check as chk
 import inet_nm.config as cfg
 import inet_nm.runner_apps as apps
-
-
-def _is_command_available(cmd):
-    return_code = subprocess.call(
-        f"which {cmd}", shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT
-    )
-    if return_code != 0:
-        print(f"{cmd} is not available! Please install first.")
-        sys.exit(1)
-
-
-def _check_filtered_nodes(**kwargs):
-    nodes = check.get_filtered_nodes(**kwargs)
-    if len(nodes) == 0:
-        print("No available nodes!")
-        sys.exit(1)
-    return nodes
-
-
-def _sanity_check(cmd, **kwargs):
-    _is_command_available(cmd)
-    return _check_filtered_nodes(**kwargs)
+import inet_nm.runner_helper as rh
 
 
 def _kill_tmux(session_name):
     output = subprocess.check_output(["tmux", "list-sessions"]).decode("utf-8")
     sessions = [line.split(":")[0] for line in output.split("\n") if line]
     for session in sessions:
         if session != session_name:
             continue
         print(f"Closing session {session}")
         subprocess.run(["tmux", "kill-session", "-t", session])
     exit(1)
 
 
-def _do_nothing(signum, frame):
-    pass
-
-
-def nm_tmux():
+def main():
+    """CLI entrypoint for starting tmux sessions."""
     parser = argparse.ArgumentParser(
         description="Starts interactive sessions for each node."
     )
     parser.add_argument(
         "-w", "--window", action="store_true", help="Open a window for each node."
     )
     parser.add_argument(
@@ -66,71 +42,37 @@
         "-x",
         "--cmd",
         type=str,
         default=None,
         help="Command to send after starting tmux session.",
     )
     cfg.config_arg(parser)
-    check.check_args(parser)
+    chk.check_args(parser)
     args = parser.parse_args()
     kwargs = vars(args)
     window = kwargs.pop("window")
     timeout = kwargs.pop("timeout")
     cmd = kwargs.pop("cmd")
     sname = kwargs.pop("session_name")
-    nodes = _sanity_check("tmux", **kwargs)
+    nodes = rh.sanity_check("tmux", **kwargs)
     signal.signal(signal.SIGINT, lambda x, y: _kill_tmux(sname))
 
     # This is a hack to keep the process alive long enough
     # to remove the lockfiles
     # It seems the tmux session will still remain but at least
     # the lockfiles will be removed...
-    signal.signal(signal.SIGHUP, _do_nothing)
+    signal.signal(signal.SIGHUP, rh.do_nothing)
     if window:
         with apps.NmTmuxWindowedRunner(nodes, default_timeout=timeout) as runner:
             runner.cmd = cmd
             runner.session_name = sname
             runner.run()
     else:
         with apps.NmTmuxPanedRunner(nodes, default_timeout=timeout) as runner:
             runner.cmd = cmd
             runner.session_name = sname
             runner.run()
     sys.exit(0)
 
 
-def nm_exec():
-    parser = argparse.ArgumentParser(
-        description="Execute command for each note environment."
-    )
-    parser.add_argument(
-        "cmd",
-        type=str,
-        help="bash command to execute, ' must be escaped and generally pay"
-        " attention to escape characters.",
-    )
-    parser.add_argument(
-        "-t",
-        "--timeout",
-        type=float,
-        default=None,
-        help="Wait until node available in seconds.",
-    )
-
-    cfg.config_arg(parser)
-    check.check_args(parser)
-    args = parser.parse_args()
-    kwargs = vars(args)
-    timeout = kwargs.pop("timeout")
-    cmd = kwargs.pop("cmd")
-    nodes = nodes = _sanity_check("/bin/bash", **kwargs)
-    # Somehow allows cleanup to happen...
-    signal.signal(signal.SIGHUP, _do_nothing)
-    try:
-        with apps.NmShellRunner(nodes, default_timeout=timeout) as runner:
-            runner.cmd = cmd
-            runner.run()
-    except KeyboardInterrupt:
-        print()
-        print("User aborted!")
-        sys.exit(1)
-    sys.exit(0)
+if __name__ == "__main__":
+    main()
```

### Comparing `inet-nm-0.0.5/src/inet_nm/update_os_board_list.py` & `inet-nm-0.0.6/src/inet_nm/cli_update_from_os.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 ):
     boards = {}
     errors = []
     for bn in board_names:
         nm_print(f"Getting features_provided for {bn}")
         env = os.environ.copy()
         env[board_env_var] = bn
-        res = subprocess.run(cmd.split(), cwd=cwd, env=env, capture_output=True)
+        # It seems resolving env vars isn't so easy
+        # As a test requires echo of a board var, let's just resolve it...
+        board_cmd = cmd.replace(f"${{{board_env_var}}}", bn)
+        res = subprocess.run(board_cmd.split(), cwd=cwd, env=env, capture_output=True)
+
         if res.returncode != 0:
             errors.append(bn)
             nm_print(f"FAILED to run {cmd} for {bn}")
         boards[bn] = res.stdout.decode().split()
     return (boards, errors)
 
 
-def cli_update_boards_from_os():
+def main():
+    """CLI entrypoint for updating the board info from the OS."""
     parser = argparse.ArgumentParser(description="Cache a list of boards")
     cfg.config_arg(parser)
     parser.add_argument("basedir", type=Path, help="Path to the board path directory")
     parser.add_argument(
         "-i",
         "--board-info",
         type=str,
@@ -78,7 +83,11 @@
                 sys.exit(1)
         bi_cfg.save(board_info)
         nm_print(f"\nUpdated {bi_cfg.file_path}")
     except KeyboardInterrupt:
         nm_print("\nUser aborted")
         sys.exit(2)
     sys.exit(0)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `inet-nm-0.0.5/src/inet_nm.egg-info/PKG-INFO` & `inet-nm-0.0.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: inet-nm
-Version: 0.0.5
-Summary: cli application for managing nodes
-Home-page: https://github.com/inetrg/inet-nm
-Author: Kevin Weiss
-Author-email: weiss.kevin604@gmail.com
-License: MIT
-Project-URL: Documentation, https://inet-nm.readthedocs.io/en/stable/
-Project-URL: Source, https://github.com/inetrg/inet-nm
-Project-URL: Changelog, https://github.com/inetrg/inet-nm/blob/master/CHANGELOG.md
-Project-URL: Tracker, https://github.com/inetrg/inet-nm/issues
-Project-URL: Download, https://pypi.org/project/inet-nm/#files
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Provides-Extra: testing
-Provides-Extra: all
-License-File: LICENSE.txt
-
 [![CI Tests](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml/badge.svg)](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml)
 [![ReadTheDocs](https://readthedocs.org/projects/inet-nm/badge/?version=latest)](https://inet-nm.readthedocs.io/en/stable/)
 [![PyPI-Server](https://img.shields.io/pypi/v/inet-nm.svg)](https://pypi.org/project/inet-nm/)
 [![Monthly Downloads](https://pepy.tech/badge/inet-nm/month)](https://pepy.tech/project/inet-nm)
 
 # inet_nm - INET Node Manager
 
@@ -82,15 +60,17 @@
 
 ## Usage
 
 Below is the usage for each of the command-line applications included in inet_nm:
 
 ### inet-nm-update-from-os
 
-This command is used to cache a list of boards and features.
+This command is used to cache a list of boards and features. The
+default commands are compatible with [RIOT OS](https://www.riot-os.org/) but
+can be overridden for other systems.
 
 ```
 $ inet-nm-update-from-os -h
 usage: inet-nm-update-from-os [-h] [-c CONFIG] [-i BOARD_INFO] [-f BOARD_FEATURES] [-n BOARD_ENV_VAR] basedir
 
 Cache a list of boards
 
@@ -185,14 +165,16 @@
 ```
 $ inet-nm-tty-from-uid -h
 usage: inet-nm-tty-from-uid [-h] [-c CONFIG] uid
 ```
 
 ## Example Workflow
 
+Up-to-date examples are available at [`docs/cli-example.md`](docs/cli-example.md).
+
 1. First update the boards list in the cache to allow for autocomplete and
 features.
 ```
 $ inet-nm-update-from-os RIOT/examples/hello-world/
 Getting features_provided for acd52832
 Getting features_provided for adafruit-clue
 ...
@@ -279,56 +261,7 @@
 
 ## License
 
 This project is licensed under the terms of the MIT license. See the LICENSE file.
 
 ---
 For any questions or contributions, please refer to the issues tab or the contributing guide.
-
-## Roadmap
-
-- Add optional power control
-    - Check if power control available for which boards
-    - Turn all ports on by default whenever checking connection
-    - Turn all unused off commissioned nodes by default once the action is complete
-    - flags to prevent power options
-    - Generic command to turn on all ports or specific nodes
-    - Caching usb locations
-- cleanup exception handling
-  - Removing lock if they have been removed before...
-```
-$ inet-nm-tmux -a
-duplicate session: default
-[exited]
-Traceback (most recent call last):
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_cli.py", line 91, in nm_tmux
-    runner.run()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 123, in run
-    self.release()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 85, in release
-    lock.release()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/filelock.py", line 89, in release
-    os.unlink(self.file_name)
-FileNotFoundError: [Errno 2] No such file or directory: '/tmp/inet_nm/locks/e8d68aaf8b4119ca21db0849a8339568.lock'
-
-During handling of the above exception, another exception occurred:
-
-Traceback (most recent call last):
-  File "/home/weiss/wd/inet-nm/.venv/bin/inet-nm-tmux", line 33, in <module>
-    sys.exit(load_entry_point('inet-nm', 'console_scripts', 'inet-nm-tmux')())
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_cli.py", line 91, in nm_tmux
-    runner.run()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 130, in __exit__
-    self.release()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 85, in release
-    lock.release()
-  File "/home/weiss/wd/inet-nm/src/inet_nm/filelock.py", line 88, in release
-    os.close(self.fd)
-OSError: [Errno 9] Bad file descriptor
-```
-- remove all or one board
-- allow user boards that will not get overwritten
-- Nice readme with some gifs of usage
-- Add a CLI way and example get the port live based off UID to handle reconnecting within tmux session
-- Improve getting started
-- Add a session or exec timeout that will abort if the call takes too long
-- Add tests that go through the cli
```

### Comparing `inet-nm-0.0.5/src/inet_nm.egg-info/SOURCES.txt` & `inet-nm-0.0.6/src/inet_nm.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -13,43 +13,52 @@
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/ci.yml
 docs/Makefile
 docs/authors.md
 docs/changelog.md
+docs/cli-example.md
 docs/conf.py
 docs/contributing.md
 docs/index.md
 docs/license.md
 docs/readme.md
 docs/requirements.txt
 docs/_static/.gitignore
 src/inet_nm/__init__.py
 src/inet_nm/_helpers.py
 src/inet_nm/check.py
+src/inet_nm/cli_check.py
+src/inet_nm/cli_commission.py
+src/inet_nm/cli_exec.py
+src/inet_nm/cli_free.py
+src/inet_nm/cli_tmux.py
+src/inet_nm/cli_tty_from_uid.py
+src/inet_nm/cli_update_commissioned.py
+src/inet_nm/cli_update_from_os.py
 src/inet_nm/commissioner.py
 src/inet_nm/config.py
 src/inet_nm/data_types.py
 src/inet_nm/filelock.py
 src/inet_nm/locking.py
 src/inet_nm/runner_apps.py
 src/inet_nm/runner_base.py
-src/inet_nm/runner_cli.py
-src/inet_nm/update_os_board_list.py
+src/inet_nm/runner_helper.py
 src/inet_nm.egg-info/PKG-INFO
 src/inet_nm.egg-info/SOURCES.txt
 src/inet_nm.egg-info/dependency_links.txt
 src/inet_nm.egg-info/entry_points.txt
 src/inet_nm.egg-info/not-zip-safe
 src/inet_nm.egg-info/requires.txt
 src/inet_nm.egg-info/top_level.txt
 tests/conftest.py
 tests/test_check.py
 tests/test_comissioner.py
 tests/test_config.py
 tests/test_data_types.py
+tests/test_example_usage.py
 tests/test_filelock.py
 tests/test_helpers.py
 tests/test_locking.py
 tests/test_runner_apps.py
 tests/test_runner_base.py
```

### Comparing `inet-nm-0.0.5/tests/test_check.py` & `inet-nm-0.0.6/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/tests/test_comissioner.py` & `inet-nm-0.0.6/tests/test_comissioner.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/tests/test_config.py` & `inet-nm-0.0.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/tests/test_data_types.py` & `inet-nm-0.0.6/tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/tests/test_filelock.py` & `inet-nm-0.0.6/tests/test_filelock.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/tests/test_helpers.py` & `inet-nm-0.0.6/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/tests/test_locking.py` & `inet-nm-0.0.6/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/tests/test_runner_apps.py` & `inet-nm-0.0.6/tests/test_runner_apps.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/tests/test_runner_base.py` & `inet-nm-0.0.6/tests/test_runner_base.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.5/tox.ini` & `inet-nm-0.0.6/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,29 @@
     SETUPTOOLS_*
 extras =
     testing
 commands =
     pytest {posargs}
 
 
+[testenv:examples]
+description = Generate the examples via pytest
+setenv =
+    TOXINIDIR = {toxinidir}
+deps =
+    -r requirements.txt
+passenv =
+    HOME
+    SETUPTOOLS_*
+extras =
+    testing
+commands =
+    pytest -k cli_example --cli-readme-mock=docs/cli-example.md {posargs}
+
+
 # To run `tox -e lint` you need to make sure you have a
 # `.pre-commit-config.yaml` file. See https://pre-commit.com
 [testenv:lint]
 description = Perform static analysis and style checks
 skip_install = True
 deps = pre-commit
 passenv =
```

