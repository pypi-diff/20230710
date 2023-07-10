# Comparing `tmp/kiara_plugin.onboarding-0.4.6.tar.gz` & `tmp/kiara_plugin.onboarding-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.onboarding-0.4.6.tar", last modified: Thu Jun 29 08:31:55 2023, max compression
+gzip compressed data, was "kiara_plugin.onboarding-0.4.7.tar", last modified: Mon Jul 10 13:50:57 2023, max compression
```

## Comparing `kiara_plugin.onboarding-0.4.6.tar` & `kiara_plugin.onboarding-0.4.7.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.458628 kiara_plugin.onboarding-0.4.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.github/workflows/build-linux.yaml.rej
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.458628 kiara_plugin.onboarding-0.4.6/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/ci/conda/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/ci/conda/kiara_plugin.onboarding/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/ci/conda/kiara_plugin.onboarding/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.458628 kiara_plugin.onboarding-0.4.6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/pipelines/example_pipeline_onboarding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.458628 kiara_plugin.onboarding-0.4.6/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1396 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.458628 kiara_plugin.onboarding-0.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.458628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/models/
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/files/import_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/utils/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-29 08:31:55.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-29 08:31:55.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:31:55.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-29 08:31:55.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:31:21.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-29 08:31:55.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 08:31:55.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.050374 kiara_plugin.onboarding-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.042374 kiara_plugin.onboarding-0.4.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.046374 kiara_plugin.onboarding-0.4.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.046374 kiara_plugin.onboarding-0.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/.github/workflows/build-linux.yaml.rej
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-10 13:50:57.050374 kiara_plugin.onboarding-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.042374 kiara_plugin.onboarding-0.4.7/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.046374 kiara_plugin.onboarding-0.4.7/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/ci/conda/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.046374 kiara_plugin.onboarding-0.4.7/ci/conda/kiara_plugin.onboarding/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/ci/conda/kiara_plugin.onboarding/meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.046374 kiara_plugin.onboarding-0.4.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.046374 kiara_plugin.onboarding-0.4.7/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.042374 kiara_plugin.onboarding-0.4.7/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.046374 kiara_plugin.onboarding-0.4.7/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.046374 kiara_plugin.onboarding-0.4.7/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.046374 kiara_plugin.onboarding-0.4.7/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.046374 kiara_plugin.onboarding-0.4.7/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/examples/pipelines/example_pipeline_onboarding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.042374 kiara_plugin.onboarding-0.4.7/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.046374 kiara_plugin.onboarding-0.4.7/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-10 13:50:57.050374 kiara_plugin.onboarding-0.4.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1396 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.042374 kiara_plugin.onboarding-0.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.042374 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.050374 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.050374 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.050374 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.050374 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/modules/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/modules/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/modules/files/import_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/modules/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.050374 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.050374 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.050374 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/utils/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.046374 kiara_plugin.onboarding-0.4.7/src/kiara_plugin.onboarding.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-10 13:50:57.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin.onboarding.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-10 13:50:57.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin.onboarding.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:50:57.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin.onboarding.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-10 13:50:57.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin.onboarding.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:50:24.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin.onboarding.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-10 13:50:57.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin.onboarding.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 13:50:57.000000 kiara_plugin.onboarding-0.4.7/src/kiara_plugin.onboarding.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.050374 kiara_plugin.onboarding-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:57.050374 kiara_plugin.onboarding-0.4.7/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-07-10 13:50:16.000000 kiara_plugin.onboarding-0.4.7/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.onboarding-0.4.6/.cruft.json` & `kiara_plugin.onboarding-0.4.7/.cruft.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.onboarding-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.onboarding-0.4.7/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/.github/workflows/build-darwin.yaml` & `kiara_plugin.onboarding-0.4.7/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/.github/workflows/build-linux.yaml` & `kiara_plugin.onboarding-0.4.7/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/.github/workflows/build-linux.yaml.rej` & `kiara_plugin.onboarding-0.4.7/.github/workflows/build-linux.yaml.rej`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/.github/workflows/build-windows.yaml` & `kiara_plugin.onboarding-0.4.7/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/.gitignore` & `kiara_plugin.onboarding-0.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/.pre-commit-config.yaml` & `kiara_plugin.onboarding-0.4.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/LICENSE` & `kiara_plugin.onboarding-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/Makefile` & `kiara_plugin.onboarding-0.4.7/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/PKG-INFO` & `kiara_plugin.onboarding-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.onboarding
-Version: 0.4.6
+Version: 0.4.7
 Summary: kiara modules for data onboarding.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.onboarding
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Keywords: kiara
```

### Comparing `kiara_plugin.onboarding-0.4.6/README.md` & `kiara_plugin.onboarding-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/ci/conda/kiara_plugin.onboarding/meta.yaml.template` & `kiara_plugin.onboarding-0.4.7/ci/conda/kiara_plugin.onboarding/meta.yaml.template`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/docs/development.md` & `kiara_plugin.onboarding-0.4.7/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/docs/index.md` & `kiara_plugin.onboarding-0.4.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.onboarding-0.4.7/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.onboarding-0.4.7/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/examples/pipelines/example_pipeline_onboarding.yaml` & `kiara_plugin.onboarding-0.4.7/examples/pipelines/example_pipeline_onboarding.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/mkdocs.yml` & `kiara_plugin.onboarding-0.4.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/pyproject.toml` & `kiara_plugin.onboarding-0.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,19 +26,20 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "kiara>=0.4.44",
+    "kiara>=0.4.46",
     "kiara_plugin.core_types>=0.4.20",
     "httpx>=0.23.0",
     "pyzenodo3>=1.0.2",
     "PyGithub>=1.58.0",
+    "pyzotero>=1.5.9"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
     "kiara[dev_documentation]"
 ]
```

### Comparing `kiara_plugin.onboarding-0.4.6/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.onboarding-0.4.7/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/scripts/documentation/gen_info_pages.py` & `kiara_plugin.onboarding-0.4.7/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/scripts/documentation/gen_module_doc.py` & `kiara_plugin.onboarding-0.4.7/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/setup.cfg` & `kiara_plugin.onboarding-0.4.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/setup.py` & `kiara_plugin.onboarding-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/__init__.py` & `kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/models/__init__.py` & `kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,14 +324,26 @@
             )
             if attach_metadata:
                 bundle.metadata["zenodo_record_data"] = record.data
 
         return bundle
 
 
+class FileFromZoteroModel(OnboardDataModel):
+
+    _kiara_model_id = "onboarding.file.from.zotero"
+
+    @classmethod
+    def accepts_uri(cls, uri: str) -> Tuple[bool, str]:
+        if uri.startswith("zotero:"):
+            return True, "uri is a zotero uri"
+        else:
+            return False, "uri is not a zotero uri, must start with 'zotero:'"
+
+
 class FileFromGithubModel(OnboardDataModel):
 
     _kiara_model_id: str = "onboarding.file.from.github"
 
     @classmethod
     def accepts_uri(cls, uri: str) -> Tuple[bool, str]:
 
@@ -371,20 +383,21 @@
             raise KiaraException(
                 msg=f"Can't parse github uri '{uri}' for single file download. Required format: 'gh:<user>/<repo>/<branch_or_tag>/<path>'"
             )
         else:
             sub_path = tokens[3]
 
         url = f"https://github.com/{tokens[0]}/{tokens[1]}/archive/refs/heads/{tokens[2]}.zip"
+        file_name = f"{tokens[1]}-{tokens[2]}.zip"
 
         archive_zip: KiaraFile
         archive_zip = download_file(  # type: ignore
             url=url,
             attach_metadata=attach_metadata,
-            file_name=f"{tokens[1]}-{tokens[2]}.zip",
+            file_name=file_name,
             return_md5_hash=False,
         )
 
         base_sub_path = f"{tokens[1]}-{tokens[2]}"
 
         if sub_path:
             if import_config.sub_path:
```

### Comparing `kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/__init__.py` & `kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/files/import_file.py` & `kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/modules/files/import_file.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py` & `kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/zenodo.py` & `kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/modules/zenodo.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/utils/download.py` & `kiara_plugin.onboarding-0.4.7/src/kiara_plugin/onboarding/utils/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 from typing import Dict, List, Mapping, Tuple, Type, Union
 
 from pydantic import BaseModel, Field
 
 from kiara.exceptions import KiaraException
 from kiara.models.filesystem import FolderImportConfig, KiaraFile, KiaraFileBundle
+from kiara.utils.files import unpack_archive
 from kiara_plugin.onboarding.models import OnboardDataModel
 
 
 class DownloadMetadata(BaseModel):
     url: str = Field(description="The url of the download request.")
     response_headers: List[Dict[str, str]] = Field(
         description="The response headers of the download request."
@@ -52,16 +53,26 @@
 ) -> Union[KiaraFile, Tuple[KiaraFile, str]]:
 
     import hashlib
 
     import httpx
     import pytz
 
+    if not file_name:
+        # TODO: make this smarter, using content-disposition headers if available
+        file_name = url.split("/")[-1]
+
     if not target:
-        tmp_file = tempfile.NamedTemporaryFile(delete=False)
+        tmp_file = tempfile.NamedTemporaryFile(delete=False, suffix=file_name)
+
+        def rm_tmp_file():
+            os.unlink(tmp_file.name)
+
+        atexit.register(rm_tmp_file)
+
         _target = Path(tmp_file.name)
     else:
         _target = Path(target)
         _target.parent.mkdir(parents=True, exist_ok=True)
 
     if return_md5_hash:
         hash_md5 = hashlib.md5()  # noqa
@@ -78,18 +89,14 @@
             for h in r.history:
                 history.append(dict(h.headers))
             for data in r.iter_bytes():
                 if return_md5_hash:
                     hash_md5.update(data)
                 f.write(data)
 
-    if not file_name:
-        # TODO: make this smarter, using content-disposition headers if available
-        file_name = url.split("/")[-1]
-
     result_file = KiaraFile.load_file(_target.as_posix(), file_name)
 
     if attach_metadata:
         metadata = {
             "url": url,
             "response_headers": history,
             "request_time": datetime.utcnow().replace(tzinfo=pytz.utc).isoformat(),
@@ -142,29 +149,30 @@
     out_dir = tempfile.mkdtemp()
 
     def del_out_dir():
         shutil.rmtree(out_dir, ignore_errors=True)
 
     atexit.register(del_out_dir)
 
-    error = None
-    try:
-        shutil.unpack_archive(tmp_file.name, out_dir)
-    except Exception:
-        # try patool, maybe we're lucky
-        try:
-            import patoolib
-
-            patoolib.extract_archive(tmp_file.name, outdir=out_dir)
-        except Exception as e:
-            error = e
-
-    if error is not None:
-        raise KiaraException(msg=f"Could not extract archive: {error}.")
+    # error = None
+    # try:
+    #     shutil.unpack_archive(tmp_file.name, out_dir)
+    # except Exception:
+    #     # try patool, maybe we're lucky
+    #     try:
+    #         import patoolib
+    #
+    #         patoolib.extract_archive(tmp_file.name, outdir=out_dir)
+    #     except Exception as e:
+    #         error = e
+    #
+    # if error is not None:
+    #     raise KiaraException(msg=f"Could not extract archive: {error}.")
 
+    unpack_archive(tmp_file.name, out_dir)
     bundle = KiaraFileBundle.import_folder(out_dir, import_config=import_config)
 
     if import_config is None:
         ic_dict = {}
     elif isinstance(import_config, FolderImportConfig):
         ic_dict = import_config.dict()
     else:
```

### Comparing `kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/PKG-INFO` & `kiara_plugin.onboarding-0.4.7/src/kiara_plugin.onboarding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.onboarding
-Version: 0.4.6
+Version: 0.4.7
 Summary: kiara modules for data onboarding.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.onboarding
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Keywords: kiara
```

### Comparing `kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/SOURCES.txt` & `kiara_plugin.onboarding-0.4.7/src/kiara_plugin.onboarding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/tests/conftest.py` & `kiara_plugin.onboarding-0.4.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.6/tests/test_job_descs.py` & `kiara_plugin.onboarding-0.4.7/tests/test_job_descs.py`

 * *Files identical despite different names*

