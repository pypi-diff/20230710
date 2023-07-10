# Comparing `tmp/bump-my-version-0.6.0.tar.gz` & `tmp/bump-my-version-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bump-my-version-0.6.0.tar", last modified: Fri Jun 23 19:40:05 2023, max compression
+gzip compressed data, was "bump-my-version-0.7.0.tar", last modified: Mon Jul 10 14:55:38 2023, max compression
```

## Comparing `bump-my-version-0.6.0.tar` & `bump-my-version-0.7.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:40:05.484678 bump-my-version-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16352 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-06-23 19:40:05.484678 bump-my-version-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:40:05.476678 bump-my-version-0.6.0/bump_my_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-06-23 19:40:05.000000 bump-my-version-0.6.0/bump_my_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-23 19:40:05.000000 bump-my-version-0.6.0/bump_my_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:40:05.000000 bump-my-version-0.6.0/bump_my_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 19:40:05.000000 bump-my-version-0.6.0/bump_my_version.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-23 19:40:05.000000 bump-my-version-0.6.0/bump_my_version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 19:40:05.000000 bump-my-version-0.6.0/bump_my_version.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:40:05.480678 bump-my-version-0.6.0/bumpversion/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    12804 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/show.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/version_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/bumpversion/yaml_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-23 19:40:05.484678 bump-my-version-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:40:05.480678 bump-my-version-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:40:05.480678 bump-my-version-0.6.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/fixtures/basic_cfg.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/fixtures/basic_cfg.toml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/fixtures/basic_cfg_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/fixtures/basic_cfg_expected.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/fixtures/basic_cfg_expected.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/fixtures/basic_cfg_expected_full.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:40:05.480678 bump-my-version-0.6.0/tests/fixtures/glob/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:40:05.480678 bump-my-version-0.6.0/tests/fixtures/glob/directory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/fixtures/glob/directory/file3.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/fixtures/glob/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/fixtures/glob/file2.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/fixtures/glob/not-text.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:40:05.484678 bump-my-version-0.6.0/tests/fixtures/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/fixtures/interpolation/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/fixtures/interpolation/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/fixtures/interpolation/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/test_autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/test_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/test_show.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/test_version_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-23 19:39:41.000000 bump-my-version-0.6.0/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.485710 bump-my-version-0.7.0/bump_my_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-10 14:55:38.000000 bump-my-version-0.7.0/bump_my_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-10 14:55:38.000000 bump-my-version-0.7.0/bump_my_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:55:38.000000 bump-my-version-0.7.0/bump_my_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 14:55:38.000000 bump-my-version-0.7.0/bump_my_version.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-10 14:55:38.000000 bump-my-version-0.7.0/bump_my_version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 14:55:38.000000 bump-my-version-0.7.0/bump_my_version.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.485710 bump-my-version-0.7.0/bumpversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/version_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/bumpversion/yaml_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/basic_cfg.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/basic_cfg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected_full.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/tests/fixtures/glob/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/tests/fixtures/glob/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/glob/directory/file3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/glob/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/glob/file2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/glob/not-text.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:38.489710 bump-my-version-0.7.0/tests/fixtures/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/interpolation/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/interpolation/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/interpolation/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/fixtures/pep440.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_version_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-10 14:55:18.000000 bump-my-version-0.7.0/tests/test_yaml.py
```

### Comparing `bump-my-version-0.6.0/CHANGELOG.md` & `bump-my-version-0.7.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,55 @@
 # Changelog
 
+## 0.7.0 (2023-07-10)
+[Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.6.0...0.7.0)
+
+### Fixes
+
+- Fixed test coverage. [3fe96f0](https://github.com/callowayproject/bump-my-version/commit/3fe96f0e244ab5be4f96ec8ecbe1ca63f1f06e6b)
+    
+- Fixed wrong pydantic version pinning. [d4b125e](https://github.com/callowayproject/bump-my-version/commit/d4b125ea1e1c0179f3f544cfffed90d27c997ff5)
+    
+- Fixed typing issue. [bfe5306](https://github.com/callowayproject/bump-my-version/commit/bfe530668d8f176843eedcd7096fcd2b85eef228)
+    
+  - Declared SourceCodeManager attributes as `ClassVar[List[str]]`
+  - `_TEST_USABLE_COMMAND`, `_COMMIT_COMMAND`, and `_ALL_TAGS_COMMAND` affected
+### New
+
+- Added tests for CLI replace command. [a53cddc](https://github.com/callowayproject/bump-my-version/commit/a53cddc3c13bb21f5432d1cd331a51027a25981f)
+    
+- Added and re-organized documentation. [c62d65e](https://github.com/callowayproject/bump-my-version/commit/c62d65e71fdc617d5435976cfa587f43b03ac92b)
+    
+- Added replace subcommand. [8722a0f](https://github.com/callowayproject/bump-my-version/commit/8722a0f84ab60cbfc254741b2a5bc0d968e423d9)
+    
+  - Works just like `bump` but
+    - doesn't do any version incrementing
+    - Will not change the configuration file
+    - Will not commit or tag
+
+  - Can use `bumpversion show new_version --increment <versionpart>` to see what the new version would be
+- Adds `short_branch_name` to version rendering context. [7f7e50c](https://github.com/callowayproject/bump-my-version/commit/7f7e50c98dc20210468a9cef34baf4374956c2e9)
+    
+  - `short_branch_name` is the branch name, lower case, containing only a-z and 0-9, and truncated to 20 characters.
+
+  Fixes #28
+### Other
+
+- Check config before tagging. [3a6e3ee](https://github.com/callowayproject/bump-my-version/commit/3a6e3eebdbc16ae509754fd977625a4c9b19d82a)
+    
+- Format version parts. [ee43bdb](https://github.com/callowayproject/bump-my-version/commit/ee43bdb18f3d96ed702094bb75b06a1338c9aa9c)
+    
+- [pre-commit.ci] auto fixes from pre-commit.com hooks. [5e6f566](https://github.com/callowayproject/bump-my-version/commit/5e6f566b3c3bc96a070780a70c82a92b817e2299)
+    
+  for more information, see https://pre-commit.ci
+- [pre-commit.ci] pre-commit autoupdate. [f1acd35](https://github.com/callowayproject/bump-my-version/commit/f1acd353aa4c58afaa15321f7a7ab9dfb12ce040)
+    
+  **updates:** - [github.com/charliermarsh/ruff-pre-commit: v0.0.272 → v0.0.275](https://github.com/charliermarsh/ruff-pre-commit/compare/v0.0.272...v0.0.275)
+
+
 ## 0.6.0 (2023-06-23)
 [Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.5.1.dev69...0.6.0)
 
 ### Fixes
 
 - Fixed `--help` and `bump` invocations. [9d965e5](https://github.com/callowayproject/bump-my-version/commit/9d965e57f2c0a41476d75ec053653416eae966c9)
```

### Comparing `bump-my-version-0.6.0/CODE_OF_CONDUCT.md` & `bump-my-version-0.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/CONTRIBUTING.md` & `bump-my-version-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/LICENSE` & `bump-my-version-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/PKG-INFO` & `bump-my-version-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.6.0
+Version: 0.7.0
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bump-my-version-0.6.0/README.md` & `bump-my-version-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/bump_my_version.egg-info/PKG-INFO` & `bump-my-version-0.7.0/bump_my_version.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.6.0
+Version: 0.7.0
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bump-my-version-0.6.0/bump_my_version.egg-info/SOURCES.txt` & `bump-my-version-0.7.0/bump_my_version.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 tests/test_yaml.py
 tests/fixtures/basic_cfg.cfg
 tests/fixtures/basic_cfg.toml
 tests/fixtures/basic_cfg_expected.json
 tests/fixtures/basic_cfg_expected.txt
 tests/fixtures/basic_cfg_expected.yaml
 tests/fixtures/basic_cfg_expected_full.json
+tests/fixtures/pep440.toml
 tests/fixtures/glob/file1.txt
 tests/fixtures/glob/file2.txt
 tests/fixtures/glob/not-text.md
 tests/fixtures/glob/directory/file3.txt
 tests/fixtures/interpolation/.bumpversion.cfg
 tests/fixtures/interpolation/pyproject.toml
 tests/fixtures/interpolation/setup.cfg
```

### Comparing `bump-my-version-0.6.0/bumpversion/aliases.py` & `bump-my-version-0.7.0/bumpversion/aliases.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/bumpversion/autocast.py` & `bump-my-version-0.7.0/bumpversion/autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/bumpversion/bump.py` & `bump-my-version-0.7.0/bumpversion/bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/bumpversion/cli.py` & `bump-my-version-0.7.0/bumpversion/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 import rich_click as click
 from click.core import Context
 
 from bumpversion import __version__
 from bumpversion.aliases import AliasedGroup
 from bumpversion.bump import do_bump
 from bumpversion.config import find_config_file, get_configuration
+from bumpversion.files import modify_files, resolve_file_config
 from bumpversion.logging import setup_logging
 from bumpversion.show import do_show, log_list
-from bumpversion.utils import get_overrides
+from bumpversion.utils import get_context, get_overrides
 
 logger = logging.getLogger(__name__)
 
 
 @click.group(
     cls=AliasedGroup,
     invoke_without_command=True,
@@ -286,7 +287,160 @@
     found_config_file = find_config_file(config_file)
     config = get_configuration(found_config_file)
 
     if not args:
         do_show("all", config=config, format_=format_, increment=increment)
     else:
         do_show(*args, config=config, format_=format_, increment=increment)
+
+
+@cli.command()
+@click.argument("files", nargs=-1, type=str)
+@click.option(
+    "--config-file",
+    metavar="FILE",
+    required=False,
+    envvar="BUMPVERSION_CONFIG_FILE",
+    type=click.Path(exists=True),
+    help="Config file to read most of the variables from.",
+)
+@click.option(
+    "-v",
+    "--verbose",
+    count=True,
+    required=False,
+    envvar="BUMPVERSION_VERBOSE",
+    help="Print verbose logging to stderr. Can specify several times for more verbosity.",
+)
+@click.option(
+    "--allow-dirty/--no-allow-dirty",
+    default=None,
+    required=False,
+    envvar="BUMPVERSION_ALLOW_DIRTY",
+    help="Don't abort if working directory is dirty, or explicitly abort if dirty.",
+)
+@click.option(
+    "--current-version",
+    metavar="VERSION",
+    required=False,
+    envvar="BUMPVERSION_CURRENT_VERSION",
+    help="Version that needs to be updated",
+)
+@click.option(
+    "--new-version",
+    metavar="VERSION",
+    required=False,
+    envvar="BUMPVERSION_NEW_VERSION",
+    help="New version that should be in the files. If not specified, it will be None.",
+)
+@click.option(
+    "--parse",
+    metavar="REGEX",
+    required=False,
+    envvar="BUMPVERSION_PARSE",
+    help="Regex parsing the version string",
+)
+@click.option(
+    "--serialize",
+    metavar="FORMAT",
+    multiple=True,
+    required=False,
+    envvar="BUMPVERSION_SERIALIZE",
+    help="How to format what is parsed back to a version",
+)
+@click.option(
+    "--search",
+    metavar="SEARCH",
+    required=False,
+    envvar="BUMPVERSION_SEARCH",
+    help="Template for complete string to search",
+)
+@click.option(
+    "--replace",
+    metavar="REPLACE",
+    required=False,
+    envvar="BUMPVERSION_REPLACE",
+    help="Template for complete string to replace",
+)
+@click.option(
+    "--no-configured-files",
+    is_flag=True,
+    envvar="BUMPVERSION_NO_CONFIGURED_FILES",
+    help=(
+        "Only replace the version in files specified on the command line, "
+        "ignoring the files from the configuration file."
+    ),
+)
+@click.option(
+    "--dry-run",
+    "-n",
+    is_flag=True,
+    envvar="BUMPVERSION_DRY_RUN",
+    help="Don't write any files, just pretend.",
+)
+def replace(
+    files: list,
+    config_file: Optional[str],
+    verbose: int,
+    allow_dirty: Optional[bool],
+    current_version: Optional[str],
+    new_version: Optional[str],
+    parse: Optional[str],
+    serialize: Optional[List[str]],
+    search: Optional[str],
+    replace: Optional[str],
+    no_configured_files: bool,
+    dry_run: bool,
+) -> None:
+    """
+    Replace the version in files.
+
+    FILES are additional file(s) to modify.
+    If you want to rewrite only files specified on the command line, use with the
+    `--no-configured-files` option.
+    """
+    setup_logging(verbose)
+
+    logger.info("Starting BumpVersion %s", __version__)
+
+    overrides = get_overrides(
+        allow_dirty=allow_dirty,
+        current_version=current_version,
+        new_version=new_version,
+        parse=parse,
+        serialize=serialize or None,
+        search=search,
+        replace=replace,
+        commit=False,
+        tag=False,
+        sign_tags=False,
+        tag_name=None,
+        tag_message=None,
+        message=None,
+        commit_args=None,
+    )
+
+    found_config_file = find_config_file(config_file)
+    config = get_configuration(found_config_file, **overrides)
+
+    config.allow_dirty = allow_dirty if allow_dirty is not None else config.allow_dirty
+    if not config.allow_dirty and config.scm_info.tool:
+        config.scm_info.tool.assert_nondirty()
+
+    if no_configured_files:
+        config.files = []
+
+    if files:
+        config.add_files(files)
+
+    version = config.version_config.parse(config.current_version)
+
+    if new_version:
+        next_version = config.version_config.parse(new_version)
+    else:
+        next_version = None
+
+    ctx = get_context(config, version, next_version)
+
+    configured_files = resolve_file_config(config.files, config.version_config)
+
+    modify_files(configured_files, version, next_version, ctx, dry_run)
```

### Comparing `bump-my-version-0.6.0/bumpversion/config.py` & `bump-my-version-0.7.0/bumpversion/config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/bumpversion/exceptions.py` & `bump-my-version-0.7.0/bumpversion/exceptions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/bumpversion/files.py` & `bump-my-version-0.7.0/bumpversion/files.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/bumpversion/functions.py` & `bump-my-version-0.7.0/bumpversion/functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/bumpversion/logging.py` & `bump-my-version-0.7.0/bumpversion/logging.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/bumpversion/scm.py` & `bump-my-version-0.7.0/bumpversion/scm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Version control system management."""
 
 import logging
 import os
+import re
 import subprocess
 from dataclasses import dataclass
 from pathlib import Path
 from tempfile import NamedTemporaryFile
-from typing import TYPE_CHECKING, List, MutableMapping, Optional, Type, Union
+from typing import TYPE_CHECKING, ClassVar, List, MutableMapping, Optional, Type, Union
 
 if TYPE_CHECKING:  # pragma: no-coverage
     from bumpversion.config import Config
 
 from bumpversion.exceptions import DirtyWorkingDirectoryError, SignedTagsError
 
 logger = logging.getLogger(__name__)
@@ -21,14 +22,15 @@
     """Information about the current source code manager and state."""
 
     tool: Optional[Type["SourceCodeManager"]] = None
     commit_sha: Optional[str] = None
     distance_to_latest_tag: Optional[int] = None
     current_version: Optional[str] = None
     branch_name: Optional[str] = None
+    short_branch_name: Optional[str] = None
     dirty: Optional[bool] = None
 
     def __str__(self):
         return self.__repr__()
 
     def __repr__(self):
         tool_name = self.tool.__name__ if self.tool else "No SCM tool"
@@ -38,17 +40,17 @@
             f"dirty={self.dirty})"
         )
 
 
 class SourceCodeManager:
     """Base class for version control systems."""
 
-    _TEST_USABLE_COMMAND: List[str] = []
-    _COMMIT_COMMAND: List[str] = []
-    _ALL_TAGS_COMMAND: List[str] = []
+    _TEST_USABLE_COMMAND: ClassVar[List[str]] = []
+    _COMMIT_COMMAND: ClassVar[List[str]] = []
+    _ALL_TAGS_COMMAND: ClassVar[List[str]] = []
 
     @classmethod
     def commit(cls, message: str, current_version: str, new_version: str, extra_args: Optional[list] = None) -> None:
         """Commit the changes."""
         extra_args = extra_args or []
 
         with NamedTemporaryFile("wb", delete=False) as f:
@@ -157,24 +159,24 @@
                 new_version=context["new_version"],
                 extra_args=extra_args,
             )
 
     @classmethod
     def tag_in_scm(cls, config: "Config", context: MutableMapping, dry_run: bool = False) -> None:
         """Tag the current commit in the source code management system."""
-        sign_tags = config.sign_tags
-        tag_name = config.tag_name.format(**context)
-        tag_message = config.tag_message.format(**context)
-        existing_tags = cls.get_all_tags()
         if not config.commit:
             logger.info("Would not tag since we are not committing")
             return
         if not config.tag:
             logger.info("Would not tag")
             return
+        sign_tags = config.sign_tags
+        tag_name = config.tag_name.format(**context)
+        tag_message = config.tag_message.format(**context)
+        existing_tags = cls.get_all_tags()
 
         do_tag = not dry_run
 
         if tag_name in existing_tags:
             logger.warning("Tag '%s' already exists. Will not tag.", tag_name)
             return
 
@@ -195,17 +197,17 @@
     def __repr__(self):
         return f"{self.__class__.__name__}"
 
 
 class Git(SourceCodeManager):
     """Git implementation."""
 
-    _TEST_USABLE_COMMAND = ["git", "rev-parse", "--git-dir"]
-    _COMMIT_COMMAND = ["git", "commit", "-F"]
-    _ALL_TAGS_COMMAND = ["git", "tag", "--list"]
+    _TEST_USABLE_COMMAND: ClassVar[List[str]] = ["git", "rev-parse", "--git-dir"]
+    _COMMIT_COMMAND: ClassVar[List[str]] = ["git", "commit", "-F"]
+    _ALL_TAGS_COMMAND: ClassVar[List[str]] = ["git", "tag", "--list"]
 
     @classmethod
     def assert_nondirty(cls) -> None:
         """Assert that the working directory is not dirty."""
         lines = [
             line.strip()
             for line in subprocess.check_output(["git", "status", "--porcelain"]).splitlines()  # noqa: S603, S607
@@ -241,19 +243,20 @@
             ]
             result = subprocess.run(git_cmd, text=True, check=True, capture_output=True)  # noqa: S603
             describe_out = result.stdout.strip().split("-")
 
             git_cmd = ["git", "rev-parse", "--abbrev-ref", "HEAD"]
             result = subprocess.run(git_cmd, text=True, check=True, capture_output=True)  # noqa: S603
             branch_name = result.stdout.strip()
+            short_branch_name = re.sub(r"([^a-zA-Z0-9]*)", "", branch_name).lower()[:20]
         except subprocess.CalledProcessError as e:
             logger.debug("Error when running git describe: %s", e.stderr)
             return SCMInfo(tool=cls)
 
-        info = SCMInfo(tool=cls, branch_name=branch_name)
+        info = SCMInfo(tool=cls, branch_name=branch_name, short_branch_name=short_branch_name)
 
         if describe_out[-1].strip() == "dirty":
             info.dirty = True
             describe_out.pop()
         else:
             info.dirty = False
 
@@ -288,17 +291,17 @@
             command += ["--message", message]
         subprocess.check_output(command)  # noqa: S603
 
 
 class Mercurial(SourceCodeManager):
     """Mercurial implementation."""
 
-    _TEST_USABLE_COMMAND = ["hg", "root"]
-    _COMMIT_COMMAND = ["hg", "commit", "--logfile"]
-    _ALL_TAGS_COMMAND = ["hg", "log", '--rev="tag()"', '--template="{tags}\n"']
+    _TEST_USABLE_COMMAND: ClassVar[List[str]] = ["hg", "root"]
+    _COMMIT_COMMAND: ClassVar[List[str]] = ["hg", "commit", "--logfile"]
+    _ALL_TAGS_COMMAND: ClassVar[List[str]] = ["hg", "log", '--rev="tag()"', '--template="{tags}\n"']
 
     @classmethod
     def latest_tag_info(cls, tag_pattern: str) -> SCMInfo:
         """Return information about the latest tag."""
         current_version = None
         re_pattern = tag_pattern.replace("*", ".*")
         result = subprocess.run(
```

### Comparing `bump-my-version-0.6.0/bumpversion/show.py` & `bump-my-version-0.7.0/bumpversion/show.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/bumpversion/utils.py` & `bump-my-version-0.7.0/bumpversion/utils.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/bumpversion/version_part.py` & `bump-my-version-0.7.0/bumpversion/version_part.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,20 @@
 
     @property
     def is_independent(self) -> bool:
         """Is the part independent of the other parts?"""
         return self.config.independent
 
     def __format__(self, format_spec: str) -> str:
-        return self.value
+        try:
+            val = int(self.value)
+        except ValueError:
+            return self.value
+        else:
+            return int.__format__(val, format_spec)
 
     def __repr__(self) -> str:
         return f"<bumpversion.VersionPart:{self.func.__class__.__name__}:{self.value}>"
 
     def __eq__(self, other: Any) -> bool:
         return self.value == other.value if isinstance(other, VersionPart) else False
 
@@ -125,15 +130,15 @@
 
     def __init__(
         self,
         parse: str,
         serialize: List[str],
         search: str,
         replace: str,
-        part_configs: Dict[str, VersionPartConfig] = None,
+        part_configs: Optional[Dict[str, VersionPartConfig]] = None,
     ):
         try:
             self.parse_regex = re.compile(parse, re.VERBOSE)
         except re.error as e:
             raise UsageError(f"--parse '{parse}' is not a valid regex.") from e
 
         self.serialize_formats = serialize
```

### Comparing `bump-my-version-0.6.0/bumpversion/yaml_dump.py` & `bump-my-version-0.7.0/bumpversion/yaml_dump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/pyproject.toml` & `bump-my-version-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["bumpversion", "version", "release"]
 dynamic = ["version"]
 dependencies = [
     "click",
-    "pydantic",
+    "pydantic<2.0.0",
     "rich-click",
     "rich",
     "tomlkit",
 ]
 
 [project.scripts]
 bump-my-version = "bumpversion.cli:cli"
@@ -206,15 +206,15 @@
 [tool.ruff.isort]
 order-by-type = true
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.bumpversion]
-current_version = "0.6.0"
+current_version = "0.7.0"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "{new_version}"
 allow_dirty = true
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<dev>dev\\d+))?"
 serialize = [
```

### Comparing `bump-my-version-0.6.0/tests/conftest.py` & `bump-my-version-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/fixtures/basic_cfg.cfg` & `bump-my-version-0.7.0/tests/fixtures/basic_cfg.cfg`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/fixtures/basic_cfg.toml` & `bump-my-version-0.7.0/tests/fixtures/basic_cfg.toml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/fixtures/basic_cfg_expected.json` & `bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected.json`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/fixtures/basic_cfg_expected.txt` & `bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/fixtures/basic_cfg_expected.yaml` & `bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected.yaml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/fixtures/basic_cfg_expected_full.json` & `bump-my-version-0.7.0/tests/fixtures/basic_cfg_expected_full.json`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/test_autocast.py` & `bump-my-version-0.7.0/tests/test_autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/test_bump.py` & `bump-my-version-0.7.0/tests/test_bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/test_cli.py` & `bump-my-version-0.7.0/tests/test_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -357,7 +357,75 @@
 
     if result.exit_code != 0:
         print(result.output)
         print(result.exception)
 
     assert result.exit_code == 0
     assert result.output.strip() == expected_output.strip()
+
+
+def test_replace(mocker, tmp_path, fixtures_path):
+    """The replace subcommand should replace the version in the file."""
+    # Arrange
+    toml_path = fixtures_path / "basic_cfg.toml"
+    config_path = tmp_path / "pyproject.toml"
+    shutil.copy(toml_path, config_path)
+
+    mocked_modify_files = mocker.patch("bumpversion.cli.modify_files")
+    runner: CliRunner = CliRunner()
+    with inside_dir(tmp_path):
+        result: Result = runner.invoke(cli.cli, ["replace", "--new-version", "1.1.0"])
+
+    if result.exit_code != 0:
+        print(result.output)
+
+    assert result.exit_code == 0
+
+    call_args = mocked_modify_files.call_args[0]
+    configured_files = call_args[0]
+    assert len(configured_files) == 3
+    actual_filenames = {f.path for f in configured_files}
+    assert actual_filenames == {"setup.py", "CHANGELOG.md", "bumpversion/__init__.py"}
+
+
+def test_replace_no_newversion(mocker, tmp_path, fixtures_path):
+    """The replace subcommand should set new_version to None in the context."""
+    # Arrange
+    toml_path = fixtures_path / "basic_cfg.toml"
+    config_path = tmp_path / "pyproject.toml"
+    shutil.copy(toml_path, config_path)
+
+    mocked_modify_files = mocker.patch("bumpversion.cli.modify_files")
+    runner: CliRunner = CliRunner()
+    with inside_dir(tmp_path):
+        result: Result = runner.invoke(cli.cli, ["replace"])
+
+    if result.exit_code != 0:
+        print(result.output)
+
+    assert result.exit_code == 0
+
+    call_args = mocked_modify_files.call_args[0]
+    assert call_args[2] is None
+
+
+def test_replace_specific_files(mocker, git_repo, fixtures_path):
+    """The replace subcommand should set the files to only the specified files."""
+    # Arrange
+    toml_path = fixtures_path / "basic_cfg.toml"
+    config_path = git_repo / "pyproject.toml"
+    shutil.copy(toml_path, config_path)
+
+    mocked_modify_files = mocker.patch("bumpversion.cli.modify_files")
+    runner: CliRunner = CliRunner()
+    with inside_dir(git_repo):
+        result: Result = runner.invoke(cli.cli, ["replace", "--no-configured-files", "VERSION"])
+
+    if result.exit_code != 0:
+        print(result.output)
+
+    assert result.exit_code == 0
+
+    call_args = mocked_modify_files.call_args[0]
+    configured_files = call_args[0]
+    assert len(configured_files) == 1
+    assert configured_files[0].path == "VERSION"
```

### Comparing `bump-my-version-0.6.0/tests/test_config.py` & `bump-my-version-0.7.0/tests/test_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Test configuration parsing."""
 import difflib
 import json
 from pathlib import Path
 from textwrap import dedent
 
 import pytest
+from click.testing import CliRunner, Result
 from pytest import param
 
 from bumpversion import config
 from tests.conftest import inside_dir
 
 
 @pytest.fixture(params=[".bumpversion.cfg", "setup.cfg"])
@@ -190,7 +191,58 @@
     cfg_path.write_text(orig_path.read_text())
     original_content = orig_path.read_text().splitlines(keepends=True)
 
     config.update_config_file(cfg_path, "1.0.0", "1.0.1")
     new_content = cfg_path.read_text().splitlines(keepends=True)
     difference = difflib.context_diff(original_content, new_content, n=0)
     assert "".join(difference) == expected_diff
+
+
+def test_pep440_config(git_repo: Path, fixtures_path: Path):
+    """
+    Check the PEP440 config file.
+    """
+    from bumpversion.utils import get_context
+    from bumpversion.bump import get_next_version
+    from bumpversion import cli
+    import subprocess
+
+    # Arrange
+
+    cfg_path = git_repo / "pyproject.toml"
+    orig_path = fixtures_path / "pep440.toml"
+    cfg_path.write_text(orig_path.read_text())
+    version_path = git_repo / "VERSION"
+    version_path.write_text("1.0.0")
+    readme_path = git_repo / "README.md"
+    runner: CliRunner = CliRunner()
+
+    with inside_dir(git_repo):
+        subprocess.run(["git", "add", "VERSION"], check=True, capture_output=True)
+        subprocess.run(["git", "commit", "-m", "initial commit"], check=True, capture_output=True)
+        subprocess.run(["git", "tag", "v1.0.0"], check=True, capture_output=True)
+
+        cfg = config.get_configuration(cfg_path)
+        ctx = get_context(cfg)
+        version = cfg.version_config.parse(cfg.current_version)
+        next_version = get_next_version(version, cfg, "patch", None)
+        next_version_str = cfg.version_config.serialize(next_version, ctx)
+        assert next_version_str == "1.0.1"
+
+        subprocess.run(["git", "checkout", "-b", "my-really-LONG-branch_name"], check=True, capture_output=True)
+        readme_path.write_text("This is my branch!")
+        result: Result = runner.invoke(cli.cli, ["bump", "dev_label", "--no-tag"])
+        assert result.exit_code == 0
+        cfg = config.get_configuration(cfg_path)
+        assert cfg.current_version == "1.0.0.dev0+myreallylongbranchna"
+
+        # try:
+        #     subprocess.run(["git", "add", "README.md"], check=True, capture_output=True)
+        #     subprocess.run(["git", "commit", "-am", "my branch commit"], check=True, capture_output=True)
+        # except subprocess.CalledProcessError as e:
+        #     print(e.stdout)
+        #     print(e.stderr)
+        #     raise
+        # result: Result = runner.invoke(cli.cli, ["bump", "dev_label", "--no-tag"])
+        # assert result.exit_code == 0
+        # cfg = config.get_configuration(cfg_path)
+        # assert cfg.current_version == "1.0.0.dev1+myreallylongbranchna"
```

### Comparing `bump-my-version-0.6.0/tests/test_files.py` & `bump-my-version-0.7.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/test_functions.py` & `bump-my-version-0.7.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/test_scm.py` & `bump-my-version-0.7.0/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/test_show.py` & `bump-my-version-0.7.0/tests/test_show.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/test_version_part.py` & `bump-my-version-0.7.0/tests/test_version_part.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.6.0/tests/test_yaml.py` & `bump-my-version-0.7.0/tests/test_yaml.py`

 * *Files identical despite different names*

