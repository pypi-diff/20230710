# Comparing `tmp/FAIRsoft-0.2.0.tar.gz` & `tmp/FAIRsoft-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FAIRsoft-0.2.0.tar", last modified: Mon Feb 27 10:48:36 2023, max compression
+gzip compressed data, was "FAIRsoft-0.2.1.tar", last modified: Mon Jul 10 11:06:17 2023, max compression
```

## Comparing `FAIRsoft-0.2.0.tar` & `FAIRsoft-0.2.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.923901 FAIRsoft-0.2.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.919901 FAIRsoft-0.2.0/FAIRsoft/
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-02-06 16:25:52.000000 FAIRsoft-0.2.0/FAIRsoft/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.919901 FAIRsoft-0.2.0/FAIRsoft/importers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.919901 FAIRsoft-0.2.0/FAIRsoft/importers/bioconda_biotools_galaxy_imp/
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-02-27 10:43:27.000000 FAIRsoft-0.2.0/FAIRsoft/importers/bioconda_biotools_galaxy_imp/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3268 2023-02-27 10:43:27.000000 FAIRsoft-0.2.0/FAIRsoft/importers/bioconda_biotools_galaxy_imp/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3585 2023-02-17 11:58:00.000000 FAIRsoft-0.2.0/FAIRsoft/importers/bioconda_biotools_galaxy_imp/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.919901 FAIRsoft-0.2.0/FAIRsoft/importers/bioconda_imp/
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-02-27 10:43:27.000000 FAIRsoft-0.2.0/FAIRsoft/importers/bioconda_imp/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     8180 2023-02-27 10:43:27.000000 FAIRsoft-0.2.0/FAIRsoft/importers/bioconda_imp/main.py
--rw-rw-rw-   0 root         (0) root         (0)     2335 2023-02-17 11:58:00.000000 FAIRsoft-0.2.0/FAIRsoft/importers/bioconda_imp/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.919901 FAIRsoft-0.2.0/FAIRsoft/importers/bioconductor_imp/
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-02-27 10:43:27.000000 FAIRsoft-0.2.0/FAIRsoft/importers/bioconductor_imp/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.923901 FAIRsoft-0.2.0/FAIRsoft/importers/opeb_metrics_imp/
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/FAIRsoft/importers/opeb_metrics_imp/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      784 2023-02-06 16:25:52.000000 FAIRsoft-0.2.0/FAIRsoft/importers/opeb_metrics_imp/import_from_file.py
--rw-rw-rw-   0 root         (0) root         (0)     2434 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/FAIRsoft/importers/opeb_metrics_imp/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3505 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/FAIRsoft/importers/opeb_metrics_imp/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.923901 FAIRsoft-0.2.0/FAIRsoft/importers/repositories_imp/
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/FAIRsoft/importers/repositories_imp/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-02-06 16:25:53.000000 FAIRsoft-0.2.0/FAIRsoft/importers/repositories_imp/importfrom_opeb.py
--rw-rw-rw-   0 root         (0) root         (0)     3702 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/FAIRsoft/importers/repositories_imp/main.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-02-06 16:25:53.000000 FAIRsoft-0.2.0/FAIRsoft/importers/repositories_imp/plus_enricher.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-02-06 16:25:53.000000 FAIRsoft-0.2.0/FAIRsoft/importers/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.923901 FAIRsoft-0.2.0/FAIRsoft/importers/sourceforge_imp/
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/FAIRsoft/importers/sourceforge_imp/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     6691 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/FAIRsoft/importers/sourceforge_imp/main.py
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/FAIRsoft/importers/sourceforge_imp/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.923901 FAIRsoft-0.2.0/FAIRsoft/importers/toolshed_imp/
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/FAIRsoft/importers/toolshed_imp/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-02-17 11:58:01.000000 FAIRsoft-0.2.0/FAIRsoft/importers/toolshed_imp/galaxy_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      362 2023-02-06 16:25:53.000000 FAIRsoft-0.2.0/FAIRsoft/importers/toolshed_imp/load_from_json.py
--rw-rw-rw-   0 root         (0) root         (0)     2749 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/FAIRsoft/importers/toolshed_imp/main.py
--rw-rw-rw-   0 root         (0) root         (0)    10845 2023-02-17 11:58:01.000000 FAIRsoft-0.2.0/FAIRsoft/importers/toolshed_imp/repos_config_importer.py
--rw-rw-rw-   0 root         (0) root         (0)     3073 2023-02-17 11:58:01.000000 FAIRsoft-0.2.0/FAIRsoft/importers/toolshed_imp/repos_metadata_importer.py
--rw-rw-rw-   0 root         (0) root         (0)     3743 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/FAIRsoft/importers/toolshed_imp/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.923901 FAIRsoft-0.2.0/FAIRsoft/indicators_evaluation/
--rw-rw-rw-   0 root         (0) root         (0)     3675 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/FAIRsoft/indicators_evaluation/FAIR_indicators_eval.py
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-02-06 16:25:53.000000 FAIRsoft-0.2.0/FAIRsoft/indicators_evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.923901 FAIRsoft-0.2.0/FAIRsoft/integration/
--rw-rw-rw-   0 root         (0) root         (0)     1134 2023-02-17 11:58:01.000000 FAIRsoft-0.2.0/FAIRsoft/integration/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    16603 2023-02-27 10:35:44.000000 FAIRsoft-0.2.0/FAIRsoft/integration/integration.py
--rw-rw-rw-   0 root         (0) root         (0)     4842 2023-02-06 16:25:54.000000 FAIRsoft-0.2.0/FAIRsoft/integration/run_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.923901 FAIRsoft-0.2.0/FAIRsoft/transformation/
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-02-06 16:43:23.000000 FAIRsoft-0.2.0/FAIRsoft/transformation/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    40027 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/FAIRsoft/transformation/meta_transformers.py
--rw-rw-rw-   0 root         (0) root         (0)     6376 2023-02-16 14:48:31.000000 FAIRsoft-0.2.0/FAIRsoft/transformation/transform_raw.py
--rw-rw-rw-   0 root         (0) root         (0)    30308 2023-02-27 10:35:44.000000 FAIRsoft-0.2.0/FAIRsoft/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.919901 FAIRsoft-0.2.0/FAIRsoft.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    10948 2023-02-27 10:48:36.000000 FAIRsoft-0.2.0/FAIRsoft.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1856 2023-02-27 10:48:36.000000 FAIRsoft-0.2.0/FAIRsoft.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-02-27 10:48:36.000000 FAIRsoft-0.2.0/FAIRsoft.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      707 2023-02-27 10:48:36.000000 FAIRsoft-0.2.0/FAIRsoft.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-02-27 10:48:36.000000 FAIRsoft-0.2.0/FAIRsoft.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-02-27 10:48:36.000000 FAIRsoft-0.2.0/FAIRsoft.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    34464 2023-02-06 16:25:54.000000 FAIRsoft-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10948 2023-02-27 10:48:36.923901 FAIRsoft-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10172 2023-02-27 10:43:29.000000 FAIRsoft-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1622 2023-02-27 10:47:35.000000 FAIRsoft-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-27 10:48:36.923901 FAIRsoft-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1684 2023-02-06 16:25:54.000000 FAIRsoft-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:48:36.923901 FAIRsoft-0.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2444 2023-02-06 16:25:54.000000 FAIRsoft-0.2.0/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)     6572 2023-02-06 16:25:54.000000 FAIRsoft-0.2.0/tests/test_transformation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.578972 FAIRsoft-0.2.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.574972 FAIRsoft-0.2.1/FAIRsoft/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-02-06 16:25:52.000000 FAIRsoft-0.2.1/FAIRsoft/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.574972 FAIRsoft-0.2.1/FAIRsoft/importers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.574972 FAIRsoft-0.2.1/FAIRsoft/importers/bioconda_biotools_galaxy_imp/
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-02-27 10:43:27.000000 FAIRsoft-0.2.1/FAIRsoft/importers/bioconda_biotools_galaxy_imp/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3268 2023-02-27 10:43:27.000000 FAIRsoft-0.2.1/FAIRsoft/importers/bioconda_biotools_galaxy_imp/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3585 2023-02-17 11:58:00.000000 FAIRsoft-0.2.1/FAIRsoft/importers/bioconda_biotools_galaxy_imp/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.574972 FAIRsoft-0.2.1/FAIRsoft/importers/bioconda_imp/
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-02-27 10:43:27.000000 FAIRsoft-0.2.1/FAIRsoft/importers/bioconda_imp/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     8180 2023-02-27 10:43:27.000000 FAIRsoft-0.2.1/FAIRsoft/importers/bioconda_imp/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     2335 2023-02-17 11:58:00.000000 FAIRsoft-0.2.1/FAIRsoft/importers/bioconda_imp/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.578972 FAIRsoft-0.2.1/FAIRsoft/importers/bioconductor_imp/
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-02-27 10:43:27.000000 FAIRsoft-0.2.1/FAIRsoft/importers/bioconductor_imp/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.578972 FAIRsoft-0.2.1/FAIRsoft/importers/opeb_metrics_imp/
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/FAIRsoft/importers/opeb_metrics_imp/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      784 2023-02-06 16:25:52.000000 FAIRsoft-0.2.1/FAIRsoft/importers/opeb_metrics_imp/import_from_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     2434 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/FAIRsoft/importers/opeb_metrics_imp/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3505 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/FAIRsoft/importers/opeb_metrics_imp/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.578972 FAIRsoft-0.2.1/FAIRsoft/importers/repositories_imp/
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/FAIRsoft/importers/repositories_imp/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-02-06 16:25:53.000000 FAIRsoft-0.2.1/FAIRsoft/importers/repositories_imp/importfrom_opeb.py
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/FAIRsoft/importers/repositories_imp/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-02-06 16:25:53.000000 FAIRsoft-0.2.1/FAIRsoft/importers/repositories_imp/plus_enricher.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-02-06 16:25:53.000000 FAIRsoft-0.2.1/FAIRsoft/importers/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.578972 FAIRsoft-0.2.1/FAIRsoft/importers/sourceforge_imp/
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/FAIRsoft/importers/sourceforge_imp/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     6691 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/FAIRsoft/importers/sourceforge_imp/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/FAIRsoft/importers/sourceforge_imp/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.578972 FAIRsoft-0.2.1/FAIRsoft/importers/toolshed_imp/
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/FAIRsoft/importers/toolshed_imp/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-02-17 11:58:01.000000 FAIRsoft-0.2.1/FAIRsoft/importers/toolshed_imp/galaxy_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      362 2023-02-06 16:25:53.000000 FAIRsoft-0.2.1/FAIRsoft/importers/toolshed_imp/load_from_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2749 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/FAIRsoft/importers/toolshed_imp/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    10845 2023-02-17 11:58:01.000000 FAIRsoft-0.2.1/FAIRsoft/importers/toolshed_imp/repos_config_importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3073 2023-02-17 11:58:01.000000 FAIRsoft-0.2.1/FAIRsoft/importers/toolshed_imp/repos_metadata_importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3743 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/FAIRsoft/importers/toolshed_imp/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.578972 FAIRsoft-0.2.1/FAIRsoft/indicators_evaluation/
+-rw-rw-rw-   0 root         (0) root         (0)     3675 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/FAIRsoft/indicators_evaluation/FAIR_indicators_eval.py
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-02-06 16:25:53.000000 FAIRsoft-0.2.1/FAIRsoft/indicators_evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.578972 FAIRsoft-0.2.1/FAIRsoft/integration/
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2023-02-17 11:58:01.000000 FAIRsoft-0.2.1/FAIRsoft/integration/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    16568 2023-07-10 10:54:31.000000 FAIRsoft-0.2.1/FAIRsoft/integration/integration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-07-10 10:54:31.000000 FAIRsoft-0.2.1/FAIRsoft/integration/run_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.578972 FAIRsoft-0.2.1/FAIRsoft/transformation/
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-02-06 16:43:23.000000 FAIRsoft-0.2.1/FAIRsoft/transformation/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    40027 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/FAIRsoft/transformation/meta_transformers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6376 2023-02-16 14:48:31.000000 FAIRsoft-0.2.1/FAIRsoft/transformation/transform_raw.py
+-rw-rw-rw-   0 root         (0) root         (0)    36404 2023-07-10 10:54:31.000000 FAIRsoft-0.2.1/FAIRsoft/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.574972 FAIRsoft-0.2.1/FAIRsoft.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    10948 2023-07-10 11:06:17.000000 FAIRsoft-0.2.1/FAIRsoft.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2023-07-10 11:06:17.000000 FAIRsoft-0.2.1/FAIRsoft.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-10 11:06:17.000000 FAIRsoft-0.2.1/FAIRsoft.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      707 2023-07-10 11:06:17.000000 FAIRsoft-0.2.1/FAIRsoft.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-10 11:06:17.000000 FAIRsoft-0.2.1/FAIRsoft.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-07-10 11:06:17.000000 FAIRsoft-0.2.1/FAIRsoft.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    34464 2023-02-06 16:25:54.000000 FAIRsoft-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10948 2023-07-10 11:06:17.578972 FAIRsoft-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10172 2023-02-27 10:43:29.000000 FAIRsoft-0.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2023-07-10 10:54:31.000000 FAIRsoft-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 11:06:17.578972 FAIRsoft-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1684 2023-02-06 16:25:54.000000 FAIRsoft-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:06:17.578972 FAIRsoft-0.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2023-02-06 16:25:54.000000 FAIRsoft-0.2.1/tests/test_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6572 2023-02-06 16:25:54.000000 FAIRsoft-0.2.1/tests/test_transformation.py
```

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/bioconda_biotools_galaxy_imp/main.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/bioconda_biotools_galaxy_imp/main.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/bioconda_biotools_galaxy_imp/utils.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/bioconda_biotools_galaxy_imp/utils.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/bioconda_imp/main.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/bioconda_imp/main.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/bioconda_imp/utils.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/bioconda_imp/utils.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/opeb_metrics_imp/import_from_file.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/opeb_metrics_imp/import_from_file.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/opeb_metrics_imp/main.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/opeb_metrics_imp/main.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/opeb_metrics_imp/utils.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/opeb_metrics_imp/utils.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/repositories_imp/main.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/repositories_imp/main.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/sourceforge_imp/main.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/sourceforge_imp/main.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/sourceforge_imp/utils.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/sourceforge_imp/utils.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/toolshed_imp/galaxy_metadata.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/toolshed_imp/galaxy_metadata.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/toolshed_imp/main.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/toolshed_imp/main.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/toolshed_imp/repos_config_importer.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/toolshed_imp/repos_config_importer.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/toolshed_imp/repos_metadata_importer.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/toolshed_imp/repos_metadata_importer.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/importers/toolshed_imp/utils.py` & `FAIRsoft-0.2.1/FAIRsoft/importers/toolshed_imp/utils.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/indicators_evaluation/FAIR_indicators_eval.py` & `FAIRsoft-0.2.1/FAIRsoft/indicators_evaluation/FAIR_indicators_eval.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/integration/cli.py` & `FAIRsoft-0.2.1/FAIRsoft/integration/cli.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/integration/integration.py` & `FAIRsoft-0.2.1/FAIRsoft/integration/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,15 +393,15 @@
         for inst in instaList:
             if inst.tags:
                 [tags.add(item) for item in inst.tags]
         newInst.tags = list(tags)
 
         # return instead of pushing to db
         inst=newInst.__dict__
-        inst['@id'] = "https://openebench.bsc.es/monitor/tool/{name}:{version}/{type}".format(name=inst['name'], version=inst['version'], type=inst['type'])
+        inst['@id'] = "https://openebench.bsc.es/monitor/tool/{name}/{type}".format(name=inst['name'], type=inst['type'])
         new_insts.append(inst)
 
     return(new_insts)
 
 
 def integrate_types(groupOfInstances):
     types = list(groupOfInstances.keys())
```

### Comparing `FAIRsoft-0.2.0/FAIRsoft/integration/run_integration.py` & `FAIRsoft-0.2.1/FAIRsoft/integration/run_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     
 @timeit
 def run_integration(loglevel=logging.INFO):
     logging.basicConfig(level=loglevel)
 
     HOST = os.getenv('HOST', 'localhost')
     PORT = os.getenv('PORT', 27017)
-    DB = os.getenv('DB', 'test')
+    DB = os.getenv('DB', 'observatory2')
     PRETOOLS = os.getenv('PRETOOLS', 'pretools') 
     TOOLS = os.getenv('TOOLS', 'tools') 
 
     STORAGE_MODE = os.getenv('STORAGE_MODE', 'db')
     if STORAGE_MODE == 'db':
         # un-integrated collection of instances (input instances)
         pretools = connect_collection(host=HOST, port=int(PORT), db=DB, collection=PRETOOLS)
```

### Comparing `FAIRsoft-0.2.0/FAIRsoft/transformation/cli.py` & `FAIRsoft-0.2.1/FAIRsoft/transformation/cli.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/transformation/meta_transformers.py` & `FAIRsoft-0.2.1/FAIRsoft/transformation/meta_transformers.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/transformation/transform_raw.py` & `FAIRsoft-0.2.1/FAIRsoft/transformation/transform_raw.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft/utils.py` & `FAIRsoft-0.2.1/FAIRsoft/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     'TOOLSHED',
     'GALAXY_METADATA',
     'SOURCEFORGE',
     'GALAXY_EU',
     'OPEB_METRICS',
     'BIOCONDA_RECIPES',
     'BIOCONDA_CONDA',
-    'REPOSITORIES'
+    'REPOSITORIES',
+    'GITHUB',
+    'BITBUCKET'
 ]
 
 # Labels of sources accross FAIRsoft pacakage. Must be consistent!!!! 
 # Present in:
 # 1.- 'sources' field in `instance`` objects (and anywhere they appear in code) 
 # 2.- toolGenerators in FAIRsoft.meta_transformers
 # if labels change in one place, they must change in the others for everythong to keep working
@@ -44,15 +46,17 @@
     'TOOLSHED':'toolshed',
     'GALAXY_METADATA':'galaxy_metadata',
     'SOURCEFORGE': 'sourceforge',
     'GALAXY_EU': 'galaxy',
     'OPEB_METRICS':'opeb_metrics',
     'BIOCONDA_RECIPES':'bioconda_recipes',
     'BIOCONDA_CONDA':'bioconda_conda',
-    'REPOSITORIES': 'repository'
+    'REPOSITORIES': 'repository',
+    'GITHUB': 'github',
+    'BITBUCKET': 'bitbucket'
 }
 
 # --------------------------------------------
 # Helper functions
 # --------------------------------------------
 def connect_collection(host:str='localhost', port:int=27017, db='test', collection:str='test'):
     '''Returns the collection object for the given collection name. 
@@ -290,62 +294,95 @@
                 # for now, a single True is enough, can be changed in the future, not allowing any False
             if True in vers_veredicts:
                 return(True)
         return(False)
 
     global struct_meta
     # TODO this list must depend on the analyzed sources. Take from config.yaml
-    struct_meta = ['biotools', 'bioconda', 'github', 'bitbucket', 'galaxy', 'toolshed', 'opeb_metrics']
+    struct_meta = ['biotools', 'bioconda', 'github', 'bitbucket', 'galaxy', 'toolshed', 'opeb_metrics', 'observatory']
     def compF2_1(self):
         '''
         Structured Metadata
         Metadata is adjusted to specific metdata formats
         The sources in struct_meta are structured. If these sources are among self.source: True. Otherwise: False
         '''
         if True in [a in struct_meta for a in self.source]:
             return(True)
         else:
             return(False)
 
     def compF2_2(self):
         '''
-        Ontologies or controlled vocabularies used
+        Whether the software is described using ontologies or controlled vocabularies.
+        Schema in observatory:
+        {
+            "vocabulary": "EDAM",
+            "term": "Topic",
+            "uri": "http://edamontology.org/topic_0003"
+        }
+        '''
+        # collect vocabularies/ontolgies used
+        def collectVeredicts(listItems, veredicts):
+            if listItems:
+                for t in listItems:
+                    if t['vocabulary'] != '':
+                        veredicts.append(True)
+                    else:
+                        veredicts.append(False)
+            
+            return(veredicts)
+
+        veredicts = []
+        veredicts = collectVeredicts(self.topics, veredicts)
+        veredicts = collectVeredicts(self.operations, veredicts)
+
+        # If at least one of the terms is described using a vocabulary/ontology: True. Otherwise: False
+        if True in veredicts:
+            return(True)
+        else:
+            return(False)
+
         '''
+        DEPRECATED:        
         # look for EDAM terms
         if self.semantics:
             for k in self.semantics.keys():
                 if self.semantics[k]:
                     return(True)
         return(False)
+        '''
 
 
     global softReg
     softReg = ['biotools', 'bioconda', 'bioconductor']
     def compF3_1(self):
         '''
         Searchability in registries
         Whether software is included in the main software registries.
-        If the source is among the software registries: True. Otherwise: Falsecource
+        If the source is among the software registries: True. Otherwise: False
         '''
         if True in [a in softReg for a in self.source]:
             return(True)
         else:
             return(False)
+        
+
 
     def compF3_2(self):
         '''
         Searchabiliy in software repositories
         Whether software can be found in any of the major software repositories e.g. GitHub, GitLab, SourceForge, 
         If the instance has an associated repository uri: True. Otherwise: False
         '''
         if len(self.repository)>0:
             return(True)
         else:
             return(False)
 
+
     def compF3_3(self):
         '''
         Searchability in literature.
         Whether software can be found in specialized literatue services e.g. EuropePMC, PubMed, Journals Site, bioArxiv.
         If the instance at least one associated publication: True. Otherwise: False
         '''
         if len(self.publication)>0:
@@ -395,15 +432,18 @@
 
     def compA1_4(self):
         '''
         Existence of test data
         Whether test data is available
         We check self.test (already a boolean)
         '''
-        return(self.test)
+        if self.test:
+            return(True)
+        else:
+            return(False)
 
     def compA1_5(self):
         '''
         NO WEB
         Existence of software source code
         Whether software source code is available 
         '''
@@ -413,33 +453,32 @@
             else:
                 return(False)
         else:
             return(False)
     
     def compA3_1(self):
         '''
-        WEB
         Registration not compulsory
         Whether homepage can be accessed without registration
         '''
-        if self.super_type == 'web':
-            return(self.operational)
-        else:
-            return(True)
+        return(self.registration_not_mandatory)
+
 
 
     def compA3_2(self):
         '''
         NO WEB
         Availability of version for free OS
         Whether the software can be used in a free operative system
         '''
         if self.super_type == 'no_web':
             if 'Linux' in self.os:
                 return(True)
+            elif 'FreeBSD' in self.os:
+                return(True)
             else:
                 return(False)
         else:
             return(True)
 
     def compA3_3(self):
         '''
@@ -495,27 +534,74 @@
         else:
             return(False)
 
     ##============== Interoperability metrics computation functions ================
     def compI1_1(self):
         '''
         Usage of standard data formats
-        Whether the input and output datatypes are formally specified and related to accepted ontologies
+        Whether the input and output datatypes are formally specified AND related to accepted ontologies
+        Exmaple: 
+        [
+            {   "vocabulary": "EDAM",
+                "term": "Sequence format",
+                "url": "http://edamontology.org/format_1929",
+                datatype: {
+                    "vocabulary": "EDAM",
+                    "term": "Sequence",
+                    "url": "http://edamontology.org/data_0006"
+                }
+            },
+            ...
+        ]
+        '''
+        # collect vocabularies/ontolgies used
+        def collectVeredicts(listItems, veredicts):
+            if listItems:
+                for t in listItems:
+                    if t['vocabulary'] != '':
+                        veredicts.append(True)
+                    else:
+                        veredicts.append(False)
+            
+            return(veredicts)
+
+        veredicts = []
+        veredicts = collectVeredicts(self.input, veredicts)
+        veredicts = collectVeredicts(self.output, veredicts)
+
+        # If at least one of the terms is described using a vocabulary/ontology: True. Otherwise: False
+        if True in veredicts:
+            return(True)
+        else:
+            return(False)
+
         '''
+        DEPRECATED
         for i in self.input:
             if 'format' in i.keys():
                 if i['format']['term'] in self.stdFormats:
                     return(True)
 
         for i in self.output:
             if 'format' in i.keys():
                 if i['format']['term'] in self.stdFormats:
                     return(True)
-
+        
         return(False)
+        '''
+    def compI1_2(self):
+        '''
+        API standard specification
+        '''
+        for item in self.documentation:
+            if item.type == 'API specification':
+                return(True)
+        
+        return False
+
 
     def compI1_3(self):
         '''
         Verificability of data formats
         Whether input/output data are specified using verifiable schemas (e.g. XDS, Json schema, ...)
         '''
         if self.compI1_1() == True:
@@ -531,32 +617,39 @@
         for term in terms:
             if term in verifiable_formats:
                 return(True)
 
         return(False)
 
 
-        return(False)
-
 
     def compI1_4(self):
         '''
         Flexibility of data format supported
         Whether the software allows to choose among various input/output data formats, or provide the necessary tools to convert other common formats into the supported ones.
         '''
+        if len(self.input)>1 and len(self.output)>1:
+            return(True)
+        else:
+            return(False)
+
+        '''
+        DEPRECATED
         ins = []
         formats = self.input + self.output
         for i in formats:
             if 'format' in i.keys():
                 ins.append(i['format']['term'])
 
         if len(ins)>1:
             return(True)
         else:
             return(False)
+        '''
+        
 
     def compI2_1(self):
         '''
         Existence of API/library version 
         Whether the software has API /library versions to be included in users' pipelines
         '''
         interTypes = ['Library', 'Web API']
@@ -590,73 +683,120 @@
 
     def compI3_2(self):
         '''
         Dependencies are provided
         Whether the software includes its dependencies or mechanisms to access them
         '''
         # checking source
-        if 'galaxyShed' in self.source:
+        if 'toolshed' in self.source:
             return(True)
         elif 'bioconda' in self.source:
             return(True)
         elif 'bioconductor' in self.source:
             return(True)
         
+        # registries 
+        accepted_registries = ['toolshed', 'bioconductor','conda', 'PyPI', 'CRAN', 'npm', 'CPAN', 'RubyGems', 'DockerHub', 'GitHub Container Registry', 'GitLab Container Registry', 'BioContainers']
+        for registry in self.registries:
+            if registry in accepted_registries:
+                return(True)
+        
         #checking links
-        sources_with_dependencies = ['bioconda', 'bioconductor', 'galaxy.']
+        sources_with_dependencies = ['bioconda', 'bioconductor', 'galaxy']
+        for url in self.links:
+            if True in  [a in url for a in sources_with_dependencies]:
+                return(True)
+        
+        return(False)
+    
+    def compI3_3(self):
+        '''
+        Dependency-aware system
+        '''
+        # registries 
+        accepted_registries = ['toolshed', 'bioconductor','conda', 'PyPI', 'CRAN', 'npm', 'CPAN', 'RubyGems']
+        for registry in self.registries:
+            if registry in accepted_registries:
+                return(True)
+        
+        #checking links
+        sources_with_dependencies = ['bioconda', 'bioconductor', 'galaxy']
         for url in self.links:
             if True in  [a in url for a in sources_with_dependencies]:
                 return(True)
         
         return(False)
 
     # ===================== Reusability ==============================================================
     def compR1_1(self):
         '''
         Existence of usage guides
         Whether software user guides are provided
-        '''
-        noGuide = ['license', 'terms of use', 'news']
-        for doc in self.documentation:
+        Documentation format: list of dictionaries
+        [
+            {
+                "type": "general",
+                "url": "https://bio.tools/api/tool/blast2go/docs/1.0.0"
+            },
+            ...
+        ]   
+        '''
+        # documentation types that are not guides for the user
+        noGuide = ['license', 'terms of use', 'news', 'contribution', 'citation', 'contact', 'changelog', 'release']
+        for individual_document in self.documentation:
             for string in noGuide:
-                if string not in doc[0].lower(): # doc[0] is the type of document
+                if string not in individual_document['type'].lower(): # doc[0] is the type of document
                     return(True)
 
         return(False)
 
 
     def compR2_1(self):
         '''
         Existence of license
         Whether license is stated
         '''
-        
+        '''
+        DEPRECATED 
+        # license can be part of the documentation
         for doc in self.documentation:
             if 'license' in doc[0].lower():
                 print('In doc')
                 return(True)
+        '''
+        for doc in self.documentation:
+            if 'license' in doc['type'].lower():
+                return(True)
+            elif 'terms of use' in doc['type'].lower():
+                return(True)
+            elif 'conditions of use' in doc['type'].lower():
+                return(True)
         
+        # or it can be specified in the license field
         if self.license:
             if len(self.license)>0:
                 for a in self.license:
                     # some licenses are actually a list of one license in old versions of ETL
-                    if type(a) == list:
-                        a = a[0]
-                    if a.lower()=='unlicensed' or a.lower()=='unknown' or a.lower()=='unlicense':
+                    license_name = a.name
+                    if type(license_name) == list:
+                        license_name = license_name[0]
+                    if license_name.lower()=='unlicensed' or license_name.lower()=='unknown' or license_name.lower()=='unlicense':
                         continue
                     else:
-                        if a:
+                        if license_name:
                             return(True)
         return(False)
         
     
     def compR2_2(self):
         '''
         Technical conditions of use
         '''
+        '''
+        DEPRECATED
         for doc in self.documentation:
             if 'conditions of use' in doc[0].lower():
                 return(True)
             elif 'terms of use' in doc[0].lower():
                 return(True)
         if self.license:
             if len(self.license)>0:
@@ -667,40 +807,85 @@
                     if a.lower()=='unlicensed' or a.lower()=='unknown' or a.lower()=='unlicense':
                         continue
                     else:
                         if a:
                             return(True)
 
         return(False)
+        '''
+        for doc in self.documentation:
+            if 'conditions of use' in doc['type'].lower():
+                return(True)
+            elif 'terms of use' in doc['type'].lower():
+                return(True)
+        if self.license:
+            if len(self.license)>0:
+                for a in self.license:
+                    # some licenses are actually a list of one license in old versions of ETL
+                    license_name = a.name
+                    if type(license_name) == list:
+                        license_name = license_name[0]
+                    if license_name.lower()=='unlicensed' or license_name.lower()=='unknown' or license_name.lower()=='unlicense':
+                        continue
+                    else:
+                        if license_name:
+                            return(True)
+        return(False)        
+    
+
+    def compR3_1(self):
+        '''
+        contribution policy
+        '''
+        for item in self.documentation:
+            if item.type == 'contribution policy':
+                return(True)
         
+        return False
     
 
-    #def compR3_1(self):
     def compR3_2(self):
         '''
         Existence of credit
         Whether credit for contributions is provided
         '''
         if len(self.authors)>0:
             return(True)
         else:
             return(False)
 
 
     def compR4_1(self):
         '''
-        Usage of version control
+        Usage of (public) version control
         Whether the software follows a version-control system
         '''
+        if self.version_control:
+            return(True)
+        else:
+            return(False)
+        
+        '''
+        DEPRECATED
         for repo in self.repository:
             if 'github' in repo or 'mercurial-scm' in repo:
                 return(True)
         return(False)
+        '''
 
-
+    def compR4_2(self):
+        '''
+        Release Policy
+        '''
+        for item in self.documentation:
+            if item.type == 'release policy':
+                return(True)
+        
+        return False
+    
 
     def FAIRscores(self):
         self.scores = FAIRscores()
         # ===================== Findability =========================
         # F1
         self.scores.F1 = (0.8*self.metrics.F1_1 
                         + 0.2*self.metrics.F1_2)
@@ -742,15 +927,15 @@
         #  A_2 not computable bc we do not have the appropriate metrics.
         #  self.A += (self.metrics.A2_1*(1/3)+self.metrics.A2_2*(2/3))*0.15
         
         # ===================== Interoperability =====================
 
         # I1
         self.scores.I1 = (0.5*self.metrics.I1_1
-                        + 0.3*self.metrics.I1_2
+                        + 0.3*self.metrics.I1_2 # I1.2 is not measured so equals 0
                         + 0.3*self.metrics.I1_3
                         + 0.2*self.metrics.I1_4)
         # I2
         self.scores.I2 = (0.5*self.metrics.I2_1
                         + 0.5*self.metrics.I2_2)
         # I3
         self.scores.I3 = (1/3)*(self.metrics.I3_1
@@ -808,37 +993,37 @@
         self.metrics.A3_1 = self.compA3_1() # Registration compulsory
         self.metrics.A3_2 = self.compA3_2() # Availability of version for free OS
         self.metrics.A3_3 = self.compA3_3() # Availability for several OS
         self.metrics.A3_4 = self.compA3_4() # Availability on free e-Infrastructures
         self.metrics.A3_5 = self.compA3_4() # Availability on several e-Infrastructures
 
         self.metrics.I1_1 = self.compI1_1()  # Usage of standard data formats
-        self.metrics.I1_2 = False # NOT FOR NOW # Usage of standard API framework
+        self.metrics.I1_2 = self.compI1_2() # ONLY EVALUATOR
         self.metrics.I1_3 = self.compI1_3() # Verificability of data formats
         self.metrics.I1_4 = self.compI1_4() # Flexibility of data format supported
         self.metrics.I1_5 = False # NOT FOR NOW # Generation of provenance information
 
         self.metrics.I2_1 = self.compI2_1() # Existance of API/library version 
         self.metrics.I2_2 = self.compI2_2() # E-infrastructure compatibility
 
         self.metrics.I3_1 = self.compI3_1()
         self.metrics.I3_2 = self.compI3_2()
-        self.metrics.I3_3 = self.compI3_2() # Same as befor, BY NOW
+        self.metrics.I3_3 = self.compI3_2() # Same as I3_2, BY NOW
 
         self.metrics.R1_1 = self.compR1_1()
         self.metrics.R1_2 = False #NOT FOR NOW
 
         self.metrics.R2_1 = self.compR2_1()
         self.metrics.R2_2 = self.compR2_2()
 
-        self.metrics.R3_1 = False # Not for now
+        self.metrics.R3_1 = self.compR3_1() # ONLY EVALUATOR
         self.metrics.R3_2 = self.compR3_2()
 
         self.metrics.R4_1 = self.compR4_1()
-        self.metrics.R4_2 = False # By now
+        self.metrics.R4_2 = self.compR4_2() # ONLY EVALUATOR
         self.metrics.R4_3 = False # By now
 
 
 class FAIRscores():
     def __init__(self):
         
         self.F = 0.0
```

### Comparing `FAIRsoft-0.2.0/FAIRsoft.egg-info/PKG-INFO` & `FAIRsoft-0.2.1/FAIRsoft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FAIRsoft
-Version: 0.2.0
+Version: 0.2.1
 Summary: FAIRsoft package for the aggregation of Life Sciences software metadata and FAIR evaluation.
 Home-page: https://gitlab.bsc.es/inb/elixir/software-observatory/FAIRsoft_ETL/-/tree/master/FAIRsoft
 Author: Eva Martin del Pico
 Author-email: Eva Martin del Pico <eva.martin@bsc.es>
 License: AGLP-3.0
 Project-URL: Bug Tracker, https://gitlab.bsc.es/inb/elixir/software-observatory/FAIRsoft_ETL/issues
 Project-URL: Repository, https://gitlab.bsc.es/inb/elixir/software-observatory/FAIRsoft_ETL/-/tree/master/FAIRsoft
```

### Comparing `FAIRsoft-0.2.0/FAIRsoft.egg-info/SOURCES.txt` & `FAIRsoft-0.2.1/FAIRsoft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/FAIRsoft.egg-info/entry_points.txt` & `FAIRsoft-0.2.1/FAIRsoft.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/LICENSE` & `FAIRsoft-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/PKG-INFO` & `FAIRsoft-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FAIRsoft
-Version: 0.2.0
+Version: 0.2.1
 Summary: FAIRsoft package for the aggregation of Life Sciences software metadata and FAIR evaluation.
 Home-page: https://gitlab.bsc.es/inb/elixir/software-observatory/FAIRsoft_ETL/-/tree/master/FAIRsoft
 Author: Eva Martin del Pico
 Author-email: Eva Martin del Pico <eva.martin@bsc.es>
 License: AGLP-3.0
 Project-URL: Bug Tracker, https://gitlab.bsc.es/inb/elixir/software-observatory/FAIRsoft_ETL/issues
 Project-URL: Repository, https://gitlab.bsc.es/inb/elixir/software-observatory/FAIRsoft_ETL/-/tree/master/FAIRsoft
```

### Comparing `FAIRsoft-0.2.0/README.md` & `FAIRsoft-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/pyproject.toml` & `FAIRsoft-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FAIRsoft"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Eva Martin del Pico", email="eva.martin@bsc.es" },
 ]
 description = "FAIRsoft package for the aggregation of Life Sciences software metadata and FAIR evaluation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `FAIRsoft-0.2.0/setup.py` & `FAIRsoft-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/tests/test_integration.py` & `FAIRsoft-0.2.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `FAIRsoft-0.2.0/tests/test_transformation.py` & `FAIRsoft-0.2.1/tests/test_transformation.py`

 * *Files identical despite different names*

