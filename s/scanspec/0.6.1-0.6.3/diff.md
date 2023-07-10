# Comparing `tmp/scanspec-0.6.1.tar.gz` & `tmp/scanspec-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanspec-0.6.1.tar", last modified: Tue Feb  7 14:55:43 2023, max compression
+gzip compressed data, was "scanspec-0.6.3.tar", last modified: Mon Jul 10 10:46:09 2023, max compression
```

## Comparing `scanspec-0.6.1.tar` & `scanspec-0.6.3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.013700 scanspec-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.001700 scanspec-0.6.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-02-07 14:55:32.000000 scanspec-0.6.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-02-07 14:55:32.000000 scanspec-0.6.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.005700 scanspec-0.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-02-07 14:55:32.000000 scanspec-0.6.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:42.997700 scanspec-0.6.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.005700 scanspec-0.6.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-02-07 14:55:32.000000 scanspec-0.6.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-07 14:55:32.000000 scanspec-0.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.005700 scanspec-0.6.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-07 14:55:32.000000 scanspec-0.6.1/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-02-07 14:55:32.000000 scanspec-0.6.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.005700 scanspec-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-02-07 14:55:32.000000 scanspec-0.6.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-02-07 14:55:32.000000 scanspec-0.6.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-02-07 14:55:32.000000 scanspec-0.6.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-02-07 14:55:32.000000 scanspec-0.6.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-07 14:55:32.000000 scanspec-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-07 14:55:32.000000 scanspec-0.6.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.005700 scanspec-0.6.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-07 14:55:32.000000 scanspec-0.6.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-02-07 14:55:32.000000 scanspec-0.6.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-07 14:55:32.000000 scanspec-0.6.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-07 14:55:32.000000 scanspec-0.6.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-07 14:55:32.000000 scanspec-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-02-07 14:55:43.013700 scanspec-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-02-07 14:55:32.000000 scanspec-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.005700 scanspec-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.005700 scanspec-0.6.1/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/explanations/technical-terms.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/explanations/why-squash-can-change-path.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/explanations/why-stack-frames.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/explanations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.005700 scanspec-0.6.1/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/how-to/iterate-a-spec.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/how-to/serialize-a-spec.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/how-to.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.009700 scanspec-0.6.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    33532 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/images/definitions.png
--rw-r--r--   0 runner    (1001) docker     (123)    38221 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/images/plot_spec.png
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/images/scanspec-logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    15557 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/images/scanspec-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.009700 scanspec-0.6.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/reference/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/reference/rest_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.009700 scanspec-0.6.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/tutorials/creating-a-spec.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/tutorials/rest-service.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-07 14:55:32.000000 scanspec-0.6.1/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-02-07 14:55:32.000000 scanspec-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-02-07 14:55:32.000000 scanspec-0.6.1/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 14:55:43.013700 scanspec-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.001700 scanspec-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.009700 scanspec-0.6.1/src/scanspec/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-07 14:55:32.000000 scanspec-0.6.1/src/scanspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-07 14:55:32.000000 scanspec-0.6.1/src/scanspec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-07 14:55:42.000000 scanspec-0.6.1/src/scanspec/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-02-07 14:55:32.000000 scanspec-0.6.1/src/scanspec/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23415 2023-02-07 14:55:32.000000 scanspec-0.6.1/src/scanspec/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-02-07 14:55:32.000000 scanspec-0.6.1/src/scanspec/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-02-07 14:55:32.000000 scanspec-0.6.1/src/scanspec/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-02-07 14:55:32.000000 scanspec-0.6.1/src/scanspec/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    23344 2023-02-07 14:55:32.000000 scanspec-0.6.1/src/scanspec/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-02-07 14:55:32.000000 scanspec-0.6.1/src/scanspec/sphinxext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.013700 scanspec-0.6.1/src/scanspec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-02-07 14:55:42.000000 scanspec-0.6.1/src/scanspec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-07 14:55:42.000000 scanspec-0.6.1/src/scanspec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 14:55:42.000000 scanspec-0.6.1/src/scanspec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-07 14:55:42.000000 scanspec-0.6.1/src/scanspec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-02-07 14:55:42.000000 scanspec-0.6.1/src/scanspec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-07 14:55:42.000000 scanspec-0.6.1/src/scanspec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:43.013700 scanspec-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:32.000000 scanspec-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-02-07 14:55:32.000000 scanspec-0.6.1/tests/test_boilerplate_removed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-02-07 14:55:32.000000 scanspec-0.6.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-07 14:55:32.000000 scanspec-0.6.1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-07 14:55:32.000000 scanspec-0.6.1/tests/test_iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-02-07 14:55:32.000000 scanspec-0.6.1/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-02-07 14:55:32.000000 scanspec-0.6.1/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    18664 2023-02-07 14:55:32.000000 scanspec-0.6.1/tests/test_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.596264 scanspec-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.584263 scanspec-0.6.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-10 10:46:00.000000 scanspec-0.6.3/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-10 10:46:00.000000 scanspec-0.6.3/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.584263 scanspec-0.6.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-10 10:46:00.000000 scanspec-0.6.3/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.580263 scanspec-0.6.3/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.584263 scanspec-0.6.3/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-10 10:46:00.000000 scanspec-0.6.3/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-10 10:46:00.000000 scanspec-0.6.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.584263 scanspec-0.6.3/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-10 10:46:00.000000 scanspec-0.6.3/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-07-10 10:46:00.000000 scanspec-0.6.3/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.588263 scanspec-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-07-10 10:46:00.000000 scanspec-0.6.3/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-10 10:46:00.000000 scanspec-0.6.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-10 10:46:00.000000 scanspec-0.6.3/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-10 10:46:00.000000 scanspec-0.6.3/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-10 10:46:00.000000 scanspec-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-10 10:46:00.000000 scanspec-0.6.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.588263 scanspec-0.6.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-10 10:46:00.000000 scanspec-0.6.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-10 10:46:00.000000 scanspec-0.6.3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-10 10:46:00.000000 scanspec-0.6.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-10 10:46:00.000000 scanspec-0.6.3/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 10:46:00.000000 scanspec-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-07-10 10:46:09.596264 scanspec-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-10 10:46:00.000000 scanspec-0.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.588263 scanspec-0.6.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.588263 scanspec-0.6.3/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/explanations/technical-terms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/explanations/why-squash-can-change-path.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/explanations/why-stack-frames.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/explanations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.588263 scanspec-0.6.3/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/how-to/iterate-a-spec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/how-to/serialize-a-spec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/how-to.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.592264 scanspec-0.6.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    33532 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/images/definitions.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38221 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/images/plot_spec.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/images/scanspec-logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    15557 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/images/scanspec-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.592264 scanspec-0.6.3/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/reference/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/reference/rest_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.592264 scanspec-0.6.3/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/tutorials/creating-a-spec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/tutorials/rest-service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-10 10:46:00.000000 scanspec-0.6.3/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-10 10:46:00.000000 scanspec-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-10 10:46:00.000000 scanspec-0.6.3/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:46:09.596264 scanspec-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.584263 scanspec-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.592264 scanspec-0.6.3/src/scanspec/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 10:46:00.000000 scanspec-0.6.3/src/scanspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 10:46:00.000000 scanspec-0.6.3/src/scanspec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 10:46:09.000000 scanspec-0.6.3/src/scanspec/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-10 10:46:00.000000 scanspec-0.6.3/src/scanspec/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23403 2023-07-10 10:46:00.000000 scanspec-0.6.3/src/scanspec/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-10 10:46:00.000000 scanspec-0.6.3/src/scanspec/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-10 10:46:00.000000 scanspec-0.6.3/src/scanspec/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10845 2023-07-10 10:46:00.000000 scanspec-0.6.3/src/scanspec/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23344 2023-07-10 10:46:00.000000 scanspec-0.6.3/src/scanspec/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-10 10:46:00.000000 scanspec-0.6.3/src/scanspec/sphinxext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.596264 scanspec-0.6.3/src/scanspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-07-10 10:46:09.000000 scanspec-0.6.3/src/scanspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-10 10:46:09.000000 scanspec-0.6.3/src/scanspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:46:09.000000 scanspec-0.6.3/src/scanspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 10:46:09.000000 scanspec-0.6.3/src/scanspec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-10 10:46:09.000000 scanspec-0.6.3/src/scanspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 10:46:09.000000 scanspec-0.6.3/src/scanspec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:09.596264 scanspec-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:00.000000 scanspec-0.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-10 10:46:00.000000 scanspec-0.6.3/tests/test_boilerplate_removed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-07-10 10:46:00.000000 scanspec-0.6.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-10 10:46:00.000000 scanspec-0.6.3/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-10 10:46:00.000000 scanspec-0.6.3/tests/test_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-10 10:46:00.000000 scanspec-0.6.3/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-10 10:46:00.000000 scanspec-0.6.3/tests/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18664 2023-07-10 10:46:00.000000 scanspec-0.6.3/tests/test_specs.py
```

### Comparing `scanspec-0.6.1/.devcontainer/Dockerfile` & `scanspec-0.6.3/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/.devcontainer/devcontainer.json` & `scanspec-0.6.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/.github/CONTRIBUTING.rst` & `scanspec-0.6.3/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/.github/actions/install_requirements/action.yml` & `scanspec-0.6.3/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/.github/dependabot.yml` & `scanspec-0.6.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/.github/pages/make_switcher.py` & `scanspec-0.6.3/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/.github/workflows/code.yml` & `scanspec-0.6.3/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/.github/workflows/docs.yml` & `scanspec-0.6.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/.github/workflows/docs_clean.yml` & `scanspec-0.6.3/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/.github/workflows/linkcheck.yml` & `scanspec-0.6.3/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/.gitignore` & `scanspec-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/.vscode/launch.json` & `scanspec-0.6.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/.vscode/settings.json` & `scanspec-0.6.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/LICENSE` & `scanspec-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/PKG-INFO` & `scanspec-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanspec
-Version: 0.6.1
+Version: 0.6.3
 Summary: Specify step and flyscan paths in a serializable, efficient and Pythonic way
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `scanspec-0.6.1/README.rst` & `scanspec-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/conf.py` & `scanspec-0.6.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/explanations/technical-terms.rst` & `scanspec-0.6.3/docs/explanations/technical-terms.rst`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/explanations/why-squash-can-change-path.rst` & `scanspec-0.6.3/docs/explanations/why-squash-can-change-path.rst`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/explanations/why-stack-frames.rst` & `scanspec-0.6.3/docs/explanations/why-stack-frames.rst`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/how-to/iterate-a-spec.rst` & `scanspec-0.6.3/docs/how-to/iterate-a-spec.rst`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/how-to/serialize-a-spec.rst` & `scanspec-0.6.3/docs/how-to/serialize-a-spec.rst`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/images/definitions.png` & `scanspec-0.6.3/docs/images/definitions.png`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/images/plot_spec.png` & `scanspec-0.6.3/docs/images/plot_spec.png`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/images/scanspec-logo.ico` & `scanspec-0.6.3/docs/images/scanspec-logo.ico`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/images/scanspec-logo.svg` & `scanspec-0.6.3/docs/images/scanspec-logo.svg`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/index.rst` & `scanspec-0.6.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/reference/api.rst` & `scanspec-0.6.3/docs/reference/api.rst`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/tutorials/creating-a-spec.rst` & `scanspec-0.6.3/docs/tutorials/creating-a-spec.rst`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/tutorials/installation.rst` & `scanspec-0.6.3/docs/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/docs/tutorials/rest-service.rst` & `scanspec-0.6.3/docs/tutorials/rest-service.rst`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/pyproject.toml` & `scanspec-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,37 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "Specify step and flyscan paths in a serializable, efficient and Pythonic way"
-dependencies = ["numpy>=1.19.3", "click", "pydantic", "typing_extensions"]
+dependencies = [
+    "numpy>=1.19.3",
+    "click==8.1.3",
+    "pydantic<2.0",
+    "typing_extensions"
+]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.rst"
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
 # Plotting
 plotting = [
     # make sure a python 3.9 compatible scipy and matplotlib are selected
     "scipy>=1.5.4",
     "matplotlib>=3.2.2",
 ]
 # REST service support
-service = ["fastapi", "uvicorn"]
+service = [
+    "fastapi==0.99",
+    "uvicorn"
+]
 # For development tests/docs
 dev = [
     "black==22.3.0",
     "mypy<1",
     "flake8-isort",
     "Flake8-pyproject",
     "pipdeptree",
```

### Comparing `scanspec-0.6.1/schema.json` & `scanspec-0.6.3/schema.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.874736328125%*

 * *Differences: {"'openapi'": "'3.1.0'",*

 * * "'paths'": "{'/valid': {'post': {'requestBody': {'content': {'application/json': {'schema': "*

 * *            "{'examples': [OrderedDict([('outer', OrderedDict([('axis', 'y'), ('start', 0.0), "*

 * *            "('stop', 10.0), ('num', 3), ('type', 'Line')])), ('inner', OrderedDict([('axis', "*

 * *            "'x'), ('start', 0.0), ('stop', 10.0), ('num', 4), ('type', 'Line')])), ('type', "*

 * *            "'Product')])]}, delete: ['example']}}}}}, '/midpoints': {'post': {'requestBody': "*

 * *          […]*

```diff
@@ -266,46 +266,53 @@
             }
         }
     },
     "info": {
         "title": "FastAPI",
         "version": "0.1.0"
     },
-    "openapi": "3.0.2",
+    "openapi": "3.1.0",
     "paths": {
         "/bounds": {
             "post": {
                 "description": "Generate bounds from a scanspec.\n\nA scanspec can produce points with lower and upper bounds.\n\nArgs:\n    request: Scanspec and formatting info.\n\nReturns:\n    BoundsResponse: Bounds of the scan",
                 "operationId": "bounds_bounds_post",
                 "requestBody": {
                     "content": {
                         "application/json": {
-                            "example": {
-                                "format": "FLOAT_LIST",
-                                "max_frames": 1024,
-                                "spec": {
-                                    "inner": {
-                                        "axis": "x",
-                                        "num": 4,
-                                        "start": 0.0,
-                                        "stop": 10.0,
-                                        "type": "Line"
-                                    },
-                                    "outer": {
-                                        "axis": "y",
-                                        "num": 3,
-                                        "start": 0.0,
-                                        "stop": 10.0,
-                                        "type": "Line"
-                                    },
-                                    "type": "Product"
-                                }
-                            },
                             "schema": {
-                                "$ref": "#/components/schemas/PointsRequest"
+                                "allOf": [
+                                    {
+                                        "$ref": "#/components/schemas/PointsRequest"
+                                    }
+                                ],
+                                "examples": [
+                                    {
+                                        "format": "FLOAT_LIST",
+                                        "max_frames": 1024,
+                                        "spec": {
+                                            "inner": {
+                                                "axis": "x",
+                                                "num": 4,
+                                                "start": 0.0,
+                                                "stop": 10.0,
+                                                "type": "Line"
+                                            },
+                                            "outer": {
+                                                "axis": "y",
+                                                "num": 3,
+                                                "start": 0.0,
+                                                "stop": 10.0,
+                                                "type": "Line"
+                                            },
+                                            "type": "Product"
+                                        }
+                                    }
+                                ],
+                                "title": "Request"
                             }
                         }
                     },
                     "required": true
                 },
                 "responses": {
                     "200": {
@@ -335,32 +342,34 @@
         "/gap": {
             "post": {
                 "description": "Generate gaps from a scanspec.\n\nA scanspec may indicate if there is a gap between two frames.\nThe array returned corresponds to whether or not there is a gap\nafter each frame.\n\nArgs:\n    request: Scanspec and formatting info.\n\nReturns:\n    GapResponse: Bounds of the scan",
                 "operationId": "gap_gap_post",
                 "requestBody": {
                     "content": {
                         "application/json": {
-                            "example": {
-                                "inner": {
-                                    "axis": "x",
-                                    "num": 4,
-                                    "start": 0.0,
-                                    "stop": 10.0,
-                                    "type": "Line"
-                                },
-                                "outer": {
-                                    "axis": "y",
-                                    "num": 3,
-                                    "start": 0.0,
-                                    "stop": 10.0,
-                                    "type": "Line"
-                                },
-                                "type": "Product"
-                            },
                             "schema": {
+                                "examples": [
+                                    {
+                                        "inner": {
+                                            "axis": "x",
+                                            "num": 4,
+                                            "start": 0.0,
+                                            "stop": 10.0,
+                                            "type": "Line"
+                                        },
+                                        "outer": {
+                                            "axis": "y",
+                                            "num": 3,
+                                            "start": 0.0,
+                                            "stop": 10.0,
+                                            "type": "Line"
+                                        },
+                                        "type": "Product"
+                                    }
+                                ],
                                 "title": "Spec"
                             }
                         }
                     },
                     "required": true
                 },
                 "responses": {
@@ -391,37 +400,44 @@
         "/midpoints": {
             "post": {
                 "description": "Generate midpoints from a scanspec.\n\nA scanspec can produce bounded points (i.e. a point is valid if an\naxis is between a minimum and and a maximum, see /bounds). The midpoints\nare the middle of each set of bounds.\n\nArgs:\n    request: Scanspec and formatting info.\n\nReturns:\n    MidpointsResponse: Midpoints of the scan",
                 "operationId": "midpoints_midpoints_post",
                 "requestBody": {
                     "content": {
                         "application/json": {
-                            "example": {
-                                "format": "FLOAT_LIST",
-                                "max_frames": 1024,
-                                "spec": {
-                                    "inner": {
-                                        "axis": "x",
-                                        "num": 4,
-                                        "start": 0.0,
-                                        "stop": 10.0,
-                                        "type": "Line"
-                                    },
-                                    "outer": {
-                                        "axis": "y",
-                                        "num": 3,
-                                        "start": 0.0,
-                                        "stop": 10.0,
-                                        "type": "Line"
-                                    },
-                                    "type": "Product"
-                                }
-                            },
                             "schema": {
-                                "$ref": "#/components/schemas/PointsRequest"
+                                "allOf": [
+                                    {
+                                        "$ref": "#/components/schemas/PointsRequest"
+                                    }
+                                ],
+                                "examples": [
+                                    {
+                                        "format": "FLOAT_LIST",
+                                        "max_frames": 1024,
+                                        "spec": {
+                                            "inner": {
+                                                "axis": "x",
+                                                "num": 4,
+                                                "start": 0.0,
+                                                "stop": 10.0,
+                                                "type": "Line"
+                                            },
+                                            "outer": {
+                                                "axis": "y",
+                                                "num": 3,
+                                                "start": 0.0,
+                                                "stop": 10.0,
+                                                "type": "Line"
+                                            },
+                                            "type": "Product"
+                                        }
+                                    }
+                                ],
+                                "title": "Request"
                             }
                         }
                     },
                     "required": true
                 },
                 "responses": {
                     "200": {
@@ -451,32 +467,34 @@
         "/smalleststep": {
             "post": {
                 "description": "Calculate the smallest step in a scan, both absolutely and per-axis.\n\nIgnore any steps of size 0.\n\nArgs:\n    spec: The spec of the scan\n\nReturns:\n    SmallestStepResponse: A description of the smallest steps in the spec",
                 "operationId": "smallest_step_smalleststep_post",
                 "requestBody": {
                     "content": {
                         "application/json": {
-                            "example": {
-                                "inner": {
-                                    "axis": "x",
-                                    "num": 4,
-                                    "start": 0.0,
-                                    "stop": 10.0,
-                                    "type": "Line"
-                                },
-                                "outer": {
-                                    "axis": "y",
-                                    "num": 3,
-                                    "start": 0.0,
-                                    "stop": 10.0,
-                                    "type": "Line"
-                                },
-                                "type": "Product"
-                            },
                             "schema": {
+                                "examples": [
+                                    {
+                                        "inner": {
+                                            "axis": "x",
+                                            "num": 4,
+                                            "start": 0.0,
+                                            "stop": 10.0,
+                                            "type": "Line"
+                                        },
+                                        "outer": {
+                                            "axis": "y",
+                                            "num": 3,
+                                            "start": 0.0,
+                                            "stop": 10.0,
+                                            "type": "Line"
+                                        },
+                                        "type": "Product"
+                                    }
+                                ],
                                 "title": "Spec"
                             }
                         }
                     },
                     "required": true
                 },
                 "responses": {
@@ -507,32 +525,34 @@
         "/valid": {
             "post": {
                 "description": "Validate wether a ScanSpec can produce a viable scan.\n\nArgs:\n    spec: The scanspec to validate\n\nReturns:\n    ValidResponse: A canonical version of the spec if it is valid.\n        An error otherwise.",
                 "operationId": "valid_valid_post",
                 "requestBody": {
                     "content": {
                         "application/json": {
-                            "example": {
-                                "inner": {
-                                    "axis": "x",
-                                    "num": 4,
-                                    "start": 0.0,
-                                    "stop": 10.0,
-                                    "type": "Line"
-                                },
-                                "outer": {
-                                    "axis": "y",
-                                    "num": 3,
-                                    "start": 0.0,
-                                    "stop": 10.0,
-                                    "type": "Line"
-                                },
-                                "type": "Product"
-                            },
                             "schema": {
+                                "examples": [
+                                    {
+                                        "inner": {
+                                            "axis": "x",
+                                            "num": 4,
+                                            "start": 0.0,
+                                            "stop": 10.0,
+                                            "type": "Line"
+                                        },
+                                        "outer": {
+                                            "axis": "y",
+                                            "num": 3,
+                                            "start": 0.0,
+                                            "stop": 10.0,
+                                            "type": "Line"
+                                        },
+                                        "type": "Product"
+                                    }
+                                ],
                                 "title": "Spec"
                             }
                         }
                     },
                     "required": true
                 },
                 "responses": {
```

### Comparing `scanspec-0.6.1/src/scanspec/cli.py` & `scanspec-0.6.3/src/scanspec/cli.py`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/src/scanspec/core.py` & `scanspec-0.6.3/src/scanspec/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -503,15 +503,15 @@
     elif check_path_changes:
         # The top level is not snaking, so make sure there is an even
         # number of iterations of any snaking axis within it so it
         # doesn't jump when this frames object is iterated a second time
         for i, frames in enumerate(stack):
             # A SnakedFrames within a non-snaking top level must repeat
             # an even number of times
-            if isinstance(frames, SnakedFrames) and np.product(path.lengths[:i]) % 2:
+            if isinstance(frames, SnakedFrames) and np.prod(path.lengths[:i]) % 2:
                 raise ValueError(
                     f"Cannot squash SnakingFrames inside a non-snaking Frames "
                     f"when they do not repeat an even number of times "
                     f"otherwise {frames.axes()} would jump in position"
                 )
     return squashed
 
@@ -537,15 +537,15 @@
         self.stack = stack
         #: Index that is next to be consumed
         self.index = start
         #: The lengths of all the stack
         self.lengths = np.array([len(f) for f in stack])
         #: Index of the end frame, one more than the last index that will be
         #: produced
-        self.end_index = np.product(self.lengths)
+        self.end_index = np.prod(self.lengths)
         if num is not None and start + num < self.end_index:
             self.end_index = start + num
 
     def consume(self, num: Optional[int] = None) -> Frames[Axis]:
         """Consume at most num frames from the Path and return as a Frames object.
 
         >>> fx = SnakedFrames({"x": np.array([1, 2])})
@@ -566,15 +566,15 @@
         self.index = end_index
         stack: Frames[Axis] = Frames(
             {}, {}, {}, np.zeros(indices.shape, dtype=np.bool_)
         )
         # Example numbers below from a 2x3x4 ZxYxX scan
         for i, frames in enumerate(self.stack):
             # Number of times each frame will repeat: Z:12, Y:4, X:1
-            repeats = np.product(self.lengths[i + 1 :])
+            repeats = np.prod(self.lengths[i + 1 :])
             # Scan indices mapped to indices within Frames object:
             # Z:000000000000111111111111
             # Y:000011112222000011112222
             # X:012301230123012301230123
             if repeats > 1:
                 dim_indices = indices // repeats
             else:
@@ -630,15 +630,15 @@
         axes = []
         for frames in self.stack:
             axes += frames.axes()
         return axes
 
     def __len__(self) -> int:
         """The number of dictionaries that will be produced if iterated over."""
-        return int(np.product([len(frames) for frames in self.stack]))
+        return int(np.prod([len(frames) for frames in self.stack]))
 
     def __iter__(self) -> Iterator[Dict[Axis, float]]:
         """Yield {axis: midpoint} for each frame in the scan."""
         path = Path(self.stack)
         while len(path):
             frames = path.consume(1)
             yield {a: frames.midpoints[a][0] for a in frames.axes()}
```

### Comparing `scanspec-0.6.1/src/scanspec/plot.py` & `scanspec-0.6.3/src/scanspec/plot.py`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/src/scanspec/regions.py` & `scanspec-0.6.3/src/scanspec/regions.py`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/src/scanspec/service.py` & `scanspec-0.6.3/src/scanspec/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 _EXAMPLE_POINTS_REQUEST = PointsRequest(
     _EXAMPLE_SPEC, max_frames=1024, format=PointsFormat.FLOAT_LIST
 )
 
 
 @app.post("/valid", response_model=ValidResponse)
 def valid(
-    spec: Spec = Body(..., example=_EXAMPLE_SPEC)
+    spec: Spec = Body(..., examples=[_EXAMPLE_SPEC])
 ) -> Union[ValidResponse, JSONResponse]:
     """Validate wether a ScanSpec can produce a viable scan.
 
     Args:
         spec: The scanspec to validate
 
     Returns:
@@ -139,15 +139,15 @@
     return ValidResponse(spec, valid_spec)
 
 
 @app.post("/midpoints", response_model=MidpointsResponse)
 def midpoints(
     request: PointsRequest = Body(
         ...,
-        example=_EXAMPLE_POINTS_REQUEST,
+        examples=[_EXAMPLE_POINTS_REQUEST],
     )
 ) -> MidpointsResponse:
     """Generate midpoints from a scanspec.
 
     A scanspec can produce bounded points (i.e. a point is valid if an
     axis is between a minimum and and a maximum, see /bounds). The midpoints
     are the middle of each set of bounds.
@@ -167,15 +167,15 @@
     )
 
 
 @app.post("/bounds", response_model=BoundsResponse)
 def bounds(
     request: PointsRequest = Body(
         ...,
-        example=_EXAMPLE_POINTS_REQUEST,
+        examples=[_EXAMPLE_POINTS_REQUEST],
     )
 ) -> BoundsResponse:
     """Generate bounds from a scanspec.
 
     A scanspec can produce points with lower and upper bounds.
 
     Args:
@@ -194,15 +194,15 @@
     )
 
 
 @app.post("/gap", response_model=GapResponse)
 def gap(
     spec: Spec = Body(
         ...,
-        example=_EXAMPLE_SPEC,
+        examples=[_EXAMPLE_SPEC],
     )
 ) -> GapResponse:
     """Generate gaps from a scanspec.
 
     A scanspec may indicate if there is a gap between two frames.
     The array returned corresponds to whether or not there is a gap
     after each frame.
@@ -217,15 +217,15 @@
     path = Path(dims)  # Convert to a path
     gap = list(path.consume().gap)
     return GapResponse(gap)
 
 
 @app.post("/smalleststep", response_model=SmallestStepResponse)
 def smallest_step(
-    spec: Spec = Body(..., example=_EXAMPLE_SPEC)
+    spec: Spec = Body(..., examples=[_EXAMPLE_SPEC])
 ) -> SmallestStepResponse:
     """Calculate the smallest step in a scan, both absolutely and per-axis.
 
     Ignore any steps of size 0.
 
     Args:
         spec: The spec of the scan
```

### Comparing `scanspec-0.6.1/src/scanspec/specs.py` & `scanspec-0.6.3/src/scanspec/specs.py`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/src/scanspec/sphinxext.py` & `scanspec-0.6.3/src/scanspec/sphinxext.py`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/src/scanspec.egg-info/PKG-INFO` & `scanspec-0.6.3/src/scanspec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanspec
-Version: 0.6.1
+Version: 0.6.3
 Summary: Specify step and flyscan paths in a serializable, efficient and Pythonic way
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `scanspec-0.6.1/src/scanspec.egg-info/SOURCES.txt` & `scanspec-0.6.3/src/scanspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/tests/test_boilerplate_removed.py` & `scanspec-0.6.3/tests/test_boilerplate_removed.py`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/tests/test_cli.py` & `scanspec-0.6.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/tests/test_errors.py` & `scanspec-0.6.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/tests/test_iteration.py` & `scanspec-0.6.3/tests/test_iteration.py`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/tests/test_serialization.py` & `scanspec-0.6.3/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/tests/test_service.py` & `scanspec-0.6.3/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `scanspec-0.6.1/tests/test_specs.py` & `scanspec-0.6.3/tests/test_specs.py`

 * *Files identical despite different names*

