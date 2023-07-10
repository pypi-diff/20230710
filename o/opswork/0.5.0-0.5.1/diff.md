# Comparing `tmp/opswork-0.5.0.tar.gz` & `tmp/opswork-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opswork-0.5.0.tar", last modified: Sun Jul  9 21:56:27 2023, max compression
+gzip compressed data, was "opswork-0.5.1.tar", last modified: Mon Jul 10 12:35:31 2023, max compression
```

## Comparing `opswork-0.5.0.tar` & `opswork-0.5.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.884142 opswork-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-09 21:56:07.000000 opswork-0.5.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-09 21:56:07.000000 opswork-0.5.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.884142 opswork-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-09 21:56:07.000000 opswork-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-09 21:56:07.000000 opswork-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.884142 opswork-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-09 21:56:07.000000 opswork-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 21:56:07.000000 opswork-0.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-09 21:56:07.000000 opswork-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-09 21:56:07.000000 opswork-0.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-09 21:56:07.000000 opswork-0.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-09 21:56:07.000000 opswork-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-09 21:56:07.000000 opswork-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-09 21:56:07.000000 opswork-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-09 21:56:07.000000 opswork-0.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-09 21:56:27.888142 opswork-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-09 21:56:07.000000 opswork-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.884142 opswork-0.5.0/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-09 21:56:07.000000 opswork-0.5.0/cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-09 21:56:07.000000 opswork-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.880142 opswork-0.5.0/recipe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.884142 opswork-0.5.0/recipe/motd/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-09 21:56:07.000000 opswork-0.5.0/recipe/motd/motd.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-09 21:56:07.000000 opswork-0.5.0/recipe/motd/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/recipe/nginx/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-09 21:56:07.000000 opswork-0.5.0/recipe/nginx/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/recipe/ping/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-09 21:56:07.000000 opswork-0.5.0/recipe/ping/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-09 21:56:07.000000 opswork-0.5.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-09 21:56:27.892142 opswork-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-09 21:56:07.000000 opswork-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.884142 opswork-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/src/opswork/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/src/opswork/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/command/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/command/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/command/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/command/recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/command/secret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/src/opswork/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/src/opswork/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/model/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/model/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/model/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/src/opswork/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/src/opswork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-09 21:56:07.000000 opswork-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/tests/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:07.000000 opswork-0.5.0/tests/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-09 21:56:07.000000 opswork-0.5.0/tests/module/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-09 21:56:07.000000 opswork-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.745150 opswork-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.741150 opswork-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 12:35:10.000000 opswork-0.5.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 12:35:10.000000 opswork-0.5.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.741150 opswork-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-10 12:35:10.000000 opswork-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-10 12:35:10.000000 opswork-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.741150 opswork-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-10 12:35:10.000000 opswork-0.5.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-10 12:35:10.000000 opswork-0.5.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-10 12:35:10.000000 opswork-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 12:35:10.000000 opswork-0.5.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-10 12:35:10.000000 opswork-0.5.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-10 12:35:10.000000 opswork-0.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-10 12:35:10.000000 opswork-0.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-10 12:35:10.000000 opswork-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-10 12:35:10.000000 opswork-0.5.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-10 12:35:31.745150 opswork-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-10 12:35:10.000000 opswork-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.741150 opswork-0.5.1/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 12:35:10.000000 opswork-0.5.1/cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-10 12:35:10.000000 opswork-0.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.741150 opswork-0.5.1/recipe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.745150 opswork-0.5.1/recipe/motd/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-10 12:35:10.000000 opswork-0.5.1/recipe/motd/motd.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-10 12:35:10.000000 opswork-0.5.1/recipe/motd/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.745150 opswork-0.5.1/recipe/nginx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-10 12:35:10.000000 opswork-0.5.1/recipe/nginx/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.745150 opswork-0.5.1/recipe/ping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-10 12:35:10.000000 opswork-0.5.1/recipe/ping/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 12:35:10.000000 opswork-0.5.1/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-10 12:35:31.749150 opswork-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-10 12:35:10.000000 opswork-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.741150 opswork-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.745150 opswork-0.5.1/src/opswork/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.745150 opswork-0.5.1/src/opswork/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/command/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/command/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/command/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/command/recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/command/secret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.745150 opswork-0.5.1/src/opswork/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.745150 opswork-0.5.1/src/opswork/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/model/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/model/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/model/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.745150 opswork-0.5.1/src/opswork/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/module/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/module/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/module/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/module/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/module/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-10 12:35:10.000000 opswork-0.5.1/src/opswork/module/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.745150 opswork-0.5.1/src/opswork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-10 12:35:31.000000 opswork-0.5.1/src/opswork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-10 12:35:31.000000 opswork-0.5.1/src/opswork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:35:31.000000 opswork-0.5.1/src/opswork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 12:35:31.000000 opswork-0.5.1/src/opswork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:35:31.000000 opswork-0.5.1/src/opswork.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-10 12:35:31.000000 opswork-0.5.1/src/opswork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 12:35:31.000000 opswork-0.5.1/src/opswork.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.745150 opswork-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-10 12:35:10.000000 opswork-0.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:31.745150 opswork-0.5.1/tests/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 12:35:10.000000 opswork-0.5.1/tests/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-10 12:35:10.000000 opswork-0.5.1/tests/module/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-10 12:35:10.000000 opswork-0.5.1/tox.ini
```

### Comparing `opswork-0.5.0/.github/workflows/release.yml` & `opswork-0.5.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/.gitignore` & `opswork-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/CODE_OF_CONDUCT.md` & `opswork-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/CONTRIBUTING.rst` & `opswork-0.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/LICENSE.txt` & `opswork-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/Makefile` & `opswork-0.5.1/Makefile`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/README.rst` & `opswork-0.5.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -134,7 +134,50 @@
 .. code-block::
 
     $ opswork recipe run <recipe_name> -h <host_name> -v key=value
 
     # Some examples
     $ opswork recipe run clivern/nginx -h example.com
     $ opswork recipe run clivern/ping -h localhost
+
+
+16. To generate a random password
+
+.. code-block::
+
+    $ opswork random password 8
+
+
+17. To add a secret
+
+.. code-block::
+
+    $ opswork secret add <secret/name> <secret_value> -t <tag>
+
+    $ opswork secret add clivern/cloud_provider/api_key xxxx-xxxx-xxxx-xxxx -t cloud_provider
+
+
+18. To list secrets
+
+.. code-block::
+
+    $ opswork secret list -o json
+
+
+19. To get a secret
+
+.. code-block::
+
+    $ opswork secret get <secret_name>
+
+    # For example
+    $ opswork secret get clivern/cloud_provider/api_key
+
+
+20. To delete a secret
+
+.. code-block::
+
+    $ opswork secret delete <secret_name>
+
+    # For example
+    $ opswork secret delete clivern/cloud_provider/api_key
```

### Comparing `opswork-0.5.0/recipe/motd/recipe.yml` & `opswork-0.5.1/recipe/motd/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/recipe/nginx/recipe.yml` & `opswork-0.5.1/recipe/nginx/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/recipe/ping/recipe.yml` & `opswork-0.5.1/recipe/ping/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/setup.cfg` & `opswork-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/setup.py` & `opswork-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/__init__.py` & `opswork-0.5.1/src/opswork/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/cli.py` & `opswork-0.5.1/src/opswork/cli.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/command/__init__.py` & `opswork-0.5.1/src/opswork/command/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/command/configs.py` & `opswork-0.5.1/src/opswork/command/configs.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/command/hosts.py` & `opswork-0.5.1/src/opswork/command/hosts.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/command/random.py` & `opswork-0.5.1/src/opswork/command/random.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/command/recipes.py` & `opswork-0.5.1/src/opswork/command/recipes.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/command/secret.py` & `opswork-0.5.1/src/opswork/command/secret.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/exception/__init__.py` & `opswork-0.5.1/src/opswork/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/model/__init__.py` & `opswork-0.5.1/src/opswork/model/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/model/host.py` & `opswork-0.5.1/src/opswork/model/host.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/model/recipe.py` & `opswork-0.5.1/src/opswork/model/recipe.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/model/secret.py` & `opswork-0.5.1/src/opswork/model/secret.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/model/task.py` & `opswork-0.5.1/src/opswork/model/task.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/module/__init__.py` & `opswork-0.5.1/src/opswork/module/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/module/config.py` & `opswork-0.5.1/src/opswork/module/config.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/module/database.py` & `opswork-0.5.1/src/opswork/module/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
         ).fetchall()
 
         cursor.close()
 
         for row in rows:
             data = json.loads(row[2])
 
-            secret = Vault(
+            secret = Secret(
                 row[0],
                 row[1],
                 data["value"],
                 data["tags"],
                 row[3],
                 row[4],
             )
```

### Comparing `opswork-0.5.0/src/opswork/module/encrypt.py` & `opswork-0.5.1/src/opswork/module/encrypt.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/module/file_system.py` & `opswork-0.5.1/src/opswork/module/file_system.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/module/logger.py` & `opswork-0.5.1/src/opswork/module/logger.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/module/output.py` & `opswork-0.5.1/src/opswork/module/output.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork/module/playbook.py` & `opswork-0.5.1/src/opswork/module/playbook.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/src/opswork.egg-info/SOURCES.txt` & `opswork-0.5.1/src/opswork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/tests/__init__.py` & `opswork-0.5.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/tests/module/test_logger.py` & `opswork-0.5.1/tests/module/test_logger.py`

 * *Files identical despite different names*

### Comparing `opswork-0.5.0/tox.ini` & `opswork-0.5.1/tox.ini`

 * *Files identical despite different names*

