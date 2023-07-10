# Comparing `tmp/causalml-0.8.0.tar.gz` & `tmp/causalml-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/causalml-0.8.0.tar", last modified: Fri Jul 17 23:35:10 2020, max compression
+gzip compressed data, was "dist/causalml-0.9.0.tar", last modified: Fri Oct 23 22:43:11 2020, max compression
```

## Comparing `causalml-0.8.0.tar` & `causalml-0.9.0.tar`

### file list

```diff
@@ -1,132 +1,84 @@
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/.github/
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 jeong      (501) staff       (20)      730 2019-12-31 20:14:48.000000 causalml-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 jeong      (501) staff       (20)      604 2019-12-31 20:14:48.000000 causalml-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 jeong      (501) staff       (20)      145 2020-07-17 22:58:30.000000 causalml-0.8.0/.gitignore
--rw-r--r--   0 jeong      (501) staff       (20)      402 2019-08-14 01:03:37.000000 causalml-0.8.0/.readthedocs.yml
--rw-r--r--   0 jeong      (501) staff       (20)      933 2020-07-17 22:58:30.000000 causalml-0.8.0/.travis.yml
--rw-r--r--   0 jeong      (501) staff       (20)     3224 2019-08-12 20:58:55.000000 causalml-0.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jeong      (501) staff       (20)     1233 2019-12-15 00:22:51.000000 causalml-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 jeong      (501) staff       (20)      561 2019-08-12 20:58:55.000000 causalml-0.8.0/LICENSE
--rw-r--r--   0 jeong      (501) staff       (20)      160 2019-08-14 01:40:27.000000 causalml-0.8.0/MANIFEST.in
--rw-r--r--   0 jeong      (501) staff       (20)    12969 2020-07-17 23:35:10.000000 causalml-0.8.0/PKG-INFO
--rw-r--r--   0 jeong      (501) staff       (20)    10517 2020-07-17 23:28:30.000000 causalml-0.8.0/README.md
--rw-r--r--   0 jeong      (501) staff       (20)      227 2019-08-12 20:58:55.000000 causalml-0.8.0/SECURITY.md
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml/
--rw-r--r--   0 jeong      (501) staff       (20)      231 2020-07-17 23:28:30.000000 causalml-0.8.0/causalml/__init__.py
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml/dataset/
--rw-r--r--   0 jeong      (501) staff       (20)      808 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/dataset/__init__.py
--rw-r--r--   0 jeong      (501) staff       (20)    11162 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/dataset/classification.py
--rw-r--r--   0 jeong      (501) staff       (20)     8749 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/dataset/regression.py
--rw-r--r--   0 jeong      (501) staff       (20)    23271 2020-01-15 17:24:23.000000 causalml-0.8.0/causalml/dataset/synthetic.py
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml/feature_selection/
--rw-r--r--   0 jeong      (501) staff       (20)       33 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/feature_selection/__init__.py
--rw-r--r--   0 jeong      (501) staff       (20)    19370 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/feature_selection/filters.py
--rw-r--r--   0 jeong      (501) staff       (20)     7977 2019-12-06 01:15:09.000000 causalml-0.8.0/causalml/features.py
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml/inference/
--rw-r--r--   0 jeong      (501) staff       (20)        0 2019-11-07 00:53:21.000000 causalml-0.8.0/causalml/inference/__init__.py
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml/inference/iv/
--rw-r--r--   0 jeong      (501) staff       (20)       38 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/inference/iv/__init__.py
--rw-r--r--   0 jeong      (501) staff       (20)     1449 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/inference/iv/iv_regression.py
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml/inference/meta/
--rw-r--r--   0 jeong      (501) staff       (20)      361 2019-11-15 18:49:03.000000 causalml-0.8.0/causalml/inference/meta/__init__.py
--rw-r--r--   0 jeong      (501) staff       (20)    10830 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/inference/meta/explainer.py
--rw-r--r--   0 jeong      (501) staff       (20)    36041 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/inference/meta/rlearner.py
--rw-r--r--   0 jeong      (501) staff       (20)    24635 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/inference/meta/slearner.py
--rw-r--r--   0 jeong      (501) staff       (20)    24569 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/inference/meta/tlearner.py
--rw-r--r--   0 jeong      (501) staff       (20)     7723 2019-12-31 20:14:48.000000 causalml-0.8.0/causalml/inference/meta/tmle.py
--rw-r--r--   0 jeong      (501) staff       (20)     3619 2019-12-23 19:16:32.000000 causalml-0.8.0/causalml/inference/meta/utils.py
--rw-r--r--   0 jeong      (501) staff       (20)    37489 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/inference/meta/xlearner.py
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml/inference/nn/
--rw-r--r--   0 jeong      (501) staff       (20)       32 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/inference/nn/__init__.py
--rw-r--r--   0 jeong      (501) staff       (20)     8464 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/inference/nn/dragonnet.py
--rw-r--r--   0 jeong      (501) staff       (20)     5960 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/inference/nn/utils.py
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml/inference/tree/
--rw-r--r--   0 jeong      (501) staff       (20)      305 2019-12-15 00:22:06.000000 causalml-0.8.0/causalml/inference/tree/__init__.py
--rw-r--r--   0 jeong      (501) staff       (20)  1214661 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml/inference/tree/causaltree.c
--rw-r--r--   0 jeong      (501) staff       (20)    15116 2020-02-19 20:30:37.000000 causalml-0.8.0/causalml/inference/tree/causaltree.pyx
--rw-r--r--   0 jeong      (501) staff       (20)    53984 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/inference/tree/models.py
--rw-r--r--   0 jeong      (501) staff       (20)     8236 2019-12-31 20:14:48.000000 causalml-0.8.0/causalml/inference/tree/plot.py
--rw-r--r--   0 jeong      (501) staff       (20)     7202 2019-12-31 20:14:48.000000 causalml-0.8.0/causalml/inference/tree/utils.py
--rw-r--r--   0 jeong      (501) staff       (20)    18605 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/match.py
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml/metrics/
--rw-r--r--   0 jeong      (501) staff       (20)      625 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/metrics/__init__.py
--rw-r--r--   0 jeong      (501) staff       (20)      970 2019-12-31 20:14:48.000000 causalml-0.8.0/causalml/metrics/classification.py
--rw-r--r--   0 jeong      (501) staff       (20)       11 2019-08-12 20:58:55.000000 causalml-0.8.0/causalml/metrics/const.py
--rw-r--r--   0 jeong      (501) staff       (20)     3186 2019-12-31 20:14:48.000000 causalml-0.8.0/causalml/metrics/regression.py
--rw-r--r--   0 jeong      (501) staff       (20)    21547 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/metrics/sensitivity.py
--rw-r--r--   0 jeong      (501) staff       (20)    35160 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/metrics/visualize.py
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml/optimize/
--rw-r--r--   0 jeong      (501) staff       (20)       41 2019-08-12 20:58:55.000000 causalml-0.8.0/causalml/optimize/__init__.py
--rw-r--r--   0 jeong      (501) staff       (20)     3398 2019-12-31 20:14:48.000000 causalml-0.8.0/causalml/optimize/policylearner.py
--rw-r--r--   0 jeong      (501) staff       (20)     9159 2020-07-17 22:58:33.000000 causalml-0.8.0/causalml/optimize/unit_selection.py
--rw-r--r--   0 jeong      (501) staff       (20)     4222 2020-07-17 22:58:33.000000 causalml-0.8.0/causalml/optimize/utils.py
--rw-r--r--   0 jeong      (501) staff       (20)     4012 2020-07-17 22:58:33.000000 causalml-0.8.0/causalml/optimize/value_optimization.py
--rw-r--r--   0 jeong      (501) staff       (20)     8168 2020-07-17 22:58:30.000000 causalml-0.8.0/causalml/propensity.py
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml.egg-info/
--rw-r--r--   0 jeong      (501) staff       (20)    12969 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml.egg-info/PKG-INFO
--rw-r--r--   0 jeong      (501) staff       (20)     3212 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml.egg-info/SOURCES.txt
--rw-r--r--   0 jeong      (501) staff       (20)        1 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml.egg-info/dependency_links.txt
--rw-r--r--   0 jeong      (501) staff       (20)      228 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml.egg-info/requires.txt
--rw-r--r--   0 jeong      (501) staff       (20)       15 2020-07-17 23:35:10.000000 causalml-0.8.0/causalml.egg-info/top_level.txt
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/docs/
--rw-r--r--   0 jeong      (501) staff       (20)     6770 2019-07-10 00:54:40.000000 causalml-0.8.0/docs/Makefile
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/docs/_build/
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/docs/_build/html/
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/docs/_build/html/_sources/
--rw-r--r--   0 jeong      (501) staff       (20)     1690 2019-07-10 00:57:58.000000 causalml-0.8.0/docs/_build/html/_sources/about.rst.txt
--rw-r--r--   0 jeong      (501) staff       (20)     1318 2019-08-12 20:58:55.000000 causalml-0.8.0/docs/_build/html/_sources/causalml.rst.txt
--rw-r--r--   0 jeong      (501) staff       (20)     4491 2020-05-07 17:56:11.000000 causalml-0.8.0/docs/_build/html/_sources/changelog.rst.txt
--rw-r--r--   0 jeong      (501) staff       (20)     3894 2020-03-13 18:15:48.000000 causalml-0.8.0/docs/_build/html/_sources/examples.rst.txt
--rw-r--r--   0 jeong      (501) staff       (20)      372 2020-01-03 21:21:51.000000 causalml-0.8.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 jeong      (501) staff       (20)      374 2019-08-12 20:58:55.000000 causalml-0.8.0/docs/_build/html/_sources/installation.rst.txt
--rw-r--r--   0 jeong      (501) staff       (20)     2597 2019-10-21 19:37:43.000000 causalml-0.8.0/docs/_build/html/_sources/interpretation.rst.txt
--rw-r--r--   0 jeong      (501) staff       (20)     5831 2020-03-13 17:56:40.000000 causalml-0.8.0/docs/_build/html/_sources/methodology.rst.txt
--rw-r--r--   0 jeong      (501) staff       (20)     1050 2019-07-10 00:53:03.000000 causalml-0.8.0/docs/_build/html/_sources/references.rst.txt
--rw-r--r--   0 jeong      (501) staff       (20)     3716 2019-12-06 01:15:09.000000 causalml-0.8.0/docs/_build/html/_sources/validation.rst.txt
--rw-r--r--   0 jeong      (501) staff       (20)     2350 2020-01-03 21:21:51.000000 causalml-0.8.0/docs/_build/html/_sources/visualization.rst.txt
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/docs/_static/
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/docs/_static/img/
--rw-r--r--   0 jeong      (501) staff       (20)    36701 2020-01-15 17:23:50.000000 causalml-0.8.0/docs/_static/img/causalml_logo.png
--rw-r--r--   0 jeong      (501) staff       (20)    60363 2019-10-21 19:37:43.000000 causalml-0.8.0/docs/_static/img/shap_vis.png
--rw-r--r--   0 jeong      (501) staff       (20)   149927 2020-01-03 21:21:51.000000 causalml-0.8.0/docs/_static/img/uplift_tree_vis.png
--rw-r--r--   0 jeong      (501) staff       (20)     1760 2020-07-17 23:28:30.000000 causalml-0.8.0/docs/about.rst
--rw-r--r--   0 jeong      (501) staff       (20)     1318 2019-08-12 20:58:55.000000 causalml-0.8.0/docs/causalml.rst
--rw-r--r--   0 jeong      (501) staff       (20)     5894 2020-07-17 23:28:30.000000 causalml-0.8.0/docs/changelog.rst
--rw-r--r--   0 jeong      (501) staff       (20)     8807 2019-10-21 18:14:29.000000 causalml-0.8.0/docs/conf.py
--rw-r--r--   0 jeong      (501) staff       (20)     3894 2020-07-17 22:58:30.000000 causalml-0.8.0/docs/examples.rst
--rw-r--r--   0 jeong      (501) staff       (20)      372 2020-01-03 21:21:51.000000 causalml-0.8.0/docs/index.rst
--rw-r--r--   0 jeong      (501) staff       (20)      374 2019-08-12 20:58:55.000000 causalml-0.8.0/docs/installation.rst
--rw-r--r--   0 jeong      (501) staff       (20)     2597 2019-10-21 19:37:43.000000 causalml-0.8.0/docs/interpretation.rst
--rw-r--r--   0 jeong      (501) staff       (20)     5831 2020-07-17 22:58:30.000000 causalml-0.8.0/docs/methodology.rst
--rw-r--r--   0 jeong      (501) staff       (20)     1050 2019-07-10 00:53:03.000000 causalml-0.8.0/docs/references.rst
--rw-r--r--   0 jeong      (501) staff       (20)    14870 2019-08-12 20:58:55.000000 causalml-0.8.0/docs/refs.bib
--rw-r--r--   0 jeong      (501) staff       (20)       85 2020-07-17 22:58:30.000000 causalml-0.8.0/docs/requirements.txt
--rw-r--r--   0 jeong      (501) staff       (20)     3716 2019-12-06 01:15:09.000000 causalml-0.8.0/docs/validation.rst
--rw-r--r--   0 jeong      (501) staff       (20)     2350 2020-01-03 21:21:51.000000 causalml-0.8.0/docs/visualization.rst
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/examples/
--rw-r--r--   0 jeong      (501) staff       (20)  1430563 2020-07-17 22:58:30.000000 causalml-0.8.0/examples/feature_interpretations_example.ipynb
--rw-r--r--   0 jeong      (501) staff       (20)  1141281 2020-07-17 22:58:30.000000 causalml-0.8.0/examples/meta_learners_with_synthetic_data.ipynb
--rw-r--r--   0 jeong      (501) staff       (20)   158917 2020-07-17 22:58:30.000000 causalml-0.8.0/examples/meta_learners_with_synthetic_data_multiple_treatment.ipynb
--rw-r--r--   0 jeong      (501) staff       (20)  1273454 2020-02-20 01:19:53.000000 causalml-0.8.0/examples/uplift_tree_visualization.ipynb
--rw-r--r--   0 jeong      (501) staff       (20)    64700 2019-12-31 20:14:48.000000 causalml-0.8.0/examples/uplift_trees_with_synthetic_data.ipynb
--rw-r--r--   0 jeong      (501) staff       (20)   698745 2020-07-17 22:58:30.000000 causalml-0.8.0/examples/validation_with_tmle.ipynb
--rw-r--r--   0 jeong      (501) staff       (20)       23 2020-07-17 22:58:30.000000 causalml-0.8.0/requirements-test.txt
--rw-r--r--   0 jeong      (501) staff       (20)      228 2020-07-17 22:58:30.000000 causalml-0.8.0/requirements.txt
--rw-r--r--   0 jeong      (501) staff       (20)      103 2020-07-17 23:35:10.000000 causalml-0.8.0/setup.cfg
--rw-r--r--   0 jeong      (501) staff       (20)     1779 2020-07-17 23:28:30.000000 causalml-0.8.0/setup.py
-drwxr-xr-x   0 jeong      (501) staff       (20)        0 2020-07-17 23:35:10.000000 causalml-0.8.0/tests/
--rw-r--r--   0 jeong      (501) staff       (20)        0 2019-08-12 20:58:55.000000 causalml-0.8.0/tests/__init__.py
--rw-r--r--   0 jeong      (501) staff       (20)     1016 2019-08-27 17:40:56.000000 causalml-0.8.0/tests/conftest.py
--rw-r--r--   0 jeong      (501) staff       (20)      291 2020-07-17 22:58:33.000000 causalml-0.8.0/tests/const.py
--rw-r--r--   0 jeong      (501) staff       (20)     2830 2020-07-17 22:58:33.000000 causalml-0.8.0/tests/test_counterfactual_unit_selection.py
--rw-r--r--   0 jeong      (501) staff       (20)     2337 2020-07-17 22:58:30.000000 causalml-0.8.0/tests/test_datasets.py
--rw-r--r--   0 jeong      (501) staff       (20)     1551 2019-08-12 20:58:55.000000 causalml-0.8.0/tests/test_features.py
--rw-r--r--   0 jeong      (501) staff       (20)     2219 2019-08-12 20:58:55.000000 causalml-0.8.0/tests/test_match.py
--rw-r--r--   0 jeong      (501) staff       (20)    25876 2020-07-17 22:58:30.000000 causalml-0.8.0/tests/test_meta_learners.py
--rw-r--r--   0 jeong      (501) staff       (20)     1031 2020-07-17 22:58:30.000000 causalml-0.8.0/tests/test_propensity.py
--rw-r--r--   0 jeong      (501) staff       (20)     6445 2020-07-17 22:58:33.000000 causalml-0.8.0/tests/test_sensitivity.py
--rw-r--r--   0 jeong      (501) staff       (20)     4629 2019-12-31 20:14:48.000000 causalml-0.8.0/tests/test_uplift_trees.py
--rw-r--r--   0 jeong      (501) staff       (20)     3159 2020-07-17 22:58:33.000000 causalml-0.8.0/tests/test_value_optimization.py
--rw-r--r--   0 jeong      (501) staff       (20)      849 2019-08-12 20:58:55.000000 causalml-0.8.0/tox.ini
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/
+-rw-r--r--   0 jing.pan   (501) staff       (20)     3224 2020-10-23 20:11:22.000000 causalml-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jing.pan   (501) staff       (20)     1233 2020-10-23 20:11:22.000000 causalml-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 jing.pan   (501) staff       (20)      561 2020-10-23 20:11:22.000000 causalml-0.9.0/LICENSE
+-rw-r--r--   0 jing.pan   (501) staff       (20)      160 2020-10-23 20:11:22.000000 causalml-0.9.0/MANIFEST.in
+-rw-r--r--   0 jing.pan   (501) staff       (20)    12969 2020-10-23 22:43:11.000000 causalml-0.9.0/PKG-INFO
+-rw-r--r--   0 jing.pan   (501) staff       (20)    10517 2020-10-23 20:11:22.000000 causalml-0.9.0/README.md
+-rw-r--r--   0 jing.pan   (501) staff       (20)      227 2020-10-23 20:11:22.000000 causalml-0.9.0/SECURITY.md
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml/
+-rw-r--r--   0 jing.pan   (501) staff       (20)      231 2020-10-23 22:41:56.000000 causalml-0.9.0/causalml/__init__.py
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml/dataset/
+-rw-r--r--   0 jing.pan   (501) staff       (20)      808 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/dataset/__init__.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)    11162 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/dataset/classification.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     8749 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/dataset/regression.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)    23271 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/dataset/synthetic.py
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml/feature_selection/
+-rw-r--r--   0 jing.pan   (501) staff       (20)       33 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/feature_selection/__init__.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)    19370 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/feature_selection/filters.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     7977 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/features.py
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml/inference/
+-rw-r--r--   0 jing.pan   (501) staff       (20)        0 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/__init__.py
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml/inference/iv/
+-rw-r--r--   0 jing.pan   (501) staff       (20)       38 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/iv/__init__.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     1449 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/iv/iv_regression.py
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml/inference/meta/
+-rw-r--r--   0 jing.pan   (501) staff       (20)      361 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/meta/__init__.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)    10830 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/meta/explainer.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)    35811 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/meta/rlearner.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)    24844 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/meta/slearner.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)    24569 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/meta/tlearner.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     7723 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/meta/tmle.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     3619 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/meta/utils.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)    37958 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/meta/xlearner.py
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml/inference/nn/
+-rw-r--r--   0 jing.pan   (501) staff       (20)       32 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/nn/__init__.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     8464 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/nn/dragonnet.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     5960 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/nn/utils.py
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml/inference/tree/
+-rw-r--r--   0 jing.pan   (501) staff       (20)      305 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/tree/__init__.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)  1208946 2020-10-23 21:49:42.000000 causalml-0.9.0/causalml/inference/tree/causaltree.c
+-rw-r--r--   0 jing.pan   (501) staff       (20)    15116 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/tree/causaltree.pyx
+-rw-r--r--   0 jing.pan   (501) staff       (20)    55477 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/tree/models.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     8236 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/tree/plot.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     7202 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/inference/tree/utils.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)    18605 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/match.py
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml/metrics/
+-rw-r--r--   0 jing.pan   (501) staff       (20)      625 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/metrics/__init__.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)      970 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/metrics/classification.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)       11 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/metrics/const.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     3186 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/metrics/regression.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)    21553 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/metrics/sensitivity.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)    35160 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/metrics/visualize.py
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml/optimize/
+-rw-r--r--   0 jing.pan   (501) staff       (20)      231 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/optimize/__init__.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     3398 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/optimize/policylearner.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     9159 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/optimize/unit_selection.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     4222 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/optimize/utils.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     4012 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/optimize/value_optimization.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     6943 2020-10-23 20:11:22.000000 causalml-0.9.0/causalml/propensity.py
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml.egg-info/
+-rw-r--r--   0 jing.pan   (501) staff       (20)    12969 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml.egg-info/PKG-INFO
+-rw-r--r--   0 jing.pan   (501) staff       (20)     1948 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml.egg-info/SOURCES.txt
+-rw-r--r--   0 jing.pan   (501) staff       (20)        1 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml.egg-info/dependency_links.txt
+-rw-r--r--   0 jing.pan   (501) staff       (20)      236 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml.egg-info/requires.txt
+-rw-r--r--   0 jing.pan   (501) staff       (20)       15 2020-10-23 22:43:11.000000 causalml-0.9.0/causalml.egg-info/top_level.txt
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/docs/
+-rw-r--r--   0 jing.pan   (501) staff       (20)       85 2020-10-23 20:11:22.000000 causalml-0.9.0/docs/requirements.txt
+-rw-r--r--   0 jing.pan   (501) staff       (20)       23 2020-10-23 20:11:22.000000 causalml-0.9.0/requirements-test.txt
+-rw-r--r--   0 jing.pan   (501) staff       (20)      236 2020-10-23 20:11:22.000000 causalml-0.9.0/requirements.txt
+-rw-r--r--   0 jing.pan   (501) staff       (20)      103 2020-10-23 22:43:11.000000 causalml-0.9.0/setup.cfg
+-rw-r--r--   0 jing.pan   (501) staff       (20)     1797 2020-10-23 20:11:22.000000 causalml-0.9.0/setup.py
+drwxr-xr-x   0 jing.pan   (501) staff       (20)        0 2020-10-23 22:43:11.000000 causalml-0.9.0/tests/
+-rw-r--r--   0 jing.pan   (501) staff       (20)        0 2020-10-23 20:11:22.000000 causalml-0.9.0/tests/__init__.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     1016 2020-10-23 20:11:22.000000 causalml-0.9.0/tests/conftest.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)      291 2020-10-23 20:11:22.000000 causalml-0.9.0/tests/const.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     2830 2020-10-23 20:11:22.000000 causalml-0.9.0/tests/test_counterfactual_unit_selection.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     2337 2020-10-23 20:11:22.000000 causalml-0.9.0/tests/test_datasets.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     1551 2020-10-23 20:11:22.000000 causalml-0.9.0/tests/test_features.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     2219 2020-10-23 20:11:22.000000 causalml-0.9.0/tests/test_match.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)    26398 2020-10-23 20:11:22.000000 causalml-0.9.0/tests/test_meta_learners.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     1624 2020-10-23 20:11:22.000000 causalml-0.9.0/tests/test_propensity.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     6225 2020-10-23 20:11:22.000000 causalml-0.9.0/tests/test_sensitivity.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     4629 2020-10-23 20:11:22.000000 causalml-0.9.0/tests/test_uplift_trees.py
+-rw-r--r--   0 jing.pan   (501) staff       (20)     3159 2020-10-23 20:11:22.000000 causalml-0.9.0/tests/test_value_optimization.py
```

### Comparing `causalml-0.8.0/CODE_OF_CONDUCT.md` & `causalml-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/CONTRIBUTING.md` & `causalml-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/LICENSE` & `causalml-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/PKG-INFO` & `causalml-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalml
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python Package for Uplift Modeling and Causal Inference with Machine Learning Algorithms
 Home-page: https://github.com/uber/causalml
 Author: Huigang Chen, Totte Harinen, Jeong-Yoon Lee, Yuchen Luo, Jing Pan, Mike Yung, Zhenyu Zhao
 Author-email: 
 License: UNKNOWN
 Description: <div align="center">
           <a href="https://github.com/uber/causalml"><img width="380px" height="140px" src="https://raw.githubusercontent.com/uber/causalml/master/docs/_static/img/causalml_logo.png"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: causalml Version: 0.8.0 Summary: Python Package for
+Metadata-Version: 2.1 Name: causalml Version: 0.9.0 Summary: Python Package for
 Uplift Modeling and Causal Inference with Machine Learning Algorithms Home-
 page: https://github.com/uber/causalml Author: Huigang Chen, Totte Harinen,
 Jeong-Yoon Lee, Yuchen Luo, Jing Pan, Mike Yung, Zhenyu Zhao Author-email:
 License: UNKNOWN Description:
    [https://raw.githubusercontent.com/uber/causalml/master/docs/_static/img/
                               causalml_logo.png]
 ------------------------------------------------------ [![PyPI Version](https:/
```

### Comparing `causalml-0.8.0/README.md` & `causalml-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/dataset/__init__.py` & `causalml-0.9.0/causalml/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/dataset/classification.py` & `causalml-0.9.0/causalml/dataset/classification.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/dataset/regression.py` & `causalml-0.9.0/causalml/dataset/regression.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/dataset/synthetic.py` & `causalml-0.9.0/causalml/dataset/synthetic.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/feature_selection/filters.py` & `causalml-0.9.0/causalml/feature_selection/filters.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/features.py` & `causalml-0.9.0/causalml/features.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/inference/iv/iv_regression.py` & `causalml-0.9.0/causalml/inference/iv/iv_regression.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/inference/meta/explainer.py` & `causalml-0.9.0/causalml/inference/meta/explainer.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/inference/meta/rlearner.py` & `causalml-0.9.0/causalml/inference/meta/rlearner.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,15 +233,15 @@
         te = self.fit_predict(X, treatment, y, p)
 
         if p is None:
             p = self.propensity
         else:
             check_p_conditions(p, self.t_groups)
 
-        if isinstance(p, np.ndarray):
+        if isinstance(p, (np.ndarray, pd.Series)):
             treatment_name = self.t_groups[0]
             p = {treatment_name: convert_pd_to_np(p)}
         elif isinstance(p, dict):
             p = {treatment_name: convert_pd_to_np(_p) for treatment_name, _p in p.items()}
 
         ate = np.zeros(self.t_groups.shape[0])
         ate_lb = np.zeros(self.t_groups.shape[0])
@@ -478,36 +478,33 @@
 
 class BaseRClassifier(BaseRLearner):
     """
     A parent class for R-learner classifier classes.
     """
 
     def __init__(self,
-                 learner=None,
                  outcome_learner=None,
                  effect_learner=None,
                  ate_alpha=.05,
                  control_name=0,
                  n_fold=5,
                  random_state=None):
         """Initialize an R-learner classifier.
 
         Args:
-            learner (optional): a model to estimate outcomes and treatment effects. Even if specified, the user
-                must still specify either the outcome learner or the effect learner.
-            outcome_learner (optional): a model to estimate outcomes. Should have a predict_proba() method.
-            effect_learner (optional): a model to estimate treatment effects. It needs to take `sample_weight` as an
-                input argument for `fit()`
+            outcome_learner: a model to estimate outcomes. Should be a classifier.
+            effect_learner: a model to estimate treatment effects. It needs to take `sample_weight` as an
+                input argument for `fit()`. Should be a regressor.
             ate_alpha (float, optional): the confidence level alpha of the ATE estimate
             control_name (str or int, optional): name of control group
             n_fold (int, optional): the number of cross validation folds for outcome_learner
             random_state (int or RandomState, optional): a seed (int) or random number generator (RandomState)
         """
         super().__init__(
-            learner=learner,
+            learner=None,
             outcome_learner=outcome_learner,
             effect_learner=effect_learner,
             ate_alpha=ate_alpha,
             control_name=control_name,
             n_fold=n_fold,
             random_state=random_state)
```

### Comparing `causalml-0.8.0/causalml/inference/meta/slearner.py` & `causalml-0.9.0/causalml/inference/meta/slearner.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,16 +135,14 @@
             te[:, i] = yhat_ts[group] - yhat_cs[group]
 
         if not return_components:
             return te
         else:
             return te, yhat_cs, yhat_ts
 
-        return te
-
     def fit_predict(self, X, treatment, y, return_ci=False, n_bootstraps=1000, bootstrap_size=10000,
                     return_components=False, verbose=True):
         """Fit the inference model of the S learner and predict treatment effects.
         Args:
             X (np.matrix, np.array, or pd.Dataframe): a feature matrix
             treatment (np.array or pd.Series): a treatment vector
             y (np.array or pd.Series): an outcome vector
@@ -439,20 +437,21 @@
             control_name (str or int, optional): name of control group
         """
         super().__init__(
             learner=learner,
             ate_alpha=ate_alpha,
             control_name=control_name)
 
-    def predict(self, X, treatment=None, y=None, verbose=True):
+    def predict(self, X, treatment=None, y=None, return_components=False, verbose=True):
         """Predict treatment effects.
         Args:
             X (np.matrix or np.array or pd.Dataframe): a feature matrix
             treatment (np.array or pd.Series, optional): a treatment vector
             y (np.array or pd.Series, optional): an outcome vector
+            return_components (bool, optional): whether to return outcome for treatment and control seperately
             verbose (bool, optional): whether to output progress logs
         Returns:
             (numpy.ndarray): Predictions of treatment effects.
         """
         X, treatment, y = convert_pd_to_np(X, treatment, y)
         yhat_cs = {}
         yhat_ts = {}
@@ -481,15 +480,18 @@
                 logger.info('Error metrics for group {}'.format(group))
                 classification_metrics(y_filt, yhat, w)
 
         te = np.zeros((X.shape[0], self.t_groups.shape[0]))
         for i, group in enumerate(self.t_groups):
             te[:, i] = yhat_ts[group] - yhat_cs[group]
 
-        return te
+        if not return_components:
+            return te
+        else:
+            return te, yhat_cs, yhat_ts
 
 
 class LRSRegressor(BaseSRegressor):
     def __init__(self, ate_alpha=.05, control_name=0):
         """Initialize an S-learner with a linear regression model.
         Args:
             ate_alpha (float, optional): the confidence level alpha of the ATE estimate
```

### Comparing `causalml-0.8.0/causalml/inference/meta/tlearner.py` & `causalml-0.9.0/causalml/inference/meta/tlearner.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/inference/meta/tmle.py` & `causalml-0.9.0/causalml/inference/meta/tmle.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/inference/meta/utils.py` & `causalml-0.9.0/causalml/inference/meta/utils.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/inference/meta/xlearner.py` & `causalml-0.9.0/causalml/inference/meta/xlearner.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         X, treatment, y = convert_pd_to_np(X, treatment, y)
         self.fit(X, treatment, y, p)
 
         if p is None:
             p = self.propensity
 
         check_p_conditions(p, self.t_groups)
-        if isinstance(p, np.ndarray):
+        if isinstance(p, (np.ndarray, pd.Series)):
             treatment_name = self.t_groups[0]
             p = {treatment_name: convert_pd_to_np(p)}
         elif isinstance(p, dict):
             p = {treatment_name: convert_pd_to_np(_p) for treatment_name, _p in p.items()}
 
         te = self.predict(X, treatment=treatment, y=y, p=p, return_components=return_components)
 
@@ -301,15 +301,15 @@
         te, dhat_cs, dhat_ts = self.fit_predict(X, treatment, y, p, return_components=True)
         X, treatment, y = convert_pd_to_np(X, treatment, y)
 
         if p is None:
             p = self.propensity
         else:
             check_p_conditions(p, self.t_groups)
-        if isinstance(p, np.ndarray):
+        if isinstance(p, (np.ndarray, pd.Series)):
             treatment_name = self.t_groups[0]
             p = {treatment_name: convert_pd_to_np(p)}
         elif isinstance(p, dict):
             p = {treatment_name: convert_pd_to_np(_p) for treatment_name, _p in p.items()}
 
         ate = np.zeros(self.t_groups.shape[0])
         ate_lb = np.zeros(self.t_groups.shape[0])
@@ -558,38 +558,49 @@
 
 class BaseXClassifier(BaseXLearner):
     """
     A parent class for X-learner classifier classes.
     """
 
     def __init__(self,
-                 learner=None,
+                 outcome_learner=None,
+                 effect_learner=None,
                  control_outcome_learner=None,
                  treatment_outcome_learner=None,
                  control_effect_learner=None,
                  treatment_effect_learner=None,
                  ate_alpha=.05,
                  control_name=0):
         """Initialize an X-learner classifier.
 
         Args:
-            learner (optional): a model to estimate outcomes or treatment effects in both the control and treatment
-                groups. Even if specified, the user must still input either the outcome learner or the effect learner
-                pair.
+            outcome_learner (optional): a model to estimate outcomes in both the control and treatment groups.
+                Should be a regressor.
+            effect_learner (optional): a model to estimate treatment effects in both the control and treatment groups.
+                Should be a classifier.
             control_outcome_learner (optional): a model to estimate outcomes in the control group.
-                Should have a predict_proba() method.
+                Should be a regressor.
             treatment_outcome_learner (optional): a model to estimate outcomes in the treatment group.
-                Should have a predict_proba() method.
-            control_effect_learner (optional): a model to estimate treatment effects in the control group
+                Should be a regressor.
+            control_effect_learner (optional): a model to estimate treatment effects in the control group.
+                Should be a classifier.
             treatment_effect_learner (optional): a model to estimate treatment effects in the treatment group
+                Should be a classifier.
             ate_alpha (float, optional): the confidence level alpha of the ATE estimate
             control_name (str or int, optional): name of control group
         """
+        if outcome_learner is not None:
+            control_outcome_learner = outcome_learner
+            treatment_outcome_learner = outcome_learner
+        if effect_learner is not None:
+            control_effect_learner = effect_learner
+            treatment_effect_learner = effect_learner
+
         super().__init__(
-            learner=learner,
+            learner=None,
             control_outcome_learner=control_outcome_learner,
             treatment_outcome_learner=treatment_outcome_learner,
             control_effect_learner=control_effect_learner,
             treatment_effect_learner=treatment_effect_learner,
             ate_alpha=ate_alpha,
             control_name=control_name)
```

### Comparing `causalml-0.8.0/causalml/inference/nn/dragonnet.py` & `causalml-0.9.0/causalml/inference/nn/dragonnet.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/inference/nn/utils.py` & `causalml-0.9.0/causalml/inference/nn/utils.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/inference/tree/causaltree.c` & `causalml-0.9.0/causalml/inference/tree/causaltree.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-/* Generated by Cython 0.29.15 */
+/* Generated by Cython 0.29.12 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/Users/jeong/miniconda3/envs/py37/lib/python3.7/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/Users/jeong/miniconda3/envs/py37/lib/python3.7/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/Users/jing.pan/anaconda3/lib/python3.7/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/Users/jing.pan/anaconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O3"
         ],
         "include_dirs": [
-            "/Users/jeong/miniconda3/envs/py37/lib/python3.7/site-packages/numpy/core/include"
+            "/Users/jing.pan/anaconda3/lib/python3.7/site-packages/numpy/core/include"
         ],
         "name": "causalml.inference.tree.causaltree",
         "sources": [
             "causalml/inference/tree/causaltree.pyx"
         ]
     },
     "module_name": "causalml.inference.tree.causaltree"
@@ -25,16 +25,16 @@
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_15"
-#define CYTHON_HEX_VERSION 0x001D0FF0
+#define CYTHON_ABI "0_29_12"
+#define CYTHON_HEX_VERSION 0x001D0CF0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -965,195 +965,195 @@
   Py_ssize_t shape[8];
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":776
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":776
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":777
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":777
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":778
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":778
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":779
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":779
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":783
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":783
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":784
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":784
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":785
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":785
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":786
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":786
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":790
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":790
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":791
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":791
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":800
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":800
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":801
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":801
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":802
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":802
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":804
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":804
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":805
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":805
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":806
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":806
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":808
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":808
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":809
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":809
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":811
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":811
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":812
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":812
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":813
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":813
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1236,42 +1236,42 @@
 struct __pyx_obj_7sklearn_4tree_10_criterion_RegressionCriterion;
 struct __pyx_obj_8causalml_9inference_4tree_10causaltree_CausalMSE;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":815
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":815
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":816
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":816
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":817
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":817
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":819
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":819
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1562,15 +1562,15 @@
   Py_buffer view;
   int flags;
   int dtype_is_object;
   __Pyx_TypeInfo *typeinfo;
 };
 
 
-/* "View.MemoryView":965
+/* "View.MemoryView":961
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 struct __pyx_memoryviewslice_obj {
@@ -1736,15 +1736,15 @@
   PyObject *(*setitem_indexed)(struct __pyx_memoryview_obj *, PyObject *, PyObject *);
   PyObject *(*convert_item_to_object)(struct __pyx_memoryview_obj *, char *);
   PyObject *(*assign_item_from_object)(struct __pyx_memoryview_obj *, char *, PyObject *);
 };
 static struct __pyx_vtabstruct_memoryview *__pyx_vtabptr_memoryview;
 
 
-/* "View.MemoryView":965
+/* "View.MemoryView":961
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 
@@ -7737,15 +7737,15 @@
   __Pyx_XDECREF(__pyx_v_te_lb);
   __Pyx_XDECREF(__pyx_v_te_ub);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":258
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":258
  *         # experimental exception made for __getbuffer__ and __releasebuffer__
  *         # -- the details of this may change.
  *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
  *             # This implementation of getbuffer is geared towards Cython
  *             # requirements, and does not yet fulfill the PEP.
  */
 
@@ -7786,344 +7786,344 @@
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":265
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":265
  * 
  *             cdef int i, ndim
  *             cdef int endian_detector = 1             # <<<<<<<<<<<<<<
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  * 
  */
   __pyx_v_endian_detector = 1;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":266
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":266
  *             cdef int i, ndim
  *             cdef int endian_detector = 1
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
  * 
  *             ndim = PyArray_NDIM(self)
  */
   __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":268
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":268
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  * 
  *             ndim = PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  */
   __pyx_v_ndim = PyArray_NDIM(__pyx_v_self);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":270
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":270
  *             ndim = PyArray_NDIM(self)
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   __pyx_t_2 = (((__pyx_v_flags & PyBUF_C_CONTIGUOUS) == PyBUF_C_CONTIGUOUS) != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":271
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":271
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):             # <<<<<<<<<<<<<<
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  */
   __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_C_CONTIGUOUS) != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":270
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":270
  *             ndim = PyArray_NDIM(self)
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   if (unlikely(__pyx_t_1)) {
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":272
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":272
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  */
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 272, __pyx_L1_error)
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":270
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":270
  *             ndim = PyArray_NDIM(self)
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":274
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   __pyx_t_2 = (((__pyx_v_flags & PyBUF_F_CONTIGUOUS) == PyBUF_F_CONTIGUOUS) != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L7_bool_binop_done;
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":275
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":275
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):             # <<<<<<<<<<<<<<
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  * 
  */
   __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_F_CONTIGUOUS) != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L7_bool_binop_done:;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":274
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   if (unlikely(__pyx_t_1)) {
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":276
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":276
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
  * 
  *             info.buf = PyArray_DATA(self)
  */
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 276, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 276, __pyx_L1_error)
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":274
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":278
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":278
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  * 
  *             info.buf = PyArray_DATA(self)             # <<<<<<<<<<<<<<
  *             info.ndim = ndim
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   __pyx_v_info->buf = PyArray_DATA(__pyx_v_self);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":279
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":279
  * 
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim             # <<<<<<<<<<<<<<
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  *                 # Allocate new buffer for strides and shape info.
  */
   __pyx_v_info->ndim = __pyx_v_ndim;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":280
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":280
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  */
   __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
   if (__pyx_t_1) {
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":283
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":283
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)             # <<<<<<<<<<<<<<
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):
  */
     __pyx_v_info->strides = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * 2) * ((size_t)__pyx_v_ndim))));
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":284
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":284
  *                 # This is allocated as one block, strides first.
  *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
  *                 info.shape = info.strides + ndim             # <<<<<<<<<<<<<<
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  */
     __pyx_v_info->shape = (__pyx_v_info->strides + __pyx_v_ndim);
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":285
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":285
  *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):             # <<<<<<<<<<<<<<
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  */
     __pyx_t_4 = __pyx_v_ndim;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":286
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":286
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]             # <<<<<<<<<<<<<<
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  *             else:
  */
       (__pyx_v_info->strides[__pyx_v_i]) = (PyArray_STRIDES(__pyx_v_self)[__pyx_v_i]);
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":287
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":287
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  *                     info.shape[i] = PyArray_DIMS(self)[i]             # <<<<<<<<<<<<<<
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  */
       (__pyx_v_info->shape[__pyx_v_i]) = (PyArray_DIMS(__pyx_v_self)[__pyx_v_i]);
     }
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":280
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":280
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  */
     goto __pyx_L9;
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":289
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":289
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL
  */
   /*else*/ {
     __pyx_v_info->strides = ((Py_ssize_t *)PyArray_STRIDES(__pyx_v_self));
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":290
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":290
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)
  */
     __pyx_v_info->shape = ((Py_ssize_t *)PyArray_DIMS(__pyx_v_self));
   }
   __pyx_L9:;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":291
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":291
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
  *             info.itemsize = PyArray_ITEMSIZE(self)
  *             info.readonly = not PyArray_ISWRITEABLE(self)
  */
   __pyx_v_info->suboffsets = NULL;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":292
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":292
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)             # <<<<<<<<<<<<<<
  *             info.readonly = not PyArray_ISWRITEABLE(self)
  * 
  */
   __pyx_v_info->itemsize = PyArray_ITEMSIZE(__pyx_v_self);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":293
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":293
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)
  *             info.readonly = not PyArray_ISWRITEABLE(self)             # <<<<<<<<<<<<<<
  * 
  *             cdef int t
  */
   __pyx_v_info->readonly = (!(PyArray_ISWRITEABLE(__pyx_v_self) != 0));
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":296
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":296
  * 
  *             cdef int t
  *             cdef char* f = NULL             # <<<<<<<<<<<<<<
  *             cdef dtype descr = <dtype>PyArray_DESCR(self)
  *             cdef int offset
  */
   __pyx_v_f = NULL;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":297
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":297
  *             cdef int t
  *             cdef char* f = NULL
  *             cdef dtype descr = <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  *             cdef int offset
  * 
  */
   __pyx_t_7 = PyArray_DESCR(__pyx_v_self);
   __pyx_t_3 = ((PyObject *)__pyx_t_7);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_descr = ((PyArray_Descr *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":300
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":300
  *             cdef int offset
  * 
  *             info.obj = self             # <<<<<<<<<<<<<<
  * 
  *             if not PyDataType_HASFIELDS(descr):
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":302
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":302
  *             info.obj = self
  * 
  *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  */
   __pyx_t_1 = ((!(PyDataType_HASFIELDS(__pyx_v_descr) != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":303
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":303
  * 
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num             # <<<<<<<<<<<<<<
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  */
     __pyx_t_4 = __pyx_v_descr->type_num;
     __pyx_v_t = __pyx_t_4;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":304
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":304
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     __pyx_t_2 = ((__pyx_v_descr->byteorder == '>') != 0);
@@ -8135,15 +8135,15 @@
     if (!__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L14_bool_binop_done;
     }
     __pyx_L15_next_or:;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":305
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":305
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"
  */
     __pyx_t_2 = ((__pyx_v_descr->byteorder == '<') != 0);
@@ -8152,235 +8152,235 @@
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L14_bool_binop_done;
     }
     __pyx_t_2 = ((!(__pyx_v_little_endian != 0)) != 0);
     __pyx_t_1 = __pyx_t_2;
     __pyx_L14_bool_binop_done:;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":304
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":304
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     if (unlikely(__pyx_t_1)) {
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":306
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":306
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  */
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 306, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(2, 306, __pyx_L1_error)
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":304
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":304
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     }
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":307
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":307
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"
  */
     switch (__pyx_v_t) {
       case NPY_BYTE:
       __pyx_v_f = ((char *)"b");
       break;
       case NPY_UBYTE:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":308
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":308
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"
  */
       __pyx_v_f = ((char *)"B");
       break;
       case NPY_SHORT:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":309
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":309
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"
  */
       __pyx_v_f = ((char *)"h");
       break;
       case NPY_USHORT:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":310
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":310
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"
  */
       __pyx_v_f = ((char *)"H");
       break;
       case NPY_INT:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":311
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":311
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"
  */
       __pyx_v_f = ((char *)"i");
       break;
       case NPY_UINT:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":312
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":312
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"
  */
       __pyx_v_f = ((char *)"I");
       break;
       case NPY_LONG:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":313
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":313
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"
  */
       __pyx_v_f = ((char *)"l");
       break;
       case NPY_ULONG:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":314
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":314
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  */
       __pyx_v_f = ((char *)"L");
       break;
       case NPY_LONGLONG:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":315
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":315
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"
  */
       __pyx_v_f = ((char *)"q");
       break;
       case NPY_ULONGLONG:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":316
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":316
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"
  */
       __pyx_v_f = ((char *)"Q");
       break;
       case NPY_FLOAT:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":317
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":317
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  */
       __pyx_v_f = ((char *)"f");
       break;
       case NPY_DOUBLE:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":318
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":318
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  */
       __pyx_v_f = ((char *)"d");
       break;
       case NPY_LONGDOUBLE:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":319
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":319
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  */
       __pyx_v_f = ((char *)"g");
       break;
       case NPY_CFLOAT:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":320
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":320
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  */
       __pyx_v_f = ((char *)"Zf");
       break;
       case NPY_CDOUBLE:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":321
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":321
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  *                 elif t == NPY_OBJECT:      f = "O"
  */
       __pyx_v_f = ((char *)"Zd");
       break;
       case NPY_CLONGDOUBLE:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":322
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":322
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_OBJECT:      f = "O"
  *                 else:
  */
       __pyx_v_f = ((char *)"Zg");
       break;
       case NPY_OBJECT:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":323
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":323
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  *                 elif t == NPY_OBJECT:      f = "O"             # <<<<<<<<<<<<<<
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  */
       __pyx_v_f = ((char *)"O");
       break;
       default:
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":325
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":325
  *                 elif t == NPY_OBJECT:      f = "O"
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
  *                 info.format = f
  *                 return
  */
       __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 325, __pyx_L1_error)
@@ -8393,91 +8393,91 @@
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(2, 325, __pyx_L1_error)
       break;
     }
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":326
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":326
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *                 info.format = f             # <<<<<<<<<<<<<<
  *                 return
  *             else:
  */
     __pyx_v_info->format = __pyx_v_f;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":327
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":327
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *                 info.format = f
  *                 return             # <<<<<<<<<<<<<<
  *             else:
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":302
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":302
  *             info.obj = self
  * 
  *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  */
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":329
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":329
  *                 return
  *             else:
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)             # <<<<<<<<<<<<<<
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0
  */
   /*else*/ {
     __pyx_v_info->format = ((char *)PyObject_Malloc(0xFF));
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":330
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":330
  *             else:
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  *                 info.format[0] = c'^' # Native data types, manual alignment             # <<<<<<<<<<<<<<
  *                 offset = 0
  *                 f = _util_dtypestring(descr, info.format + 1,
  */
     (__pyx_v_info->format[0]) = '^';
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":331
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":331
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0             # <<<<<<<<<<<<<<
  *                 f = _util_dtypestring(descr, info.format + 1,
  *                                       info.format + _buffer_format_string_len,
  */
     __pyx_v_offset = 0;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":332
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":332
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0
  *                 f = _util_dtypestring(descr, info.format + 1,             # <<<<<<<<<<<<<<
  *                                       info.format + _buffer_format_string_len,
  *                                       &offset)
  */
     __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_descr, (__pyx_v_info->format + 1), (__pyx_v_info->format + 0xFF), (&__pyx_v_offset)); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(2, 332, __pyx_L1_error)
     __pyx_v_f = __pyx_t_9;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":335
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":335
  *                                       info.format + _buffer_format_string_len,
  *                                       &offset)
  *                 f[0] = c'\0' # Terminate format string             # <<<<<<<<<<<<<<
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  */
     (__pyx_v_f[0]) = '\x00';
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":258
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":258
  *         # experimental exception made for __getbuffer__ and __releasebuffer__
  *         # -- the details of this may change.
  *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
  *             # This implementation of getbuffer is geared towards Cython
  *             # requirements, and does not yet fulfill the PEP.
  */
 
@@ -8501,15 +8501,15 @@
   }
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_descr);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":337
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":337
  *                 f[0] = c'\0' # Terminate format string
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  */
 
@@ -8525,111 +8525,111 @@
 }
 
 static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__releasebuffer__", 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":338
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":338
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   __pyx_t_1 = (PyArray_HASFIELDS(__pyx_v_self) != 0);
   if (__pyx_t_1) {
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":339
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":339
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)             # <<<<<<<<<<<<<<
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  *                 PyObject_Free(info.strides)
  */
     PyObject_Free(__pyx_v_info->format);
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":338
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":338
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":340
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":340
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.strides)
  *                 # info.shape was stored after info.strides in the same block
  */
   __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
   if (__pyx_t_1) {
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":341
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":341
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  *                 PyObject_Free(info.strides)             # <<<<<<<<<<<<<<
  *                 # info.shape was stored after info.strides in the same block
  * 
  */
     PyObject_Free(__pyx_v_info->strides);
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":340
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":340
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.strides)
  *                 # info.shape was stored after info.strides in the same block
  */
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":337
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":337
  *                 f[0] = c'\0' # Terminate format string
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":821
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":821
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":822
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":822
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 822, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":821
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":821
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8640,43 +8640,43 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":824
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":824
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":825
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":825
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 825, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":824
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":824
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8687,43 +8687,43 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":827
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":827
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":828
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":828
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":827
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":827
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8734,43 +8734,43 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":830
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":830
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":831
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":831
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 831, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":830
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":830
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -8781,43 +8781,43 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":833
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":833
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":834
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":834
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 834, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":833
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":833
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -8828,89 +8828,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":836
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":836
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":837
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":837
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":838
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":838
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":837
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":837
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":840
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":840
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":836
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":836
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":842
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":842
  *         return ()
  * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
  *     # Recursive utility function used in __getbuffer__ to get format
  *     # string. The new location in the format string is returned.
  */
 
@@ -8931,33 +8931,33 @@
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_t_7;
   long __pyx_t_8;
   char *__pyx_t_9;
   __Pyx_RefNannySetupContext("_util_dtypestring", 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":847
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":847
  * 
  *     cdef dtype child
  *     cdef int endian_detector = 1             # <<<<<<<<<<<<<<
  *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  *     cdef tuple fields
  */
   __pyx_v_endian_detector = 1;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":848
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":848
  *     cdef dtype child
  *     cdef int endian_detector = 1
  *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
  *     cdef tuple fields
  * 
  */
   __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":851
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":851
  *     cdef tuple fields
  * 
  *     for childname in descr.names:             # <<<<<<<<<<<<<<
  *         fields = descr.fields[childname]
  *         child, new_offset = fields
  */
   if (unlikely(__pyx_v_descr->names == Py_None)) {
@@ -8972,15 +8972,15 @@
     #else
     __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 851, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_childname, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":852
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":852
  * 
  *     for childname in descr.names:
  *         fields = descr.fields[childname]             # <<<<<<<<<<<<<<
  *         child, new_offset = fields
  * 
  */
     if (unlikely(__pyx_v_descr->fields == Py_None)) {
@@ -8989,15 +8989,15 @@
     }
     __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_descr->fields, __pyx_v_childname); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 852, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (!(likely(PyTuple_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(2, 852, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_fields, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":853
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":853
  *     for childname in descr.names:
  *         fields = descr.fields[childname]
  *         child, new_offset = fields             # <<<<<<<<<<<<<<
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  */
     if (likely(__pyx_v_fields != Py_None)) {
@@ -9024,15 +9024,15 @@
     }
     if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_dtype))))) __PYX_ERR(2, 853, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_child, ((PyArray_Descr *)__pyx_t_3));
     __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_new_offset, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":855
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":855
  *         child, new_offset = fields
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  */
     __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 855, __pyx_L1_error)
@@ -9041,37 +9041,37 @@
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 855, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_6 = ((((__pyx_v_end - __pyx_v_f) - ((int)__pyx_t_5)) < 15) != 0);
     if (unlikely(__pyx_t_6)) {
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":856
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":856
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  */
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 856, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(2, 856, __pyx_L1_error)
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":855
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":855
  *         child, new_offset = fields
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  */
     }
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":858
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":858
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     __pyx_t_7 = ((__pyx_v_child->byteorder == '>') != 0);
@@ -9083,15 +9083,15 @@
     if (!__pyx_t_7) {
     } else {
       __pyx_t_6 = __pyx_t_7;
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_L8_next_or:;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":859
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":859
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  *             (child.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
  *             raise ValueError(u"Non-native byte order not supported")
  *             # One could encode it in the format string and have Cython
  */
     __pyx_t_7 = ((__pyx_v_child->byteorder == '<') != 0);
@@ -9100,46 +9100,46 @@
       __pyx_t_6 = __pyx_t_7;
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_t_7 = ((!(__pyx_v_little_endian != 0)) != 0);
     __pyx_t_6 = __pyx_t_7;
     __pyx_L7_bool_binop_done:;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":858
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":858
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     if (unlikely(__pyx_t_6)) {
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":860
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":860
  *         if ((child.byteorder == c'>' and little_endian) or
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *             # One could encode it in the format string and have Cython
  *             # complain instead, BUT: < and > in format strings also imply
  */
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 860, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(2, 860, __pyx_L1_error)
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":858
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":858
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     }
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":870
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":870
  * 
  *         # Output padding bytes
  *         while offset[0] < new_offset:             # <<<<<<<<<<<<<<
  *             f[0] = 120 # "x"; pad byte
  *             f += 1
  */
     while (1) {
@@ -9147,108 +9147,108 @@
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_new_offset, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 870, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 870, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (!__pyx_t_6) break;
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":871
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":871
  *         # Output padding bytes
  *         while offset[0] < new_offset:
  *             f[0] = 120 # "x"; pad byte             # <<<<<<<<<<<<<<
  *             f += 1
  *             offset[0] += 1
  */
       (__pyx_v_f[0]) = 0x78;
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":872
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":872
  *         while offset[0] < new_offset:
  *             f[0] = 120 # "x"; pad byte
  *             f += 1             # <<<<<<<<<<<<<<
  *             offset[0] += 1
  * 
  */
       __pyx_v_f = (__pyx_v_f + 1);
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":873
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":873
  *             f[0] = 120 # "x"; pad byte
  *             f += 1
  *             offset[0] += 1             # <<<<<<<<<<<<<<
  * 
  *         offset[0] += child.itemsize
  */
       __pyx_t_8 = 0;
       (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + 1);
     }
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":875
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":875
  *             offset[0] += 1
  * 
  *         offset[0] += child.itemsize             # <<<<<<<<<<<<<<
  * 
  *         if not PyDataType_HASFIELDS(child):
  */
     __pyx_t_8 = 0;
     (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + __pyx_v_child->elsize);
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":877
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":877
  *         offset[0] += child.itemsize
  * 
  *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
  *             t = child.type_num
  *             if end - f < 5:
  */
     __pyx_t_6 = ((!(PyDataType_HASFIELDS(__pyx_v_child) != 0)) != 0);
     if (__pyx_t_6) {
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":878
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":878
  * 
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num             # <<<<<<<<<<<<<<
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")
  */
       __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_child->type_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 878, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":879
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":879
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num
  *             if end - f < 5:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError(u"Format string allocated too short.")
  * 
  */
       __pyx_t_6 = (((__pyx_v_end - __pyx_v_f) < 5) != 0);
       if (unlikely(__pyx_t_6)) {
 
-        /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":880
+        /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":880
  *             t = child.type_num
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  */
         __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 880, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_Raise(__pyx_t_4, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __PYX_ERR(2, 880, __pyx_L1_error)
 
-        /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":879
+        /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":879
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num
  *             if end - f < 5:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError(u"Format string allocated too short.")
  * 
  */
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":883
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":883
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"             # <<<<<<<<<<<<<<
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_BYTE); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 883, __pyx_L1_error)
@@ -9258,15 +9258,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 883, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 98;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":884
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":884
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"             # <<<<<<<<<<<<<<
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UBYTE); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 884, __pyx_L1_error)
@@ -9276,15 +9276,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 884, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 66;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":885
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":885
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"             # <<<<<<<<<<<<<<
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_SHORT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 885, __pyx_L1_error)
@@ -9294,15 +9294,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 885, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x68;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":886
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":886
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"             # <<<<<<<<<<<<<<
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_USHORT); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 886, __pyx_L1_error)
@@ -9312,15 +9312,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 886, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 72;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":887
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":887
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"             # <<<<<<<<<<<<<<
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_INT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 887, __pyx_L1_error)
@@ -9330,15 +9330,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 887, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x69;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":888
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":888
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 888, __pyx_L1_error)
@@ -9348,15 +9348,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 888, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 73;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":889
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":889
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"             # <<<<<<<<<<<<<<
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 889, __pyx_L1_error)
@@ -9366,15 +9366,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 889, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x6C;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":890
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":890
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 890, __pyx_L1_error)
@@ -9384,15 +9384,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 890, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 76;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":891
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":891
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"             # <<<<<<<<<<<<<<
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGLONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 891, __pyx_L1_error)
@@ -9402,15 +9402,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 891, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x71;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":892
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":892
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"             # <<<<<<<<<<<<<<
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONGLONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 892, __pyx_L1_error)
@@ -9420,15 +9420,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 892, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 81;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":893
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":893
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"             # <<<<<<<<<<<<<<
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_FLOAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 893, __pyx_L1_error)
@@ -9438,15 +9438,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 893, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x66;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":894
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":894
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_DOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 894, __pyx_L1_error)
@@ -9456,15 +9456,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 894, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x64;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":895
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":895
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"             # <<<<<<<<<<<<<<
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 895, __pyx_L1_error)
@@ -9474,15 +9474,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 895, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x67;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":896
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":896
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf             # <<<<<<<<<<<<<<
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CFLOAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 896, __pyx_L1_error)
@@ -9494,15 +9494,15 @@
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x66;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":897
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":897
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd             # <<<<<<<<<<<<<<
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 897, __pyx_L1_error)
@@ -9514,15 +9514,15 @@
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x64;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":898
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":898
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg             # <<<<<<<<<<<<<<
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  *             else:
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CLONGDOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 898, __pyx_L1_error)
@@ -9534,15 +9534,15 @@
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x67;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":899
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":899
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"             # <<<<<<<<<<<<<<
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_OBJECT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 899, __pyx_L1_error)
@@ -9552,15 +9552,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 899, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (likely(__pyx_t_6)) {
         (__pyx_v_f[0]) = 79;
         goto __pyx_L15;
       }
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":901
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":901
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
  *             f += 1
  *         else:
  */
       /*else*/ {
@@ -9571,67 +9571,67 @@
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_Raise(__pyx_t_4, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __PYX_ERR(2, 901, __pyx_L1_error)
       }
       __pyx_L15:;
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":902
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":902
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *             f += 1             # <<<<<<<<<<<<<<
  *         else:
  *             # Cython ignores struct boundary information ("T{...}"),
  */
       __pyx_v_f = (__pyx_v_f + 1);
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":877
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":877
  *         offset[0] += child.itemsize
  * 
  *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
  *             t = child.type_num
  *             if end - f < 5:
  */
       goto __pyx_L13;
     }
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":906
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":906
  *             # Cython ignores struct boundary information ("T{...}"),
  *             # so don't output it
  *             f = _util_dtypestring(child, f, end, offset)             # <<<<<<<<<<<<<<
  *     return f
  * 
  */
     /*else*/ {
       __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_child, __pyx_v_f, __pyx_v_end, __pyx_v_offset); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(2, 906, __pyx_L1_error)
       __pyx_v_f = __pyx_t_9;
     }
     __pyx_L13:;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":851
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":851
  *     cdef tuple fields
  * 
  *     for childname in descr.names:             # <<<<<<<<<<<<<<
  *         fields = descr.fields[childname]
  *         child, new_offset = fields
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":907
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":907
  *             # so don't output it
  *             f = _util_dtypestring(child, f, end, offset)
  *     return f             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_f;
   goto __pyx_L0;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":842
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":842
  *         return ()
  * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
  *     # Recursive utility function used in __getbuffer__ to get format
  *     # string. The new location in the format string is returned.
  */
 
@@ -9648,138 +9648,138 @@
   __Pyx_XDECREF(__pyx_v_childname);
   __Pyx_XDECREF(__pyx_v_new_offset);
   __Pyx_XDECREF(__pyx_v_t);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1022
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1022
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1023
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1023
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1024
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1024
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1022
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1022
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1026
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1026
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1027
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1028
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1028
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1029
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1029
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1028
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1028
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1030
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1030
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1026
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1026
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1034
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_array()
  */
 
@@ -9792,15 +9792,15 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1035
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
   {
@@ -9808,53 +9808,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1036
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1036
  * cdef inline int import_array() except -1:
  *     try:
  *         _import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1036, __pyx_L3_error)
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1035
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1037
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1037
  *     try:
  *         _import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1037, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1038
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1038
  *         _import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1038, __pyx_L5_except_error)
@@ -9862,30 +9862,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1038, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1035
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1034
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_array()
  */
 
@@ -9900,15 +9900,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1040
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9921,15 +9921,15 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1041
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -9937,53 +9937,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1042
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1042
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1042, __pyx_L3_error)
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1041
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1043
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1043, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1044
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1044
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1044, __pyx_L5_except_error)
@@ -9991,30 +9991,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1044, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1041
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1040
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10029,15 +10029,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+/* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1046
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10050,15 +10050,15 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1047
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -10066,81 +10066,81 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1048
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1048
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1048, __pyx_L3_error)
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1047
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1049
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1049
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1049, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1050
+      /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1050
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1050, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1050, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+    /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1047
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1046
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -12912,189 +12912,150 @@
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":373
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
+ * 
  */
   __pyx_t_1 = (__pyx_v_self->obj != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
     /* "View.MemoryView":374
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)             # <<<<<<<<<<<<<<
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  * 
+ *         cdef int i
  */
     __Pyx_ReleaseBuffer((&__pyx_v_self->view));
 
     /* "View.MemoryView":373
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
- */
-    goto __pyx_L3;
-  }
-
-  /* "View.MemoryView":375
- *         if self.obj is not None:
- *             __Pyx_ReleaseBuffer(&self.view)
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
- * 
- *             (<__pyx_buffer *> &self.view).obj = NULL
- */
-  __pyx_t_2 = ((((Py_buffer *)(&__pyx_v_self->view))->obj == Py_None) != 0);
-  if (__pyx_t_2) {
-
-    /* "View.MemoryView":377
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
- * 
- *             (<__pyx_buffer *> &self.view).obj = NULL             # <<<<<<<<<<<<<<
- *             Py_DECREF(Py_None)
  * 
  */
-    ((Py_buffer *)(&__pyx_v_self->view))->obj = NULL;
-
-    /* "View.MemoryView":378
- * 
- *             (<__pyx_buffer *> &self.view).obj = NULL
- *             Py_DECREF(Py_None)             # <<<<<<<<<<<<<<
- * 
- *         cdef int i
- */
-    Py_DECREF(Py_None);
-
-    /* "View.MemoryView":375
- *         if self.obj is not None:
- *             __Pyx_ReleaseBuffer(&self.view)
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
- * 
- *             (<__pyx_buffer *> &self.view).obj = NULL
- */
   }
-  __pyx_L3:;
 
-  /* "View.MemoryView":382
+  /* "View.MemoryView":378
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
   __pyx_t_2 = ((__pyx_v_self->lock != NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":383
+    /* "View.MemoryView":379
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):             # <<<<<<<<<<<<<<
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  */
     __pyx_t_3 = __pyx_memoryview_thread_locks_used;
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
       __pyx_v_i = __pyx_t_5;
 
-      /* "View.MemoryView":384
+      /* "View.MemoryView":380
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
       __pyx_t_2 = (((__pyx_memoryview_thread_locks[__pyx_v_i]) == __pyx_v_self->lock) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":385
+        /* "View.MemoryView":381
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1             # <<<<<<<<<<<<<<
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  */
         __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used - 1);
 
-        /* "View.MemoryView":386
+        /* "View.MemoryView":382
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
         __pyx_t_2 = ((__pyx_v_i != __pyx_memoryview_thread_locks_used) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":388
+          /* "View.MemoryView":384
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])             # <<<<<<<<<<<<<<
  *                     break
  *             else:
  */
           __pyx_t_6 = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
           __pyx_t_7 = (__pyx_memoryview_thread_locks[__pyx_v_i]);
 
-          /* "View.MemoryView":387
+          /* "View.MemoryView":383
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (             # <<<<<<<<<<<<<<
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break
  */
           (__pyx_memoryview_thread_locks[__pyx_v_i]) = __pyx_t_6;
           (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]) = __pyx_t_7;
 
-          /* "View.MemoryView":386
+          /* "View.MemoryView":382
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
         }
 
-        /* "View.MemoryView":389
+        /* "View.MemoryView":385
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break             # <<<<<<<<<<<<<<
  *             else:
  *                 PyThread_free_lock(self.lock)
  */
         goto __pyx_L6_break;
 
-        /* "View.MemoryView":384
+        /* "View.MemoryView":380
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
       }
     }
     /*else*/ {
 
-      /* "View.MemoryView":391
+      /* "View.MemoryView":387
  *                     break
  *             else:
  *                 PyThread_free_lock(self.lock)             # <<<<<<<<<<<<<<
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  */
       PyThread_free_lock(__pyx_v_self->lock);
     }
     __pyx_L6_break:;
 
-    /* "View.MemoryView":382
+    /* "View.MemoryView":378
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
   }
@@ -13107,15 +13068,15 @@
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":393
+/* "View.MemoryView":389
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -13130,107 +13091,107 @@
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   char *__pyx_t_7;
   __Pyx_RefNannySetupContext("get_item_pointer", 0);
 
-  /* "View.MemoryView":395
+  /* "View.MemoryView":391
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf             # <<<<<<<<<<<<<<
  * 
  *         for dim, idx in enumerate(index):
  */
   __pyx_v_itemp = ((char *)__pyx_v_self->view.buf);
 
-  /* "View.MemoryView":397
+  /* "View.MemoryView":393
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_v_index)) || PyTuple_CheckExact(__pyx_v_index)) {
     __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 397, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 393, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 397, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 393, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 393, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 393, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 393, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 393, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 397, __pyx_L1_error)
+          else __PYX_ERR(1, 393, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_1;
     __pyx_t_1 = (__pyx_t_1 + 1);
 
-    /* "View.MemoryView":398
+    /* "View.MemoryView":394
  * 
  *         for dim, idx in enumerate(index):
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)             # <<<<<<<<<<<<<<
  * 
  *         return itemp
  */
-    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 398, __pyx_L1_error)
-    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(1, 398, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 394, __pyx_L1_error)
+    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(1, 394, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_7;
 
-    /* "View.MemoryView":397
+    /* "View.MemoryView":393
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":400
+  /* "View.MemoryView":396
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  *         return itemp             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_itemp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":393
+  /* "View.MemoryView":389
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -13242,15 +13203,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":403
+/* "View.MemoryView":399
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -13277,143 +13238,143 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   char *__pyx_t_6;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "View.MemoryView":404
+  /* "View.MemoryView":400
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
   __pyx_t_1 = (__pyx_v_index == __pyx_builtin_Ellipsis);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":405
+    /* "View.MemoryView":401
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:
  *             return self             # <<<<<<<<<<<<<<
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __pyx_r = ((PyObject *)__pyx_v_self);
     goto __pyx_L0;
 
-    /* "View.MemoryView":404
+    /* "View.MemoryView":400
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
   }
 
-  /* "View.MemoryView":407
+  /* "View.MemoryView":403
  *             return self
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         cdef char *itemp
  */
-  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 407, __pyx_L1_error)
+  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (likely(__pyx_t_3 != Py_None)) {
     PyObject* sequence = __pyx_t_3;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(1, 407, __pyx_L1_error)
+      __PYX_ERR(1, 403, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_t_5);
     #else
-    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 407, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 407, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 407, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 403, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_indices = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "View.MemoryView":410
+  /* "View.MemoryView":406
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 410, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 406, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":411
+    /* "View.MemoryView":407
  *         cdef char *itemp
  *         if have_slices:
  *             return memview_slice(self, indices)             # <<<<<<<<<<<<<<
  *         else:
  *             itemp = self.get_item_pointer(indices)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 411, __pyx_L1_error)
+    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":410
+    /* "View.MemoryView":406
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
   }
 
-  /* "View.MemoryView":413
+  /* "View.MemoryView":409
  *             return memview_slice(self, indices)
  *         else:
  *             itemp = self.get_item_pointer(indices)             # <<<<<<<<<<<<<<
  *             return self.convert_item_to_object(itemp)
  * 
  */
   /*else*/ {
-    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(1, 413, __pyx_L1_error)
+    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(1, 409, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_6;
 
-    /* "View.MemoryView":414
+    /* "View.MemoryView":410
  *         else:
  *             itemp = self.get_item_pointer(indices)
  *             return self.convert_item_to_object(itemp)             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(memoryview self, object index, object value):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 414, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 410, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":403
+  /* "View.MemoryView":399
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -13428,15 +13389,15 @@
   __Pyx_XDECREF(__pyx_v_have_slices);
   __Pyx_XDECREF(__pyx_v_indices);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":416
+/* "View.MemoryView":412
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -13461,182 +13422,182 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   __Pyx_RefNannySetupContext("__setitem__", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "View.MemoryView":417
+  /* "View.MemoryView":413
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
   __pyx_t_1 = (__pyx_v_self->view.readonly != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":418
+    /* "View.MemoryView":414
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 418, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 418, __pyx_L1_error)
+    __PYX_ERR(1, 414, __pyx_L1_error)
 
-    /* "View.MemoryView":417
+    /* "View.MemoryView":413
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":420
+  /* "View.MemoryView":416
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         if have_slices:
  */
-  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
+  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (likely(__pyx_t_2 != Py_None)) {
     PyObject* sequence = __pyx_t_2;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(1, 420, __pyx_L1_error)
+      __PYX_ERR(1, 416, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     #else
-    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 420, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 416, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_3;
   __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_index, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "View.MemoryView":422
+  /* "View.MemoryView":418
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 422, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 418, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":423
+    /* "View.MemoryView":419
  * 
  *         if have_slices:
  *             obj = self.is_slice(value)             # <<<<<<<<<<<<<<
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 423, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_obj = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":424
+    /* "View.MemoryView":420
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 424, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 420, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":425
+      /* "View.MemoryView":421
  *             obj = self.is_slice(value)
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)             # <<<<<<<<<<<<<<
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)
  */
-      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 425, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 421, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 425, __pyx_L1_error)
+      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 421, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "View.MemoryView":424
+      /* "View.MemoryView":420
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":427
+    /* "View.MemoryView":423
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)             # <<<<<<<<<<<<<<
  *         else:
  *             self.setitem_indexed(index, value)
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 427, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(1, 427, __pyx_L1_error)
-      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 427, __pyx_L1_error)
+      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(1, 423, __pyx_L1_error)
+      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":422
+    /* "View.MemoryView":418
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":429
+  /* "View.MemoryView":425
  *                 self.setitem_slice_assign_scalar(self[index], value)
  *         else:
  *             self.setitem_indexed(index, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef is_slice(self, obj):
  */
   /*else*/ {
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 429, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 425, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":416
+  /* "View.MemoryView":412
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -13653,15 +13614,15 @@
   __Pyx_XDECREF(__pyx_v_have_slices);
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":431
+/* "View.MemoryView":427
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -13676,26 +13637,26 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   __Pyx_RefNannySetupContext("is_slice", 0);
   __Pyx_INCREF(__pyx_v_obj);
 
-  /* "View.MemoryView":432
+  /* "View.MemoryView":428
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_obj, __pyx_memoryview_type); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":433
+    /* "View.MemoryView":429
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
     {
@@ -13703,59 +13664,59 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
-        /* "View.MemoryView":434
+        /* "View.MemoryView":430
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 434, __pyx_L4_error)
+        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 430, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":435
+        /* "View.MemoryView":431
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)             # <<<<<<<<<<<<<<
  *             except TypeError:
  *                 return None
  */
-        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 435, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 431, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
 
-        /* "View.MemoryView":434
+        /* "View.MemoryView":430
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 434, __pyx_L4_error)
+        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 430, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_v_obj);
         __Pyx_GIVEREF(__pyx_v_obj);
         PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_obj);
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_6);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_7);
         __pyx_t_6 = 0;
         __pyx_t_7 = 0;
-        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 434, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 430, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF_SET(__pyx_v_obj, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "View.MemoryView":433
+        /* "View.MemoryView":429
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       }
@@ -13764,30 +13725,30 @@
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L9_try_end;
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "View.MemoryView":436
+      /* "View.MemoryView":432
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  *             except TypeError:             # <<<<<<<<<<<<<<
  *                 return None
  * 
  */
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError);
       if (__pyx_t_9) {
         __Pyx_AddTraceback("View.MemoryView.memoryview.is_slice", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(1, 436, __pyx_L6_except_error)
+        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(1, 432, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":437
+        /* "View.MemoryView":433
  *                                  self.dtype_is_object)
  *             except TypeError:
  *                 return None             # <<<<<<<<<<<<<<
  * 
  *         return obj
  */
         __Pyx_XDECREF(__pyx_r);
@@ -13796,15 +13757,15 @@
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L7_except_return;
       }
       goto __pyx_L6_except_error;
       __pyx_L6_except_error:;
 
-      /* "View.MemoryView":433
+      /* "View.MemoryView":429
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       __Pyx_XGIVEREF(__pyx_t_3);
@@ -13817,36 +13778,36 @@
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       goto __pyx_L0;
       __pyx_L9_try_end:;
     }
 
-    /* "View.MemoryView":432
+    /* "View.MemoryView":428
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
   }
 
-  /* "View.MemoryView":439
+  /* "View.MemoryView":435
  *                 return None
  * 
  *         return obj             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assignment(self, dst, src):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_obj);
   __pyx_r = __pyx_v_obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":431
+  /* "View.MemoryView":427
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -13860,102 +13821,98 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":441
+/* "View.MemoryView":437
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
 static PyObject *__pyx_memoryview_setitem_slice_assignment(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_dst, PyObject *__pyx_v_src) {
   __Pyx_memviewslice __pyx_v_dst_slice;
   __Pyx_memviewslice __pyx_v_src_slice;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_memviewslice *__pyx_t_1;
-  __Pyx_memviewslice *__pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   int __pyx_t_4;
-  int __pyx_t_5;
-  int __pyx_t_6;
   __Pyx_RefNannySetupContext("setitem_slice_assignment", 0);
 
-  /* "View.MemoryView":445
+  /* "View.MemoryView":441
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(1, 445, __pyx_L1_error)
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 445, __pyx_L1_error)
+  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(1, 441, __pyx_L1_error)
 
-  /* "View.MemoryView":446
+  /* "View.MemoryView":442
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],             # <<<<<<<<<<<<<<
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  */
-  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(1, 446, __pyx_L1_error)
-  __pyx_t_2 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice)); if (unlikely(__pyx_t_2 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 446, __pyx_L1_error)
+  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(1, 442, __pyx_L1_error)
 
-  /* "View.MemoryView":447
+  /* "View.MemoryView":443
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 447, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 447, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 447, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 447, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 443, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 443, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 443, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 443, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "View.MemoryView":445
+  /* "View.MemoryView":441
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  __pyx_t_6 = __pyx_memoryview_copy_contents((__pyx_t_1[0]), (__pyx_t_2[0]), __pyx_t_4, __pyx_t_5, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 445, __pyx_L1_error)
+  __pyx_t_4 = __pyx_memoryview_copy_contents((__pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice))[0]), (__pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice))[0]), __pyx_t_2, __pyx_t_3, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 441, __pyx_L1_error)
 
-  /* "View.MemoryView":441
+  /* "View.MemoryView":437
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("View.MemoryView.memoryview.setitem_slice_assignment", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":449
+/* "View.MemoryView":445
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
@@ -13963,218 +13920,216 @@
   int __pyx_v_array[0x80];
   void *__pyx_v_tmp;
   void *__pyx_v_item;
   __Pyx_memviewslice *__pyx_v_dst_slice;
   __Pyx_memviewslice __pyx_v_tmp_slice;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_memviewslice *__pyx_t_1;
-  int __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_t_3;
   int __pyx_t_4;
-  int __pyx_t_5;
-  char const *__pyx_t_6;
+  char const *__pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
-  PyObject *__pyx_t_12 = NULL;
   __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 0);
 
-  /* "View.MemoryView":451
+  /* "View.MemoryView":447
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  *         cdef int array[128]
  *         cdef void *tmp = NULL             # <<<<<<<<<<<<<<
  *         cdef void *item
  * 
  */
   __pyx_v_tmp = NULL;
 
-  /* "View.MemoryView":456
+  /* "View.MemoryView":452
  *         cdef __Pyx_memviewslice *dst_slice
  *         cdef __Pyx_memviewslice tmp_slice
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)             # <<<<<<<<<<<<<<
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  */
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_dst, (&__pyx_v_tmp_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 456, __pyx_L1_error)
-  __pyx_v_dst_slice = __pyx_t_1;
+  __pyx_v_dst_slice = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_dst, (&__pyx_v_tmp_slice));
 
-  /* "View.MemoryView":458
+  /* "View.MemoryView":454
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
-  __pyx_t_2 = ((((size_t)__pyx_v_self->view.itemsize) > (sizeof(__pyx_v_array))) != 0);
-  if (__pyx_t_2) {
+  __pyx_t_1 = ((((size_t)__pyx_v_self->view.itemsize) > (sizeof(__pyx_v_array))) != 0);
+  if (__pyx_t_1) {
 
-    /* "View.MemoryView":459
+    /* "View.MemoryView":455
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)             # <<<<<<<<<<<<<<
  *             if tmp == NULL:
  *                 raise MemoryError
  */
     __pyx_v_tmp = PyMem_Malloc(__pyx_v_self->view.itemsize);
 
-    /* "View.MemoryView":460
+    /* "View.MemoryView":456
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
-    __pyx_t_2 = ((__pyx_v_tmp == NULL) != 0);
-    if (unlikely(__pyx_t_2)) {
+    __pyx_t_1 = ((__pyx_v_tmp == NULL) != 0);
+    if (unlikely(__pyx_t_1)) {
 
-      /* "View.MemoryView":461
+      /* "View.MemoryView":457
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  *                 raise MemoryError             # <<<<<<<<<<<<<<
  *             item = tmp
  *         else:
  */
-      PyErr_NoMemory(); __PYX_ERR(1, 461, __pyx_L1_error)
+      PyErr_NoMemory(); __PYX_ERR(1, 457, __pyx_L1_error)
 
-      /* "View.MemoryView":460
+      /* "View.MemoryView":456
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
     }
 
-    /* "View.MemoryView":462
+    /* "View.MemoryView":458
  *             if tmp == NULL:
  *                 raise MemoryError
  *             item = tmp             # <<<<<<<<<<<<<<
  *         else:
  *             item = <void *> array
  */
     __pyx_v_item = __pyx_v_tmp;
 
-    /* "View.MemoryView":458
+    /* "View.MemoryView":454
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":464
+  /* "View.MemoryView":460
  *             item = tmp
  *         else:
  *             item = <void *> array             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
   /*else*/ {
     __pyx_v_item = ((void *)__pyx_v_array);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":466
+  /* "View.MemoryView":462
  *             item = <void *> array
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value
  */
   /*try:*/ {
 
-    /* "View.MemoryView":467
+    /* "View.MemoryView":463
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
-    __pyx_t_2 = (__pyx_v_self->dtype_is_object != 0);
-    if (__pyx_t_2) {
+    __pyx_t_1 = (__pyx_v_self->dtype_is_object != 0);
+    if (__pyx_t_1) {
 
-      /* "View.MemoryView":468
+      /* "View.MemoryView":464
  *         try:
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value             # <<<<<<<<<<<<<<
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)
  */
       (((PyObject **)__pyx_v_item)[0]) = ((PyObject *)__pyx_v_value);
 
-      /* "View.MemoryView":467
+      /* "View.MemoryView":463
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
       goto __pyx_L8;
     }
 
-    /* "View.MemoryView":470
+    /* "View.MemoryView":466
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else*/ {
-      __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 470, __pyx_L6_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 466, __pyx_L6_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L8:;
 
-    /* "View.MemoryView":474
+    /* "View.MemoryView":470
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
-    __pyx_t_2 = ((__pyx_v_self->view.suboffsets != NULL) != 0);
-    if (__pyx_t_2) {
+    __pyx_t_1 = ((__pyx_v_self->view.suboffsets != NULL) != 0);
+    if (__pyx_t_1) {
 
-      /* "View.MemoryView":475
+      /* "View.MemoryView":471
  * 
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)             # <<<<<<<<<<<<<<
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  *                                 item, self.dtype_is_object)
  */
-      __pyx_t_3 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 475, __pyx_L6_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_2 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 471, __pyx_L6_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "View.MemoryView":474
+      /* "View.MemoryView":470
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
     }
 
-    /* "View.MemoryView":476
+    /* "View.MemoryView":472
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,             # <<<<<<<<<<<<<<
  *                                 item, self.dtype_is_object)
  *         finally:
  */
     __pyx_memoryview_slice_assign_scalar(__pyx_v_dst_slice, __pyx_v_dst->view.ndim, __pyx_v_self->view.itemsize, __pyx_v_item, __pyx_v_self->dtype_is_object);
   }
 
-  /* "View.MemoryView":479
+  /* "View.MemoryView":475
  *                                 item, self.dtype_is_object)
  *         finally:
  *             PyMem_Free(tmp)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_indexed(self, index, value):
  */
   /*finally:*/ {
@@ -14182,67 +14137,67 @@
       PyMem_Free(__pyx_v_tmp);
       goto __pyx_L7;
     }
     __pyx_L6_error:;
     /*exception exit:*/{
       __Pyx_PyThreadState_declare
       __Pyx_PyThreadState_assign
-      __pyx_t_7 = 0; __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0;
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
-      if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9) < 0)) __Pyx_ErrFetch(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
+      __pyx_t_6 = 0; __pyx_t_7 = 0; __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0;
+      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_9, &__pyx_t_10, &__pyx_t_11);
+      if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8) < 0)) __Pyx_ErrFetch(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
+      __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
       __Pyx_XGOTREF(__pyx_t_8);
       __Pyx_XGOTREF(__pyx_t_9);
       __Pyx_XGOTREF(__pyx_t_10);
       __Pyx_XGOTREF(__pyx_t_11);
-      __Pyx_XGOTREF(__pyx_t_12);
-      __pyx_t_4 = __pyx_lineno; __pyx_t_5 = __pyx_clineno; __pyx_t_6 = __pyx_filename;
+      __pyx_t_3 = __pyx_lineno; __pyx_t_4 = __pyx_clineno; __pyx_t_5 = __pyx_filename;
       {
         PyMem_Free(__pyx_v_tmp);
       }
       if (PY_MAJOR_VERSION >= 3) {
+        __Pyx_XGIVEREF(__pyx_t_9);
         __Pyx_XGIVEREF(__pyx_t_10);
         __Pyx_XGIVEREF(__pyx_t_11);
-        __Pyx_XGIVEREF(__pyx_t_12);
-        __Pyx_ExceptionReset(__pyx_t_10, __pyx_t_11, __pyx_t_12);
+        __Pyx_ExceptionReset(__pyx_t_9, __pyx_t_10, __pyx_t_11);
       }
+      __Pyx_XGIVEREF(__pyx_t_6);
       __Pyx_XGIVEREF(__pyx_t_7);
       __Pyx_XGIVEREF(__pyx_t_8);
-      __Pyx_XGIVEREF(__pyx_t_9);
-      __Pyx_ErrRestore(__pyx_t_7, __pyx_t_8, __pyx_t_9);
-      __pyx_t_7 = 0; __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0;
-      __pyx_lineno = __pyx_t_4; __pyx_clineno = __pyx_t_5; __pyx_filename = __pyx_t_6;
+      __Pyx_ErrRestore(__pyx_t_6, __pyx_t_7, __pyx_t_8);
+      __pyx_t_6 = 0; __pyx_t_7 = 0; __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0;
+      __pyx_lineno = __pyx_t_3; __pyx_clineno = __pyx_t_4; __pyx_filename = __pyx_t_5;
       goto __pyx_L1_error;
     }
     __pyx_L7:;
   }
 
-  /* "View.MemoryView":449
+  /* "View.MemoryView":445
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("View.MemoryView.memoryview.setitem_slice_assign_scalar", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":481
+/* "View.MemoryView":477
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -14250,36 +14205,36 @@
   char *__pyx_v_itemp;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("setitem_indexed", 0);
 
-  /* "View.MemoryView":482
+  /* "View.MemoryView":478
  * 
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)             # <<<<<<<<<<<<<<
  *         self.assign_item_from_object(itemp, value)
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(1, 482, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(1, 478, __pyx_L1_error)
   __pyx_v_itemp = __pyx_t_1;
 
-  /* "View.MemoryView":483
+  /* "View.MemoryView":479
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 483, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 479, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":481
+  /* "View.MemoryView":477
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -14292,15 +14247,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":485
+/* "View.MemoryView":481
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -14319,39 +14274,39 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   size_t __pyx_t_10;
   int __pyx_t_11;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
-  /* "View.MemoryView":488
+  /* "View.MemoryView":484
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef bytes bytesitem
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 488, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 484, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":491
+  /* "View.MemoryView":487
  *         cdef bytes bytesitem
  * 
  *         bytesitem = itemp[:self.view.itemsize]             # <<<<<<<<<<<<<<
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  */
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 491, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_bytesitem = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":492
+  /* "View.MemoryView":488
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
   {
@@ -14359,24 +14314,24 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "View.MemoryView":493
+      /* "View.MemoryView":489
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)             # <<<<<<<<<<<<<<
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 493, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 489, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 493, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 489, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = NULL;
       __pyx_t_8 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -14385,94 +14340,94 @@
           __Pyx_DECREF_SET(__pyx_t_5, function);
           __pyx_t_8 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 489, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 489, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       {
-        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 489, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_9);
         if (__pyx_t_7) {
           __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_6);
         __Pyx_INCREF(__pyx_v_bytesitem);
         __Pyx_GIVEREF(__pyx_v_bytesitem);
         PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_bytesitem);
         __pyx_t_6 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 489, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_result = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "View.MemoryView":492
+      /* "View.MemoryView":488
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     }
 
-    /* "View.MemoryView":497
+    /* "View.MemoryView":493
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
     /*else:*/ {
       __pyx_t_10 = strlen(__pyx_v_self->view.format); 
       __pyx_t_11 = ((__pyx_t_10 == 1) != 0);
       if (__pyx_t_11) {
 
-        /* "View.MemoryView":498
+        /* "View.MemoryView":494
  *         else:
  *             if len(self.view.format) == 1:
  *                 return result[0]             # <<<<<<<<<<<<<<
  *             return result
  * 
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 498, __pyx_L5_except_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 494, __pyx_L5_except_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_r = __pyx_t_1;
         __pyx_t_1 = 0;
         goto __pyx_L6_except_return;
 
-        /* "View.MemoryView":497
+        /* "View.MemoryView":493
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
       }
 
-      /* "View.MemoryView":499
+      /* "View.MemoryView":495
  *             if len(self.view.format) == 1:
  *                 return result[0]
  *             return result             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
       __Pyx_XDECREF(__pyx_r);
@@ -14483,52 +14438,52 @@
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "View.MemoryView":494
+    /* "View.MemoryView":490
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:             # <<<<<<<<<<<<<<
  *             raise ValueError("Unable to convert item to object")
  *         else:
  */
     __Pyx_ErrFetch(&__pyx_t_1, &__pyx_t_5, &__pyx_t_9);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 494, __pyx_L5_except_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 490, __pyx_L5_except_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_1, __pyx_t_6);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_ErrRestore(__pyx_t_1, __pyx_t_5, __pyx_t_9);
     __pyx_t_1 = 0; __pyx_t_5 = 0; __pyx_t_9 = 0;
     if (__pyx_t_8) {
       __Pyx_AddTraceback("View.MemoryView.memoryview.convert_item_to_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(1, 494, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(1, 490, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "View.MemoryView":495
+      /* "View.MemoryView":491
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 495, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 491, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(1, 495, __pyx_L5_except_error)
+      __PYX_ERR(1, 491, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "View.MemoryView":492
+    /* "View.MemoryView":488
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -14540,15 +14495,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":485
+  /* "View.MemoryView":481
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -14566,15 +14521,15 @@
   __Pyx_XDECREF(__pyx_v_bytesitem);
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":501
+/* "View.MemoryView":497
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -14597,88 +14552,88 @@
   PyObject *__pyx_t_10 = NULL;
   char *__pyx_t_11;
   char *__pyx_t_12;
   char *__pyx_t_13;
   char *__pyx_t_14;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
-  /* "View.MemoryView":504
+  /* "View.MemoryView":500
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef char c
  *         cdef bytes bytesvalue
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 504, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 500, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":509
+  /* "View.MemoryView":505
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
   __pyx_t_2 = PyTuple_Check(__pyx_v_value); 
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "View.MemoryView":510
+    /* "View.MemoryView":506
  * 
  *         if isinstance(value, tuple):
  *             bytesvalue = struct.pack(self.view.format, *value)             # <<<<<<<<<<<<<<
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 510, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 506, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "View.MemoryView":509
+    /* "View.MemoryView":505
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":512
+  /* "View.MemoryView":508
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)             # <<<<<<<<<<<<<<
  * 
  *         for i, c in enumerate(bytesvalue):
  */
   /*else*/ {
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 512, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 508, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 512, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 508, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -14687,102 +14642,102 @@
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 508, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 508, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 508, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_1);
       __Pyx_INCREF(__pyx_v_value);
       __Pyx_GIVEREF(__pyx_v_value);
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 508, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 508, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":514
+  /* "View.MemoryView":510
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
   __pyx_t_9 = 0;
   if (unlikely(__pyx_v_bytesvalue == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' is not iterable");
-    __PYX_ERR(1, 514, __pyx_L1_error)
+    __PYX_ERR(1, 510, __pyx_L1_error)
   }
   __Pyx_INCREF(__pyx_v_bytesvalue);
   __pyx_t_10 = __pyx_v_bytesvalue;
   __pyx_t_12 = PyBytes_AS_STRING(__pyx_t_10);
   __pyx_t_13 = (__pyx_t_12 + PyBytes_GET_SIZE(__pyx_t_10));
   for (__pyx_t_14 = __pyx_t_12; __pyx_t_14 < __pyx_t_13; __pyx_t_14++) {
     __pyx_t_11 = __pyx_t_14;
     __pyx_v_c = (__pyx_t_11[0]);
 
-    /* "View.MemoryView":515
+    /* "View.MemoryView":511
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
     __pyx_v_i = __pyx_t_9;
 
-    /* "View.MemoryView":514
+    /* "View.MemoryView":510
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
     __pyx_t_9 = (__pyx_t_9 + 1);
 
-    /* "View.MemoryView":515
+    /* "View.MemoryView":511
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
     (__pyx_v_itemp[__pyx_v_i]) = __pyx_v_c;
   }
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "View.MemoryView":501
+  /* "View.MemoryView":497
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -14802,15 +14757,15 @@
   __Pyx_XDECREF(__pyx_v_struct);
   __Pyx_XDECREF(__pyx_v_bytesvalue);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":518
+/* "View.MemoryView":514
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -14842,15 +14797,15 @@
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
 
-  /* "View.MemoryView":519
+  /* "View.MemoryView":515
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
   __pyx_t_2 = ((__pyx_v_flags & PyBUF_WRITABLE) != 0);
@@ -14860,268 +14815,268 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (__pyx_v_self->view.readonly != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":520
+    /* "View.MemoryView":516
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 520, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 516, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 520, __pyx_L1_error)
+    __PYX_ERR(1, 516, __pyx_L1_error)
 
-    /* "View.MemoryView":519
+    /* "View.MemoryView":515
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":522
+  /* "View.MemoryView":518
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_ND) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":523
+    /* "View.MemoryView":519
  * 
  *         if flags & PyBUF_ND:
  *             info.shape = self.view.shape             # <<<<<<<<<<<<<<
  *         else:
  *             info.shape = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.shape;
     __pyx_v_info->shape = __pyx_t_4;
 
-    /* "View.MemoryView":522
+    /* "View.MemoryView":518
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
     goto __pyx_L6;
   }
 
-  /* "View.MemoryView":525
+  /* "View.MemoryView":521
  *             info.shape = self.view.shape
  *         else:
  *             info.shape = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_STRIDES:
  */
   /*else*/ {
     __pyx_v_info->shape = NULL;
   }
   __pyx_L6:;
 
-  /* "View.MemoryView":527
+  /* "View.MemoryView":523
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_STRIDES) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":528
+    /* "View.MemoryView":524
  * 
  *         if flags & PyBUF_STRIDES:
  *             info.strides = self.view.strides             # <<<<<<<<<<<<<<
  *         else:
  *             info.strides = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.strides;
     __pyx_v_info->strides = __pyx_t_4;
 
-    /* "View.MemoryView":527
+    /* "View.MemoryView":523
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
     goto __pyx_L7;
   }
 
-  /* "View.MemoryView":530
+  /* "View.MemoryView":526
  *             info.strides = self.view.strides
  *         else:
  *             info.strides = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_INDIRECT:
  */
   /*else*/ {
     __pyx_v_info->strides = NULL;
   }
   __pyx_L7:;
 
-  /* "View.MemoryView":532
+  /* "View.MemoryView":528
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_INDIRECT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":533
+    /* "View.MemoryView":529
  * 
  *         if flags & PyBUF_INDIRECT:
  *             info.suboffsets = self.view.suboffsets             # <<<<<<<<<<<<<<
  *         else:
  *             info.suboffsets = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.suboffsets;
     __pyx_v_info->suboffsets = __pyx_t_4;
 
-    /* "View.MemoryView":532
+    /* "View.MemoryView":528
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
     goto __pyx_L8;
   }
 
-  /* "View.MemoryView":535
+  /* "View.MemoryView":531
  *             info.suboffsets = self.view.suboffsets
  *         else:
  *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
   /*else*/ {
     __pyx_v_info->suboffsets = NULL;
   }
   __pyx_L8:;
 
-  /* "View.MemoryView":537
+  /* "View.MemoryView":533
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":538
+    /* "View.MemoryView":534
  * 
  *         if flags & PyBUF_FORMAT:
  *             info.format = self.view.format             # <<<<<<<<<<<<<<
  *         else:
  *             info.format = NULL
  */
     __pyx_t_5 = __pyx_v_self->view.format;
     __pyx_v_info->format = __pyx_t_5;
 
-    /* "View.MemoryView":537
+    /* "View.MemoryView":533
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":540
+  /* "View.MemoryView":536
  *             info.format = self.view.format
  *         else:
  *             info.format = NULL             # <<<<<<<<<<<<<<
  * 
  *         info.buf = self.view.buf
  */
   /*else*/ {
     __pyx_v_info->format = NULL;
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":542
+  /* "View.MemoryView":538
  *             info.format = NULL
  * 
  *         info.buf = self.view.buf             # <<<<<<<<<<<<<<
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  */
   __pyx_t_6 = __pyx_v_self->view.buf;
   __pyx_v_info->buf = __pyx_t_6;
 
-  /* "View.MemoryView":543
+  /* "View.MemoryView":539
  * 
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim             # <<<<<<<<<<<<<<
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  */
   __pyx_t_7 = __pyx_v_self->view.ndim;
   __pyx_v_info->ndim = __pyx_t_7;
 
-  /* "View.MemoryView":544
+  /* "View.MemoryView":540
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize             # <<<<<<<<<<<<<<
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  */
   __pyx_t_8 = __pyx_v_self->view.itemsize;
   __pyx_v_info->itemsize = __pyx_t_8;
 
-  /* "View.MemoryView":545
+  /* "View.MemoryView":541
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len             # <<<<<<<<<<<<<<
  *         info.readonly = self.view.readonly
  *         info.obj = self
  */
   __pyx_t_8 = __pyx_v_self->view.len;
   __pyx_v_info->len = __pyx_t_8;
 
-  /* "View.MemoryView":546
+  /* "View.MemoryView":542
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly             # <<<<<<<<<<<<<<
  *         info.obj = self
  * 
  */
   __pyx_t_1 = __pyx_v_self->view.readonly;
   __pyx_v_info->readonly = __pyx_t_1;
 
-  /* "View.MemoryView":547
+  /* "View.MemoryView":543
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  *         info.obj = self             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "View.MemoryView":518
+  /* "View.MemoryView":514
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -15143,15 +15098,15 @@
     __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
   }
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":553
+/* "View.MemoryView":549
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -15172,49 +15127,49 @@
   struct __pyx_memoryviewslice_obj *__pyx_v_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":554
+  /* "View.MemoryView":550
  *     @property
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&result.from_slice)
  *         return result
  */
-  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 554, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(1, 554, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(1, 550, __pyx_L1_error)
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":555
+  /* "View.MemoryView":551
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)             # <<<<<<<<<<<<<<
  *         return result
  * 
  */
-  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 555, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 551, __pyx_L1_error)
 
-  /* "View.MemoryView":556
+  /* "View.MemoryView":552
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  *         return result             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":553
+  /* "View.MemoryView":549
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -15226,15 +15181,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":559
+/* "View.MemoryView":555
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
@@ -15252,42 +15207,42 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4base___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":560
+  /* "View.MemoryView":556
  *     @property
  *     def base(self):
  *         return self.obj             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->obj);
   __pyx_r = __pyx_v_self->obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":559
+  /* "View.MemoryView":555
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":563
+/* "View.MemoryView":559
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -15311,41 +15266,41 @@
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":564
+  /* "View.MemoryView":560
  *     @property
  *     def shape(self):
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 564, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
   for (__pyx_t_4 = __pyx_v_self->view.shape; __pyx_t_4 < __pyx_t_3; __pyx_t_4++) {
     __pyx_t_2 = __pyx_t_4;
     __pyx_v_length = (__pyx_t_2[0]);
-    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 564, __pyx_L1_error)
+    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 560, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 564, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 560, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 564, __pyx_L1_error)
+  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":563
+  /* "View.MemoryView":559
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -15357,15 +15312,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":567
+/* "View.MemoryView":563
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -15390,73 +15345,73 @@
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":568
+  /* "View.MemoryView":564
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
   __pyx_t_1 = ((__pyx_v_self->view.strides == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":570
+    /* "View.MemoryView":566
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 570, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 566, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 570, __pyx_L1_error)
+    __PYX_ERR(1, 566, __pyx_L1_error)
 
-    /* "View.MemoryView":568
+    /* "View.MemoryView":564
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
   }
 
-  /* "View.MemoryView":572
+  /* "View.MemoryView":568
  *             raise ValueError("Buffer view does not expose strides")
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = (__pyx_v_self->view.strides + __pyx_v_self->view.ndim);
   for (__pyx_t_5 = __pyx_v_self->view.strides; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
     __pyx_t_3 = __pyx_t_5;
     __pyx_v_stride = (__pyx_t_3[0]);
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 572, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 568, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(1, 572, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(1, 568, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":567
+  /* "View.MemoryView":563
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -15468,15 +15423,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":575
+/* "View.MemoryView":571
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -15501,77 +15456,77 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   Py_ssize_t *__pyx_t_6;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":576
+  /* "View.MemoryView":572
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->view.suboffsets == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":577
+    /* "View.MemoryView":573
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 577, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 573, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__24, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 577, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__24, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 573, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":576
+    /* "View.MemoryView":572
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
   }
 
-  /* "View.MemoryView":579
+  /* "View.MemoryView":575
  *             return (-1,) * self.view.ndim
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = (__pyx_v_self->view.suboffsets + __pyx_v_self->view.ndim);
   for (__pyx_t_6 = __pyx_v_self->view.suboffsets; __pyx_t_6 < __pyx_t_5; __pyx_t_6++) {
     __pyx_t_4 = __pyx_t_6;
     __pyx_v_suboffset = (__pyx_t_4[0]);
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 575, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(1, 579, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(1, 575, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":575
+  /* "View.MemoryView":571
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -15583,15 +15538,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":582
+/* "View.MemoryView":578
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -15610,29 +15565,29 @@
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4ndim___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":583
+  /* "View.MemoryView":579
  *     @property
  *     def ndim(self):
  *         return self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 583, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":582
+  /* "View.MemoryView":578
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -15643,15 +15598,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":586
+/* "View.MemoryView":582
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -15670,29 +15625,29 @@
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_8itemsize___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":587
+  /* "View.MemoryView":583
  *     @property
  *     def itemsize(self):
  *         return self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 587, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":586
+  /* "View.MemoryView":582
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -15703,15 +15658,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":590
+/* "View.MemoryView":586
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -15732,35 +15687,35 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":591
+  /* "View.MemoryView":587
  *     @property
  *     def nbytes(self):
  *         return self.size * self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 591, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 587, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 591, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 587, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 591, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 587, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":590
+  /* "View.MemoryView":586
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -15773,15 +15728,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":594
+/* "View.MemoryView":590
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -15807,98 +15762,98 @@
   int __pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":595
+  /* "View.MemoryView":591
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
   __pyx_t_1 = (__pyx_v_self->_size == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":596
+    /* "View.MemoryView":592
  *     def size(self):
  *         if self._size is None:
  *             result = 1             # <<<<<<<<<<<<<<
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  */
     __Pyx_INCREF(__pyx_int_1);
     __pyx_v_result = __pyx_int_1;
 
-    /* "View.MemoryView":598
+    /* "View.MemoryView":594
  *             result = 1
  * 
  *             for length in self.view.shape[:self.view.ndim]:             # <<<<<<<<<<<<<<
  *                 result *= length
  * 
  */
     __pyx_t_4 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
     for (__pyx_t_5 = __pyx_v_self->view.shape; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
       __pyx_t_3 = __pyx_t_5;
-      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 598, __pyx_L1_error)
+      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 594, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "View.MemoryView":599
+      /* "View.MemoryView":595
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  *                 result *= length             # <<<<<<<<<<<<<<
  * 
  *             self._size = result
  */
-      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 599, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 595, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_6);
       __pyx_t_6 = 0;
     }
 
-    /* "View.MemoryView":601
+    /* "View.MemoryView":597
  *                 result *= length
  * 
  *             self._size = result             # <<<<<<<<<<<<<<
  * 
  *         return self._size
  */
     __Pyx_INCREF(__pyx_v_result);
     __Pyx_GIVEREF(__pyx_v_result);
     __Pyx_GOTREF(__pyx_v_self->_size);
     __Pyx_DECREF(__pyx_v_self->_size);
     __pyx_v_self->_size = __pyx_v_result;
 
-    /* "View.MemoryView":595
+    /* "View.MemoryView":591
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
   }
 
-  /* "View.MemoryView":603
+  /* "View.MemoryView":599
  *             self._size = result
  * 
  *         return self._size             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_size);
   __pyx_r = __pyx_v_self->_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":594
+  /* "View.MemoryView":590
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -15911,15 +15866,15 @@
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":605
+/* "View.MemoryView":601
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
@@ -15938,68 +15893,68 @@
 
 static Py_ssize_t __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_10__len__(struct __pyx_memoryview_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "View.MemoryView":606
+  /* "View.MemoryView":602
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->view.ndim >= 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":607
+    /* "View.MemoryView":603
  *     def __len__(self):
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]             # <<<<<<<<<<<<<<
  * 
  *         return 0
  */
     __pyx_r = (__pyx_v_self->view.shape[0]);
     goto __pyx_L0;
 
-    /* "View.MemoryView":606
+    /* "View.MemoryView":602
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
   }
 
-  /* "View.MemoryView":609
+  /* "View.MemoryView":605
  *             return self.view.shape[0]
  * 
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":605
+  /* "View.MemoryView":601
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":611
+/* "View.MemoryView":607
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -16020,64 +15975,64 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "View.MemoryView":612
+  /* "View.MemoryView":608
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":613
+  /* "View.MemoryView":609
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))             # <<<<<<<<<<<<<<
  * 
  *     def __str__(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 613, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 609, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "View.MemoryView":612
+  /* "View.MemoryView":608
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":611
+  /* "View.MemoryView":607
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -16090,15 +16045,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":615
+/* "View.MemoryView":611
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -16118,43 +16073,43 @@
 static PyObject *__pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_14__str__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "View.MemoryView":616
+  /* "View.MemoryView":612
  * 
  *     def __str__(self):
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":615
+  /* "View.MemoryView":611
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -16166,15 +16121,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":619
+/* "View.MemoryView":615
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -16192,62 +16147,60 @@
 }
 
 static PyObject *__pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_16is_c_contig(struct __pyx_memoryview_obj *__pyx_v_self) {
   __Pyx_memviewslice *__pyx_v_mslice;
   __Pyx_memviewslice __pyx_v_tmp;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_memviewslice *__pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("is_c_contig", 0);
 
-  /* "View.MemoryView":622
+  /* "View.MemoryView":618
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  */
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 622, __pyx_L1_error)
-  __pyx_v_mslice = __pyx_t_1;
+  __pyx_v_mslice = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp));
 
-  /* "View.MemoryView":623
+  /* "View.MemoryView":619
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def is_f_contig(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 623, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 619, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":619
+  /* "View.MemoryView":615
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("View.MemoryView.memoryview.is_c_contig", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":625
+/* "View.MemoryView":621
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -16265,62 +16218,60 @@
 }
 
 static PyObject *__pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_18is_f_contig(struct __pyx_memoryview_obj *__pyx_v_self) {
   __Pyx_memviewslice *__pyx_v_mslice;
   __Pyx_memviewslice __pyx_v_tmp;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_memviewslice *__pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("is_f_contig", 0);
 
-  /* "View.MemoryView":628
+  /* "View.MemoryView":624
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  */
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 628, __pyx_L1_error)
-  __pyx_v_mslice = __pyx_t_1;
+  __pyx_v_mslice = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp));
 
-  /* "View.MemoryView":629
+  /* "View.MemoryView":625
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def copy(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 629, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 625, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":625
+  /* "View.MemoryView":621
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("View.MemoryView.memoryview.is_f_contig", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":631
+/* "View.MemoryView":627
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -16342,57 +16293,57 @@
   int __pyx_v_flags;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("copy", 0);
 
-  /* "View.MemoryView":633
+  /* "View.MemoryView":629
  *     def copy(self):
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &mslice)
  */
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_F_CONTIGUOUS));
 
-  /* "View.MemoryView":635
+  /* "View.MemoryView":631
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  * 
  *         slice_copy(self, &mslice)             # <<<<<<<<<<<<<<
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,
  *                                    self.view.itemsize,
  */
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_mslice));
 
-  /* "View.MemoryView":636
+  /* "View.MemoryView":632
  * 
  *         slice_copy(self, &mslice)
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                    self.view.itemsize,
  *                                    flags|PyBUF_C_CONTIGUOUS,
  */
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 636, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 632, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":641
+  /* "View.MemoryView":637
  *                                    self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &mslice)             # <<<<<<<<<<<<<<
  * 
  *     def copy_fortran(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 641, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 637, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":631
+  /* "View.MemoryView":627
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -16403,15 +16354,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":643
+/* "View.MemoryView":639
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -16434,57 +16385,57 @@
   int __pyx_v_flags;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("copy_fortran", 0);
 
-  /* "View.MemoryView":645
+  /* "View.MemoryView":641
  *     def copy_fortran(self):
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &src)
  */
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_C_CONTIGUOUS));
 
-  /* "View.MemoryView":647
+  /* "View.MemoryView":643
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  * 
  *         slice_copy(self, &src)             # <<<<<<<<<<<<<<
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,
  *                                 self.view.itemsize,
  */
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_src));
 
-  /* "View.MemoryView":648
+  /* "View.MemoryView":644
  * 
  *         slice_copy(self, &src)
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                 self.view.itemsize,
  *                                 flags|PyBUF_F_CONTIGUOUS,
  */
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 648, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 644, __pyx_L1_error)
   __pyx_v_dst = __pyx_t_1;
 
-  /* "View.MemoryView":653
+  /* "View.MemoryView":649
  *                                 self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &dst)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 653, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 649, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":643
+  /* "View.MemoryView":639
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -16602,15 +16553,15 @@
   __Pyx_AddTraceback("View.MemoryView.memoryview.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":657
+/* "View.MemoryView":653
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -16619,64 +16570,64 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("memoryview_cwrapper", 0);
 
-  /* "View.MemoryView":658
+  /* "View.MemoryView":654
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)             # <<<<<<<<<<<<<<
  *     result.typeinfo = typeinfo
  *     return result
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_o);
   __Pyx_GIVEREF(__pyx_v_o);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_o);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryview_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":659
+  /* "View.MemoryView":655
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
   __pyx_v_result->typeinfo = __pyx_v_typeinfo;
 
-  /* "View.MemoryView":660
+  /* "View.MemoryView":656
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_check')
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":657
+  /* "View.MemoryView":653
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -16690,54 +16641,54 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":663
+/* "View.MemoryView":659
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *__pyx_v_o) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("memoryview_check", 0);
 
-  /* "View.MemoryView":664
+  /* "View.MemoryView":660
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):
  *     return isinstance(o, memoryview)             # <<<<<<<<<<<<<<
  * 
  * cdef tuple _unellipsify(object index, int ndim):
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_o, __pyx_memoryview_type); 
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":663
+  /* "View.MemoryView":659
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":666
+/* "View.MemoryView":662
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -16760,243 +16711,243 @@
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   __Pyx_RefNannySetupContext("_unellipsify", 0);
 
-  /* "View.MemoryView":671
+  /* "View.MemoryView":667
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
   __pyx_t_1 = PyTuple_Check(__pyx_v_index); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":672
+    /* "View.MemoryView":668
  *     """
  *     if not isinstance(index, tuple):
  *         tup = (index,)             # <<<<<<<<<<<<<<
  *     else:
  *         tup = index
  */
-    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 672, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 668, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_index);
     __Pyx_GIVEREF(__pyx_v_index);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_index);
     __pyx_v_tup = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":671
+    /* "View.MemoryView":667
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":674
+  /* "View.MemoryView":670
  *         tup = (index,)
  *     else:
  *         tup = index             # <<<<<<<<<<<<<<
  * 
  *     result = []
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_v_index);
     __pyx_v_tup = __pyx_v_index;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":676
+  /* "View.MemoryView":672
  *         tup = index
  * 
  *     result = []             # <<<<<<<<<<<<<<
  *     have_slices = False
  *     seen_ellipsis = False
  */
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 676, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_result = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":677
+  /* "View.MemoryView":673
  * 
  *     result = []
  *     have_slices = False             # <<<<<<<<<<<<<<
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  */
   __pyx_v_have_slices = 0;
 
-  /* "View.MemoryView":678
+  /* "View.MemoryView":674
  *     result = []
  *     have_slices = False
  *     seen_ellipsis = False             # <<<<<<<<<<<<<<
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  */
   __pyx_v_seen_ellipsis = 0;
 
-  /* "View.MemoryView":679
+  /* "View.MemoryView":675
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_t_3 = __pyx_int_0;
   if (likely(PyList_CheckExact(__pyx_v_tup)) || PyTuple_CheckExact(__pyx_v_tup)) {
     __pyx_t_4 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 679, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 675, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 679, __pyx_L1_error)
+    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 675, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_4))) {
         if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 675, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 675, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       } else {
         if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 675, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 675, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       }
     } else {
       __pyx_t_7 = __pyx_t_6(__pyx_t_4);
       if (unlikely(!__pyx_t_7)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 679, __pyx_L1_error)
+          else __PYX_ERR(1, 675, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_7);
     }
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_3);
-    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 679, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 675, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "View.MemoryView":680
+    /* "View.MemoryView":676
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
     __pyx_t_2 = (__pyx_v_item == __pyx_builtin_Ellipsis);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":681
+      /* "View.MemoryView":677
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
       __pyx_t_1 = ((!(__pyx_v_seen_ellipsis != 0)) != 0);
       if (__pyx_t_1) {
 
-        /* "View.MemoryView":682
+        /* "View.MemoryView":678
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 682, __pyx_L1_error)
-        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 682, __pyx_L1_error)
+        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 678, __pyx_L1_error)
+        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 678, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
             __Pyx_INCREF(__pyx_slice__5);
             __Pyx_GIVEREF(__pyx_slice__5);
             PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__5);
           }
         }
-        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 682, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 678, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-        /* "View.MemoryView":683
+        /* "View.MemoryView":679
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True             # <<<<<<<<<<<<<<
  *             else:
  *                 result.append(slice(None))
  */
         __pyx_v_seen_ellipsis = 1;
 
-        /* "View.MemoryView":681
+        /* "View.MemoryView":677
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":685
+      /* "View.MemoryView":681
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__5); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 685, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__5); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 681, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":686
+      /* "View.MemoryView":682
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  */
       __pyx_v_have_slices = 1;
 
-      /* "View.MemoryView":680
+      /* "View.MemoryView":676
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":688
+    /* "View.MemoryView":684
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
     /*else*/ {
@@ -17008,40 +16959,40 @@
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = ((!(PyIndex_Check(__pyx_v_item) != 0)) != 0);
       __pyx_t_1 = __pyx_t_10;
       __pyx_L9_bool_binop_done:;
       if (unlikely(__pyx_t_1)) {
 
-        /* "View.MemoryView":689
+        /* "View.MemoryView":685
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  *                 raise TypeError("Cannot index with type '%s'" % type(item))             # <<<<<<<<<<<<<<
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  */
-        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 689, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 685, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 689, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 685, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_Raise(__pyx_t_11, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __PYX_ERR(1, 689, __pyx_L1_error)
+        __PYX_ERR(1, 685, __pyx_L1_error)
 
-        /* "View.MemoryView":688
+        /* "View.MemoryView":684
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
       }
 
-      /* "View.MemoryView":691
+      /* "View.MemoryView":687
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  *             have_slices = have_slices or isinstance(item, slice)             # <<<<<<<<<<<<<<
  *             result.append(item)
  * 
  */
       __pyx_t_10 = (__pyx_v_have_slices != 0);
@@ -17052,120 +17003,120 @@
       }
       __pyx_t_10 = PySlice_Check(__pyx_v_item); 
       __pyx_t_2 = (__pyx_t_10 != 0);
       __pyx_t_1 = __pyx_t_2;
       __pyx_L11_bool_binop_done:;
       __pyx_v_have_slices = __pyx_t_1;
 
-      /* "View.MemoryView":692
+      /* "View.MemoryView":688
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  *             result.append(item)             # <<<<<<<<<<<<<<
  * 
  *     nslices = ndim - len(result)
  */
-      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 692, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 688, __pyx_L1_error)
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":679
+    /* "View.MemoryView":675
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":694
+  /* "View.MemoryView":690
  *             result.append(item)
  * 
  *     nslices = ndim - len(result)             # <<<<<<<<<<<<<<
  *     if nslices:
  *         result.extend([slice(None)] * nslices)
  */
-  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 694, __pyx_L1_error)
+  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 690, __pyx_L1_error)
   __pyx_v_nslices = (__pyx_v_ndim - __pyx_t_5);
 
-  /* "View.MemoryView":695
+  /* "View.MemoryView":691
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
   __pyx_t_1 = (__pyx_v_nslices != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":696
+    /* "View.MemoryView":692
  *     nslices = ndim - len(result)
  *     if nslices:
  *         result.extend([slice(None)] * nslices)             # <<<<<<<<<<<<<<
  * 
  *     return have_slices or nslices, tuple(result)
  */
-    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 696, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 692, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
         __Pyx_INCREF(__pyx_slice__5);
         __Pyx_GIVEREF(__pyx_slice__5);
         PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__5);
       }
     }
-    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 696, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 692, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "View.MemoryView":695
+    /* "View.MemoryView":691
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
   }
 
-  /* "View.MemoryView":698
+  /* "View.MemoryView":694
  *         result.extend([slice(None)] * nslices)
  * 
  *     return have_slices or nslices, tuple(result)             # <<<<<<<<<<<<<<
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  */
   __Pyx_XDECREF(__pyx_r);
   if (!__pyx_v_have_slices) {
   } else {
-    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 698, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 694, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L14_bool_binop_done;
   }
-  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 698, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_L14_bool_binop_done:;
-  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 698, __pyx_L1_error)
+  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 698, __pyx_L1_error)
+  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_r = ((PyObject*)__pyx_t_11);
   __pyx_t_11 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":666
+  /* "View.MemoryView":662
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -17183,15 +17134,15 @@
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":700
+/* "View.MemoryView":696
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -17202,60 +17153,60 @@
   Py_ssize_t *__pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   __Pyx_RefNannySetupContext("assert_direct_dimensions", 0);
 
-  /* "View.MemoryView":701
+  /* "View.MemoryView":697
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")
  */
   __pyx_t_2 = (__pyx_v_suboffsets + __pyx_v_ndim);
   for (__pyx_t_3 = __pyx_v_suboffsets; __pyx_t_3 < __pyx_t_2; __pyx_t_3++) {
     __pyx_t_1 = __pyx_t_3;
     __pyx_v_suboffset = (__pyx_t_1[0]);
 
-    /* "View.MemoryView":702
+    /* "View.MemoryView":698
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
     __pyx_t_4 = ((__pyx_v_suboffset >= 0) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":703
+      /* "View.MemoryView":699
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 703, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 699, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(1, 703, __pyx_L1_error)
+      __PYX_ERR(1, 699, __pyx_L1_error)
 
-      /* "View.MemoryView":702
+      /* "View.MemoryView":698
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":700
+  /* "View.MemoryView":696
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -17268,15 +17219,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":710
+/* "View.MemoryView":706
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -17309,529 +17260,529 @@
   PyObject *(*__pyx_t_8)(PyObject *);
   PyObject *__pyx_t_9 = NULL;
   Py_ssize_t __pyx_t_10;
   int __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   __Pyx_RefNannySetupContext("memview_slice", 0);
 
-  /* "View.MemoryView":711
+  /* "View.MemoryView":707
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim             # <<<<<<<<<<<<<<
  *     cdef bint negative_step
  *     cdef __Pyx_memviewslice src, dst
  */
   __pyx_v_new_ndim = 0;
   __pyx_v_suboffset_dim = -1;
 
-  /* "View.MemoryView":718
+  /* "View.MemoryView":714
  * 
  * 
  *     memset(&dst, 0, sizeof(dst))             # <<<<<<<<<<<<<<
  * 
  *     cdef _memoryviewslice memviewsliceobj
  */
   (void)(memset((&__pyx_v_dst), 0, (sizeof(__pyx_v_dst))));
 
-  /* "View.MemoryView":722
+  /* "View.MemoryView":718
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 722, __pyx_L1_error)
+      __PYX_ERR(1, 718, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "View.MemoryView":724
+  /* "View.MemoryView":720
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":725
+    /* "View.MemoryView":721
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview             # <<<<<<<<<<<<<<
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  */
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 725, __pyx_L1_error)
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 721, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_memviewsliceobj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":726
+    /* "View.MemoryView":722
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, &src)
  */
     __pyx_v_p_src = (&__pyx_v_memviewsliceobj->from_slice);
 
-    /* "View.MemoryView":724
+    /* "View.MemoryView":720
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":728
+  /* "View.MemoryView":724
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  *         slice_copy(memview, &src)             # <<<<<<<<<<<<<<
  *         p_src = &src
  * 
  */
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_src));
 
-    /* "View.MemoryView":729
+    /* "View.MemoryView":725
  *     else:
  *         slice_copy(memview, &src)
  *         p_src = &src             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_v_p_src = (&__pyx_v_src);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":735
+  /* "View.MemoryView":731
  * 
  * 
  *     dst.memview = p_src.memview             # <<<<<<<<<<<<<<
  *     dst.data = p_src.data
  * 
  */
   __pyx_t_4 = __pyx_v_p_src->memview;
   __pyx_v_dst.memview = __pyx_t_4;
 
-  /* "View.MemoryView":736
+  /* "View.MemoryView":732
  * 
  *     dst.memview = p_src.memview
  *     dst.data = p_src.data             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_5 = __pyx_v_p_src->data;
   __pyx_v_dst.data = __pyx_t_5;
 
-  /* "View.MemoryView":741
+  /* "View.MemoryView":737
  * 
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst             # <<<<<<<<<<<<<<
  *     cdef int *p_suboffset_dim = &suboffset_dim
  *     cdef Py_ssize_t start, stop, step
  */
   __pyx_v_p_dst = (&__pyx_v_dst);
 
-  /* "View.MemoryView":742
+  /* "View.MemoryView":738
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst
  *     cdef int *p_suboffset_dim = &suboffset_dim             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t start, stop, step
  *     cdef bint have_start, have_stop, have_step
  */
   __pyx_v_p_suboffset_dim = (&__pyx_v_suboffset_dim);
 
-  /* "View.MemoryView":746
+  /* "View.MemoryView":742
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
   __pyx_t_6 = 0;
   if (likely(PyList_CheckExact(__pyx_v_indices)) || PyTuple_CheckExact(__pyx_v_indices)) {
     __pyx_t_3 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 746, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 742, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 746, __pyx_L1_error)
+    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 742, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 742, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 742, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 742, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 742, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       }
     } else {
       __pyx_t_9 = __pyx_t_8(__pyx_t_3);
       if (unlikely(!__pyx_t_9)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 746, __pyx_L1_error)
+          else __PYX_ERR(1, 742, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_9);
     }
     __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_9);
     __pyx_t_9 = 0;
     __pyx_v_dim = __pyx_t_6;
     __pyx_t_6 = (__pyx_t_6 + 1);
 
-    /* "View.MemoryView":747
+    /* "View.MemoryView":743
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
     __pyx_t_2 = (PyIndex_Check(__pyx_v_index) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":751
+      /* "View.MemoryView":747
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  *                 index, 0, 0, # start, stop, step             # <<<<<<<<<<<<<<
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  */
-      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 751, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 747, __pyx_L1_error)
 
-      /* "View.MemoryView":748
+      /* "View.MemoryView":744
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 748, __pyx_L1_error)
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 744, __pyx_L1_error)
 
-      /* "View.MemoryView":747
+      /* "View.MemoryView":743
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":754
+    /* "View.MemoryView":750
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
     __pyx_t_2 = (__pyx_v_index == Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":755
+      /* "View.MemoryView":751
  *                 False)
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1             # <<<<<<<<<<<<<<
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  */
       (__pyx_v_p_dst->shape[__pyx_v_new_ndim]) = 1;
 
-      /* "View.MemoryView":756
+      /* "View.MemoryView":752
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0             # <<<<<<<<<<<<<<
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1
  */
       (__pyx_v_p_dst->strides[__pyx_v_new_ndim]) = 0;
 
-      /* "View.MemoryView":757
+      /* "View.MemoryView":753
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1             # <<<<<<<<<<<<<<
  *             new_ndim += 1
  *         else:
  */
       (__pyx_v_p_dst->suboffsets[__pyx_v_new_ndim]) = -1L;
 
-      /* "View.MemoryView":758
+      /* "View.MemoryView":754
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  *         else:
  *             start = index.start or 0
  */
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
 
-      /* "View.MemoryView":754
+      /* "View.MemoryView":750
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":760
+    /* "View.MemoryView":756
  *             new_ndim += 1
  *         else:
  *             start = index.start or 0             # <<<<<<<<<<<<<<
  *             stop = index.stop or 0
  *             step = index.step or 0
  */
     /*else*/ {
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 760, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 756, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 760, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 756, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 760, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 756, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L7_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L7_bool_binop_done:;
       __pyx_v_start = __pyx_t_10;
 
-      /* "View.MemoryView":761
+      /* "View.MemoryView":757
  *         else:
  *             start = index.start or 0
  *             stop = index.stop or 0             # <<<<<<<<<<<<<<
  *             step = index.step or 0
  * 
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 761, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 757, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 761, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 757, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 761, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 757, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L9_bool_binop_done:;
       __pyx_v_stop = __pyx_t_10;
 
-      /* "View.MemoryView":762
+      /* "View.MemoryView":758
  *             start = index.start or 0
  *             stop = index.stop or 0
  *             step = index.step or 0             # <<<<<<<<<<<<<<
  * 
  *             have_start = index.start is not None
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 762, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 758, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 762, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 758, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 762, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 758, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L11_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L11_bool_binop_done:;
       __pyx_v_step = __pyx_t_10;
 
-      /* "View.MemoryView":764
+      /* "View.MemoryView":760
  *             step = index.step or 0
  * 
  *             have_start = index.start is not None             # <<<<<<<<<<<<<<
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 764, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 760, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_start = __pyx_t_1;
 
-      /* "View.MemoryView":765
+      /* "View.MemoryView":761
  * 
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None             # <<<<<<<<<<<<<<
  *             have_step = index.step is not None
  * 
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 765, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 761, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_stop = __pyx_t_1;
 
-      /* "View.MemoryView":766
+      /* "View.MemoryView":762
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None             # <<<<<<<<<<<<<<
  * 
  *             slice_memviewslice(
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 766, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 762, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_step = __pyx_t_1;
 
-      /* "View.MemoryView":768
+      /* "View.MemoryView":764
  *             have_step = index.step is not None
  * 
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 768, __pyx_L1_error)
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 764, __pyx_L1_error)
 
-      /* "View.MemoryView":774
+      /* "View.MemoryView":770
  *                 have_start, have_stop, have_step,
  *                 True)
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":746
+    /* "View.MemoryView":742
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":776
+  /* "View.MemoryView":772
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":777
+    /* "View.MemoryView":773
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":778
+    /* "View.MemoryView":774
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_dtype_func,
  *                                     memview.dtype_is_object)
  */
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 778, __pyx_L1_error) }
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 774, __pyx_L1_error) }
 
-    /* "View.MemoryView":779
+    /* "View.MemoryView":775
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  *     else:
  */
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 779, __pyx_L1_error) }
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 775, __pyx_L1_error) }
 
-    /* "View.MemoryView":777
+    /* "View.MemoryView":773
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 777, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 773, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 777, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 773, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":776
+    /* "View.MemoryView":772
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
   }
 
-  /* "View.MemoryView":782
+  /* "View.MemoryView":778
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":783
+    /* "View.MemoryView":779
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,
  *                                     memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 782, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "View.MemoryView":782
+    /* "View.MemoryView":778
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 782, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 778, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":710
+  /* "View.MemoryView":706
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -17845,15 +17796,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_memviewsliceobj);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":807
+/* "View.MemoryView":803
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -17861,95 +17812,95 @@
   Py_ssize_t __pyx_v_new_shape;
   int __pyx_v_negative_step;
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "View.MemoryView":827
+  /* "View.MemoryView":823
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
   __pyx_t_1 = ((!(__pyx_v_is_slice != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":829
+    /* "View.MemoryView":825
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
     __pyx_t_1 = ((__pyx_v_start < 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":830
+      /* "View.MemoryView":826
  * 
  *         if start < 0:
  *             start += shape             # <<<<<<<<<<<<<<
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  */
       __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-      /* "View.MemoryView":829
+      /* "View.MemoryView":825
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
     }
 
-    /* "View.MemoryView":831
+    /* "View.MemoryView":827
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
     __pyx_t_1 = (0 <= __pyx_v_start);
     if (__pyx_t_1) {
       __pyx_t_1 = (__pyx_v_start < __pyx_v_shape);
     }
     __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":832
+      /* "View.MemoryView":828
  *             start += shape
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)             # <<<<<<<<<<<<<<
  *     else:
  * 
  */
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 832, __pyx_L1_error)
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 828, __pyx_L1_error)
 
-      /* "View.MemoryView":831
+      /* "View.MemoryView":827
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
     }
 
-    /* "View.MemoryView":827
+    /* "View.MemoryView":823
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":835
+  /* "View.MemoryView":831
  *     else:
  * 
  *         negative_step = have_step != 0 and step < 0             # <<<<<<<<<<<<<<
  * 
  *         if have_step and step == 0:
  */
   /*else*/ {
@@ -17960,15 +17911,15 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step < 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L6_bool_binop_done:;
     __pyx_v_negative_step = __pyx_t_2;
 
-    /* "View.MemoryView":837
+    /* "View.MemoryView":833
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
     __pyx_t_1 = (__pyx_v_have_step != 0);
@@ -17978,639 +17929,639 @@
       goto __pyx_L9_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step == 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L9_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":838
+      /* "View.MemoryView":834
  * 
  *         if have_step and step == 0:
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 838, __pyx_L1_error)
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 834, __pyx_L1_error)
 
-      /* "View.MemoryView":837
+      /* "View.MemoryView":833
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
     }
 
-    /* "View.MemoryView":841
+    /* "View.MemoryView":837
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
     __pyx_t_2 = (__pyx_v_have_start != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":842
+      /* "View.MemoryView":838
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
       __pyx_t_2 = ((__pyx_v_start < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":843
+        /* "View.MemoryView":839
  *         if have_start:
  *             if start < 0:
  *                 start += shape             # <<<<<<<<<<<<<<
  *                 if start < 0:
  *                     start = 0
  */
         __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-        /* "View.MemoryView":844
+        /* "View.MemoryView":840
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
         __pyx_t_2 = ((__pyx_v_start < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":845
+          /* "View.MemoryView":841
  *                 start += shape
  *                 if start < 0:
  *                     start = 0             # <<<<<<<<<<<<<<
  *             elif start >= shape:
  *                 if negative_step:
  */
           __pyx_v_start = 0;
 
-          /* "View.MemoryView":844
+          /* "View.MemoryView":840
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
         }
 
-        /* "View.MemoryView":842
+        /* "View.MemoryView":838
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
         goto __pyx_L12;
       }
 
-      /* "View.MemoryView":846
+      /* "View.MemoryView":842
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
       __pyx_t_2 = ((__pyx_v_start >= __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":847
+        /* "View.MemoryView":843
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
         __pyx_t_2 = (__pyx_v_negative_step != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":848
+          /* "View.MemoryView":844
  *             elif start >= shape:
  *                 if negative_step:
  *                     start = shape - 1             # <<<<<<<<<<<<<<
  *                 else:
  *                     start = shape
  */
           __pyx_v_start = (__pyx_v_shape - 1);
 
-          /* "View.MemoryView":847
+          /* "View.MemoryView":843
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
           goto __pyx_L14;
         }
 
-        /* "View.MemoryView":850
+        /* "View.MemoryView":846
  *                     start = shape - 1
  *                 else:
  *                     start = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
         /*else*/ {
           __pyx_v_start = __pyx_v_shape;
         }
         __pyx_L14:;
 
-        /* "View.MemoryView":846
+        /* "View.MemoryView":842
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
       }
       __pyx_L12:;
 
-      /* "View.MemoryView":841
+      /* "View.MemoryView":837
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
       goto __pyx_L11;
     }
 
-    /* "View.MemoryView":852
+    /* "View.MemoryView":848
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":853
+        /* "View.MemoryView":849
  *         else:
  *             if negative_step:
  *                 start = shape - 1             # <<<<<<<<<<<<<<
  *             else:
  *                 start = 0
  */
         __pyx_v_start = (__pyx_v_shape - 1);
 
-        /* "View.MemoryView":852
+        /* "View.MemoryView":848
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
         goto __pyx_L15;
       }
 
-      /* "View.MemoryView":855
+      /* "View.MemoryView":851
  *                 start = shape - 1
  *             else:
  *                 start = 0             # <<<<<<<<<<<<<<
  * 
  *         if have_stop:
  */
       /*else*/ {
         __pyx_v_start = 0;
       }
       __pyx_L15:;
     }
     __pyx_L11:;
 
-    /* "View.MemoryView":857
+    /* "View.MemoryView":853
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
     __pyx_t_2 = (__pyx_v_have_stop != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":858
+      /* "View.MemoryView":854
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
       __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":859
+        /* "View.MemoryView":855
  *         if have_stop:
  *             if stop < 0:
  *                 stop += shape             # <<<<<<<<<<<<<<
  *                 if stop < 0:
  *                     stop = 0
  */
         __pyx_v_stop = (__pyx_v_stop + __pyx_v_shape);
 
-        /* "View.MemoryView":860
+        /* "View.MemoryView":856
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
         __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":861
+          /* "View.MemoryView":857
  *                 stop += shape
  *                 if stop < 0:
  *                     stop = 0             # <<<<<<<<<<<<<<
  *             elif stop > shape:
  *                 stop = shape
  */
           __pyx_v_stop = 0;
 
-          /* "View.MemoryView":860
+          /* "View.MemoryView":856
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
         }
 
-        /* "View.MemoryView":858
+        /* "View.MemoryView":854
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
         goto __pyx_L17;
       }
 
-      /* "View.MemoryView":862
+      /* "View.MemoryView":858
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
       __pyx_t_2 = ((__pyx_v_stop > __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":863
+        /* "View.MemoryView":859
  *                     stop = 0
  *             elif stop > shape:
  *                 stop = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
         __pyx_v_stop = __pyx_v_shape;
 
-        /* "View.MemoryView":862
+        /* "View.MemoryView":858
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
       }
       __pyx_L17:;
 
-      /* "View.MemoryView":857
+      /* "View.MemoryView":853
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
       goto __pyx_L16;
     }
 
-    /* "View.MemoryView":865
+    /* "View.MemoryView":861
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":866
+        /* "View.MemoryView":862
  *         else:
  *             if negative_step:
  *                 stop = -1             # <<<<<<<<<<<<<<
  *             else:
  *                 stop = shape
  */
         __pyx_v_stop = -1L;
 
-        /* "View.MemoryView":865
+        /* "View.MemoryView":861
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
         goto __pyx_L19;
       }
 
-      /* "View.MemoryView":868
+      /* "View.MemoryView":864
  *                 stop = -1
  *             else:
  *                 stop = shape             # <<<<<<<<<<<<<<
  * 
  *         if not have_step:
  */
       /*else*/ {
         __pyx_v_stop = __pyx_v_shape;
       }
       __pyx_L19:;
     }
     __pyx_L16:;
 
-    /* "View.MemoryView":870
+    /* "View.MemoryView":866
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
     __pyx_t_2 = ((!(__pyx_v_have_step != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":871
+      /* "View.MemoryView":867
  * 
  *         if not have_step:
  *             step = 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_step = 1;
 
-      /* "View.MemoryView":870
+      /* "View.MemoryView":866
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
     }
 
-    /* "View.MemoryView":875
+    /* "View.MemoryView":871
  * 
  *         with cython.cdivision(True):
  *             new_shape = (stop - start) // step             # <<<<<<<<<<<<<<
  * 
  *             if (stop - start) - step * new_shape:
  */
     __pyx_v_new_shape = ((__pyx_v_stop - __pyx_v_start) / __pyx_v_step);
 
-    /* "View.MemoryView":877
+    /* "View.MemoryView":873
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     __pyx_t_2 = (((__pyx_v_stop - __pyx_v_start) - (__pyx_v_step * __pyx_v_new_shape)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":878
+      /* "View.MemoryView":874
  * 
  *             if (stop - start) - step * new_shape:
  *                 new_shape += 1             # <<<<<<<<<<<<<<
  * 
  *         if new_shape < 0:
  */
       __pyx_v_new_shape = (__pyx_v_new_shape + 1);
 
-      /* "View.MemoryView":877
+      /* "View.MemoryView":873
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     }
 
-    /* "View.MemoryView":880
+    /* "View.MemoryView":876
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
     __pyx_t_2 = ((__pyx_v_new_shape < 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":881
+      /* "View.MemoryView":877
  * 
  *         if new_shape < 0:
  *             new_shape = 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_new_shape = 0;
 
-      /* "View.MemoryView":880
+      /* "View.MemoryView":876
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
     }
 
-    /* "View.MemoryView":884
+    /* "View.MemoryView":880
  * 
  * 
  *         dst.strides[new_ndim] = stride * step             # <<<<<<<<<<<<<<
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset
  */
     (__pyx_v_dst->strides[__pyx_v_new_ndim]) = (__pyx_v_stride * __pyx_v_step);
 
-    /* "View.MemoryView":885
+    /* "View.MemoryView":881
  * 
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape             # <<<<<<<<<<<<<<
  *         dst.suboffsets[new_ndim] = suboffset
  * 
  */
     (__pyx_v_dst->shape[__pyx_v_new_ndim]) = __pyx_v_new_shape;
 
-    /* "View.MemoryView":886
+    /* "View.MemoryView":882
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_dst->suboffsets[__pyx_v_new_ndim]) = __pyx_v_suboffset;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":889
+  /* "View.MemoryView":885
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
   __pyx_t_2 = (((__pyx_v_suboffset_dim[0]) < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":890
+    /* "View.MemoryView":886
  * 
  *     if suboffset_dim[0] < 0:
  *         dst.data += start * stride             # <<<<<<<<<<<<<<
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  */
     __pyx_v_dst->data = (__pyx_v_dst->data + (__pyx_v_start * __pyx_v_stride));
 
-    /* "View.MemoryView":889
+    /* "View.MemoryView":885
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
     goto __pyx_L23;
   }
 
-  /* "View.MemoryView":892
+  /* "View.MemoryView":888
  *         dst.data += start * stride
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride             # <<<<<<<<<<<<<<
  * 
  *     if suboffset >= 0:
  */
   /*else*/ {
     __pyx_t_3 = (__pyx_v_suboffset_dim[0]);
     (__pyx_v_dst->suboffsets[__pyx_t_3]) = ((__pyx_v_dst->suboffsets[__pyx_t_3]) + (__pyx_v_start * __pyx_v_stride));
   }
   __pyx_L23:;
 
-  /* "View.MemoryView":894
+  /* "View.MemoryView":890
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":895
+    /* "View.MemoryView":891
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
     __pyx_t_2 = ((!(__pyx_v_is_slice != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":896
+      /* "View.MemoryView":892
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
       __pyx_t_2 = ((__pyx_v_new_ndim == 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":897
+        /* "View.MemoryView":893
  *         if not is_slice:
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  */
         __pyx_v_dst->data = ((((char **)__pyx_v_dst->data)[0]) + __pyx_v_suboffset);
 
-        /* "View.MemoryView":896
+        /* "View.MemoryView":892
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
         goto __pyx_L26;
       }
 
-      /* "View.MemoryView":899
+      /* "View.MemoryView":895
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "             # <<<<<<<<<<<<<<
  *                                      "must be indexed and not sliced", dim)
  *         else:
  */
       /*else*/ {
 
-        /* "View.MemoryView":900
+        /* "View.MemoryView":896
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  *                                      "must be indexed and not sliced", dim)             # <<<<<<<<<<<<<<
  *         else:
  *             suboffset_dim[0] = new_ndim
  */
-        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 899, __pyx_L1_error)
+        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 895, __pyx_L1_error)
       }
       __pyx_L26:;
 
-      /* "View.MemoryView":895
+      /* "View.MemoryView":891
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
       goto __pyx_L25;
     }
 
-    /* "View.MemoryView":902
+    /* "View.MemoryView":898
  *                                      "must be indexed and not sliced", dim)
  *         else:
  *             suboffset_dim[0] = new_ndim             # <<<<<<<<<<<<<<
  * 
  *     return 0
  */
     /*else*/ {
       (__pyx_v_suboffset_dim[0]) = __pyx_v_new_ndim;
     }
     __pyx_L25:;
 
-    /* "View.MemoryView":894
+    /* "View.MemoryView":890
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
   }
 
-  /* "View.MemoryView":904
+  /* "View.MemoryView":900
  *             suboffset_dim[0] = new_ndim
  * 
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":807
+  /* "View.MemoryView":803
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -18626,15 +18577,15 @@
     #endif
   }
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":910
+/* "View.MemoryView":906
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -18648,280 +18599,280 @@
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   __Pyx_RefNannySetupContext("pybuffer_index", 0);
 
-  /* "View.MemoryView":912
+  /* "View.MemoryView":908
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t itemsize = view.itemsize
  *     cdef char *resultp
  */
   __pyx_v_suboffset = -1L;
 
-  /* "View.MemoryView":913
+  /* "View.MemoryView":909
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  *     cdef Py_ssize_t itemsize = view.itemsize             # <<<<<<<<<<<<<<
  *     cdef char *resultp
  * 
  */
   __pyx_t_1 = __pyx_v_view->itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":916
+  /* "View.MemoryView":912
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
   __pyx_t_2 = ((__pyx_v_view->ndim == 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":917
+    /* "View.MemoryView":913
  * 
  *     if view.ndim == 0:
  *         shape = view.len / itemsize             # <<<<<<<<<<<<<<
  *         stride = itemsize
  *     else:
  */
     if (unlikely(__pyx_v_itemsize == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
-      __PYX_ERR(1, 917, __pyx_L1_error)
+      __PYX_ERR(1, 913, __pyx_L1_error)
     }
     else if (sizeof(Py_ssize_t) == sizeof(long) && (!(((Py_ssize_t)-1) > 0)) && unlikely(__pyx_v_itemsize == (Py_ssize_t)-1)  && unlikely(UNARY_NEG_WOULD_OVERFLOW(__pyx_v_view->len))) {
       PyErr_SetString(PyExc_OverflowError, "value too large to perform division");
-      __PYX_ERR(1, 917, __pyx_L1_error)
+      __PYX_ERR(1, 913, __pyx_L1_error)
     }
     __pyx_v_shape = (__pyx_v_view->len / __pyx_v_itemsize);
 
-    /* "View.MemoryView":918
+    /* "View.MemoryView":914
  *     if view.ndim == 0:
  *         shape = view.len / itemsize
  *         stride = itemsize             # <<<<<<<<<<<<<<
  *     else:
  *         shape = view.shape[dim]
  */
     __pyx_v_stride = __pyx_v_itemsize;
 
-    /* "View.MemoryView":916
+    /* "View.MemoryView":912
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":920
+  /* "View.MemoryView":916
  *         stride = itemsize
  *     else:
  *         shape = view.shape[dim]             # <<<<<<<<<<<<<<
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  */
   /*else*/ {
     __pyx_v_shape = (__pyx_v_view->shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":921
+    /* "View.MemoryView":917
  *     else:
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]             # <<<<<<<<<<<<<<
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]
  */
     __pyx_v_stride = (__pyx_v_view->strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":922
+    /* "View.MemoryView":918
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
     __pyx_t_2 = ((__pyx_v_view->suboffsets != NULL) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":923
+      /* "View.MemoryView":919
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]             # <<<<<<<<<<<<<<
  * 
  *     if index < 0:
  */
       __pyx_v_suboffset = (__pyx_v_view->suboffsets[__pyx_v_dim]);
 
-      /* "View.MemoryView":922
+      /* "View.MemoryView":918
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":925
+  /* "View.MemoryView":921
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
   __pyx_t_2 = ((__pyx_v_index < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":926
+    /* "View.MemoryView":922
  * 
  *     if index < 0:
  *         index += view.shape[dim]             # <<<<<<<<<<<<<<
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  */
     __pyx_v_index = (__pyx_v_index + (__pyx_v_view->shape[__pyx_v_dim]));
 
-    /* "View.MemoryView":927
+    /* "View.MemoryView":923
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
     __pyx_t_2 = ((__pyx_v_index < 0) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "View.MemoryView":928
+      /* "View.MemoryView":924
  *         index += view.shape[dim]
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     if index >= shape:
  */
-      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 928, __pyx_L1_error)
+      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 924, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 928, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 924, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 928, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 924, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 928, __pyx_L1_error)
+      __PYX_ERR(1, 924, __pyx_L1_error)
 
-      /* "View.MemoryView":927
+      /* "View.MemoryView":923
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
     }
 
-    /* "View.MemoryView":925
+    /* "View.MemoryView":921
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
   }
 
-  /* "View.MemoryView":930
+  /* "View.MemoryView":926
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
   __pyx_t_2 = ((__pyx_v_index >= __pyx_v_shape) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":931
+    /* "View.MemoryView":927
  * 
  *     if index >= shape:
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     resultp = bufp + index * stride
  */
-    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 931, __pyx_L1_error)
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 931, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 931, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 931, __pyx_L1_error)
+    __PYX_ERR(1, 927, __pyx_L1_error)
 
-    /* "View.MemoryView":930
+    /* "View.MemoryView":926
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
   }
 
-  /* "View.MemoryView":933
+  /* "View.MemoryView":929
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     resultp = bufp + index * stride             # <<<<<<<<<<<<<<
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset
  */
   __pyx_v_resultp = (__pyx_v_bufp + (__pyx_v_index * __pyx_v_stride));
 
-  /* "View.MemoryView":934
+  /* "View.MemoryView":930
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":935
+    /* "View.MemoryView":931
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset             # <<<<<<<<<<<<<<
  * 
  *     return resultp
  */
     __pyx_v_resultp = ((((char **)__pyx_v_resultp)[0]) + __pyx_v_suboffset);
 
-    /* "View.MemoryView":934
+    /* "View.MemoryView":930
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
   }
 
-  /* "View.MemoryView":937
+  /* "View.MemoryView":933
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  *     return resultp             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_resultp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":910
+  /* "View.MemoryView":906
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -18932,15 +18883,15 @@
   __Pyx_AddTraceback("View.MemoryView.pybuffer_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":943
+/* "View.MemoryView":939
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -18957,90 +18908,90 @@
   long __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_t_9;
 
-  /* "View.MemoryView":944
+  /* "View.MemoryView":940
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:
  *     cdef int ndim = memslice.memview.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  */
   __pyx_t_1 = __pyx_v_memslice->memview->view.ndim;
   __pyx_v_ndim = __pyx_t_1;
 
-  /* "View.MemoryView":946
+  /* "View.MemoryView":942
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  *     cdef Py_ssize_t *shape = memslice.shape             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t *strides = memslice.strides
  * 
  */
   __pyx_t_2 = __pyx_v_memslice->shape;
   __pyx_v_shape = __pyx_t_2;
 
-  /* "View.MemoryView":947
+  /* "View.MemoryView":943
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  *     cdef Py_ssize_t *strides = memslice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = __pyx_v_memslice->strides;
   __pyx_v_strides = __pyx_t_2;
 
-  /* "View.MemoryView":951
+  /* "View.MemoryView":947
  * 
  *     cdef int i, j
  *     for i in range(ndim / 2):             # <<<<<<<<<<<<<<
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  */
   __pyx_t_3 = (__pyx_v_ndim / 2);
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_4; __pyx_t_1+=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":952
+    /* "View.MemoryView":948
  *     cdef int i, j
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i             # <<<<<<<<<<<<<<
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]
  */
     __pyx_v_j = ((__pyx_v_ndim - 1) - __pyx_v_i);
 
-    /* "View.MemoryView":953
+    /* "View.MemoryView":949
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]             # <<<<<<<<<<<<<<
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  */
     __pyx_t_5 = (__pyx_v_strides[__pyx_v_j]);
     __pyx_t_6 = (__pyx_v_strides[__pyx_v_i]);
     (__pyx_v_strides[__pyx_v_i]) = __pyx_t_5;
     (__pyx_v_strides[__pyx_v_j]) = __pyx_t_6;
 
-    /* "View.MemoryView":954
+    /* "View.MemoryView":950
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]             # <<<<<<<<<<<<<<
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  */
     __pyx_t_6 = (__pyx_v_shape[__pyx_v_j]);
     __pyx_t_5 = (__pyx_v_shape[__pyx_v_i]);
     (__pyx_v_shape[__pyx_v_i]) = __pyx_t_6;
     (__pyx_v_shape[__pyx_v_j]) = __pyx_t_5;
 
-    /* "View.MemoryView":956
+    /* "View.MemoryView":952
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_i]) >= 0) != 0);
@@ -19050,44 +19001,44 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_j]) >= 0) != 0);
     __pyx_t_7 = __pyx_t_8;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_7) {
 
-      /* "View.MemoryView":957
+      /* "View.MemoryView":953
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")             # <<<<<<<<<<<<<<
  * 
  *     return 1
  */
-      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 957, __pyx_L1_error)
+      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 953, __pyx_L1_error)
 
-      /* "View.MemoryView":956
+      /* "View.MemoryView":952
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":959
+  /* "View.MemoryView":955
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  *     return 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":943
+  /* "View.MemoryView":939
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -19103,15 +19054,15 @@
     #endif
   }
   __pyx_r = 0;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":976
+/* "View.MemoryView":972
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
@@ -19126,100 +19077,100 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "View.MemoryView":977
+  /* "View.MemoryView":973
  * 
  *     def __dealloc__(self):
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
   __PYX_XDEC_MEMVIEW((&__pyx_v_self->from_slice), 1);
 
-  /* "View.MemoryView":976
+  /* "View.MemoryView":972
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":979
+/* "View.MemoryView":975
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
 static PyObject *__pyx_memoryviewslice_convert_item_to_object(struct __pyx_memoryviewslice_obj *__pyx_v_self, char *__pyx_v_itemp) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
-  /* "View.MemoryView":980
+  /* "View.MemoryView":976
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->to_object_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":981
+    /* "View.MemoryView":977
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)             # <<<<<<<<<<<<<<
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 981, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 977, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":980
+    /* "View.MemoryView":976
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
   }
 
-  /* "View.MemoryView":983
+  /* "View.MemoryView":979
  *             return self.to_object_func(itemp)
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 983, __pyx_L1_error)
+    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 979, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":979
+  /* "View.MemoryView":975
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
@@ -19230,15 +19181,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":985
+/* "View.MemoryView":981
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -19246,58 +19197,58 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
-  /* "View.MemoryView":986
+  /* "View.MemoryView":982
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->to_dtype_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":987
+    /* "View.MemoryView":983
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)             # <<<<<<<<<<<<<<
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)
  */
-    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 987, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 983, __pyx_L1_error)
 
-    /* "View.MemoryView":986
+    /* "View.MemoryView":982
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":989
+  /* "View.MemoryView":985
  *             self.to_dtype_func(itemp, value)
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   /*else*/ {
-    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 989, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 985, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":985
+  /* "View.MemoryView":981
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -19310,15 +19261,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":992
+/* "View.MemoryView":988
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -19336,27 +19287,27 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_16_memoryviewslice_4base___get__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":993
+  /* "View.MemoryView":989
  *     @property
  *     def base(self):
  *         return self.from_object             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->from_object);
   __pyx_r = __pyx_v_self->from_object;
   goto __pyx_L0;
 
-  /* "View.MemoryView":992
+  /* "View.MemoryView":988
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -19470,15 +19421,15 @@
   __Pyx_AddTraceback("View.MemoryView._memoryviewslice.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":999
+/* "View.MemoryView":995
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -19495,351 +19446,351 @@
   Py_buffer __pyx_t_5;
   Py_ssize_t *__pyx_t_6;
   Py_ssize_t *__pyx_t_7;
   Py_ssize_t *__pyx_t_8;
   Py_ssize_t __pyx_t_9;
   __Pyx_RefNannySetupContext("memoryview_fromslice", 0);
 
-  /* "View.MemoryView":1007
+  /* "View.MemoryView":1003
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   __pyx_t_1 = ((((PyObject *)__pyx_v_memviewslice.memview) == Py_None) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1008
+    /* "View.MemoryView":1004
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:
  *         return None             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1007
+    /* "View.MemoryView":1003
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   }
 
-  /* "View.MemoryView":1013
+  /* "View.MemoryView":1009
  * 
  * 
  *     result = _memoryviewslice(None, 0, dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     result.from_slice = memviewslice
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1013, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1009, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1013, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1009, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_3, 0, Py_None);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_0);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1013, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1009, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1015
+  /* "View.MemoryView":1011
  *     result = _memoryviewslice(None, 0, dtype_is_object)
  * 
  *     result.from_slice = memviewslice             # <<<<<<<<<<<<<<
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  */
   __pyx_v_result->from_slice = __pyx_v_memviewslice;
 
-  /* "View.MemoryView":1016
+  /* "View.MemoryView":1012
  * 
  *     result.from_slice = memviewslice
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)             # <<<<<<<<<<<<<<
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  */
   __PYX_INC_MEMVIEW((&__pyx_v_memviewslice), 1);
 
-  /* "View.MemoryView":1018
+  /* "View.MemoryView":1014
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base             # <<<<<<<<<<<<<<
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1018, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1014, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_result->from_object);
   __Pyx_DECREF(__pyx_v_result->from_object);
   __pyx_v_result->from_object = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1019
+  /* "View.MemoryView":1015
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  *     result.typeinfo = memviewslice.memview.typeinfo             # <<<<<<<<<<<<<<
  * 
  *     result.view = memviewslice.memview.view
  */
   __pyx_t_4 = __pyx_v_memviewslice.memview->typeinfo;
   __pyx_v_result->__pyx_base.typeinfo = __pyx_t_4;
 
-  /* "View.MemoryView":1021
+  /* "View.MemoryView":1017
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  *     result.view = memviewslice.memview.view             # <<<<<<<<<<<<<<
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  */
   __pyx_t_5 = __pyx_v_memviewslice.memview->view;
   __pyx_v_result->__pyx_base.view = __pyx_t_5;
 
-  /* "View.MemoryView":1022
+  /* "View.MemoryView":1018
  * 
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data             # <<<<<<<<<<<<<<
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  */
   __pyx_v_result->__pyx_base.view.buf = ((void *)__pyx_v_memviewslice.data);
 
-  /* "View.MemoryView":1023
+  /* "View.MemoryView":1019
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim             # <<<<<<<<<<<<<<
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)
  */
   __pyx_v_result->__pyx_base.view.ndim = __pyx_v_ndim;
 
-  /* "View.MemoryView":1024
+  /* "View.MemoryView":1020
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None             # <<<<<<<<<<<<<<
  *     Py_INCREF(Py_None)
  * 
  */
   ((Py_buffer *)(&__pyx_v_result->__pyx_base.view))->obj = Py_None;
 
-  /* "View.MemoryView":1025
+  /* "View.MemoryView":1021
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  */
   Py_INCREF(Py_None);
 
-  /* "View.MemoryView":1027
+  /* "View.MemoryView":1023
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
   __pyx_t_1 = ((((struct __pyx_memoryview_obj *)__pyx_v_memviewslice.memview)->flags & PyBUF_WRITABLE) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1028
+    /* "View.MemoryView":1024
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  *         result.flags = PyBUF_RECORDS             # <<<<<<<<<<<<<<
  *     else:
  *         result.flags = PyBUF_RECORDS_RO
  */
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS;
 
-    /* "View.MemoryView":1027
+    /* "View.MemoryView":1023
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":1030
+  /* "View.MemoryView":1026
  *         result.flags = PyBUF_RECORDS
  *     else:
  *         result.flags = PyBUF_RECORDS_RO             # <<<<<<<<<<<<<<
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  */
   /*else*/ {
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS_RO;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":1032
+  /* "View.MemoryView":1028
  *         result.flags = PyBUF_RECORDS_RO
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape             # <<<<<<<<<<<<<<
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides
  * 
  */
   __pyx_v_result->__pyx_base.view.shape = ((Py_ssize_t *)__pyx_v_result->from_slice.shape);
 
-  /* "View.MemoryView":1033
+  /* "View.MemoryView":1029
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_v_result->__pyx_base.view.strides = ((Py_ssize_t *)__pyx_v_result->from_slice.strides);
 
-  /* "View.MemoryView":1036
+  /* "View.MemoryView":1032
  * 
  * 
  *     result.view.suboffsets = NULL             # <<<<<<<<<<<<<<
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
   __pyx_v_result->__pyx_base.view.suboffsets = NULL;
 
-  /* "View.MemoryView":1037
+  /* "View.MemoryView":1033
  * 
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  */
   __pyx_t_7 = (__pyx_v_result->from_slice.suboffsets + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->from_slice.suboffsets; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
     __pyx_v_suboffset = (__pyx_t_6[0]);
 
-    /* "View.MemoryView":1038
+    /* "View.MemoryView":1034
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
     __pyx_t_1 = ((__pyx_v_suboffset >= 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1039
+      /* "View.MemoryView":1035
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_result->__pyx_base.view.suboffsets = ((Py_ssize_t *)__pyx_v_result->from_slice.suboffsets);
 
-      /* "View.MemoryView":1040
+      /* "View.MemoryView":1036
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break             # <<<<<<<<<<<<<<
  * 
  *     result.view.len = result.view.itemsize
  */
       goto __pyx_L6_break;
 
-      /* "View.MemoryView":1038
+      /* "View.MemoryView":1034
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
     }
   }
   __pyx_L6_break:;
 
-  /* "View.MemoryView":1042
+  /* "View.MemoryView":1038
  *             break
  * 
  *     result.view.len = result.view.itemsize             # <<<<<<<<<<<<<<
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length
  */
   __pyx_t_9 = __pyx_v_result->__pyx_base.view.itemsize;
   __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
 
-  /* "View.MemoryView":1043
+  /* "View.MemoryView":1039
  * 
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:             # <<<<<<<<<<<<<<
  *         result.view.len *= length
  * 
  */
   __pyx_t_7 = (__pyx_v_result->__pyx_base.view.shape + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->__pyx_base.view.shape; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
-    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1043, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1039, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":1044
+    /* "View.MemoryView":1040
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length             # <<<<<<<<<<<<<<
  * 
  *     result.to_object_func = to_object_func
  */
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1044, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1040, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1044, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1040, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 1044, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 1040, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
   }
 
-  /* "View.MemoryView":1046
+  /* "View.MemoryView":1042
  *         result.view.len *= length
  * 
  *     result.to_object_func = to_object_func             # <<<<<<<<<<<<<<
  *     result.to_dtype_func = to_dtype_func
  * 
  */
   __pyx_v_result->to_object_func = __pyx_v_to_object_func;
 
-  /* "View.MemoryView":1047
+  /* "View.MemoryView":1043
  * 
  *     result.to_object_func = to_object_func
  *     result.to_dtype_func = to_dtype_func             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result->to_dtype_func = __pyx_v_to_dtype_func;
 
-  /* "View.MemoryView":1049
+  /* "View.MemoryView":1045
  *     result.to_dtype_func = to_dtype_func
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":999
+  /* "View.MemoryView":995
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -19853,115 +19804,115 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1052
+/* "View.MemoryView":1048
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
- *                                                    __Pyx_memviewslice *mslice) except NULL:
+ *                                                    __Pyx_memviewslice *mslice):
  *     cdef _memoryviewslice obj
  */
 
 static __Pyx_memviewslice *__pyx_memoryview_get_slice_from_memoryview(struct __pyx_memoryview_obj *__pyx_v_memview, __Pyx_memviewslice *__pyx_v_mslice) {
   struct __pyx_memoryviewslice_obj *__pyx_v_obj = 0;
   __Pyx_memviewslice *__pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("get_slice_from_memview", 0);
 
-  /* "View.MemoryView":1055
- *                                                    __Pyx_memviewslice *mslice) except NULL:
+  /* "View.MemoryView":1051
+ *                                                    __Pyx_memviewslice *mslice):
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1056
+    /* "View.MemoryView":1052
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview             # <<<<<<<<<<<<<<
  *         return &obj.from_slice
  *     else:
  */
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 1056, __pyx_L1_error)
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 1052, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_obj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":1057
+    /* "View.MemoryView":1053
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview
  *         return &obj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, mslice)
  */
     __pyx_r = (&__pyx_v_obj->from_slice);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1055
- *                                                    __Pyx_memviewslice *mslice) except NULL:
+    /* "View.MemoryView":1051
+ *                                                    __Pyx_memviewslice *mslice):
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
   }
 
-  /* "View.MemoryView":1059
+  /* "View.MemoryView":1055
  *         return &obj.from_slice
  *     else:
  *         slice_copy(memview, mslice)             # <<<<<<<<<<<<<<
  *         return mslice
  * 
  */
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, __pyx_v_mslice);
 
-    /* "View.MemoryView":1060
+    /* "View.MemoryView":1056
  *     else:
  *         slice_copy(memview, mslice)
  *         return mslice             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_slice_copy')
  */
     __pyx_r = __pyx_v_mslice;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1052
+  /* "View.MemoryView":1048
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
- *                                                    __Pyx_memviewslice *mslice) except NULL:
+ *                                                    __Pyx_memviewslice *mslice):
  *     cdef _memoryviewslice obj
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("View.MemoryView.get_slice_from_memview", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __Pyx_WriteUnraisable("View.MemoryView.get_slice_from_memview", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_obj);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1063
+/* "View.MemoryView":1059
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
@@ -19974,158 +19925,158 @@
   Py_ssize_t *__pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   __Pyx_RefNannySetupContext("slice_copy", 0);
 
-  /* "View.MemoryView":1067
+  /* "View.MemoryView":1063
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  * 
  *     shape = memview.view.shape             # <<<<<<<<<<<<<<
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets
  */
   __pyx_t_1 = __pyx_v_memview->view.shape;
   __pyx_v_shape = __pyx_t_1;
 
-  /* "View.MemoryView":1068
+  /* "View.MemoryView":1064
  * 
  *     shape = memview.view.shape
  *     strides = memview.view.strides             # <<<<<<<<<<<<<<
  *     suboffsets = memview.view.suboffsets
  * 
  */
   __pyx_t_1 = __pyx_v_memview->view.strides;
   __pyx_v_strides = __pyx_t_1;
 
-  /* "View.MemoryView":1069
+  /* "View.MemoryView":1065
  *     shape = memview.view.shape
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets             # <<<<<<<<<<<<<<
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  */
   __pyx_t_1 = __pyx_v_memview->view.suboffsets;
   __pyx_v_suboffsets = __pyx_t_1;
 
-  /* "View.MemoryView":1071
+  /* "View.MemoryView":1067
  *     suboffsets = memview.view.suboffsets
  * 
  *     dst.memview = <__pyx_memoryview *> memview             # <<<<<<<<<<<<<<
  *     dst.data = <char *> memview.view.buf
  * 
  */
   __pyx_v_dst->memview = ((struct __pyx_memoryview_obj *)__pyx_v_memview);
 
-  /* "View.MemoryView":1072
+  /* "View.MemoryView":1068
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  *     dst.data = <char *> memview.view.buf             # <<<<<<<<<<<<<<
  * 
  *     for dim in range(memview.view.ndim):
  */
   __pyx_v_dst->data = ((char *)__pyx_v_memview->view.buf);
 
-  /* "View.MemoryView":1074
+  /* "View.MemoryView":1070
  *     dst.data = <char *> memview.view.buf
  * 
  *     for dim in range(memview.view.ndim):             # <<<<<<<<<<<<<<
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  */
   __pyx_t_2 = __pyx_v_memview->view.ndim;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_dim = __pyx_t_4;
 
-    /* "View.MemoryView":1075
+    /* "View.MemoryView":1071
  * 
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]             # <<<<<<<<<<<<<<
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  */
     (__pyx_v_dst->shape[__pyx_v_dim]) = (__pyx_v_shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":1076
+    /* "View.MemoryView":1072
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]             # <<<<<<<<<<<<<<
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  * 
  */
     (__pyx_v_dst->strides[__pyx_v_dim]) = (__pyx_v_strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":1077
+    /* "View.MemoryView":1073
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object')
  */
     if ((__pyx_v_suboffsets != 0)) {
       __pyx_t_5 = (__pyx_v_suboffsets[__pyx_v_dim]);
     } else {
       __pyx_t_5 = -1L;
     }
     (__pyx_v_dst->suboffsets[__pyx_v_dim]) = __pyx_t_5;
   }
 
-  /* "View.MemoryView":1063
+  /* "View.MemoryView":1059
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1080
+/* "View.MemoryView":1076
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
 static PyObject *__pyx_memoryview_copy_object(struct __pyx_memoryview_obj *__pyx_v_memview) {
   __Pyx_memviewslice __pyx_v_memviewslice;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("memoryview_copy", 0);
 
-  /* "View.MemoryView":1083
+  /* "View.MemoryView":1079
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)             # <<<<<<<<<<<<<<
  *     return memoryview_copy_from_slice(memview, &memviewslice)
  * 
  */
   __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_memviewslice));
 
-  /* "View.MemoryView":1084
+  /* "View.MemoryView":1080
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)
  *     return memoryview_copy_from_slice(memview, &memviewslice)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1084, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1080, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1080
+  /* "View.MemoryView":1076
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
@@ -20136,15 +20087,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1087
+/* "View.MemoryView":1083
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -20156,99 +20107,99 @@
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *(*__pyx_t_3)(char *);
   int (*__pyx_t_4)(char *, PyObject *);
   PyObject *__pyx_t_5 = NULL;
   __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 0);
 
-  /* "View.MemoryView":1094
+  /* "View.MemoryView":1090
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1095
+    /* "View.MemoryView":1091
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func             # <<<<<<<<<<<<<<
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  */
     __pyx_t_3 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_object_func;
     __pyx_v_to_object_func = __pyx_t_3;
 
-    /* "View.MemoryView":1096
+    /* "View.MemoryView":1092
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func             # <<<<<<<<<<<<<<
  *     else:
  *         to_object_func = NULL
  */
     __pyx_t_4 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_dtype_func;
     __pyx_v_to_dtype_func = __pyx_t_4;
 
-    /* "View.MemoryView":1094
+    /* "View.MemoryView":1090
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1098
+  /* "View.MemoryView":1094
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  *         to_object_func = NULL             # <<<<<<<<<<<<<<
  *         to_dtype_func = NULL
  * 
  */
   /*else*/ {
     __pyx_v_to_object_func = NULL;
 
-    /* "View.MemoryView":1099
+    /* "View.MemoryView":1095
  *     else:
  *         to_object_func = NULL
  *         to_dtype_func = NULL             # <<<<<<<<<<<<<<
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  */
     __pyx_v_to_dtype_func = NULL;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1101
+  /* "View.MemoryView":1097
  *         to_dtype_func = NULL
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,             # <<<<<<<<<<<<<<
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "View.MemoryView":1103
+  /* "View.MemoryView":1099
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1101, __pyx_L1_error)
+  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1097, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1087
+  /* "View.MemoryView":1083
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -20259,81 +20210,81 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1109
+/* "View.MemoryView":1105
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
 static Py_ssize_t abs_py_ssize_t(Py_ssize_t __pyx_v_arg) {
   Py_ssize_t __pyx_r;
   int __pyx_t_1;
 
-  /* "View.MemoryView":1110
+  /* "View.MemoryView":1106
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_arg < 0) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1111
+    /* "View.MemoryView":1107
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:
  *         return -arg             # <<<<<<<<<<<<<<
  *     else:
  *         return arg
  */
     __pyx_r = (-__pyx_v_arg);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1110
+    /* "View.MemoryView":1106
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
   }
 
-  /* "View.MemoryView":1113
+  /* "View.MemoryView":1109
  *         return -arg
  *     else:
  *         return arg             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_get_best_slice_order')
  */
   /*else*/ {
     __pyx_r = __pyx_v_arg;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1109
+  /* "View.MemoryView":1105
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1116
+/* "View.MemoryView":1112
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
@@ -20343,187 +20294,187 @@
   Py_ssize_t __pyx_v_f_stride;
   char __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1121
+  /* "View.MemoryView":1117
  *     """
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t f_stride = 0
  * 
  */
   __pyx_v_c_stride = 0;
 
-  /* "View.MemoryView":1122
+  /* "View.MemoryView":1118
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0
  *     cdef Py_ssize_t f_stride = 0             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
   __pyx_v_f_stride = 0;
 
-  /* "View.MemoryView":1124
+  /* "View.MemoryView":1120
  *     cdef Py_ssize_t f_stride = 0
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  */
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1125
+    /* "View.MemoryView":1121
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1126
+      /* "View.MemoryView":1122
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_c_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1127
+      /* "View.MemoryView":1123
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
       goto __pyx_L4_break;
 
-      /* "View.MemoryView":1125
+      /* "View.MemoryView":1121
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L4_break:;
 
-  /* "View.MemoryView":1129
+  /* "View.MemoryView":1125
  *             break
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  */
   __pyx_t_1 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_1;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1130
+    /* "View.MemoryView":1126
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1131
+      /* "View.MemoryView":1127
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_f_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1132
+      /* "View.MemoryView":1128
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  */
       goto __pyx_L7_break;
 
-      /* "View.MemoryView":1130
+      /* "View.MemoryView":1126
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L7_break:;
 
-  /* "View.MemoryView":1134
+  /* "View.MemoryView":1130
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
   __pyx_t_2 = ((abs_py_ssize_t(__pyx_v_c_stride) <= abs_py_ssize_t(__pyx_v_f_stride)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1135
+    /* "View.MemoryView":1131
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  *         return 'C'             # <<<<<<<<<<<<<<
  *     else:
  *         return 'F'
  */
     __pyx_r = 'C';
     goto __pyx_L0;
 
-    /* "View.MemoryView":1134
+    /* "View.MemoryView":1130
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
   }
 
-  /* "View.MemoryView":1137
+  /* "View.MemoryView":1133
  *         return 'C'
  *     else:
  *         return 'F'             # <<<<<<<<<<<<<<
  * 
  * @cython.cdivision(True)
  */
   /*else*/ {
     __pyx_r = 'F';
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1116
+  /* "View.MemoryView":1112
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1140
+/* "View.MemoryView":1136
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
@@ -20536,61 +20487,61 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
 
-  /* "View.MemoryView":1147
+  /* "View.MemoryView":1143
  * 
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  */
   __pyx_v_src_extent = (__pyx_v_src_shape[0]);
 
-  /* "View.MemoryView":1148
+  /* "View.MemoryView":1144
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  */
   __pyx_v_dst_extent = (__pyx_v_dst_shape[0]);
 
-  /* "View.MemoryView":1149
+  /* "View.MemoryView":1145
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  */
   __pyx_v_src_stride = (__pyx_v_src_strides[0]);
 
-  /* "View.MemoryView":1150
+  /* "View.MemoryView":1146
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
   __pyx_v_dst_stride = (__pyx_v_dst_strides[0]);
 
-  /* "View.MemoryView":1152
+  /* "View.MemoryView":1148
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1153
+    /* "View.MemoryView":1149
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     __pyx_t_2 = ((__pyx_v_src_stride > 0) != 0);
@@ -20602,267 +20553,267 @@
     __pyx_t_2 = ((__pyx_v_dst_stride > 0) != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L5_bool_binop_done;
     }
 
-    /* "View.MemoryView":1154
+    /* "View.MemoryView":1150
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):             # <<<<<<<<<<<<<<
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  */
     __pyx_t_2 = (((size_t)__pyx_v_src_stride) == __pyx_v_itemsize);
     if (__pyx_t_2) {
       __pyx_t_2 = (__pyx_v_itemsize == ((size_t)__pyx_v_dst_stride));
     }
     __pyx_t_3 = (__pyx_t_2 != 0);
     __pyx_t_1 = __pyx_t_3;
     __pyx_L5_bool_binop_done:;
 
-    /* "View.MemoryView":1153
+    /* "View.MemoryView":1149
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1155
+      /* "View.MemoryView":1151
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)             # <<<<<<<<<<<<<<
  *        else:
  *            for i in range(dst_extent):
  */
       (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, (__pyx_v_itemsize * __pyx_v_dst_extent)));
 
-      /* "View.MemoryView":1153
+      /* "View.MemoryView":1149
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
       goto __pyx_L4;
     }
 
-    /* "View.MemoryView":1157
+    /* "View.MemoryView":1153
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  *            for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  */
     /*else*/ {
       __pyx_t_4 = __pyx_v_dst_extent;
       __pyx_t_5 = __pyx_t_4;
       for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
         __pyx_v_i = __pyx_t_6;
 
-        /* "View.MemoryView":1158
+        /* "View.MemoryView":1154
  *        else:
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)             # <<<<<<<<<<<<<<
  *                src_data += src_stride
  *                dst_data += dst_stride
  */
         (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, __pyx_v_itemsize));
 
-        /* "View.MemoryView":1159
+        /* "View.MemoryView":1155
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride             # <<<<<<<<<<<<<<
  *                dst_data += dst_stride
  *     else:
  */
         __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-        /* "View.MemoryView":1160
+        /* "View.MemoryView":1156
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  *                dst_data += dst_stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(dst_extent):
  */
         __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
       }
     }
     __pyx_L4:;
 
-    /* "View.MemoryView":1152
+    /* "View.MemoryView":1148
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1162
+  /* "View.MemoryView":1158
  *                dst_data += dst_stride
  *     else:
  *         for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *             _copy_strided_to_strided(src_data, src_strides + 1,
  *                                      dst_data, dst_strides + 1,
  */
   /*else*/ {
     __pyx_t_4 = __pyx_v_dst_extent;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "View.MemoryView":1163
+      /* "View.MemoryView":1159
  *     else:
  *         for i in range(dst_extent):
  *             _copy_strided_to_strided(src_data, src_strides + 1,             # <<<<<<<<<<<<<<
  *                                      dst_data, dst_strides + 1,
  *                                      src_shape + 1, dst_shape + 1,
  */
       _copy_strided_to_strided(__pyx_v_src_data, (__pyx_v_src_strides + 1), __pyx_v_dst_data, (__pyx_v_dst_strides + 1), (__pyx_v_src_shape + 1), (__pyx_v_dst_shape + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize);
 
-      /* "View.MemoryView":1167
+      /* "View.MemoryView":1163
  *                                      src_shape + 1, dst_shape + 1,
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride             # <<<<<<<<<<<<<<
  *             dst_data += dst_stride
  * 
  */
       __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-      /* "View.MemoryView":1168
+      /* "View.MemoryView":1164
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride
  *             dst_data += dst_stride             # <<<<<<<<<<<<<<
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,
  */
       __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1140
+  /* "View.MemoryView":1136
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1170
+/* "View.MemoryView":1166
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
 static void copy_strided_to_strided(__Pyx_memviewslice *__pyx_v_src, __Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize) {
 
-  /* "View.MemoryView":1173
+  /* "View.MemoryView":1169
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  *     _copy_strided_to_strided(src.data, src.strides, dst.data, dst.strides,             # <<<<<<<<<<<<<<
  *                              src.shape, dst.shape, ndim, itemsize)
  * 
  */
   _copy_strided_to_strided(__pyx_v_src->data, __pyx_v_src->strides, __pyx_v_dst->data, __pyx_v_dst->strides, __pyx_v_src->shape, __pyx_v_dst->shape, __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1170
+  /* "View.MemoryView":1166
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1177
+/* "View.MemoryView":1173
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
- *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
+ *     cdef int i
  */
 
 static Py_ssize_t __pyx_memoryview_slice_get_size(__Pyx_memviewslice *__pyx_v_src, int __pyx_v_ndim) {
-  Py_ssize_t __pyx_v_shape;
+  int __pyx_v_i;
   Py_ssize_t __pyx_v_size;
   Py_ssize_t __pyx_r;
   Py_ssize_t __pyx_t_1;
-  Py_ssize_t *__pyx_t_2;
-  Py_ssize_t *__pyx_t_3;
-  Py_ssize_t *__pyx_t_4;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  int __pyx_t_4;
 
-  /* "View.MemoryView":1179
- * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:
+  /* "View.MemoryView":1176
  *     "Return the size of the memory occupied by the slice in number of bytes"
- *     cdef Py_ssize_t shape, size = src.memview.view.itemsize             # <<<<<<<<<<<<<<
+ *     cdef int i
+ *     cdef Py_ssize_t size = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  * 
- *     for shape in src.shape[:ndim]:
+ *     for i in range(ndim):
  */
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_size = __pyx_t_1;
 
-  /* "View.MemoryView":1181
- *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
+  /* "View.MemoryView":1178
+ *     cdef Py_ssize_t size = src.memview.view.itemsize
  * 
- *     for shape in src.shape[:ndim]:             # <<<<<<<<<<<<<<
- *         size *= shape
+ *     for i in range(ndim):             # <<<<<<<<<<<<<<
+ *         size *= src.shape[i]
  * 
  */
-  __pyx_t_3 = (__pyx_v_src->shape + __pyx_v_ndim);
-  for (__pyx_t_4 = __pyx_v_src->shape; __pyx_t_4 < __pyx_t_3; __pyx_t_4++) {
-    __pyx_t_2 = __pyx_t_4;
-    __pyx_v_shape = (__pyx_t_2[0]);
+  __pyx_t_2 = __pyx_v_ndim;
+  __pyx_t_3 = __pyx_t_2;
+  for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
+    __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1182
+    /* "View.MemoryView":1179
  * 
- *     for shape in src.shape[:ndim]:
- *         size *= shape             # <<<<<<<<<<<<<<
+ *     for i in range(ndim):
+ *         size *= src.shape[i]             # <<<<<<<<<<<<<<
  * 
  *     return size
  */
-    __pyx_v_size = (__pyx_v_size * __pyx_v_shape);
+    __pyx_v_size = (__pyx_v_size * (__pyx_v_src->shape[__pyx_v_i]));
   }
 
-  /* "View.MemoryView":1184
- *         size *= shape
+  /* "View.MemoryView":1181
+ *         size *= src.shape[i]
  * 
  *     return size             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_fill_contig_strides_array')
  */
   __pyx_r = __pyx_v_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1177
+  /* "View.MemoryView":1173
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
- *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
+ *     cdef int i
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1187
+/* "View.MemoryView":1184
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
@@ -20870,121 +20821,121 @@
   int __pyx_v_idx;
   Py_ssize_t __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1196
+  /* "View.MemoryView":1193
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
   __pyx_t_1 = ((__pyx_v_order == 'F') != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1197
+    /* "View.MemoryView":1194
  * 
  *     if order == 'F':
  *         for idx in range(ndim):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
- *             stride *= shape[idx]
+ *             stride = stride * shape[idx]
  */
     __pyx_t_2 = __pyx_v_ndim;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_idx = __pyx_t_4;
 
-      /* "View.MemoryView":1198
+      /* "View.MemoryView":1195
  *     if order == 'F':
  *         for idx in range(ndim):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
- *             stride *= shape[idx]
+ *             stride = stride * shape[idx]
  *     else:
  */
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1199
+      /* "View.MemoryView":1196
  *         for idx in range(ndim):
  *             strides[idx] = stride
- *             stride *= shape[idx]             # <<<<<<<<<<<<<<
+ *             stride = stride * shape[idx]             # <<<<<<<<<<<<<<
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  */
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
 
-    /* "View.MemoryView":1196
+    /* "View.MemoryView":1193
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1201
- *             stride *= shape[idx]
+  /* "View.MemoryView":1198
+ *             stride = stride * shape[idx]
  *     else:
  *         for idx in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
- *             stride *= shape[idx]
+ *             stride = stride * shape[idx]
  */
   /*else*/ {
     for (__pyx_t_2 = (__pyx_v_ndim - 1); __pyx_t_2 > -1; __pyx_t_2-=1) {
       __pyx_v_idx = __pyx_t_2;
 
-      /* "View.MemoryView":1202
+      /* "View.MemoryView":1199
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
- *             stride *= shape[idx]
+ *             stride = stride * shape[idx]
  * 
  */
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1203
+      /* "View.MemoryView":1200
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride
- *             stride *= shape[idx]             # <<<<<<<<<<<<<<
+ *             stride = stride * shape[idx]             # <<<<<<<<<<<<<<
  * 
  *     return stride
  */
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1205
- *             stride *= shape[idx]
+  /* "View.MemoryView":1202
+ *             stride = stride * shape[idx]
  * 
  *     return stride             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  */
   __pyx_r = __pyx_v_stride;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1187
+  /* "View.MemoryView":1184
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1208
+/* "View.MemoryView":1205
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -20997,222 +20948,222 @@
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   struct __pyx_memoryview_obj *__pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
 
-  /* "View.MemoryView":1219
+  /* "View.MemoryView":1216
  *     cdef void *result
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  */
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1220
+  /* "View.MemoryView":1217
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef size_t size = slice_get_size(src, ndim)             # <<<<<<<<<<<<<<
  * 
  *     result = malloc(size)
  */
   __pyx_v_size = __pyx_memoryview_slice_get_size(__pyx_v_src, __pyx_v_ndim);
 
-  /* "View.MemoryView":1222
+  /* "View.MemoryView":1219
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  *     result = malloc(size)             # <<<<<<<<<<<<<<
  *     if not result:
  *         _err(MemoryError, NULL)
  */
   __pyx_v_result = malloc(__pyx_v_size);
 
-  /* "View.MemoryView":1223
+  /* "View.MemoryView":1220
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_result != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1224
+    /* "View.MemoryView":1221
  *     result = malloc(size)
  *     if not result:
  *         _err(MemoryError, NULL)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 1224, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 1221, __pyx_L1_error)
 
-    /* "View.MemoryView":1223
+    /* "View.MemoryView":1220
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
   }
 
-  /* "View.MemoryView":1227
+  /* "View.MemoryView":1224
  * 
  * 
  *     tmpslice.data = <char *> result             # <<<<<<<<<<<<<<
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  */
   __pyx_v_tmpslice->data = ((char *)__pyx_v_result);
 
-  /* "View.MemoryView":1228
+  /* "View.MemoryView":1225
  * 
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview             # <<<<<<<<<<<<<<
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  */
   __pyx_t_4 = __pyx_v_src->memview;
   __pyx_v_tmpslice->memview = __pyx_t_4;
 
-  /* "View.MemoryView":1229
+  /* "View.MemoryView":1226
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1
  */
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1230
+    /* "View.MemoryView":1227
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]             # <<<<<<<<<<<<<<
  *         tmpslice.suboffsets[i] = -1
  * 
  */
     (__pyx_v_tmpslice->shape[__pyx_v_i]) = (__pyx_v_src->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1231
+    /* "View.MemoryView":1228
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,
  */
     (__pyx_v_tmpslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1233
+  /* "View.MemoryView":1230
  *         tmpslice.suboffsets[i] = -1
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,             # <<<<<<<<<<<<<<
  *                               ndim, order)
  * 
  */
   (void)(__pyx_fill_contig_strides_array((&(__pyx_v_tmpslice->shape[0])), (&(__pyx_v_tmpslice->strides[0])), __pyx_v_itemsize, __pyx_v_ndim, __pyx_v_order));
 
-  /* "View.MemoryView":1237
+  /* "View.MemoryView":1234
  * 
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0
  */
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1238
+    /* "View.MemoryView":1235
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
     __pyx_t_2 = (((__pyx_v_tmpslice->shape[__pyx_v_i]) == 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1239
+      /* "View.MemoryView":1236
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0             # <<<<<<<<<<<<<<
  * 
  *     if slice_is_contig(src[0], order, ndim):
  */
       (__pyx_v_tmpslice->strides[__pyx_v_i]) = 0;
 
-      /* "View.MemoryView":1238
+      /* "View.MemoryView":1235
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1241
+  /* "View.MemoryView":1238
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
   __pyx_t_2 = (__pyx_memviewslice_is_contig((__pyx_v_src[0]), __pyx_v_order, __pyx_v_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1242
+    /* "View.MemoryView":1239
  * 
  *     if slice_is_contig(src[0], order, ndim):
  *         memcpy(result, src.data, size)             # <<<<<<<<<<<<<<
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  */
     (void)(memcpy(__pyx_v_result, __pyx_v_src->data, __pyx_v_size));
 
-    /* "View.MemoryView":1241
+    /* "View.MemoryView":1238
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":1244
+  /* "View.MemoryView":1241
  *         memcpy(result, src.data, size)
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   /*else*/ {
     copy_strided_to_strided(__pyx_v_src, __pyx_v_tmpslice, __pyx_v_ndim, __pyx_v_itemsize);
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":1246
+  /* "View.MemoryView":1243
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1208
+  /* "View.MemoryView":1205
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -21228,15 +21179,15 @@
     #endif
   }
   __pyx_r = NULL;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1251
+/* "View.MemoryView":1248
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -21248,57 +21199,57 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_extents", 0);
 
-  /* "View.MemoryView":1254
+  /* "View.MemoryView":1251
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  *                                                         (i, extent1, extent2))             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err_dim')
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1254, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1254, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1254, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1254, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":1253
+  /* "View.MemoryView":1250
  * cdef int _err_extents(int i, Py_ssize_t extent1,
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %             # <<<<<<<<<<<<<<
  *                                                         (i, extent1, extent2))
  * 
  */
-  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1253, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1253, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_4, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __PYX_ERR(1, 1253, __pyx_L1_error)
+  __PYX_ERR(1, 1250, __pyx_L1_error)
 
-  /* "View.MemoryView":1251
+  /* "View.MemoryView":1248
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -21313,15 +21264,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1257
+/* "View.MemoryView":1254
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -21334,26 +21285,26 @@
   PyObject *__pyx_t_4 = NULL;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_dim", 0);
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1258
+  /* "View.MemoryView":1255
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:
  *     raise error(msg.decode('ascii') % dim)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err')
  */
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1258, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1258, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1258, __pyx_L1_error)
+  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_INCREF(__pyx_v_error);
   __pyx_t_3 = __pyx_v_error; __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -21363,22 +21314,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1258, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 1258, __pyx_L1_error)
+  __PYX_ERR(1, 1255, __pyx_L1_error)
 
-  /* "View.MemoryView":1257
+  /* "View.MemoryView":1254
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -21394,15 +21345,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1261
+/* "View.MemoryView":1258
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -21416,32 +21367,32 @@
   PyObject *__pyx_t_5 = NULL;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err", 0);
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1262
+  /* "View.MemoryView":1259
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_msg != NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":1263
+    /* "View.MemoryView":1260
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))             # <<<<<<<<<<<<<<
  *     else:
  *         raise error
  */
-    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1263, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_error);
     __pyx_t_4 = __pyx_v_error; __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -21449,43 +21400,43 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1263, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 1263, __pyx_L1_error)
+    __PYX_ERR(1, 1260, __pyx_L1_error)
 
-    /* "View.MemoryView":1262
+    /* "View.MemoryView":1259
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
   }
 
-  /* "View.MemoryView":1265
+  /* "View.MemoryView":1262
  *         raise error(msg.decode('ascii'))
  *     else:
  *         raise error             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_contents')
  */
   /*else*/ {
     __Pyx_Raise(__pyx_v_error, 0, 0, 0);
-    __PYX_ERR(1, 1265, __pyx_L1_error)
+    __PYX_ERR(1, 1262, __pyx_L1_error)
   }
 
-  /* "View.MemoryView":1261
+  /* "View.MemoryView":1258
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -21501,15 +21452,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1268
+/* "View.MemoryView":1265
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -21528,119 +21479,119 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   void *__pyx_t_7;
   int __pyx_t_8;
 
-  /* "View.MemoryView":1276
+  /* "View.MemoryView":1273
  *     Check for overlapping memory and verify the shapes.
  *     """
  *     cdef void *tmpdata = NULL             # <<<<<<<<<<<<<<
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  */
   __pyx_v_tmpdata = NULL;
 
-  /* "View.MemoryView":1277
+  /* "View.MemoryView":1274
  *     """
  *     cdef void *tmpdata = NULL
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  */
   __pyx_t_1 = __pyx_v_src.memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1279
+  /* "View.MemoryView":1276
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)             # <<<<<<<<<<<<<<
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False
  */
   __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_src), __pyx_v_src_ndim);
 
-  /* "View.MemoryView":1280
+  /* "View.MemoryView":1277
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False             # <<<<<<<<<<<<<<
  *     cdef bint direct_copy = False
  *     cdef __Pyx_memviewslice tmp
  */
   __pyx_v_broadcasting = 0;
 
-  /* "View.MemoryView":1281
+  /* "View.MemoryView":1278
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False             # <<<<<<<<<<<<<<
  *     cdef __Pyx_memviewslice tmp
  * 
  */
   __pyx_v_direct_copy = 0;
 
-  /* "View.MemoryView":1284
+  /* "View.MemoryView":1281
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
   __pyx_t_2 = ((__pyx_v_src_ndim < __pyx_v_dst_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1285
+    /* "View.MemoryView":1282
  * 
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  */
     __pyx_memoryview_broadcast_leading((&__pyx_v_src), __pyx_v_src_ndim, __pyx_v_dst_ndim);
 
-    /* "View.MemoryView":1284
+    /* "View.MemoryView":1281
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1286
+  /* "View.MemoryView":1283
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
   __pyx_t_2 = ((__pyx_v_dst_ndim < __pyx_v_src_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1287
+    /* "View.MemoryView":1284
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)             # <<<<<<<<<<<<<<
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)
  */
     __pyx_memoryview_broadcast_leading((&__pyx_v_dst), __pyx_v_dst_ndim, __pyx_v_src_ndim);
 
-    /* "View.MemoryView":1286
+    /* "View.MemoryView":1283
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1289
+  /* "View.MemoryView":1286
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
   __pyx_t_3 = __pyx_v_dst_ndim;
@@ -21648,420 +21599,420 @@
   if (((__pyx_t_3 > __pyx_t_4) != 0)) {
     __pyx_t_5 = __pyx_t_3;
   } else {
     __pyx_t_5 = __pyx_t_4;
   }
   __pyx_v_ndim = __pyx_t_5;
 
-  /* "View.MemoryView":1291
+  /* "View.MemoryView":1288
  *     cdef int ndim = max(src_ndim, dst_ndim)
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  */
   __pyx_t_5 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_5;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1292
+    /* "View.MemoryView":1289
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
     __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) != (__pyx_v_dst.shape[__pyx_v_i])) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1293
+      /* "View.MemoryView":1290
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
       __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) == 1) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":1294
+        /* "View.MemoryView":1291
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  *                 broadcasting = True             # <<<<<<<<<<<<<<
  *                 src.strides[i] = 0
  *             else:
  */
         __pyx_v_broadcasting = 1;
 
-        /* "View.MemoryView":1295
+        /* "View.MemoryView":1292
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  *                 src.strides[i] = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  */
         (__pyx_v_src.strides[__pyx_v_i]) = 0;
 
-        /* "View.MemoryView":1293
+        /* "View.MemoryView":1290
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":1297
+      /* "View.MemoryView":1294
  *                 src.strides[i] = 0
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])             # <<<<<<<<<<<<<<
  * 
  *         if src.suboffsets[i] >= 0:
  */
       /*else*/ {
-        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1297, __pyx_L1_error)
+        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1294, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":1292
+      /* "View.MemoryView":1289
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
     }
 
-    /* "View.MemoryView":1299
+    /* "View.MemoryView":1296
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
     __pyx_t_2 = (((__pyx_v_src.suboffsets[__pyx_v_i]) >= 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1300
+      /* "View.MemoryView":1297
  * 
  *         if src.suboffsets[i] >= 0:
  *             _err_dim(ValueError, "Dimension %d is not direct", i)             # <<<<<<<<<<<<<<
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  */
-      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1300, __pyx_L1_error)
+      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1297, __pyx_L1_error)
 
-      /* "View.MemoryView":1299
+      /* "View.MemoryView":1296
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1302
+  /* "View.MemoryView":1299
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
   __pyx_t_2 = (__pyx_slices_overlap((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1304
+    /* "View.MemoryView":1301
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
     __pyx_t_2 = ((!(__pyx_memviewslice_is_contig(__pyx_v_src, __pyx_v_order, __pyx_v_ndim) != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1305
+      /* "View.MemoryView":1302
  * 
  *         if not slice_is_contig(src, order, ndim):
  *             order = get_best_order(&dst, ndim)             # <<<<<<<<<<<<<<
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  */
       __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim);
 
-      /* "View.MemoryView":1304
+      /* "View.MemoryView":1301
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
     }
 
-    /* "View.MemoryView":1307
+    /* "View.MemoryView":1304
  *             order = get_best_order(&dst, ndim)
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)             # <<<<<<<<<<<<<<
  *         src = tmp
  * 
  */
-    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(1, 1307, __pyx_L1_error)
+    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(1, 1304, __pyx_L1_error)
     __pyx_v_tmpdata = __pyx_t_7;
 
-    /* "View.MemoryView":1308
+    /* "View.MemoryView":1305
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  *         src = tmp             # <<<<<<<<<<<<<<
  * 
  *     if not broadcasting:
  */
     __pyx_v_src = __pyx_v_tmp;
 
-    /* "View.MemoryView":1302
+    /* "View.MemoryView":1299
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
   }
 
-  /* "View.MemoryView":1310
+  /* "View.MemoryView":1307
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_broadcasting != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1313
+    /* "View.MemoryView":1310
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'C', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1314
+      /* "View.MemoryView":1311
  * 
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)             # <<<<<<<<<<<<<<
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  */
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'C', __pyx_v_ndim);
 
-      /* "View.MemoryView":1313
+      /* "View.MemoryView":1310
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
       goto __pyx_L12;
     }
 
-    /* "View.MemoryView":1315
+    /* "View.MemoryView":1312
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'F', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1316
+      /* "View.MemoryView":1313
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)             # <<<<<<<<<<<<<<
  * 
  *         if direct_copy:
  */
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'F', __pyx_v_ndim);
 
-      /* "View.MemoryView":1315
+      /* "View.MemoryView":1312
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
     }
     __pyx_L12:;
 
-    /* "View.MemoryView":1318
+    /* "View.MemoryView":1315
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
     __pyx_t_2 = (__pyx_v_direct_copy != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1320
+      /* "View.MemoryView":1317
  *         if direct_copy:
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  */
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-      /* "View.MemoryView":1321
+      /* "View.MemoryView":1318
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))             # <<<<<<<<<<<<<<
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  */
       (void)(memcpy(__pyx_v_dst.data, __pyx_v_src.data, __pyx_memoryview_slice_get_size((&__pyx_v_src), __pyx_v_ndim)));
 
-      /* "View.MemoryView":1322
+      /* "View.MemoryView":1319
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  *             free(tmpdata)
  *             return 0
  */
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-      /* "View.MemoryView":1323
+      /* "View.MemoryView":1320
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)             # <<<<<<<<<<<<<<
  *             return 0
  * 
  */
       free(__pyx_v_tmpdata);
 
-      /* "View.MemoryView":1324
+      /* "View.MemoryView":1321
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  *             return 0             # <<<<<<<<<<<<<<
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):
  */
       __pyx_r = 0;
       goto __pyx_L0;
 
-      /* "View.MemoryView":1318
+      /* "View.MemoryView":1315
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
     }
 
-    /* "View.MemoryView":1310
+    /* "View.MemoryView":1307
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1326
+  /* "View.MemoryView":1323
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = (__pyx_v_order == 'F');
   if (__pyx_t_2) {
     __pyx_t_2 = ('F' == __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim));
   }
   __pyx_t_8 = (__pyx_t_2 != 0);
   if (__pyx_t_8) {
 
-    /* "View.MemoryView":1329
+    /* "View.MemoryView":1326
  * 
  * 
  *         transpose_memslice(&src)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&dst)
  * 
  */
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1329, __pyx_L1_error)
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1326, __pyx_L1_error)
 
-    /* "View.MemoryView":1330
+    /* "View.MemoryView":1327
  * 
  *         transpose_memslice(&src)
  *         transpose_memslice(&dst)             # <<<<<<<<<<<<<<
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  */
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1330, __pyx_L1_error)
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1327, __pyx_L1_error)
 
-    /* "View.MemoryView":1326
+    /* "View.MemoryView":1323
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1332
+  /* "View.MemoryView":1329
  *         transpose_memslice(&dst)
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  */
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1333
+  /* "View.MemoryView":1330
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)             # <<<<<<<<<<<<<<
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  */
   copy_strided_to_strided((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1334
+  /* "View.MemoryView":1331
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  *     free(tmpdata)
  */
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1336
+  /* "View.MemoryView":1333
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  *     free(tmpdata)             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
   free(__pyx_v_tmpdata);
 
-  /* "View.MemoryView":1337
+  /* "View.MemoryView":1334
  * 
  *     free(tmpdata)
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1268
+  /* "View.MemoryView":1265
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -22077,217 +22028,217 @@
     #endif
   }
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1340
+/* "View.MemoryView":1337
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
 static void __pyx_memoryview_broadcast_leading(__Pyx_memviewslice *__pyx_v_mslice, int __pyx_v_ndim, int __pyx_v_ndim_other) {
   int __pyx_v_i;
   int __pyx_v_offset;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "View.MemoryView":1344
+  /* "View.MemoryView":1341
  *                             int ndim_other) nogil:
  *     cdef int i
  *     cdef int offset = ndim_other - ndim             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
   __pyx_v_offset = (__pyx_v_ndim_other - __pyx_v_ndim);
 
-  /* "View.MemoryView":1346
+  /* "View.MemoryView":1343
  *     cdef int offset = ndim_other - ndim
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  */
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1347
+    /* "View.MemoryView":1344
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]             # <<<<<<<<<<<<<<
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  */
     (__pyx_v_mslice->shape[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1348
+    /* "View.MemoryView":1345
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  */
     (__pyx_v_mslice->strides[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-    /* "View.MemoryView":1349
+    /* "View.MemoryView":1346
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]             # <<<<<<<<<<<<<<
  * 
  *     for i in range(offset):
  */
     (__pyx_v_mslice->suboffsets[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->suboffsets[__pyx_v_i]);
   }
 
-  /* "View.MemoryView":1351
+  /* "View.MemoryView":1348
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  *     for i in range(offset):             # <<<<<<<<<<<<<<
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  */
   __pyx_t_1 = __pyx_v_offset;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1352
+    /* "View.MemoryView":1349
  * 
  *     for i in range(offset):
  *         mslice.shape[i] = 1             # <<<<<<<<<<<<<<
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1
  */
     (__pyx_v_mslice->shape[__pyx_v_i]) = 1;
 
-    /* "View.MemoryView":1353
+    /* "View.MemoryView":1350
  *     for i in range(offset):
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i] = -1
  * 
  */
     (__pyx_v_mslice->strides[__pyx_v_i]) = (__pyx_v_mslice->strides[0]);
 
-    /* "View.MemoryView":1354
+    /* "View.MemoryView":1351
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_mslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1340
+  /* "View.MemoryView":1337
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1362
+/* "View.MemoryView":1359
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_dtype_is_object, int __pyx_v_ndim, int __pyx_v_inc) {
   int __pyx_t_1;
 
-  /* "View.MemoryView":1366
+  /* "View.MemoryView":1363
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
   __pyx_t_1 = (__pyx_v_dtype_is_object != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1367
+    /* "View.MemoryView":1364
  * 
  *     if dtype_is_object:
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,             # <<<<<<<<<<<<<<
  *                                            dst.strides, ndim, inc)
  * 
  */
     __pyx_memoryview_refcount_objects_in_slice_with_gil(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_inc);
 
-    /* "View.MemoryView":1366
+    /* "View.MemoryView":1363
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
   }
 
-  /* "View.MemoryView":1362
+  /* "View.MemoryView":1359
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1371
+/* "View.MemoryView":1368
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
   __Pyx_RefNannyDeclarations
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("refcount_objects_in_slice_with_gil", 0);
 
-  /* "View.MemoryView":1374
+  /* "View.MemoryView":1371
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  *     refcount_objects_in_slice(data, shape, strides, ndim, inc)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  */
   __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, __pyx_v_shape, __pyx_v_strides, __pyx_v_ndim, __pyx_v_inc);
 
-  /* "View.MemoryView":1371
+  /* "View.MemoryView":1368
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "View.MemoryView":1377
+/* "View.MemoryView":1374
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
@@ -22296,178 +22247,178 @@
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   __Pyx_RefNannySetupContext("refcount_objects_in_slice", 0);
 
-  /* "View.MemoryView":1381
+  /* "View.MemoryView":1378
  *     cdef Py_ssize_t i
  * 
  *     for i in range(shape[0]):             # <<<<<<<<<<<<<<
  *         if ndim == 1:
  *             if inc:
  */
   __pyx_t_1 = (__pyx_v_shape[0]);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1382
+    /* "View.MemoryView":1379
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
     __pyx_t_4 = ((__pyx_v_ndim == 1) != 0);
     if (__pyx_t_4) {
 
-      /* "View.MemoryView":1383
+      /* "View.MemoryView":1380
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
       __pyx_t_4 = (__pyx_v_inc != 0);
       if (__pyx_t_4) {
 
-        /* "View.MemoryView":1384
+        /* "View.MemoryView":1381
  *         if ndim == 1:
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])
  */
         Py_INCREF((((PyObject **)__pyx_v_data)[0]));
 
-        /* "View.MemoryView":1383
+        /* "View.MemoryView":1380
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
         goto __pyx_L6;
       }
 
-      /* "View.MemoryView":1386
+      /* "View.MemoryView":1383
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  */
       /*else*/ {
         Py_DECREF((((PyObject **)__pyx_v_data)[0]));
       }
       __pyx_L6:;
 
-      /* "View.MemoryView":1382
+      /* "View.MemoryView":1379
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":1388
+    /* "View.MemoryView":1385
  *                 Py_DECREF((<PyObject **> data)[0])
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                       ndim - 1, inc)
  * 
  */
     /*else*/ {
 
-      /* "View.MemoryView":1389
+      /* "View.MemoryView":1386
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  *                                       ndim - 1, inc)             # <<<<<<<<<<<<<<
  * 
  *         data += strides[0]
  */
       __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_inc);
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":1391
+    /* "View.MemoryView":1388
  *                                       ndim - 1, inc)
  * 
  *         data += strides[0]             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_v_data = (__pyx_v_data + (__pyx_v_strides[0]));
   }
 
-  /* "View.MemoryView":1377
+  /* "View.MemoryView":1374
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1397
+/* "View.MemoryView":1394
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize, void *__pyx_v_item, int __pyx_v_dtype_is_object) {
 
-  /* "View.MemoryView":1400
+  /* "View.MemoryView":1397
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  */
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1401
+  /* "View.MemoryView":1398
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,             # <<<<<<<<<<<<<<
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)
  */
   __pyx_memoryview__slice_assign_scalar(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_itemsize, __pyx_v_item);
 
-  /* "View.MemoryView":1403
+  /* "View.MemoryView":1400
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1397
+  /* "View.MemoryView":1394
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1407
+/* "View.MemoryView":1404
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -22476,118 +22427,118 @@
   Py_ssize_t __pyx_v_stride;
   Py_ssize_t __pyx_v_extent;
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
 
-  /* "View.MemoryView":1411
+  /* "View.MemoryView":1408
  *                               size_t itemsize, void *item) nogil:
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t extent = shape[0]
  * 
  */
   __pyx_v_stride = (__pyx_v_strides[0]);
 
-  /* "View.MemoryView":1412
+  /* "View.MemoryView":1409
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]
  *     cdef Py_ssize_t extent = shape[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
   __pyx_v_extent = (__pyx_v_shape[0]);
 
-  /* "View.MemoryView":1414
+  /* "View.MemoryView":1411
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1415
+    /* "View.MemoryView":1412
  * 
  *     if ndim == 1:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             memcpy(data, item, itemsize)
  *             data += stride
  */
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1416
+      /* "View.MemoryView":1413
  *     if ndim == 1:
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)             # <<<<<<<<<<<<<<
  *             data += stride
  *     else:
  */
       (void)(memcpy(__pyx_v_data, __pyx_v_item, __pyx_v_itemsize));
 
-      /* "View.MemoryView":1417
+      /* "View.MemoryView":1414
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  *             data += stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(extent):
  */
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
 
-    /* "View.MemoryView":1414
+    /* "View.MemoryView":1411
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1419
+  /* "View.MemoryView":1416
  *             data += stride
  *     else:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  */
   /*else*/ {
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1420
+      /* "View.MemoryView":1417
  *     else:
  *         for i in range(extent):
  *             _slice_assign_scalar(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                 ndim - 1, itemsize, item)
  *             data += stride
  */
       __pyx_memoryview__slice_assign_scalar(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize, __pyx_v_item);
 
-      /* "View.MemoryView":1422
+      /* "View.MemoryView":1419
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  *             data += stride             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1407
+  /* "View.MemoryView":1404
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -23009,20 +22960,15 @@
 
 static PyTypeObject __pyx_type_8causalml_9inference_4tree_10causaltree_CausalMSE = {
   PyVarObject_HEAD_INIT(0, 0)
   "causalml.inference.tree.causaltree.CausalMSE", /*tp_name*/
   sizeof(struct __pyx_obj_8causalml_9inference_4tree_10causaltree_CausalMSE), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_8causalml_9inference_4tree_10causaltree_CausalMSE, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -23067,17 +23013,14 @@
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -23198,20 +23141,15 @@
 
 static PyTypeObject __pyx_type___pyx_array = {
   PyVarObject_HEAD_INIT(0, 0)
   "causalml.inference.tree.causaltree.array", /*tp_name*/
   sizeof(struct __pyx_array_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_array, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -23256,17 +23194,14 @@
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
@@ -23317,20 +23252,15 @@
 
 static PyTypeObject __pyx_type___pyx_MemviewEnum = {
   PyVarObject_HEAD_INIT(0, 0)
   "causalml.inference.tree.causaltree.Enum", /*tp_name*/
   sizeof(struct __pyx_MemviewEnum_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_Enum, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -23375,17 +23305,14 @@
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -23578,20 +23505,15 @@
 
 static PyTypeObject __pyx_type___pyx_memoryview = {
   PyVarObject_HEAD_INIT(0, 0)
   "causalml.inference.tree.causaltree.memoryview", /*tp_name*/
   sizeof(struct __pyx_memoryview_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_memoryview, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -23636,17 +23558,14 @@
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
   PyObject *o = __pyx_tp_new_memoryview(t, a, k);
   if (unlikely(!o)) return 0;
@@ -23716,20 +23635,15 @@
 
 static PyTypeObject __pyx_type___pyx_memoryviewslice = {
   PyVarObject_HEAD_INIT(0, 0)
   "causalml.inference.tree.causaltree._memoryviewslice", /*tp_name*/
   sizeof(struct __pyx_memoryviewslice_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc__memoryviewslice, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -23782,17 +23696,14 @@
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
@@ -24079,17 +23990,17 @@
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 55, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 258, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(2, 856, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 1038, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 151, __pyx_L1_error)
-  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 404, __pyx_L1_error)
-  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 613, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 832, __pyx_L1_error)
+  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 400, __pyx_L1_error)
+  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 609, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 828, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -24143,81 +24054,81 @@
  *                 if verbose:
  *                     now = pd.datetime.today()
  */
   __pyx_slice__5 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__5)) __PYX_ERR(0, 355, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__5);
   __Pyx_GIVEREF(__pyx_slice__5);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":272
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":272
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_C_contiguous); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":276
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":276
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
  * 
  *             info.buf = PyArray_DATA(self)
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_Fortran_contiguou); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":306
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":306
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":856
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":856
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 856, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":880
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":880
  *             t = child.type_num
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor_2); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 880, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1038
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1038
  *         _import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 1038, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "../../miniconda3/envs/py37/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1044
+  /* "../../anaconda3/lib/python3.7/site-packages/Cython/Includes/numpy/__init__.pxd":1044
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 1044, __pyx_L1_error)
@@ -24294,66 +24205,66 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
 
-  /* "View.MemoryView":418
+  /* "View.MemoryView":414
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 418, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
 
-  /* "View.MemoryView":495
+  /* "View.MemoryView":491
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 495, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
 
-  /* "View.MemoryView":520
+  /* "View.MemoryView":516
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 520, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
 
-  /* "View.MemoryView":570
+  /* "View.MemoryView":566
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 570, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
 
-  /* "View.MemoryView":577
+  /* "View.MemoryView":573
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__24 = PyTuple_New(1); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 577, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_New(1); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 573, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
   PyTuple_SET_ITEM(__pyx_tuple__24, 0, __pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "(tree fragment)":2
@@ -24371,22 +24282,22 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
 
-  /* "View.MemoryView":703
+  /* "View.MemoryView":699
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 703, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 699, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -24700,23 +24611,23 @@
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(1, 330, __pyx_L1_error)
   __pyx_memoryview_type = &__pyx_type___pyx_memoryview;
   __pyx_vtabptr__memoryviewslice = &__pyx_vtable__memoryviewslice;
   __pyx_vtable__memoryviewslice.__pyx_base = *__pyx_vtabptr_memoryview;
   __pyx_vtable__memoryviewslice.__pyx_base.convert_item_to_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *))__pyx_memoryviewslice_convert_item_to_object;
   __pyx_vtable__memoryviewslice.__pyx_base.assign_item_from_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *, PyObject *))__pyx_memoryviewslice_assign_item_from_object;
   __pyx_type___pyx_memoryviewslice.tp_base = __pyx_memoryview_type;
-  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 965, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 961, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_memoryviewslice.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_memoryviewslice.tp_dictoffset && __pyx_type___pyx_memoryviewslice.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_memoryviewslice.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(1, 965, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 965, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(1, 961, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 961, __pyx_L1_error)
   __pyx_memoryviewslice_type = &__pyx_type___pyx_memoryviewslice;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -25457,37 +25368,37 @@
   __pyx_t_4[3] = PyThread_allocate_lock();
   __pyx_t_4[4] = PyThread_allocate_lock();
   __pyx_t_4[5] = PyThread_allocate_lock();
   __pyx_t_4[6] = PyThread_allocate_lock();
   __pyx_t_4[7] = PyThread_allocate_lock();
   memcpy(&(__pyx_memoryview_thread_locks[0]), __pyx_t_4, sizeof(__pyx_memoryview_thread_locks[0]) * (8));
 
-  /* "View.MemoryView":549
+  /* "View.MemoryView":545
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 549, __pyx_L1_error)
+  __pyx_t_2 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 545, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_2) < 0) __PYX_ERR(1, 549, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_2) < 0) __PYX_ERR(1, 545, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_memoryview_type);
 
-  /* "View.MemoryView":995
+  /* "View.MemoryView":991
  *         return self.from_object
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 995, __pyx_L1_error)
+  __pyx_t_2 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 991, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_2) < 0) __PYX_ERR(1, 995, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_2) < 0) __PYX_ERR(1, 991, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_memoryviewslice_type);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
@@ -27755,51 +27666,51 @@
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto GOOD;
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto GOOD;
 #endif
 #if CYTHON_USE_PYTYPE_LOOKUP
-    object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
+    object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto BAD;
 #else
-    object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
+    object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto BAD;
 #endif
-    reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
+    reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto BAD;
     if (reduce_ex == object_reduce_ex) {
 #if CYTHON_USE_PYTYPE_LOOKUP
-        object_reduce = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+        object_reduce = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto BAD;
 #else
-        object_reduce = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+        object_reduce = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto BAD;
 #endif
-        reduce = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce); if (unlikely(!reduce)) goto __PYX_BAD;
+        reduce = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce); if (unlikely(!reduce)) goto BAD;
         if (reduce == object_reduce || __Pyx_setup_reduce_is_named(reduce, __pyx_n_s_reduce_cython)) {
-            reduce_cython = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_cython); if (unlikely(!reduce_cython)) goto __PYX_BAD;
-            ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-            ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+            reduce_cython = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_cython); if (unlikely(!reduce_cython)) goto BAD;
+            ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto BAD;
+            ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto BAD;
             setstate = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate);
             if (!setstate) PyErr_Clear();
             if (!setstate || __Pyx_setup_reduce_is_named(setstate, __pyx_n_s_setstate_cython)) {
-                setstate_cython = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate_cython); if (unlikely(!setstate_cython)) goto __PYX_BAD;
-                ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-                ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+                setstate_cython = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate_cython); if (unlikely(!setstate_cython)) goto BAD;
+                ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto BAD;
+                ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto BAD;
             }
             PyType_Modified((PyTypeObject*)type_obj);
         }
     }
-    goto __PYX_GOOD;
-__PYX_BAD:
+    goto GOOD;
+BAD:
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
-__PYX_GOOD:
+GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
@@ -28448,17 +28359,14 @@
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-    0,
-#endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
     }
     return 0;
@@ -28959,14 +28867,15 @@
                     case 0:
                         z.real = 1;
                         z.imag = 0;
                         return z;
                     case 1:
                         return a;
                     case 2:
+                        z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(a, a);
                     case 3:
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, a);
                     case 4:
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
@@ -29113,14 +29022,15 @@
                     case 0:
                         z.real = 1;
                         z.imag = 0;
                         return z;
                     case 1:
                         return a;
                     case 2:
+                        z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(a, a);
                     case 3:
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, a);
                     case 4:
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
```

### Comparing `causalml-0.8.0/causalml/inference/tree/causaltree.pyx` & `causalml-0.9.0/causalml/inference/tree/causaltree.pyx`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/inference/tree/models.py` & `causalml-0.9.0/causalml/inference/tree/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 #          Totte Harinen <totte@uber.com>
 
 from collections import defaultdict
 import numpy as np
 import scipy.stats as stats
 import pandas as pd
 from sklearn.utils.testing import ignore_warnings
-
+from collections import defaultdict
+from joblib import Parallel, delayed
+import multiprocessing as mp
 
 class DecisionTree:
     """ Tree Node Class
 
     Tree node class to contain all the statistics of the tree node.
 
     Parameters
@@ -172,22 +174,27 @@
         Returns
         -------
         self : object
         """
         assert len(X) == len(y) and len(X) == len(treatment), 'Data length must be equal for X, treatment, and y.'
 
         self.treatment_group = list(set(treatment))
+        self.feature_imp_dict = defaultdict(float)
 
         self.fitted_uplift_tree = self.growDecisionTreeFrom(
             X, treatment, y, evaluationFunction=self.evaluationFunction,
             max_depth=self.max_depth, min_samples_leaf=self.min_samples_leaf,
             depth=1, min_samples_treatment=self.min_samples_treatment,
             n_reg=self.n_reg, parentNodeSummary=None
         )
-        return self
+
+        self.feature_importances_ = np.zeros(X.shape[1])
+        for col, imp in self.feature_imp_dict.items():
+            self.feature_importances_[col] = imp
+        self.feature_importances_ /= self.feature_importances_.sum()  # normalize to add to 1
 
     # Prune Trees
     def prune(self, X, treatment, y, minGain=0.0001, rule='maxAbsDiff'):
         """ Prune the uplift model.
         Args
         ----
         X : ndarray, shape = [num_samples, num_features]
@@ -955,15 +962,15 @@
                                                          min_samples_treatment=min_samples_treatment,
                                                          n_reg=n_reg,
                                                          parentNodeSummary=currentNodeSummary)
 
                 rightNodeSummary = self.tree_node_summary(w_r, y_r,
                                                           min_samples_treatment=min_samples_treatment,
                                                           n_reg=n_reg,
-                                                          parentNodeSummary=parentNodeSummary)
+                                                          parentNodeSummary=currentNodeSummary)
 
                 # check the split validity on min_samples_treatment
                 if set(leftNodeSummary.keys()) != set(rightNodeSummary.keys()):
                     continue
                 node_mst = 10**8
                 for ti in leftNodeSummary:
                     node_mst = np.min([node_mst, leftNodeSummary[ti][1]])
@@ -972,20 +979,22 @@
                     continue
                 # evaluate the split
 
                 if evaluationFunction == self.evaluate_CTS:
                     leftScore1 = evaluationFunction(leftNodeSummary)
                     rightScore2 = evaluationFunction(rightNodeSummary)
                     gain = (currentScore - p * leftScore1 - (1 - p) * rightScore2)
+                    gain_for_imp = (len(X) * currentScore - len(X_l) * leftScore1 - len(X_r) * rightScore2)
                 else:
                     if (self.control_name in leftNodeSummary and
                         self.control_name in rightNodeSummary):
                         leftScore1 = evaluationFunction(leftNodeSummary, control_name=self.control_name)
                         rightScore2 = evaluationFunction(rightNodeSummary, control_name=self.control_name)
                         gain = (p * leftScore1 + (1 - p) * rightScore2 - currentScore)
+                        gain_for_imp = (len(X_l) * leftScore1 + len(X_r) * rightScore2 - len(X) * currentScore)
                         if self.normalization:
                             norm_factor = self.normI(currentNodeSummary,
                                                      leftNodeSummary,
                                                      rightNodeSummary,
                                                      self.control_name,
                                                      alpha=0.9)
                         else:
@@ -994,14 +1003,15 @@
                     else:
                         gain = 0
                 if (gain > bestGain and len(X_l) > min_samples_leaf and len(X_r) > min_samples_leaf):
                     bestGain = gain
                     bestAttribute = (col, value)
                     best_set_left = [X_l, w_l, y_l]
                     best_set_right = [X_r, w_r, y_r]
+                    self.feature_imp_dict[bestAttribute[0]] += gain_for_imp
 
         dcY = {'impurity': '%.3f' % currentScore, 'samples': '%d' % len(X)}
         # Add treatment size
         dcY['group_size'] = ''
         for treatment_group in currentNodeSummary:
             dcY['group_size'] += ' ' + treatment_group + ': ' + str(currentNodeSummary[treatment_group][1])
         dcY['upliftScore'] = [round(upliftScore[0], 4), round(upliftScore[1], 4)]
@@ -1196,28 +1206,30 @@
                  random_state=2019,
                  max_depth=5,
                  min_samples_leaf=100,
                  min_samples_treatment=10,
                  n_reg=10,
                  evaluationFunction=None,
                  control_name=None,
-                 normalization=True):
+                 normalization=True,
+                 n_jobs=-1):
         """
         Initialize the UpliftRandomForestClassifier class.
         """
         self.classes_ = {}
         self.n_estimators = n_estimators
         self.max_features = max_features
         self.random_state = random_state
         self.max_depth = max_depth
         self.min_samples_leaf = min_samples_leaf
         self.min_samples_treatment = min_samples_treatment
         self.n_reg = n_reg
         self.evaluationFunction = evaluationFunction
         self.control_name = control_name
+        self.n_jobs = n_jobs
 
         # Create forest
         self.uplift_forest = []
         for _ in range(n_estimators):
             uplift_tree = UpliftTreeClassifier(
                 max_features=self.max_features, max_depth=self.max_depth,
                 min_samples_leaf=self.min_samples_leaf,
@@ -1225,14 +1237,17 @@
                 n_reg=self.n_reg,
                 evaluationFunction=self.evaluationFunction,
                 control_name=self.control_name,
                 normalization=normalization)
 
             self.uplift_forest.append(uplift_tree)
 
+        if self.n_jobs == -1:
+            self.n_jobs = mp.cpu_count()
+
     def fit(self, X, treatment, y):
         """
         Fit the UpliftRandomForestClassifier.
 
         Args
         ----
         X : ndarray, shape = [num_samples, num_features]
@@ -1250,21 +1265,30 @@
         treatment_group_keys = list(set(treatment))
         treatment_group_keys.remove(self.control_name)
         treatment_group_keys.sort()
         self.classes_ = {}
         for i, treatment_group_key in enumerate(treatment_group_keys):
             self.classes_[treatment_group_key] = i
 
-        # Bootstrap
-        for tree_i in range(len(self.uplift_forest)):
-            bt_index = np.random.choice(len(X), len(X))
-            x_train_bt = X[bt_index]
-            y_train_bt = y[bt_index]
-            treatment_train_bt = treatment[bt_index]
-            self.uplift_forest[tree_i].fit(X=x_train_bt, treatment=treatment_train_bt, y=y_train_bt)
+        self.uplift_forest = (
+            Parallel(n_jobs=self.n_jobs)
+            (delayed(self.bootstrap)(X, treatment, y, tree) for tree in self.uplift_forest)
+        )
+
+        all_importances = [tree.feature_importances_ for tree in self.uplift_forest]
+        self.feature_importances_ = np.mean(all_importances, axis=0)
+        self.feature_importances_ /= self.feature_importances_.sum()  # normalize to add to 1
+
+    def bootstrap(self, X, treatment, y, tree):
+        bt_index = np.random.choice(len(X), len(X))
+        x_train_bt = X[bt_index]
+        y_train_bt = y[bt_index]
+        treatment_train_bt = treatment[bt_index]
+        tree.fit(X=x_train_bt, treatment=treatment_train_bt, y=y_train_bt)
+        return tree
 
     @ignore_warnings(category=FutureWarning)
     def predict(self, X, full_output=False):
         '''
         Returns the recommended treatment group and predicted optimal
         probability conditional on using the recommended treatment group.
 
@@ -1275,16 +1299,20 @@
 
         full_output : bool, optional (default=False)
             Whether the UpliftTree algorithm returns upliftScores, pred_nodes
             alongside the recommended treatment group and p_hat in the treatment group.
 
         Returns
         -------
+        y_pred_list : ndarray, shape = (num_samples, num_treatments])
+            An ndarray  containing the predicted delta in each treatment group,
+            the best treatment group and the maximum delta.
+        
         df_res : DataFrame, shape = [num_samples, (num_treatments + 1)]
-            A DataFrame containing the predicted delta in each treatment group,
+            If full_output, a DataFrame containing the predicted delta in each treatment group,
             the best treatment group and the maximum delta.
 
         '''
         df_res = pd.DataFrame()
         y_pred_ensemble = dict()
         y_pred_list = np.zeros((X.shape[0], len(self.classes_)))
 
@@ -1317,8 +1345,11 @@
             if treatment_group != self.control_name:
                 delta_cols.append('delta_%s' % (treatment_group))
                 df_res['delta_%s' % (treatment_group)] = df_res[treatment_group] - df_res[self.control_name]
                 # Add deltas to results list
                 y_pred_list[:, self.classes_[treatment_group]] = df_res['delta_%s' % (treatment_group)].values
         df_res['max_delta'] = df_res[delta_cols].max(axis=1)
 
-        return y_pred_list
+        if full_output:
+            return df_res
+        else:
+            return y_pred_list
```

### Comparing `causalml-0.8.0/causalml/inference/tree/plot.py` & `causalml-0.9.0/causalml/inference/tree/plot.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/inference/tree/utils.py` & `causalml-0.9.0/causalml/inference/tree/utils.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/match.py` & `causalml-0.9.0/causalml/match.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/metrics/__init__.py` & `causalml-0.9.0/causalml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/metrics/classification.py` & `causalml-0.9.0/causalml/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/metrics/regression.py` & `causalml-0.9.0/causalml/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/metrics/sensitivity.py` & `causalml-0.9.0/causalml/metrics/sensitivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,17 +71,14 @@
         treatment (np.array): a treatment vector (1 if treated, otherwise 0)
     """
     assert p.shape[0] == treatment.shape[0]
     adj = alpha * (1 - treatment)
     return adj
 
 
-from ..inference.meta.tlearner import BaseTLearner
-
-
 class Sensitivity(object):
     """ A Sensitivity Check class to support Placebo Treatment, Irrelevant Additional Confounder
     and Subset validation refutation methods to verify causal inference.
 
     Reference: https://github.com/microsoft/dowhy/blob/master/dowhy/causal_refuters/
     """
 
@@ -133,14 +130,15 @@
             treatment (np.array): a treatment vector (1 if treated, otherwise 0)
             y (np.array): an outcome vector
         Returns:
             (numpy.ndarray): Mean and confidence interval (LB, UB) of the ATE estimate.
         """
 
         learner = self.learner
+        from ..inference.meta.tlearner import BaseTLearner
         if isinstance(learner, BaseTLearner):
             ate, ate_lower, ate_upper = learner.estimate_ate(X=X, treatment=treatment, y=y)
         else:
             try:
                 ate, ate_lower, ate_upper = learner.estimate_ate(X=X, p=p, treatment=treatment, y=y)
             except TypeError:
                 ate, ate_lower, ate_upper = learner.estimate_ate(X=X, treatment=treatment, y=y, return_ci=True)
```

### Comparing `causalml-0.8.0/causalml/metrics/visualize.py` & `causalml-0.9.0/causalml/metrics/visualize.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/optimize/policylearner.py` & `causalml-0.9.0/causalml/optimize/policylearner.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/optimize/unit_selection.py` & `causalml-0.9.0/causalml/optimize/unit_selection.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/optimize/utils.py` & `causalml-0.9.0/causalml/optimize/utils.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml/optimize/value_optimization.py` & `causalml-0.9.0/causalml/optimize/value_optimization.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/causalml.egg-info/PKG-INFO` & `causalml-0.9.0/causalml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalml
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python Package for Uplift Modeling and Causal Inference with Machine Learning Algorithms
 Home-page: https://github.com/uber/causalml
 Author: Huigang Chen, Totte Harinen, Jeong-Yoon Lee, Yuchen Luo, Jing Pan, Mike Yung, Zhenyu Zhao
 Author-email: 
 License: UNKNOWN
 Description: <div align="center">
           <a href="https://github.com/uber/causalml"><img width="380px" height="140px" src="https://raw.githubusercontent.com/uber/causalml/master/docs/_static/img/causalml_logo.png"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: causalml Version: 0.8.0 Summary: Python Package for
+Metadata-Version: 2.1 Name: causalml Version: 0.9.0 Summary: Python Package for
 Uplift Modeling and Causal Inference with Machine Learning Algorithms Home-
 page: https://github.com/uber/causalml Author: Huigang Chen, Totte Harinen,
 Jeong-Yoon Lee, Yuchen Luo, Jing Pan, Mike Yung, Zhenyu Zhao Author-email:
 License: UNKNOWN Description:
    [https://raw.githubusercontent.com/uber/causalml/master/docs/_static/img/
                               causalml_logo.png]
 ------------------------------------------------------ [![PyPI Version](https:/
```

### Comparing `causalml-0.8.0/setup.py` & `causalml-0.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 try:
     from numpy import get_include as np_get_include
 except ImportError:
     dist.Distribution().fetch_build_eggs(['numpy'])
     from numpy import get_include as np_get_include
 
 
-with open("README.md", "r") as f:
+with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 
 with open("requirements.txt") as f:
     requirements = f.readlines()
 
 extensions = [
```

### Comparing `causalml-0.8.0/tests/conftest.py` & `causalml-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/tests/test_counterfactual_unit_selection.py` & `causalml-0.9.0/tests/test_counterfactual_unit_selection.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/tests/test_datasets.py` & `causalml-0.9.0/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/tests/test_features.py` & `causalml-0.9.0/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/tests/test_match.py` & `causalml-0.9.0/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/tests/test_meta_learners.py` & `causalml-0.9.0/tests/test_meta_learners.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,26 +525,39 @@
     propensity_model.fit(X=df[x_names].values, y=df['treatment_group_key'].values)
     df['propensity_score'] = propensity_model.predict_proba(df[x_names].values)[:, 1]
 
     df_train, df_test = train_test_split(df,
                                          test_size=0.2,
                                          random_state=RANDOM_SEED)
 
+    # specify all 4 learners
     uplift_model = BaseXClassifier(control_outcome_learner=XGBClassifier(),
                                    control_effect_learner=XGBRegressor(),
                                    treatment_outcome_learner=XGBClassifier(),
                                    treatment_effect_learner=XGBRegressor())
 
     uplift_model.fit(X=df_train[x_names].values,
                      treatment=df_train['treatment_group_key'].values,
                      y=df_train[CONVERSION].values)
 
     tau_pred = uplift_model.predict(X=df_test[x_names].values,
                                   p=df_test['propensity_score'].values)
 
+    # specify 2 learners
+    uplift_model = BaseXClassifier(outcome_learner=XGBClassifier(),
+                                   effect_learner=XGBRegressor())
+
+    uplift_model.fit(X=df_train[x_names].values,
+                     treatment=df_train['treatment_group_key'].values,
+                     y=df_train[CONVERSION].values)
+
+    tau_pred = uplift_model.predict(X=df_test[x_names].values,
+                                  p=df_test['propensity_score'].values)
+
+    # calculate metrics
     auuc_metrics = pd.DataFrame({'tau_pred': tau_pred.flatten(),
                                  'W': df_test['treatment_group_key'].values,
                                  CONVERSION: df_test[CONVERSION].values,
                                  'treatment_effect_col': df_test['treatment_effect'].values})
 
     cumgain = get_cumgain(auuc_metrics,
                           outcome_col=CONVERSION,
```

### Comparing `causalml-0.8.0/tests/test_propensity.py` & `causalml-0.9.0/tests/test_propensity.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,53 @@
-from causalml.propensity import ElasticNetPropensityModel, GradientBoostedPropensityModel
+from causalml.propensity import (
+    ElasticNetPropensityModel,
+    GradientBoostedPropensityModel,
+    LogisticRegressionPropensityModel
+)
 from causalml.metrics import roc_auc_score
 
 
 from .const import RANDOM_SEED
 
 
+def test_logistic_regression_propensity_model(generate_regression_data):
+    y, X, treatment, tau, b, e = generate_regression_data()
+
+    pm = LogisticRegressionPropensityModel(random_state=RANDOM_SEED)
+    ps = pm.fit_predict(X, treatment)
+
+    assert roc_auc_score(treatment, ps) > .5
+
+
+def test_logistic_regression_propensity_model_model_kwargs(generate_regression_data):
+    y, X, treatment, tau, b, e = generate_regression_data()
+
+    pm = LogisticRegressionPropensityModel(random_state=123)
+
+    assert pm.model.random_state == 123
+
+
 def test_elasticnet_propensity_model(generate_regression_data):
     y, X, treatment, tau, b, e = generate_regression_data()
 
     pm = ElasticNetPropensityModel(random_state=RANDOM_SEED)
     ps = pm.fit_predict(X, treatment)
 
     assert roc_auc_score(treatment, ps) > .5
 
+
 def test_gradientboosted_propensity_model(generate_regression_data):
     y, X, treatment, tau, b, e = generate_regression_data()
 
     pm = GradientBoostedPropensityModel(random_state=RANDOM_SEED)
     ps = pm.fit_predict(X, treatment)
 
     assert roc_auc_score(treatment, ps) > .5
 
+
 def test_gradientboosted_propensity_model_earlystopping(generate_regression_data):
     y, X, treatment, tau, b, e = generate_regression_data()
 
     pm = GradientBoostedPropensityModel(random_state=RANDOM_SEED, early_stop=True)
     ps = pm.fit_predict(X, treatment)
 
     assert roc_auc_score(treatment, ps) > .5
```

### Comparing `causalml-0.8.0/tests/test_sensitivity.py` & `causalml-0.9.0/tests/test_sensitivity.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,15 @@
 from causalml.dataset import synthetic_data
 from causalml.inference.meta import BaseXLearner
 from causalml.metrics.sensitivity import Sensitivity
 from causalml.metrics.sensitivity import SensitivityPlaceboTreatment, SensitivityRandomCause
 from causalml.metrics.sensitivity import SensitivityRandomReplace, SensitivitySelectionBias
 from causalml.metrics.sensitivity import one_sided, alignment, one_sided_att, alignment_att
 
-RANDOM_SEED = 42
-N_SAMPLE = 1000
-ERROR_THRESHOLD = .5
-NUM_FEATURES = 6
-
-TREATMENT_COL = 'treatment'
-SCORE_COL = 'score'
-GROUP_COL = 'group'
-OUTCOME_COL = 'outcome'
-
-CONTROL_NAME = 'control'
-TREATMENT_NAMES = [CONTROL_NAME, 'treatment1', 'treatment2', 'treatment3']
-CONVERSION = 'conversion'
+from .const import TREATMENT_COL, SCORE_COL, OUTCOME_COL, NUM_FEATURES
 
 
 def test_Sensitivity():
     y, X, treatment, tau, b, e = synthetic_data(mode=1, n=100000, p=NUM_FEATURES, sigma=1.0)
 
     # generate the dataset format for sensitivity analysis
     INFERENCE_FEATURES = ['feature_' + str(i) for i in range(NUM_FEATURES)]
```

### Comparing `causalml-0.8.0/tests/test_uplift_trees.py` & `causalml-0.9.0/tests/test_uplift_trees.py`

 * *Files identical despite different names*

### Comparing `causalml-0.8.0/tests/test_value_optimization.py` & `causalml-0.9.0/tests/test_value_optimization.py`

 * *Files identical despite different names*

