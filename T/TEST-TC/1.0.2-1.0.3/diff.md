# Comparing `tmp/TEST_TC-1.0.2.tar.gz` & `tmp/TEST_TC-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-1.0.2.tar", last modified: Thu Jul  6 16:33:17 2023, max compression
+gzip compressed data, was "TEST_TC-1.0.3.tar", last modified: Mon Jul 10 10:37:46 2023, max compression
```

## Comparing `TEST_TC-1.0.2.tar` & `TEST_TC-1.0.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-06 16:33:17.352578 TEST_TC-1.0.2/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-06 16:33:17.120307 TEST_TC-1.0.2/LIB_tc/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-06 16:33:17.170168 TEST_TC-1.0.2/LIB_tc/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-06 16:33:17.000000 TEST_TC-1.0.2/LIB_tc/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1556 2023-07-06 16:33:17.000000 TEST_TC-1.0.2/LIB_tc/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-06 16:33:17.000000 TEST_TC-1.0.2/LIB_tc/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      198 2023-07-06 16:33:17.000000 TEST_TC-1.0.2/LIB_tc/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-06 16:33:17.000000 TEST_TC-1.0.2/LIB_tc/TEST_TC.egg-info/top_level.txt
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-06 16:33:17.173673 TEST_TC-1.0.2/LIB_tc/test_tc/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-06 16:25:42.000000 TEST_TC-1.0.2/LIB_tc/test_tc/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-06 16:33:17.195618 TEST_TC-1.0.2/LIB_tc/test_tc/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-1.0.2/LIB_tc/test_tc/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5672 2023-07-06 15:55:17.000000 TEST_TC-1.0.2/LIB_tc/test_tc/algorithms/algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14234 2023-07-06 15:55:17.000000 TEST_TC-1.0.2/LIB_tc/test_tc/algorithms/experiment_model.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15589 2023-07-06 15:55:17.000000 TEST_TC-1.0.2/LIB_tc/test_tc/algorithms/prophet_utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-06 16:33:17.205585 TEST_TC-1.0.2/LIB_tc/test_tc/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-1.0.2/LIB_tc/test_tc/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4304 2023-07-06 15:55:17.000000 TEST_TC-1.0.2/LIB_tc/test_tc/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-06 16:33:17.219044 TEST_TC-1.0.2/LIB_tc/test_tc/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-1.0.2/LIB_tc/test_tc/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7301 2023-07-06 15:55:17.000000 TEST_TC-1.0.2/LIB_tc/test_tc/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-06 16:33:17.234990 TEST_TC-1.0.2/LIB_tc/test_tc/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-1.0.2/LIB_tc/test_tc/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    13243 2023-07-06 15:55:17.000000 TEST_TC-1.0.2/LIB_tc/test_tc/datapreparation/datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3627 2023-07-06 15:55:17.000000 TEST_TC-1.0.2/LIB_tc/test_tc/datapreparation/prep.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-06 16:33:17.240487 TEST_TC-1.0.2/LIB_tc/test_tc/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-1.0.2/LIB_tc/test_tc/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-06 16:33:17.266432 TEST_TC-1.0.2/LIB_tc/test_tc/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-1.0.2/LIB_tc/test_tc/datavisualization/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     8228 2023-07-06 15:55:17.000000 TEST_TC-1.0.2/LIB_tc/test_tc/datavisualization/plotPrediction.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14733 2023-07-06 15:55:17.000000 TEST_TC-1.0.2/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    11197 2023-07-06 15:55:17.000000 TEST_TC-1.0.2/LIB_tc/test_tc/datavisualization/visualization.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-06 16:33:17.297366 TEST_TC-1.0.2/LIB_tc/test_tc/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-1.0.2/LIB_tc/test_tc/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-07-04 08:52:33.000000 TEST_TC-1.0.2/LIB_tc/test_tc/utility/constants.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-07-04 08:52:33.000000 TEST_TC-1.0.2/LIB_tc/test_tc/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2731 2023-07-06 15:55:17.000000 TEST_TC-1.0.2/LIB_tc/test_tc/utility/experiment_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2038 2023-06-27 17:28:54.000000 TEST_TC-1.0.2/LIB_tc/test_tc/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6293 2023-06-28 21:02:59.000000 TEST_TC-1.0.2/LIB_tc/test_tc/utility/tele_logger.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-06 16:33:17.351580 TEST_TC-1.0.2/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.0.2/README.md
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1130 2023-07-06 16:31:28.000000 TEST_TC-1.0.2/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-06 16:33:17.353574 TEST_TC-1.0.2/setup.cfg
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-06 16:33:17.347106 TEST_TC-1.0.2/tests/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-06-27 17:28:54.000000 TEST_TC-1.0.2/tests/test_algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3411 2023-06-27 17:28:54.000000 TEST_TC-1.0.2/tests/test_datahandler.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    11110 2023-07-04 08:52:34.000000 TEST_TC-1.0.2/tests/test_datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2688 2023-07-04 08:52:34.000000 TEST_TC-1.0.2/tests/test_evaluations.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-06-27 17:28:54.000000 TEST_TC-1.0.2/tests/test_exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4438 2023-07-04 08:52:34.000000 TEST_TC-1.0.2/tests/test_experiment_job.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4045 2023-07-04 08:52:34.000000 TEST_TC-1.0.2/tests/test_experiment_models.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2086 2023-07-04 08:52:34.000000 TEST_TC-1.0.2/tests/test_experiment_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2977 2023-07-04 08:52:34.000000 TEST_TC-1.0.2/tests/test_prep.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-06-27 17:28:54.000000 TEST_TC-1.0.2/tests/test_prophet_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2116 2023-06-28 16:32:49.000000 TEST_TC-1.0.2/tests/test_resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3089 2023-06-27 17:28:54.000000 TEST_TC-1.0.2/tests/test_tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 10:37:46.674176 TEST_TC-1.0.3/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 10:37:46.481521 TEST_TC-1.0.3/LIB_tc/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 10:37:46.529603 TEST_TC-1.0.3/LIB_tc/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-10 10:37:46.000000 TEST_TC-1.0.3/LIB_tc/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1556 2023-07-10 10:37:46.000000 TEST_TC-1.0.3/LIB_tc/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-10 10:37:46.000000 TEST_TC-1.0.3/LIB_tc/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      213 2023-07-10 10:37:46.000000 TEST_TC-1.0.3/LIB_tc/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-10 10:37:46.000000 TEST_TC-1.0.3/LIB_tc/TEST_TC.egg-info/top_level.txt
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 10:37:46.532604 TEST_TC-1.0.3/LIB_tc/test_tc/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-10 10:34:00.000000 TEST_TC-1.0.3/LIB_tc/test_tc/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 10:37:46.549714 TEST_TC-1.0.3/LIB_tc/test_tc/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5672 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/algorithms/algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14234 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/algorithms/experiment_model.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15589 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/algorithms/prophet_utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 10:37:46.557714 TEST_TC-1.0.3/LIB_tc/test_tc/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4304 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 10:37:46.565836 TEST_TC-1.0.3/LIB_tc/test_tc/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7301 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 10:37:46.579742 TEST_TC-1.0.3/LIB_tc/test_tc/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    13243 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/datapreparation/datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3627 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/datapreparation/prep.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 10:37:46.583740 TEST_TC-1.0.3/LIB_tc/test_tc/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 10:37:46.600770 TEST_TC-1.0.3/LIB_tc/test_tc/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/datavisualization/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     8228 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/datavisualization/plotPrediction.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15046 2023-07-10 10:36:28.000000 TEST_TC-1.0.3/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14591 2023-07-10 10:36:42.000000 TEST_TC-1.0.3/LIB_tc/test_tc/datavisualization/visualization.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 10:37:46.623359 TEST_TC-1.0.3/LIB_tc/test_tc/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/utility/constants.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2717 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/utility/experiment_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2038 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6293 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/LIB_tc/test_tc/utility/tele_logger.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-10 10:37:46.672164 TEST_TC-1.0.3/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.0.3/README.md
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1148 2023-07-10 10:31:23.000000 TEST_TC-1.0.3/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-10 10:37:46.674176 TEST_TC-1.0.3/setup.cfg
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 10:37:46.667154 TEST_TC-1.0.3/tests/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-06-27 17:28:54.000000 TEST_TC-1.0.3/tests/test_algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3411 2023-06-27 17:28:54.000000 TEST_TC-1.0.3/tests/test_datahandler.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    11110 2023-07-04 08:52:34.000000 TEST_TC-1.0.3/tests/test_datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2688 2023-07-04 08:52:34.000000 TEST_TC-1.0.3/tests/test_evaluations.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-06-27 17:28:54.000000 TEST_TC-1.0.3/tests/test_exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4438 2023-07-04 08:52:34.000000 TEST_TC-1.0.3/tests/test_experiment_job.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4045 2023-07-04 08:52:34.000000 TEST_TC-1.0.3/tests/test_experiment_models.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2086 2023-07-04 08:52:34.000000 TEST_TC-1.0.3/tests/test_experiment_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2977 2023-07-04 08:52:34.000000 TEST_TC-1.0.3/tests/test_prep.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-06-27 17:28:54.000000 TEST_TC-1.0.3/tests/test_prophet_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2116 2023-06-28 16:32:49.000000 TEST_TC-1.0.3/tests/test_resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3089 2023-06-27 17:28:54.000000 TEST_TC-1.0.3/tests/test_tele_logger.py
```

### Comparing `TEST_TC-1.0.2/LIB_tc/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-1.0.3/LIB_tc/TEST_TC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/algorithms/algorithm.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/algorithms/experiment_model.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/algorithms/experiment_model.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/algorithms/prophet_utils.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/algorithms/prophet_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/analytics/evaluationMetrics.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/analytics/evaluationMetrics.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/datahandler/datahandler.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/datahandler/datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/datapreparation/datapreparation_utils.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/datapreparation/datapreparation_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/datapreparation/prep.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/datapreparation/prep.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/datavisualization/plotPrediction.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/datavisualization/plotPrediction.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py`

 * *Files 3% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 
         Returns
         -------
         str
             result of test
         """
 
-        df = df.dropna()
+        df = self.df.dropna()
 
         time_series = df[self.target]
         time_series.index = df[self.data]
 
         dftest = adfuller(time_series, autolag="AIC")
         dfoutput = pd.Series(dftest[0:3], index=["Test Statistic", "p-value", "#Lags Used"])
         DF = dfoutput["p-value"] < 0.05
@@ -274,46 +274,51 @@
         Returns
         -------
         tuple
             tuple that containing figure for autocorrelation and partial autocorrelation
 
         """
 
-        autocorr = acf(self.df.dropna()[self.target], nlags=n_lags)
+        trend = self.additive_decomposition()[0]
+        time_series = self.df[self.target] - trend
+
+        autocorr = acf(time_series.dropna(), nlags=n_lags)[1:]
         fig1 = px.bar(
-            autocorr,
-            labels={"index": "Lag"},
+            x=np.arange(autocorr.shape[0]) + 1,
+            y=autocorr,
+            labels={"x": "Lag", "y": "Autocorrelazione"},
             title="Autocorrelazione",
             template=dict(
                 layout=go.Layout(
                     title_font=dict(family="Rockwell", size=24, color="red"),
                     font=dict(color="green"),
                 )
             ),
         )
         fig1.update_layout(showlegend=False)
 
-        p_autocorr = pacf(self.df.dropna()[self.target], nlags=n_lags)
-        fig2 = px.bar(
-            p_autocorr,
-            labels={"index": "Lag"},
-            title="Autocorrelazione parziale",
-            template=dict(
-                layout=go.Layout(
-                    title_font=dict(family="Rockwell", size=24, color="red"),
-                    font=dict(color="green"),
-                )
-            ),
-        )
-        fig2.update_layout(showlegend=False)
+        # p_autocorr = pacf(time_series.dropna(), nlags=n_lags)[1:]
+        # fig2 = px.bar(
+        #     x=np.arange(p_autocorr.shape[0]) + 1,
+        #     y=p_autocorr,
+        #     labels={"x": "Lag", "y": "Autocorrelazione"},
+        #     title="Autocorrelazione parziale",
+        #     template=dict(
+        #         layout=go.Layout(
+        #             title_font=dict(family="Rockwell", size=24, color="red"),
+        #             font=dict(color="green"),
+        #         )
+        #     ),
+        # )
+        # fig2.update_layout(showlegend=False)
 
         # fig1.show()
         # fig2.show()
 
-        return (fig1, fig2)
+        return [fig1]
 
     # Decomposizione Additiva (Trend + Seasonality + Residual)
     def additive_decomposition(self) -> tuple:
 
         """Compute and plot additive decompostion
 
         Parameters
@@ -326,18 +331,19 @@
         """
         df = self.df.dropna()
 
         df = pd.DataFrame({'ds': df[self.data], 'y': df[self.target]})
         m = Prophet()
         m.fit(df)
         future_df = m.make_future_dataframe(periods=0)
-        forecast = m.predict(future_df)
+        forecast = m.predict(df[["ds"]])
 
         fig = plot_components_plotly(m, forecast)
 
+        forecast = forecast.set_index("ds")
         return (forecast["trend"], forecast["weekly"], fig)
 
     def boxplots_seasons(self) -> plt.figure:
         
         """Creates a boxplot showing weekday-season effects
 
         Parameters
```

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/datavisualization/visualization.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/datavisualization/visualization.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from __future__ import annotations
 
+import itertools
+
 import numpy as np
 import pandas as pd
 import geopandas as gpd
 
+from scipy.cluster.hierarchy import dendrogram, linkage
+from scipy.spatial.distance import squareform
+
+import matplotlib.pyplot as plt
 from dtaidistance import dtw
 from dtaidistance import dtw_visualisation as dtwvis
 
 import matplotlib.pyplot as plt
 import plotly
 import plotly.express as px
 import plotly.graph_objects as go
@@ -187,15 +193,15 @@
             template=dict(
                 layout=go.Layout(
                     title_font=dict(family="Rockwell", size=24, color="red"),
                     font=dict(color="green"),
                 )
             ),
         )
-        # fig.show()
+        fig.update_traces(textinfo="label+percent parent")
 
         return fig
 
     def boxplot(self, df: pd.DataFrame, variable: str):
         
         """Boxplot of aggregated data
 
@@ -222,44 +228,47 @@
                     font=dict(color="green"),
                 )
             ),
         )
 
         return fig
 
-    def DTW(self, df: pd.DataFrame, column: str, val1: str, val2: str):
+    def DTW(self, df: pd.DataFrame, column: str, data: str, val1: str, val2: str) -> tuple:
 
         """compute distance between two time series
 
         Parameters
         ----------
         df : pd.DataFrame
             dataframe result of conteggi function
         column : str
             name of one column aggregate on
+        data : str
+            name of data column
         val1: str
             name of column modality
         val2 : str
             name of column modality
 
         Returns
         -------
         tuple
             tuple containing a figure that representing distance between time series and the value of distance
 
         """
 
-        x = df[df[column] == val1][self.target].values
-        y = df[df[column] == val2][self.target].values
+        df_sort = df.sort_values(data)
+        x = df_sort[df_sort[column] == val1][self.target].values
+        y = df_sort[df_sort[column] == val2][self.target].values       
 
         # Normalize time series
         x = x / x.max()
         y = y / y.max()
 
-        distance = dtw.distance(x, y, use_pruning=True)
+        distance = dtw.distance_fast(x, y, use_pruning=True)
         path = dtw.warping_path(x, y)
 
         fig, ax = plt.subplots(2, 1, figsize=(20, 9))
         dtwvis.plot_warping(x, y, path, fig=fig, axs=ax)
 
         ax[0].set_title(
             f"Dynamic Time Warping, {column} ({val1}-{val2})",
@@ -274,14 +283,89 @@
         ax[1].set_ylabel(self.target, fontsize=12)
         fig.tight_layout()
 
         normalized_distance = distance / np.sqrt(len(x) * len(y))
 
         return (fig, normalized_distance)
     
+    def DTW_distance_matrix(self, df: pd.DataFrame, column: str, data: str) -> tuple:
+
+        """computes DTW distance matrix of all sub time series of a column
+
+        Parameters
+        ----------
+        df : pd.DataFrame
+            dataframe result of conteggi function
+        column : str
+            name of one column aggregate on
+        data : str
+            name of data column
+
+        Returns
+        -------
+        tuple
+            tuple containing the matrix and the plot of matrix
+        """
+
+        df_sort = df.sort_values(data)
+
+        lista = [(df_sort[df_sort[column] == i][self.target].values.astype(np.double),i)
+         for i in df_sort[column].unique()]
+
+        lista_time_series = [i[0]/i[0].max() for i in lista]
+        len_time_series = [len(i[0]) for i in lista]
+        len_matrix_time_series = np.array([i[0]*i[1] for i in itertools.product([len(i[0]) for i in len_time_series],repeat=2)])
+        len_matrix_time_series.shape = (21,21)
+        distance_matrix = dtw.distance_matrix_fast(lista_time_series)
+        
+        distance_matrix_normalized = distance_matrix / len_matrix_time_series
+
+        fig = px.imshow(distance_matrix_normalized, text_auto=True, template=dict(
+                layout=go.Layout(
+                    title_font=dict(family="Rockwell", size=24, color="grey"),
+                    font=dict(color="green"),
+                width=800,
+                height=700,
+                title=f"Distance matrix ({column})",
+                )))
+
+        fig.update_layout(
+            xaxis = dict(
+                tickmode = 'array',
+                tickvals = [i for i in range(21)],
+                ticktext = [i[1] for i in lista],tickfont=dict(family='Rockwell', color='green', size=10)
+            ),
+            yaxis = dict(
+                tickmode = 'array',
+                tickvals = [i for i in range(21)],
+                ticktext = [i[1] for i in lista],tickangle=-45,tickfont=dict(family='Rockwell', color='green', size=10)
+            )           
+        )
+
+        return (fig,distance_matrix_normalized)
+
+    def plot_distance_matrix(self, distance_matrix: np.ndarray):
+        
+        dists = squareform(distance_matrix)
+        linkage_matrix = linkage(dists, "ward",optimal_ordering=0)
+        
+        dendr = plt.figure(figsize=(10,6))
+        dendrogram(linkage_matrix, labels=[i[1] for i in lista],leaf_rotation=0,orientation="right")
+        plt.title("DTW distance - dendrogramm")
+        plt.tick_params(
+            axis='x',          # changes apply to the x-axis
+            which='both',      # both major and minor ticks are affected
+            bottom=False,      # ticks along the bottom edge are off
+            top=False,         # ticks along the top edge are off
+            labelbottom=False) # labels along the bottom edge are off
+        for pos in ['right', 'top', 'bottom', 'left']:
+            plt.gca().spines[pos].set_visible(False)
+        
+        return dendr
+
     def add_geographical_info(
         self, target: str, region: str, df_geo: gpd.GeoDataFrame, region_geo: str
     ) -> gpd.GeoDataFrame:
         
         """Aggregates df on "spatial_variable" and joins with the "regions" geodataframe on "join_variable"
 
         Parameters
```

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/utility/constants.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/utility/constants.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/utility/exceptions.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/utility/experiment_utils.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/utility/experiment_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pandas as pd
 
-from tc_uc4.utility.constants import code_to_region_name, code_to_speciality
+from .constants import code_to_region_name, code_to_speciality
 
 
 def add_mapped_columns(
     hierarchy: dict[str, str], df: pd.DataFrame, conversion: dict[str, str]
 ) -> tuple[pd.DataFrame, dict[str, str]]:
     """Adds columns in the dataframe "df" according to a given hierarchy and conversion dictionary.
```

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/utility/resources.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/utility/resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/LIB_tc/test_tc/utility/tele_logger.py` & `TEST_TC-1.0.3/LIB_tc/test_tc/utility/tele_logger.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/README.md` & `TEST_TC-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/pyproject.toml` & `TEST_TC-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 [project] 
 name = "TEST_TC"
 authors = [{name = "Skienda", email= "f.ischiboni@skienda.it"}]
 description = "Lo scopo di questa libreria è fornire uno strumento completo per il rilascio di modelli predittivi basati su serie temporali nell'ambito della Telemedicina, al fine di supportare la gestione e la pianificazione delle attività sulla Piattaforma Nazionale di Telemedicina (PNT)"
 requires-python = ">=3.9"
 classifiers = [ "Programming Language :: Python :: 3"]
-dependencies = ["geopandas==0.13.0","holidays==0.24","numpy==1.25.0","pandas==2.0.2","prophet==1.1.1",
+dependencies = ["geopandas==0.13.0","holidays==0.24","numpy==1.23.5","pandas==2.0.2","prophet==1.1.1",
                 "scikit_learn==1.2.2","tabulate==0.9.0","tomli==2.0.1","typing_extensions==4.6.3", "pytest==7.3.1",
-                "mlflow==2.4.0", "statsmodels==0.14.0"]
+                "mlflow==2.4.0", "statsmodels==0.14.0", "holidays==0.24"]
 dynamic = ["version"]
 
 [tool.setuptools.packages.find]
 where = ["./LIB_tc/"]
 include = ["*"] # or define list of packages
 exclude = []
 namespaces = false
```

### Comparing `TEST_TC-1.0.2/tests/test_algorithm.py` & `TEST_TC-1.0.3/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/tests/test_datahandler.py` & `TEST_TC-1.0.3/tests/test_datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/tests/test_datapreparation_utils.py` & `TEST_TC-1.0.3/tests/test_datapreparation_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/tests/test_evaluations.py` & `TEST_TC-1.0.3/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/tests/test_exceptions.py` & `TEST_TC-1.0.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/tests/test_experiment_job.py` & `TEST_TC-1.0.3/tests/test_experiment_job.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/tests/test_experiment_models.py` & `TEST_TC-1.0.3/tests/test_experiment_models.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/tests/test_experiment_utils.py` & `TEST_TC-1.0.3/tests/test_experiment_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/tests/test_prep.py` & `TEST_TC-1.0.3/tests/test_prep.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/tests/test_prophet_utils.py` & `TEST_TC-1.0.3/tests/test_prophet_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/tests/test_resources.py` & `TEST_TC-1.0.3/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.2/tests/test_tele_logger.py` & `TEST_TC-1.0.3/tests/test_tele_logger.py`

 * *Files identical despite different names*

