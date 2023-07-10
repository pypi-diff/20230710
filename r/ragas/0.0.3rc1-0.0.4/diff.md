# Comparing `tmp/ragas-0.0.3rc1.tar.gz` & `tmp/ragas-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragas-0.0.3rc1.tar", last modified: Fri Jun  9 07:33:07 2023, max compression
+gzip compressed data, was "ragas-0.0.4.tar", last modified: Mon Jul 10 07:38:47 2023, max compression
```

## Comparing `ragas-0.0.3rc1.tar` & `ragas-0.0.4.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.577437 ragas-0.0.3rc1/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.561436 ragas-0.0.3rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-09 07:33:07.577437 ragas-0.0.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/docs/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/docs/metrics.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/examples/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/examples/quickstart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/experiments/assesments/
--rw-r--r--   0 runner    (1001) docker     (123)    22724 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/assesments/metrics_assesments.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.565436 ragas-0.0.3rc1/experiments/baselines/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/experiments/baselines/fiqa/
--rw-r--r--   0 runner    (1001) docker     (123)    47444 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/fiqa/fiqa_baseline.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/fiqa/improving-baselines.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/experiments/baselines/hotpotqa/
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/hotpotqa/explore-dataset.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.573436 ragas-0.0.3rc1/experiments/baselines/wikiqa/
--rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/wikiqa/failed_wikis
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/wikiqa/wikiqa_docs.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/wikiqa/wikiqa_llamaindex_baseline.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/references.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.573436 ragas-0.0.3rc1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 07:33:07.577437 ragas-0.0.3rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.565436 ragas-0.0.3rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.573436 ragas-0.0.3rc1/src/ragas/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-09 07:33:07.000000 ragas-0.0.3rc1/src/ragas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.573436 ragas-0.0.3rc1/src/ragas/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/metrics/answer_relevance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/metrics/context_relevance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/metrics/factual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/metrics/llms.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.573436 ragas-0.0.3rc1/src/ragas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-09 07:33:07.000000 ragas-0.0.3rc1/src/ragas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-09 07:33:07.000000 ragas-0.0.3rc1/src/ragas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 07:33:07.000000 ragas-0.0.3rc1/src/ragas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-09 07:33:07.000000 ragas-0.0.3rc1/src/ragas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 07:33:07.000000 ragas-0.0.3rc1/src/ragas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.565436 ragas-0.0.3rc1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.573436 ragas-0.0.3rc1/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/tests/benchmarks/benchmark_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/tests/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.577437 ragas-0.0.3rc1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/tests/unit/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/tests/unit/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.665151 ragas-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 07:38:22.000000 ragas-0.0.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.653150 ragas-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.657150 ragas-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-10 07:38:22.000000 ragas-0.0.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-10 07:38:22.000000 ragas-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-10 07:38:22.000000 ragas-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 07:38:22.000000 ragas-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-10 07:38:22.000000 ragas-0.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-10 07:38:47.665151 ragas-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-10 07:38:22.000000 ragas-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.657150 ragas-0.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.657150 ragas-0.0.4/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-10 07:38:22.000000 ragas-0.0.4/docs/assets/bar-graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-07-10 07:38:22.000000 ragas-0.0.4/docs/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.657150 ragas-0.0.4/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-10 07:38:22.000000 ragas-0.0.4/docs/guides/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-10 07:38:22.000000 ragas-0.0.4/docs/metrics.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-10 07:38:22.000000 ragas-0.0.4/docs/quickstart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.657150 ragas-0.0.4/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-10 07:38:22.000000 ragas-0.0.4/experiments/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.657150 ragas-0.0.4/experiments/assesments/
+-rw-r--r--   0 runner    (1001) docker     (123)    26468 2023-07-10 07:38:22.000000 ragas-0.0.4/experiments/assesments/metrics_assesments.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.653150 ragas-0.0.4/experiments/baselines/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.657150 ragas-0.0.4/experiments/baselines/fiqa/
+-rw-r--r--   0 runner    (1001) docker     (123)    47254 2023-07-10 07:38:22.000000 ragas-0.0.4/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 07:38:23.000000 ragas-0.0.4/experiments/baselines/fiqa/fiqa_baseline.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-07-10 07:38:23.000000 ragas-0.0.4/experiments/baselines/fiqa/improving-baselines.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.661151 ragas-0.0.4/experiments/baselines/hotpotqa/
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-10 07:38:23.000000 ragas-0.0.4/experiments/baselines/hotpotqa/explore-dataset.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.661151 ragas-0.0.4/experiments/baselines/wikiqa/
+-rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-07-10 07:38:23.000000 ragas-0.0.4/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-10 07:38:23.000000 ragas-0.0.4/experiments/baselines/wikiqa/failed_wikis
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-10 07:38:23.000000 ragas-0.0.4/experiments/baselines/wikiqa/wikiqa_docs.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 07:38:23.000000 ragas-0.0.4/experiments/baselines/wikiqa/wikiqa_llamaindex_baseline.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-10 07:38:23.000000 ragas-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-10 07:38:23.000000 ragas-0.0.4/references.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.661151 ragas-0.0.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 07:38:23.000000 ragas-0.0.4/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 07:38:23.000000 ragas-0.0.4/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 07:38:47.665151 ragas-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.653150 ragas-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.661151 ragas-0.0.4/src/ragas/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-10 07:38:23.000000 ragas-0.0.4/src/ragas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-10 07:38:23.000000 ragas-0.0.4/src/ragas/_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 07:38:47.000000 ragas-0.0.4/src/ragas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-10 07:38:23.000000 ragas-0.0.4/src/ragas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 07:38:23.000000 ragas-0.0.4/src/ragas/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.665151 ragas-0.0.4/src/ragas/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-10 07:38:23.000000 ragas-0.0.4/src/ragas/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-07-10 07:38:23.000000 ragas-0.0.4/src/ragas/metrics/answer_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-10 07:38:23.000000 ragas-0.0.4/src/ragas/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-10 07:38:23.000000 ragas-0.0.4/src/ragas/metrics/context_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-07-10 07:38:23.000000 ragas-0.0.4/src/ragas/metrics/factual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-10 07:38:23.000000 ragas-0.0.4/src/ragas/metrics/llms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-10 07:38:23.000000 ragas-0.0.4/src/ragas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.661151 ragas-0.0.4/src/ragas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-10 07:38:47.000000 ragas-0.0.4/src/ragas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-10 07:38:47.000000 ragas-0.0.4/src/ragas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:38:47.000000 ragas-0.0.4/src/ragas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-10 07:38:47.000000 ragas-0.0.4/src/ragas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 07:38:47.000000 ragas-0.0.4/src/ragas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.653150 ragas-0.0.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.665151 ragas-0.0.4/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-10 07:38:23.000000 ragas-0.0.4/tests/benchmarks/benchmark_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-10 07:38:23.000000 ragas-0.0.4/tests/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:38:47.665151 ragas-0.0.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-10 07:38:23.000000 ragas-0.0.4/tests/unit/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 07:38:23.000000 ragas-0.0.4/tests/unit/test_simple.py
```

### Comparing `ragas-0.0.3rc1/.github/workflows/ci.yaml` & `ragas-0.0.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3rc1/.github/workflows/python-publish.yml` & `ragas-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3rc1/.gitignore` & `ragas-0.0.4/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -162,7 +162,8 @@
 # Ragas specific
 ragas/_version.py
 experiments/**/data
 experiments/**/storage
 **/fil-result/
 experiments/baselines/fiqa/datasets
 src/ragas/_version.py
+.python-version
```

### Comparing `ragas-0.0.3rc1/LICENSE` & `ragas-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3rc1/Makefile` & `ragas-0.0.4/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[33m%-30s\033[0m %s\n", $$1, $$2}'
 
 .PHONY: format lint type style clean run-benchmarks
 format: ## Running code formatter: black and isort
 	@echo "(isort) Ordering imports..."
 	@isort .
 	@echo "(black) Formatting codebase..."
-	@black --config pyproject.toml src tests examples experiments
+	@black --config pyproject.toml src tests docs experiments
 	@echo "(black) Formatting stubs..."
 	@find src -name "*.pyi" ! -name "*_pb2*" -exec black --pyi --config pyproject.toml {} \;
 	@echo "(ruff) Running fix only..."
-	@ruff check src examples tests --fix-only
+	@ruff check src docs tests --fix-only
 lint: ## Running lint checker: ruff
 	@echo "(ruff) Linting development project..."
-	@ruff check src examples tests
+	@ruff check src docs tests
 type: ## Running type checker: pyright
 	@echo "(pyright) Typechecking codebase..."
 	@pyright src
 clean: ## Clean all generated files
 	@echo "Cleaning all generated files..."
 	@cd $(GIT_ROOT)/docs && make clean
 	@cd $(GIT_ROOT) || exit 1
 	@find . -type f -name '*.py[co]' -delete -o -type d -name __pycache__ -delete
 run-ci: format lint type ## Running all CI checks
 run-benchmarks: ## Run benchmarks
 	@echo "Running benchmarks..."
-	@cd $(GIT_ROOT)/tests/benchmarks && python benchmark.py 
+	@cd $(GIT_ROOT)/tests/benchmarks && python benchmark_eval.py
 test: ## Run tests
 	@echo "Running tests..."
 	@pytest tests/unit
```

### Comparing `ragas-0.0.3rc1/docs/assets/logo.png` & `ragas-0.0.4/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3rc1/examples/data_prep.py` & `ragas-0.0.4/docs/guides/data_prep.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3rc1/experiments/README.md` & `ragas-0.0.4/experiments/README.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3rc1/experiments/assesments/metrics_assesments.ipynb` & `ragas-0.0.4/experiments/assesments/metrics_assesments.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9713673562885803%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, '- Faithfulness NLI\\n'), (5, '        - generated non "*

 * *            "factual answer for measuring faithfulness agreement.\\n')], delete: [5, 1]}}, 1: "*

 * *            "{'execution_count': 6}, 2: {'execution_count': 7, 'source': "*

 * *            '[\'os.chdir("/Users/shahules/belar/src/")\']}, 3: {\'execution_count\': 8}, 4: '*

 * *            "{'execution_count': 9}, 6: {'execution_count': 10}, 7: {'execution_count': 11}, 9: "*

 * *            "{'execution_count': 12, 'outputs': {0 […]*

```diff
@@ -2,19 +2,19 @@
     "cells": [
         {
             "cell_type": "markdown",
             "id": "d341594d",
             "metadata": {},
             "source": [
                 "## Logs\n",
-                "- Factuality NLI\n",
+                "- Faithfulness NLI\n",
                 "    - Without CoT\n",
                 "    - With CoT ( WIN)  \n",
                 "    - WikiQA \n",
-                "        - generated non factual answer for measuring factuality agreement.\n",
+                "        - generated non factual answer for measuring faithfulness agreement.\n",
                 "        - Kendall Score = 0.7\n",
                 "    - HotPotQA\n",
                 "        - Accuracy = 0.75 \n",
                 "    - Possible Improvements \n",
                 "        - improve statement generation\n",
                 "\n",
                 "- Relevance scores\n",
@@ -28,15 +28,15 @@
                 "        - WikiQA\n",
                 "            - kendall score = 0.63\n",
                 "            "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 6,
             "id": "7bfb2480",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
@@ -55,35 +55,35 @@
                 "import numpy as np\n",
                 "import random\n",
                 "from scipy.stats import kendalltau, spearmanr"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 7,
             "id": "e4168502",
             "metadata": {},
             "outputs": [],
             "source": [
-                "os.chdir('/Users/shahules/belar/src/')"
+                "os.chdir(\"/Users/shahules/belar/src/\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 8,
             "id": "9adac051",
             "metadata": {},
             "outputs": [],
             "source": [
                 "OPENAI_KEY = json.load(open(\"/Users/shahules/openai-key.json\"))[\"jj\"]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 9,
             "id": "21e09881",
             "metadata": {},
             "outputs": [],
             "source": [
                 "os.environ[\"OPENAI_API_KEY\"] = OPENAI_KEY"
             ]
         },
@@ -93,15 +93,15 @@
             "metadata": {},
             "source": [
                 "## OpenAI API"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 10,
             "id": "4bce4c53",
             "metadata": {},
             "outputs": [],
             "source": [
                 "openai.api_key = OPENAI_KEY\n",
                 "\n",
                 "\n",
@@ -118,15 +118,15 @@
                 "        n=kwargs.get(\"n\", 1),\n",
                 "    )\n",
                 "    return response"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 11,
             "id": "4d9b4e31",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def json_logger(data, filename=\"nli_check\"):\n",
                 "    output = json.load(open(filename + \".json\"))\n",
                 "    output.append(data)\n",
@@ -140,24 +140,24 @@
             "metadata": {},
             "source": [
                 "## Datasets"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 12,
             "id": "f9f4280e",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "Found cached dataset parquet (/Users/shahules/.cache/huggingface/datasets/explodinggradients___parquet/explodinggradients--ragas-wikiqa-5b5116e5cb909aca/0.0.0/2a3b91fbd88a2c90d1dbbb32b460cf621d31bd5b05b934492fdef7d8d6f236ec)\n",
-                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:00<00:00, 242.78it/s]\n"
+                        "100%|\u2588| 1/\n"
                     ]
                 }
             ],
             "source": [
                 "wikiqa_ragas = load_dataset(\"explodinggradients/ragas-wikiqa\")"
             ]
         },
@@ -167,21 +167,22 @@
             "metadata": {},
             "source": [
                 "## Correlation"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 124,
             "id": "eca20daf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "def get_corr(target, prediction):\n",
-                "    return [kendalltau(x, y).correlation for x, y in zip(target, predictions)]"
+                "def get_corr(targets, predictions):\n",
+                "    scores = [kendalltau(x, y).correlation for x, y in zip(targets, predictions)]\n",
+                "    return [score if not np.isnan(score) else 0 for score in scores]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d5563146",
             "metadata": {},
             "source": [
@@ -189,15 +190,15 @@
                 "- Generate question and answer pair from `generated answer`.\n",
                 "- Given `context`, ask these questions\n",
                 "- Verify answer correctness"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 14,
             "id": "f3e35532",
             "metadata": {},
             "outputs": [],
             "source": [
                 "Question_generation = \"\"\"Given a text, extract {} noun phrases and create questions for each based on given text.\n",
                 "text: Albert Einstein was a German-born theoretical physicist, widely acknowledged to be one of the greatest and most influential physicists of all time. Best known for developing the theory of relativity, he also made important contributions to the development of the theory of quantum mechanics.\n",
                 "A: Germany\n",
@@ -221,15 +222,15 @@
                 "Number of incorrect answers:1\n",
                 "{}\n",
                 "Number of incorrect answers:\"\"\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 15,
             "id": "335081e3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def QAQG_fun(question, context, answer):\n",
                 "    \"\"\"\n",
                 "    returns number of factual inconsistencies.\n",
@@ -257,30 +258,30 @@
                 "    )\n",
                 "    output = llm(Answer_verification.format(prompt))[\"choices\"][0][\"text\"].strip()\n",
                 "    return int(output)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 16,
             "id": "b2642e5b",
             "metadata": {},
             "outputs": [],
             "source": [
                 "answer = \"The actress who played Lolita, Sue Lyon, was 14 at the time of filming.\"\n",
                 "question = \"What was the age of Sue Lyon when she played Lolita?\"\n",
                 "context = \"\"\"\n",
                 "Lolita is a 1962 psychological comedy-drama film[5] directed by Stanley Kubrick and based on the 1955 novel of the same title by Vladimir Nabokov, who is also credited with writing the screenplay. The film follows Humbert Humbert, a middle-aged literature lecturer who becomes sexually infatuated with Dolores Haze (nicknamed \"Lolita\"), a young adolescent girl. It stars James Mason, Shelley Winters, Peter Sellers and, as the titular character, Sue Lyon.\n",
                 "\n",
                 "Owing to restrictions imposed by the Motion Picture Production Code, the film toned down the most provocative aspects of the novel, sometimes leaving much to the audience's imagination. The actress who played Lolita, Sue Lyon, was 14 at the time of filming.\"\"\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 17,
             "id": "26ca4af4",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -289,15 +290,15 @@
                 },
                 {
                     "data": {
                         "text/plain": [
                             "0"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "QAQG_fun(question, context, answer)"
             ]
@@ -310,15 +311,15 @@
                 "## G-Eval\n",
                 "- Define criterions to evaluate model.\n",
                 "- Normalize `score = prob(s) * s`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 138,
             "id": "ca1c56d6",
             "metadata": {},
             "outputs": [],
             "source": [
                 "relevence = \"\"\"\n",
                 "Evaluation Criteria.\\n\n",
                 "Relevance (1-5) - how relevant is the reply to the given question.\n",
@@ -327,20 +328,62 @@
                 "2. The reply should include only required information to answer the question.\n",
                 "3. Penalize replies that contain redundancies and excess information.\n",
                 "4. Assign a score for Relevance on a scale of 1 to 5, where 1 is the lowest and\n",
                 "5 is the highest based on the Evaluation Criteria.\n",
                 "\n",
                 "question:{}\n",
                 "reply:{}\n",
+                "score:\"\"\"\n",
+                "\n",
+                "faithfulness = \"\"\"\n",
+                "Evaluation Criteria.\\n\n",
+                "Faithfulness (1-5) - how factually consistant is the reply with the given context.\n",
+                "1. Read the reply and compare it to the question. Check if the given reply\n",
+                "actually answers the question correctly, and if the reply is factualy consistent with the context.\n",
+                "2. Assign a score for faithfulness on a scale of 1 to 5, where 1 is the lowest and\n",
+                "5 is the highest based on the Evaluation Criteria.\n",
+                "\n",
+                "context: {}\n",
+                "question:{}\n",
+                "reply:{}\n",
                 "score:\"\"\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 156,
+            "id": "541c1423",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def gpt_faithfulness(question: list, context: list, answer: list):\n",
+                "    prompt = [\n",
+                "        faithfulness.format(c, q, a) for c, q, a in zip(question, context, answer)\n",
+                "    ]\n",
+                "    output = [output for output in llm(prompt)[\"choices\"]]\n",
+                "    scores = [(out[\"text\"].strip()) for out in output]\n",
+                "    scores = [\n",
+                "        int(score) if score in [\"1\", \"2\", \"3\", \"4\", \"5\"] else 1 for score in scores\n",
+                "    ]\n",
+                "    return scores\n",
+                "\n",
+                "\n",
+                "def gpt_relevance(question: list, answer: list):\n",
+                "    prompt = [relevence.format(q, a) for q, a in zip(question, answer)]\n",
+                "    output = [output for output in llm(prompt)[\"choices\"]]\n",
+                "    scores = [(out[\"text\"].strip()) for out in output]\n",
+                "    scores = [\n",
+                "        int(score) if score in [\"1\", \"2\", \"3\", \"4\", \"5\"] else 1 for score in scores\n",
+                "    ]\n",
+                "    return scores"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 89,
             "id": "cd7fed9c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def g_eval(question, context, answer):\n",
                 "    prompt = relevence.format(question, answer)\n",
                 "    output = llm(prompt)[\"choices\"][0]\n",
@@ -348,49 +391,98 @@
                 "    score = int(output[\"text\"].strip())\n",
                 "    print(score)\n",
                 "    return prob * score"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 90,
             "id": "35113558",
             "metadata": {},
             "outputs": [],
             "source": [
                 "question = \"Which year did Lolita release?\"\n",
                 "answer = \"Lolita film released in 1947.\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 54,
             "id": "4e82d0df",
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "5\n"
-                    ]
-                },
+                    "data": {
+                        "text/plain": [
+                            "5"
+                        ]
+                    },
+                    "execution_count": 54,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "gpt_relevance(question, answer)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 151,
+            "id": "a79b1780",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "q, a, c = (\n",
+                "    wikiqa_ragas[\"train\"][0][\"question\"],\n",
+                "    wikiqa_ragas[\"train\"][0][\"generated_without_rag\"],\n",
+                "    wikiqa_ragas[\"train\"][0][\"context\"],\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 152,
+            "id": "f25b046f",
+            "metadata": {},
+            "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "3.5533440372846865"
+                            "[4]"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 152,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "g_eval(question, context, answer)"
+                "gpt_faithfulness([q], [c], [a])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 91,
+            "id": "e158274f",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[4]"
+                        ]
+                    },
+                    "execution_count": 91,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "gpt_relevance([q], [a])"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6dce1baa",
             "metadata": {},
             "source": [
@@ -404,112 +496,176 @@
             "metadata": {},
             "source": [
                 "### QGen scoring method"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 35,
             "id": "cc263805",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from ragas.metrics.answer_relevance import QGen"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 36,
             "id": "38deaf06",
             "metadata": {},
             "outputs": [],
             "source": [
                 "t5_qgen = QGen(\"t5-base\", \"cpu\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 146,
             "id": "45942810",
             "metadata": {},
             "outputs": [],
             "source": [
-                "def predict_relevance(examples):\n",
+                "def predict_(examples):\n",
                 "    scores = {}\n",
                 "    questions = examples[\"question\"]\n",
+                "    context = examples[\"context\"]\n",
                 "    for col in COLUMNS:\n",
                 "        passage = examples[col]\n",
                 "        inputs = list(zip(questions, passage))\n",
-                "        scores[f\"{col}_relevance\"] = t5_qgen.predict(inputs, show_progress=False)\n",
+                "        # scores[f\"{col}_relevance\"] = t5_qgen.predict(inputs, show_progress=False)\n",
+                "        scores[f\"{col}_relevance\"] = gpt_faithfulness(questions, context, passage)\n",
                 "    return scores"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b1410f3c",
             "metadata": {},
             "source": [
                 "- We assume `generated_with_rag > correct_answer > incorrect_answer` for relevancy."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 142,
             "id": "ab00e4fe",
             "metadata": {},
             "outputs": [],
             "source": [
                 "COLUMNS = [\"generated_with_rag\", \"correct_answer\", \"incorrect_answer\"]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 130,
+            "execution_count": 139,
             "id": "e705767d",
             "metadata": {
                 "scrolled": false
             },
+            "outputs": [],
+            "source": [
+                "output = wikiqa_ragas[\"train\"].map(predict_relevance, batched=True, batch_size=10)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "3ab21cdf",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "predictions = [[item[f\"{k}_relevance\"] for k in COLUMNS] for item in output]\n",
+                "target = [[2, 1, 0] for i in range(len(output))]\n",
+                "np.mean(get_corr(target, predictions))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "6b2c5e1c",
+            "metadata": {},
+            "source": []
+        },
+        {
+            "cell_type": "markdown",
+            "id": "608a7ddb",
+            "metadata": {},
+            "source": [
+                "Relevance\n",
+                "\n",
+                "- 0.6337284370533437 for wikiQA gpt 3.5\n",
+                "\n",
+                "- 0.6831823238905629 For wikiwa t5"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "89d8ccbc",
+            "metadata": {},
+            "source": [
+                "## Faithfulness"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 157,
+            "id": "2f26f435",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "COLUMNS = [\"generated_with_rag\", \"correct_answer\", \"generated_without_rag\"]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 158,
+            "id": "a3a8fc48",
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Loading cached processed dataset at /Users/shahules/.cache/huggingface/datasets/explodinggradients___parquet/explodinggradients--ragas-wikiqa-5b5116e5cb909aca/0.0.0/2a3b91fbd88a2c90d1dbbb32b460cf621d31bd5b05b934492fdef7d8d6f236ec/cache-6b548dfc2a4d5a4f.arrow\n"
+                        "          \r"
                     ]
                 }
             ],
             "source": [
-                "output = (\n",
-                "    wikiqa_ragas[\"train\"]\n",
-                "    .select(range(0, 10))\n",
-                "    .map(predict_relevance, batched=True, batch_size=4)\n",
-                ")"
+                "output = wikiqa_ragas[\"train\"].map(predict_relevance, batched=True, batch_size=10)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 131,
-            "id": "3ab21cdf",
+            "execution_count": 159,
+            "id": "57f0b521",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "0.6518583971423787"
+                            "0.48110338184466117"
                         ]
                     },
-                    "execution_count": 131,
+                    "execution_count": 159,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "predictions = [[item[f\"{k}_relevance\"] for k in COLUMNS] for item in output]\n",
+                "predictions = [[item[f\"{k}_facuality\"] for k in COLUMNS] for item in output]\n",
                 "target = [[2, 1, 0] for i in range(len(output))]\n",
-                "get_corr(target, predictions)"
+                "np.mean(get_corr(target, predictions))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "c10aee98",
+            "metadata": {},
+            "source": [
+                "0.48110338184466117 for GPT3.5"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3d562351",
             "metadata": {},
             "source": [
@@ -570,15 +726,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "cefd9923",
             "metadata": {},
             "source": [
-                "## Factuality on HotpotQA\n"
+                "## Faithfulness on HotpotQA\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 134,
             "id": "2316c8dd",
             "metadata": {},
@@ -722,23 +878,23 @@
         {
             "cell_type": "code",
             "execution_count": 142,
             "id": "84f39785",
             "metadata": {},
             "outputs": [],
             "source": [
-                "def predict_factuality(examples):\n",
+                "def predict_faithfulness(examples, scoring_fun=NLI.score):\n",
                 "    scores = {}\n",
                 "    questions = examples[\"question\"]\n",
                 "    contexts = examples[\"answer_context\"]\n",
                 "    for col in COLUMNS:\n",
                 "        answers = examples[col]\n",
                 "        while True:\n",
                 "            try:\n",
-                "                scores[f\"{col}_factual\"] = NLI.score(questions, contexts, answers)\n",
+                "                scores[f\"{col}_factual\"] = scoring_fun(questions, contexts, answers)\n",
                 "            except Exception as e:\n",
                 "                print(e)\n",
                 "                continue\n",
                 "            break\n",
                 "    return scores"
             ]
         },
@@ -754,15 +910,15 @@
                     "text": [
                         "Loading cached processed dataset at /Users/shahules/.cache/huggingface/datasets/hotpot_qa/distractor/1.0.0/133b9501f892e5193babbad937bee3b4899deb4691ef4d791e6ac0111c875bb5/cache-d51f81546b2858f1.arrow\n"
                     ]
                 }
             ],
             "source": [
                 "COLUMNS = [\"answer\", \"false_answer\"]\n",
-                "hotpot_qa = hotpot_qa.map(predict_factuality, batched=True, batch_size=8)"
+                "hotpot_qa = hotpot_qa.map(predict_faithfulness, batched=True, batch_size=8)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 164,
             "id": "ca2cd14d",
             "metadata": {},
```

### Comparing `ragas-0.0.3rc1/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb` & `ragas-0.0.4/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983436367303433%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(4, 'url = (\\n'), (5, '    "*

 * *            '"https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/{}.zip".format(\\n\'), '*

 * *            "(6, '        dataset\\n'), (7, '    )\\n'), (8, ')\\n')], delete: [4]}}, 4: "*

 * *            "{'source': {insert: [(2, '\\n')], delete: [2]}}, 5: {'source': {insert: [(0, "*

 * *            '\'corpus_df = corpus_df.rename(columns={"_id": "corpus-id", "text": '*

 * *            '"ground_truth"})\\n\')], delete: [2, 1, 0]}}, 6: {\'source\ […]*

```diff
@@ -44,15 +44,19 @@
                 }
             ],
             "source": [
                 "from beir import util\n",
                 "from beir.datasets.data_loader import GenericDataLoader\n",
                 "\n",
                 "dataset = \"fiqa\"\n",
-                "url = \"https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/{}.zip\".format(dataset)\n",
+                "url = (\n",
+                "    \"https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/{}.zip\".format(\n",
+                "        dataset\n",
+                "    )\n",
+                ")\n",
                 "data_path = util.download_and_unzip(url, \"datasets\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "ad0b72cf",
@@ -214,15 +218,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "with open(os.path.join(data_path, \"corpus.jsonl\")) as f:\n",
                 "    cs = [pd.Series(json.loads(l)) for l in f.readlines()]\n",
-                "    \n",
+                "\n",
                 "corpus_df = pd.DataFrame(cs)\n",
                 "corpus_df"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
@@ -295,17 +299,15 @@
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "corpus_df = corpus_df.rename(columns={\n",
-                "    \"_id\": \"corpus-id\", \"text\": \"ground_truth\"\n",
-                "})\n",
+                "corpus_df = corpus_df.rename(columns={\"_id\": \"corpus-id\", \"text\": \"ground_truth\"})\n",
                 "corpus_df = corpus_df.drop(columns=[\"title\", \"metadata\"])\n",
                 "corpus_df[\"corpus-id\"] = corpus_df[\"corpus-id\"].astype(int)\n",
                 "corpus_df.head()"
             ]
         },
         {
             "cell_type": "code",
@@ -383,17 +385,15 @@
                 }
             ],
             "source": [
                 "with open(os.path.join(data_path, \"queries.jsonl\")) as f:\n",
                 "    qs = [pd.Series(json.loads(l)) for l in f.readlines()]\n",
                 "\n",
                 "queries_df = pd.DataFrame(qs)\n",
-                "queries_df = queries_df.rename(columns={\n",
-                "    \"_id\": \"query-id\", \"text\": \"question\"\n",
-                "})\n",
+                "queries_df = queries_df.rename(columns={\"_id\": \"query-id\", \"text\": \"question\"})\n",
                 "queries_df = queries_df.drop(columns=[\"metadata\"])\n",
                 "queries_df[\"query-id\"] = queries_df[\"query-id\"].astype(int)\n",
                 "queries_df.head()"
             ]
         },
         {
             "cell_type": "code",
@@ -470,18 +470,18 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "splits = [\"dev\", \"test\", \"train\"]\n",
                 "split_df = {}\n",
                 "for s in splits:\n",
-                "    split_df[s] = pd.read_csv(\n",
-                "        os.path.join(data_path, f\"qrels/{s}.tsv\"), sep=\"\\t\"\n",
-                "    ).drop(columns=[\"score\"])\n",
-                "    \n",
+                "    split_df[s] = pd.read_csv(os.path.join(data_path, f\"qrels/{s}.tsv\"), sep=\"\\t\").drop(\n",
+                "        columns=[\"score\"]\n",
+                "    )\n",
+                "\n",
                 "split_df[\"dev\"].head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "id": "97ea4840",
@@ -511,18 +511,22 @@
             "outputs": [],
             "source": [
                 "final_split_df = {}\n",
                 "for split in split_df:\n",
                 "    df = queries_df.merge(split_df[split], on=\"query-id\")\n",
                 "    df = df.merge(corpus_df, on=\"corpus-id\")\n",
                 "    df = df.drop(columns=[\"corpus-id\"])\n",
-                "    grouped = df.groupby('query-id').apply(lambda x: pd.Series({\n",
-                "        'question': x['question'].sample().values[0],\n",
-                "        'ground_truths': x['ground_truth'].tolist()\n",
-                "    }))\n",
+                "    grouped = df.groupby(\"query-id\").apply(\n",
+                "        lambda x: pd.Series(\n",
+                "            {\n",
+                "                \"question\": x[\"question\"].sample().values[0],\n",
+                "                \"ground_truths\": x[\"ground_truth\"].tolist(),\n",
+                "            }\n",
+                "        )\n",
+                "    )\n",
                 "\n",
                 "    grouped = grouped.reset_index()\n",
                 "    grouped = grouped.drop(columns=\"query-id\")\n",
                 "    final_split_df[split] = grouped"
             ]
         },
         {
@@ -793,19 +797,16 @@
                 "# change if new\n",
                 "path_to_ds_repo = \"../../../../datasets/fiqa/\"\n",
                 "import os\n",
                 "\n",
                 "assert os.path.exists(path_to_ds_repo), f\"{path_to_ds_repo} doesnot exist!\"\n",
                 "\n",
                 "for s in final_split_df:\n",
-                "    final_split_df[s].to_csv(\n",
-                "        os.path.join(path_to_ds_repo, f\"{s}.csv\"),\n",
-                "        index=False\n",
-                "    )\n",
-                "    \n",
+                "    final_split_df[s].to_csv(os.path.join(path_to_ds_repo, f\"{s}.csv\"), index=False)\n",
+                "\n",
                 "corpus_df.to_csv(os.path.join(path_to_ds_repo, \"corpus.csv\"), index=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8a661977",
             "metadata": {},
@@ -1005,26 +1006,19 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "# make nodes\n",
                 "from llama_index.node_parser import SimpleNodeParser\n",
                 "from langchain.text_splitter import TokenTextSplitter\n",
                 "\n",
-                "spliter = TokenTextSplitter(\n",
-                "    chunk_size = 100,\n",
-                "    chunk_overlap = 50\n",
-                ")\n",
+                "spliter = TokenTextSplitter(chunk_size=100, chunk_overlap=50)\n",
                 "\n",
-                "parser = SimpleNodeParser(\n",
-                "    text_splitter=spliter\n",
-                ")\n",
+                "parser = SimpleNodeParser(text_splitter=spliter)\n",
                 "\n",
-                "nodes = parser.get_nodes_from_documents(\n",
-                "    documents=docs\n",
-                ")"
+                "nodes = parser.get_nodes_from_documents(documents=docs)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 89,
             "id": "3bf6c119",
             "metadata": {},
@@ -1084,24 +1078,20 @@
             "execution_count": 92,
             "id": "66be5435",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# create index\n",
                 "index = GPTVectorStoreIndex.from_documents(\n",
-                "    documents=docs, \n",
+                "    documents=docs,\n",
                 "    service_context=openai_sc,\n",
                 ")\n",
                 "\n",
                 "# query with embed_model specified\n",
-                "qe = index.as_query_engine(\n",
-                "    mode=\"embedding\", \n",
-                "    verbose=True, \n",
-                "    service_context=openai_sc\n",
-                ")"
+                "qe = index.as_query_engine(mode=\"embedding\", verbose=True, service_context=openai_sc)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 93,
             "id": "4b3d899a",
             "metadata": {},
@@ -1167,18 +1157,15 @@
                 "storage_context = StorageContext.from_defaults(persist_dir=\"./storage\")\n",
                 "\n",
                 "# load index\n",
                 "index = load_index_from_storage(storage_context)\n",
                 "\n",
                 "# query with embed_model specified\n",
                 "qe = index.as_query_engine(\n",
-                "    mode=\"embedding\", \n",
-                "    verbose=True, \n",
-                "    service_context=openai_sc,\n",
-                "    use_async = False\n",
+                "    mode=\"embedding\", verbose=True, service_context=openai_sc, use_async=False\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 94,
             "id": "9816be1b",
@@ -1191,23 +1178,21 @@
                 ")\n",
                 "from llama_index.retrievers import VectorIndexRetriever\n",
                 "from llama_index.query_engine import RetrieverQueryEngine\n",
                 "from llama_index.indices.postprocessor import SimilarityPostprocessor\n",
                 "\n",
                 "# configure retriever\n",
                 "retriever = VectorIndexRetriever(\n",
-                "    index=index, \n",
+                "    index=index,\n",
                 "    similarity_top_k=3,\n",
                 ")\n",
                 "\n",
                 "# configure response synthesizer\n",
                 "response_synthesizer = ResponseSynthesizer.from_args(\n",
-                "    node_postprocessors=[\n",
-                "        SimilarityPostprocessor(similarity_cutoff=0.7)\n",
-                "    ]\n",
+                "    node_postprocessors=[SimilarityPostprocessor(similarity_cutoff=0.7)]\n",
                 ")\n",
                 "\n",
                 "# assemble query engine\n",
                 "qe = RetrieverQueryEngine(\n",
                 "    retriever=retriever,\n",
                 "    response_synthesizer=response_synthesizer,\n",
                 ")"
@@ -1253,17 +1238,18 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "def generate_response(row):\n",
                 "    r = qe.query(row[\"question\"])\n",
                 "    row[\"answer\"] = r.response\n",
                 "    row[\"contexts\"] = [sn.node.text for sn in r.source_nodes]\n",
-                "    \n",
+                "\n",
                 "    return row\n",
                 "\n",
+                "\n",
                 "# generate_response(test_ds[0])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 97,
             "id": "76037e00",
@@ -1523,21 +1509,18 @@
                     },
                     "execution_count": 98,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from ragas.metrics import factuality, answer_relevancy, context_relevancy\n",
+                "from ragas.metrics import faithfulness, answer_relevancy, context_relevancy\n",
                 "from ragas import evaluate\n",
                 "\n",
-                "evaluate(\n",
-                "    gen_ds, \n",
-                "    metrics=[factuality, answer_relevancy, context_relevancy]\n",
-                ")"
+                "evaluate(gen_ds, metrics=[faithfulness, answer_relevancy, context_relevancy])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "997df8cc",
             "metadata": {},
```

### Comparing `ragas-0.0.3rc1/experiments/baselines/fiqa/improving-baselines.ipynb` & `ragas-0.0.4/experiments/baselines/fiqa/improving-baselines.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9819807746468152%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['Found cached dataset fiqa "*

 * *            "(/home/jjmachan/.cache/huggingface/datasets/explodinggradients___fiqa/main/1.0.0/3dc7b639f5b4b16509a3299a2ceb78bf5fe98ee6b5fee25e7d5e4d290c88efb8)\\n']}}}, "*

 * *            '4: {\'source\': {insert: [(11, \'    mode="embedding", verbose=True, '*

 * *            "service_context=openai_sc, use_async=False\\n')], delete: [14, 13, 12, 11]}}, 5: "*

 * *            "{'source': {insert: [(10, '    index=index,\\n'), (16, '    "*

 * *            "n […]*

```diff
@@ -18,15 +18,15 @@
             "id": "25157da5",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Found cached dataset fiqa (/home/jjmachan/.cache/huggingface/datasets/explodinggradients___fiqa/main/1.0.0/953cfddc4a440cf2e290172be2563e5b51a953f2e4266940fc2b311e135cea69)\n"
+                        "Found cached dataset fiqa (/home/jjmachan/.cache/huggingface/datasets/explodinggradients___fiqa/main/1.0.0/3dc7b639f5b4b16509a3299a2ceb78bf5fe98ee6b5fee25e7d5e4d290c88efb8)\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
                             "Dataset({\n",
                             "    features: ['question', 'ground_truths'],\n",
@@ -93,18 +93,15 @@
                 "storage_context = StorageContext.from_defaults(persist_dir=\"./storage\")\n",
                 "\n",
                 "# load index\n",
                 "index = load_index_from_storage(storage_context)\n",
                 "\n",
                 "# query with embed_model specified\n",
                 "qe = index.as_query_engine(\n",
-                "    mode=\"embedding\", \n",
-                "    verbose=True, \n",
-                "    service_context=openai_sc,\n",
-                "    use_async = False\n",
+                "    mode=\"embedding\", verbose=True, service_context=openai_sc, use_async=False\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "c149a4be",
@@ -117,23 +114,21 @@
                 ")\n",
                 "from llama_index.retrievers import VectorIndexRetriever\n",
                 "from llama_index.query_engine import RetrieverQueryEngine\n",
                 "from llama_index.indices.postprocessor import SimilarityPostprocessor\n",
                 "\n",
                 "# configure retriever\n",
                 "retriever = VectorIndexRetriever(\n",
-                "    index=index, \n",
+                "    index=index,\n",
                 "    similarity_top_k=1,\n",
                 ")\n",
                 "\n",
                 "# configure response synthesizer\n",
                 "response_synthesizer = ResponseSynthesizer.from_args(\n",
-                "    node_postprocessors=[\n",
-                "        SimilarityPostprocessor(similarity_cutoff=0.7)\n",
-                "    ]\n",
+                "    node_postprocessors=[SimilarityPostprocessor(similarity_cutoff=0.7)]\n",
                 ")\n",
                 "\n",
                 "# assemble query engine\n",
                 "qe = RetrieverQueryEngine(\n",
                 "    retriever=retriever,\n",
                 "    response_synthesizer=response_synthesizer,\n",
                 ")"
@@ -146,17 +141,18 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "def generate_response(row):\n",
                 "    r = qe.query(row[\"question\"])\n",
                 "    row[\"answer\"] = r.response\n",
                 "    row[\"contexts\"] = [sn.node.text for sn in r.source_nodes]\n",
-                "    \n",
+                "\n",
                 "    return row\n",
                 "\n",
+                "\n",
                 "# generate_response(test_ds[0])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "id": "1d5afb7c",
@@ -268,18 +264,15 @@
                 }
             ],
             "source": [
                 "# evaluate\n",
                 "from ragas.metrics import factuality, answer_relevancy, context_relevancy\n",
                 "from ragas import evaluate\n",
                 "\n",
-                "evaluate(\n",
-                "    gen_ds, \n",
-                "    metrics=[factuality, answer_relevancy, context_relevancy]\n",
-                ")"
+                "evaluate(gen_ds, metrics=[factuality, answer_relevancy, context_relevancy])"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "43b21990",
             "metadata": {},
             "source": [
@@ -300,18 +293,15 @@
                 "storage_context = StorageContext.from_defaults(persist_dir=\"./storage\")\n",
                 "\n",
                 "# load index\n",
                 "index = load_index_from_storage(storage_context)\n",
                 "\n",
                 "# query with embed_model specified\n",
                 "qe = index.as_query_engine(\n",
-                "    mode=\"embedding\", \n",
-                "    verbose=True, \n",
-                "    service_context=openai_sc,\n",
-                "    use_async = False\n",
+                "    mode=\"embedding\", verbose=True, service_context=openai_sc, use_async=False\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "a2f5e91e",
@@ -324,23 +314,21 @@
                 ")\n",
                 "from llama_index.retrievers import VectorIndexRetriever\n",
                 "from llama_index.query_engine import RetrieverQueryEngine\n",
                 "from llama_index.indices.postprocessor import SimilarityPostprocessor\n",
                 "\n",
                 "# configure retriever\n",
                 "retriever = VectorIndexRetriever(\n",
-                "    index=index, \n",
+                "    index=index,\n",
                 "    similarity_top_k=1,\n",
                 ")\n",
                 "\n",
                 "# configure response synthesizer\n",
                 "response_synthesizer = ResponseSynthesizer.from_args(\n",
-                "    node_postprocessors=[\n",
-                "        SimilarityPostprocessor(similarity_cutoff=0.7)\n",
-                "    ]\n",
+                "    node_postprocessors=[SimilarityPostprocessor(similarity_cutoff=0.7)]\n",
                 ")\n",
                 "\n",
                 "# assemble query engine\n",
                 "qe = RetrieverQueryEngine(\n",
                 "    retriever=retriever,\n",
                 "    response_synthesizer=response_synthesizer,\n",
                 ")"
@@ -353,23 +341,24 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "def generate_response(row):\n",
                 "    r = qe.query(row[\"question\"])\n",
                 "    row[\"answer\"] = r.response\n",
                 "    row[\"contexts\"] = [sn.node.text for sn in r.source_nodes]\n",
-                "    \n",
+                "\n",
                 "    return row\n",
                 "\n",
+                "\n",
                 "# generate_response(test_ds[0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 7,
             "id": "661ad12b",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
                             "model_id": "",
@@ -380,56 +369,57 @@
                             "Map:   0%|          | 0/30 [00:00<?, ? examples/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Retrying langchain.llms.openai.completion_with_retry.<locals>._completion_with_retry in 4.0 seconds as it raised RateLimitError: You exceeded your current quota, please check your plan and billing details..\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/plain": [
                             "Dataset({\n",
                             "    features: ['question', 'ground_truths', 'answer', 'contexts'],\n",
                             "    num_rows: 30\n",
                             "})"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "gen_ds = fiqa_test.select(range(30)).map(generate_response)\n",
                 "gen_ds"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 8,
             "id": "96e08092",
             "metadata": {},
             "outputs": [
                 {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "46e26286ecbc4a0891f8ee228898ca20",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Downloading model.safetensors:   0%|          | 0.00/892M [00:00<?, ?B/s]"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/home/jjmachan/miniconda3/envs/bench/lib/python3.10/site-packages/transformers/models/t5/tokenization_t5_fast.py:155: FutureWarning: This tokenizer was incorrectly instantiated with a model max length of 512 which will be corrected in Transformers v5.\n",
-                        "For now, this behavior is kept to avoid breaking backwards compatibility when padding/encoding with `truncation is True`.\n",
-                        "- Be aware that you SHOULD NOT rely on t5-base automatically truncating your input to 512 when padding/encoding.\n",
-                        "- If you want to encode/pad to sequences longer than 512 you can either instantiate this tokenizer with `model_max_length` or pass `max_length` when encoding/padding.\n",
-                        "- To avoid this warning, please instantiate this tokenizer with `model_max_length` set to your preferred value.\n",
-                        "  warnings.warn(\n",
-                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 2/2 [00:57<00:00, 28.53s/it]\n"
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 2/2 [00:56<00:00, 28.39s/it]\n"
                     ]
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
                             "model_id": "",
                             "version_major": 2,
@@ -442,15 +432,15 @@
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:04<00:00,  4.47s/it]\n"
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:08<00:00,  8.04s/it]\n"
                     ]
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
                             "model_id": "",
                             "version_major": 2,
@@ -463,89 +453,134 @@
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:11<00:00, 11.58s/it]\n"
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:18<00:00, 18.73s/it]\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "{'NLI_score': 0.798888888888889, 'answer_relevancy': 0.8641, 'context_relavency': 0.8236333333333333, 'ragas_score': 0.8280100357048794}"
+                            "{'ragas_score': 0.8386, 'factuality': 0.8289, 'answer_relevancy': 0.8646, 'context_relavency': 0.8236}"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# evaluate\n",
                 "from ragas.metrics import factuality, answer_relevancy, context_relevancy\n",
                 "from ragas import evaluate\n",
                 "\n",
-                "evaluate(\n",
-                "    gen_ds, \n",
-                "    metrics=[factuality, answer_relevancy, context_relevancy]\n",
-                ")"
+                "evaluate(gen_ds, metrics=[factuality, answer_relevancy, context_relevancy])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 14,
+            "id": "87054feb",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "da6babe02adf49369a6d708487eeb068",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Creating CSV from Arrow format:   0%|          | 0/1 [00:00<?, ?ba/s]"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "82699"
+                        ]
+                    },
+                    "execution_count": 14,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# save to fiqa hub\n",
+                "import os\n",
+                "\n",
+                "path_to_dataset = \"../../../../datasets/fiqa/\"\n",
+                "\n",
+                "gen_ds.to_csv(os.path.join(path_to_dataset, \"baseline_chunk100_k1.csv\"))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8b957401",
             "metadata": {},
             "source": [
                 "## Cohere Rerank"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 16,
             "id": "15f4c130",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from llama_index.indices.postprocessor.cohere_rerank import CohereRerank\n",
                 "import os\n",
                 "\n",
-                "top_k = 4  \n",
+                "top_k = 4\n",
                 "cohere_rerank = CohereRerank(api_key=os.environ[\"COHERE_API_KEY\"], top_n=top_k)\n",
                 "reranking_qe = index.as_query_engine(\n",
                 "    similarity_top_k=top_k,\n",
                 "    node_postprocessors=[cohere_rerank],\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 17,
             "id": "6a73b189",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def generate_response(row):\n",
                 "    r = reranking_qe.query(row[\"question\"])\n",
                 "    row[\"answer\"] = r.response\n",
                 "    row[\"contexts\"] = [sn.node.text for sn in r.source_nodes]\n",
-                "    \n",
+                "\n",
                 "    return row\n",
                 "\n",
+                "\n",
                 "# generate_response(fiqa_test[0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 18,
             "id": "32bd4281",
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Parameter 'function'=<function generate_response at 0x7f832ef4f010> of the transform datasets.arrow_dataset.Dataset._map_single couldn't be hashed properly, a random hash was used instead. Make sure your transforms and parameters are serializable with pickle or dill for the dataset fingerprinting and caching to work. If you reuse this transform, the caching mechanism will consider it to be different from the previous calls and recompute everything. This warning is only showed once. Subsequent hashing failures won't be showed.\n"
+                    ]
+                },
+                {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
                             "model_id": "",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
@@ -560,15 +595,15 @@
                         "text/plain": [
                             "Dataset({\n",
                             "    features: ['question', 'ground_truths', 'answer', 'contexts'],\n",
                             "    num_rows: 30\n",
                             "})"
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "gen_ds = fiqa_test.select(range(30)).map(generate_response)\n",
                 "gen_ds"
@@ -641,24 +676,44 @@
                 }
             ],
             "source": [
                 "# evaluate\n",
                 "from ragas.metrics import factuality, answer_relevancy, context_relevancy\n",
                 "from ragas import evaluate\n",
                 "\n",
-                "evaluate(\n",
-                "    gen_ds, \n",
-                "    metrics=[factuality, answer_relevancy, context_relevancy]\n",
-                ")"
+                "evaluate(gen_ds, metrics=[factuality, answer_relevancy, context_relevancy])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "4301895f",
+            "metadata": {},
+            "outputs": [
+                {
+                    "ename": "NameError",
+                    "evalue": "name 'gen_ds' is not defined",
+                    "output_type": "error",
+                    "traceback": [
+                        "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
+                        "\u001b[0;31mNameError\u001b[0m                                 Traceback (most recent call last)",
+                        "Cell \u001b[0;32mIn[3], line 1\u001b[0m\n\u001b[0;32m----> 1\u001b[0m evals[\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mcohere_reranked\u001b[39m\u001b[38;5;124m\"\u001b[39m] \u001b[38;5;241m=\u001b[39m \u001b[43mgen_ds\u001b[49m\n\u001b[1;32m      2\u001b[0m evals\n",
+                        "\u001b[0;31mNameError\u001b[0m: name 'gen_ds' is not defined"
+                    ]
+                }
+            ],
+            "source": [
+                "evals[\"cohere_reranked\"] = gen_ds\n",
+                "evals"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a0991e58",
+            "id": "02cb461c",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
@@ -672,13 +727,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `ragas-0.0.3rc1/experiments/baselines/hotpotqa/explore-dataset.ipynb` & `ragas-0.0.4/experiments/baselines/hotpotqa/explore-dataset.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3rc1/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb` & `ragas-0.0.4/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3rc1/pyproject.toml` & `ragas-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3rc1/references.md` & `ragas-0.0.4/references.md`

 * *Files 14% similar despite different names*

```diff
@@ -22,30 +22,30 @@
 00000150: 7574 686f 723d 7b5a 6861 6e67 2065 7420  uthor={Zhang et 
 00000160: 616c 2e7d 2c20 7965 6172 3d7b 3230 3139  al.}, year={2019
 00000170: 7d2c 0a44 4f49 3d68 7474 7073 3a2f 2f64  },.DOI=https://d
 00000180: 6f69 2e6f 7267 2f31 302e 3438 3535 302f  oi.org/10.48550/
 00000190: 6172 5869 762e 3139 3034 2e30 3936 3735  arXiv.1904.09675
 000001a0: 0a7d 0a0a 406d 6973 637b 0a74 6974 6c65  .}..@misc{.title
 000001b0: 3d7b 4f6e 2046 6169 7468 6675 6c6e 6573  ={On Faithfulnes
-000001c0: 7320 616e 6420 4661 6374 7561 6c69 7479  s and Factuality
-000001d0: 2069 6e20 4162 7374 7261 6374 6976 6520   in Abstractive 
-000001e0: 5375 6d6d 6172 697a 6174 696f 6e7d 2c0a  Summarization},.
-000001f0: 6175 7468 6f72 3d7b 4d61 796e 657a 2a20  author={Maynez* 
-00000200: 6574 2061 6c2e 7d2c 2079 6561 723d 7b32  et al.}, year={2
-00000210: 3032 307d 2c0a 444f 493d 6874 7470 733a  020},.DOI=https:
-00000220: 2f2f 646f 692e 6f72 672f 3130 2e34 3835  //doi.org/10.485
-00000230: 3530 2f61 7258 6976 2e32 3030 352e 3030  50/arXiv.2005.00
-00000240: 3636 310a 7d0a 0a40 6d69 7363 7b0a 7469  661.}..@misc{.ti
-00000250: 746c 653d 7b51 5e32 3a20 4576 616c 7561  tle={Q^2: Evalua
-00000260: 7469 6e67 2046 6163 7475 616c 2043 6f6e  ting Factual Con
-00000270: 7369 7374 656e 6379 2069 6e20 4b6e 6f77  sistency in Know
-00000280: 6c65 6467 652d 4772 6f75 6e64 6564 2044  ledge-Grounded D
-00000290: 6961 6c6f 6775 6573 2076 6961 2051 7565  ialogues via Que
-000002a0: 7374 696f 6e20 4765 6e65 7261 7469 6f6e  stion Generation
-000002b0: 2061 6e64 2051 7565 7374 696f 6e20 416e   and Question An
-000002c0: 7377 6572 696e 677d 2c0a 6175 7468 6f72  swering},.author
-000002d0: 3d7b 486f 6e6f 7669 6368 2065 7420 616c  ={Honovich et al
-000002e0: 2e7d 2c20 7965 6172 3d7b 3230 3231 7d2c  .}, year={2021},
-000002f0: 0a44 4f49 3d68 7474 7073 3a2f 2f64 6f69  .DOI=https://doi
-00000300: 2e6f 7267 2f31 302e 3438 3535 302f 6172  .org/10.48550/ar
-00000310: 5869 762e 3231 3034 2e30 3832 3032 0a7d  Xiv.2104.08202.}
-00000320: 0a0a 6060 600a                           ..```.
+000001c0: 7320 616e 6420 4661 6974 6866 756c 6e65  s and Faithfulne
+000001d0: 7373 2069 6e20 4162 7374 7261 6374 6976  ss in Abstractiv
+000001e0: 6520 5375 6d6d 6172 697a 6174 696f 6e7d  e Summarization}
+000001f0: 2c0a 6175 7468 6f72 3d7b 4d61 796e 657a  ,.author={Maynez
+00000200: 2a20 6574 2061 6c2e 7d2c 2079 6561 723d  * et al.}, year=
+00000210: 7b32 3032 307d 2c0a 444f 493d 6874 7470  {2020},.DOI=http
+00000220: 733a 2f2f 646f 692e 6f72 672f 3130 2e34  s://doi.org/10.4
+00000230: 3835 3530 2f61 7258 6976 2e32 3030 352e  8550/arXiv.2005.
+00000240: 3030 3636 310a 7d0a 0a40 6d69 7363 7b0a  00661.}..@misc{.
+00000250: 7469 746c 653d 7b51 5e32 3a20 4576 616c  title={Q^2: Eval
+00000260: 7561 7469 6e67 2046 6163 7475 616c 2043  uating Factual C
+00000270: 6f6e 7369 7374 656e 6379 2069 6e20 4b6e  onsistency in Kn
+00000280: 6f77 6c65 6467 652d 4772 6f75 6e64 6564  owledge-Grounded
+00000290: 2044 6961 6c6f 6775 6573 2076 6961 2051   Dialogues via Q
+000002a0: 7565 7374 696f 6e20 4765 6e65 7261 7469  uestion Generati
+000002b0: 6f6e 2061 6e64 2051 7565 7374 696f 6e20  on and Question 
+000002c0: 416e 7377 6572 696e 677d 2c0a 6175 7468  Answering},.auth
+000002d0: 6f72 3d7b 486f 6e6f 7669 6368 2065 7420  or={Honovich et 
+000002e0: 616c 2e7d 2c20 7965 6172 3d7b 3230 3231  al.}, year={2021
+000002f0: 7d2c 0a44 4f49 3d68 7474 7073 3a2f 2f64  },.DOI=https://d
+00000300: 6f69 2e6f 7267 2f31 302e 3438 3535 302f  oi.org/10.48550/
+00000310: 6172 5869 762e 3231 3034 2e30 3832 3032  arXiv.2104.08202
+00000320: 0a7d 0a0a 6060 600a                      .}..```.
```

### Comparing `ragas-0.0.3rc1/src/ragas/evaluation.py` & `ragas-0.0.4/src/ragas/evaluation.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 from dataclasses import dataclass
 from enum import Enum
 
 import numpy as np
 from datasets import Dataset, concatenate_datasets
 
+from ragas._analytics import EvaluationEvent, track
 from ragas.metrics.base import Metric
 
 EvaluationMode = Enum("EvaluationMode", "generative retrieval grounded")
 
 
 def get_evaluation_mode(ds: Dataset):
     """
     validates the dataset and returns the evaluation type
 
     possible evaluation types
     1. (q,a,c)
-    2. (q)
+    2. (q,a)
     3. (q,c)
     4. (g,a)
     """
     ...
 
 
 def evaluate(
@@ -58,39 +59,50 @@
     Dataset({
         features: ['question', 'ground_truths', 'answer', 'contexts'],
         num_rows: 30
     })
 
     >>> result = evaluate(dataset)
     >>> print(result["ragas_score"])
-    {'ragas_score': 0.860, 'context_relavency': 0.817, 'factuality': 0.892,
+    {'ragas_score': 0.860, 'context_relavency': 0.817, 'faithfulness': 0.892,
     'answer_relevancy': 0.874}
     ```
     """
     if dataset is None:
         raise ValueError("Provide dataset!")
 
     # TODO: validate EvaluationMode here
     # evaluation_mode = get_evaluation_mode(dataset)
 
     # TODO: check if all the metrics are compatible with the evaluation mode
 
     if metrics is None:
-        from ragas.metrics import answer_relevancy, context_relevancy, factuality
+        from ragas.metrics import answer_relevancy, context_relevancy, faithfulness
 
-        metrics = [answer_relevancy, context_relevancy, factuality]
+        metrics = [answer_relevancy, context_relevancy, faithfulness]
 
     # run the evaluation on dataset with different metrics
     # initialize all the models in the metrics
     [m.init_model() for m in metrics]
 
     scores = []
     for metric in metrics:
         scores.append(metric.score(dataset).select_columns(metric.name))
 
+    # log the evaluation event
+    metrics_names = [m.name for m in metrics]
+    track(
+        EvaluationEvent(
+            event_type="evaluation",
+            metrics=metrics_names,
+            evaluation_mode="",
+            num_rows=dataset.shape[0],
+        )
+    )
+
     return Result(scores=concatenate_datasets(scores, axis=1), dataset=dataset)
 
 
 @dataclass
 class Result(dict):
     scores: Dataset
     dataset: Dataset | None = None
@@ -103,35 +115,23 @@
             self[cn] = value
             values.append(value)
 
         # harmonic mean of all the scores we have
         if len(values) == 3:
             self["ragas_score"] = len(values) / np.sum(1.0 / np.array(values))
 
-    def describe(self):
-        description = {}
-        for cn in self.scores.column_names:
-            description[cn] = {
-                "mean": np.mean(self.scores[cn]),
-                "25%": np.percentile(self.scores[cn], 25),
-                "50%": np.percentile(self.scores[cn], 50),
-                "75%": np.percentile(self.scores[cn], 75),
-                "min": np.min(self.scores[cn]),
-                "max": np.max(self.scores[cn]),
-                "std": np.std(self.scores[cn]),
-            }
-        return description
-
     def to_pandas(self, batch_size: int | None = None, batched: bool = False):
         if self.dataset is None:
             raise ValueError("dataset is not provided for the results class")
         assert self.scores.shape[0] == self.dataset.shape[0]
         result_ds = concatenate_datasets([self.dataset, self.scores], axis=1)
 
         return result_ds.to_pandas(batch_size=batch_size, batched=batched)
 
     def __repr__(self) -> str:
         scores = self.copy()
-        ragas_score = scores.pop("ragas_score")
-        score_strs = [f"'ragas_score': {ragas_score:0.3f}"]
-        score_strs.extend([f"'{k}': {v:0.3f}" for k, v in scores.items()])
+        score_strs = []
+        if "ragas_score" in scores:
+            ragas_score = scores.pop("ragas_score")
+            score_strs += f"'ragas_score': {ragas_score:0.4f}"
+        score_strs.extend([f"'{k}': {v:0.4f}" for k, v in scores.items()])
         return "{" + ", ".join(score_strs) + "}"
```

### Comparing `ragas-0.0.3rc1/src/ragas/metrics/answer_relevance.py` & `ragas-0.0.4/src/ragas/metrics/answer_relevance.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3rc1/src/ragas/metrics/base.py` & `ragas-0.0.4/src/ragas/metrics/base.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3rc1/src/ragas/metrics/context_relevance.py` & `ragas-0.0.4/src/ragas/metrics/context_relevance.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3rc1/src/ragas/metrics/factual.py` & `ragas-0.0.4/src/ragas/metrics/factual.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,20 +53,20 @@
 statements:\n{}
 Now, read the following statements and determine whether they are supported by the information present in the context. Provide a brief explanation for each statement. Also provide a Final Answer (Yes/No) at the end. 
 Answer:
 """  # noqa: E501
 
 
 @dataclass
-class Factuality(Metric):
+class Faithfulness(Metric):
     batch_size: int = 15
 
     @property
     def name(self):
-        return "factuality"
+        return "faithfulness"
 
     def init_model(self: t.Self):
         pass
 
     def score(self: t.Self, dataset: Dataset) -> Dataset:
         scores = []
         for batch in tqdm(self.get_batches(len(dataset))):
@@ -120,8 +120,8 @@
                 )
 
             scores.append(1 - score)
 
         return ds.add_column(f"{self.name}", scores)  # type: ignore
 
 
-factuality = Factuality()
+faithfulness = Faithfulness()
```

### Comparing `ragas-0.0.3rc1/src/ragas/metrics/llms.py` & `ragas-0.0.4/src/ragas/metrics/llms.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3rc1/src/ragas/utils.py` & `ragas-0.0.4/src/ragas/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 from __future__ import annotations
 
+import logging
+import os
 import typing as t
+from functools import lru_cache
 from warnings import warn
 
 import torch
 from torch import device as Device
 
 DEVICES = ["cpu", "cuda"]
+DEBUG_ENV_VAR = "RAGAS_DEBUG"
 
 
 def device_check(device: t.Literal["cpu", "cuda"] | Device) -> torch.device:
     if isinstance(device, Device):
         return device
     if device not in DEVICES:
         raise ValueError(f"Invalid device {device}")
     if device == "cuda" and not torch.cuda.is_available():
         warn("cuda not available, using cpu")
         device = "cpu"
 
     return torch.device(device)
+
+
+@lru_cache(maxsize=1)
+def get_debug_mode() -> bool:
+    if os.environ.get(DEBUG_ENV_VAR, str(False)).lower() == "true":
+        logging.basicConfig(level=logging.DEBUG)
+        return True
+    else:
+        return False
```

### Comparing `ragas-0.0.3rc1/src/ragas.egg-info/SOURCES.txt` & `ragas-0.0.4/src/ragas.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 Makefile
 README.md
 pyproject.toml
 references.md
 .github/workflows/ci.yaml
 .github/workflows/python-publish.yml
 docs/metrics.md
+docs/quickstart.ipynb
+docs/assets/bar-graph.svg
 docs/assets/logo.png
-examples/data_prep.py
-examples/quickstart.ipynb
+docs/guides/data_prep.py
 experiments/README.md
 experiments/assesments/metrics_assesments.ipynb
 experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
 experiments/baselines/fiqa/fiqa_baseline.tar.gz
 experiments/baselines/fiqa/improving-baselines.ipynb
 experiments/baselines/hotpotqa/explore-dataset.ipynb
 experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
 experiments/baselines/wikiqa/failed_wikis
 experiments/baselines/wikiqa/wikiqa_docs.tar.gz
 experiments/baselines/wikiqa/wikiqa_llamaindex_baseline.tar.gz
 requirements/dev.txt
 requirements/test.txt
 src/ragas/__init__.py
+src/ragas/_analytics.py
 src/ragas/_version.py
 src/ragas/evaluation.py
 src/ragas/exceptions.py
 src/ragas/utils.py
 src/ragas.egg-info/PKG-INFO
 src/ragas.egg-info/SOURCES.txt
 src/ragas.egg-info/dependency_links.txt
```

### Comparing `ragas-0.0.3rc1/tests/benchmarks/benchmark_eval.py` & `ragas-0.0.4/tests/benchmarks/benchmark_eval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 
 from datasets import Dataset
 from torch.cuda import is_available
 
 from ragas import evaluate
-from ragas.metrics import answer_relevancy, context_relavancy, factuality
+from ragas.metrics import answer_relevancy, context_relevancy, faithfulness
 
 DEVICE = "cuda" if is_available() else "cpu"
 
 PATH_TO_DATSET_GIT_REPO = "../../../datasets/fiqa/"
 assert os.path.isdir(PATH_TO_DATSET_GIT_REPO), "Dataset not found"
 ds = Dataset.from_json(os.path.join(PATH_TO_DATSET_GIT_REPO, "gen_ds.json"))
 assert isinstance(ds, Dataset)
 
 if __name__ == "__main__":
     result = evaluate(
         ds,
-        metrics=[answer_relevancy, context_relavancy, factuality],
+        metrics=[answer_relevancy, context_relevancy, faithfulness],
     )
     print(result)
```

### Comparing `ragas-0.0.3rc1/tests/benchmarks/utils.py` & `ragas-0.0.4/tests/benchmarks/utils.py`

 * *Files identical despite different names*

