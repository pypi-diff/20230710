# Comparing `tmp/FLAML-2.0.0rc2.tar.gz` & `tmp/FLAML-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAML-2.0.0rc2.tar", last modified: Mon Jun 26 17:08:09 2023, max compression
+gzip compressed data, was "FLAML-2.0.0rc3.tar", last modified: Mon Jul 10 21:08:47 2023, max compression
```

## Comparing `FLAML-2.0.0rc2.tar` & `FLAML-2.0.0rc3.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.751581 FLAML-2.0.0rc2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.731581 FLAML-2.0.0rc2/FLAML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-06-26 17:08:09.000000 FLAML-2.0.0rc2/FLAML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-26 17:08:09.000000 FLAML-2.0.0rc2/FLAML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:08:09.000000 FLAML-2.0.0rc2/FLAML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-26 17:08:09.000000 FLAML-2.0.0rc2/FLAML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 17:08:09.000000 FLAML-2.0.0rc2/FLAML.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-06-26 17:08:09.751581 FLAML-2.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.735581 FLAML-2.0.0rc2/flaml/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.735581 FLAML-2.0.0rc2/flaml/autogen/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.735581 FLAML-2.0.0rc2/flaml/autogen/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/agent/assistant_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/agent/math_user_proxy_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/agent/user_proxy_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    18621 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/code_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.735581 FLAML-2.0.0rc2/flaml/autogen/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.735581 FLAML-2.0.0rc2/flaml/autogen/oai/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/oai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47084 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/oai/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/autogen/oai/openai_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.735581 FLAML-2.0.0rc2/flaml/automl/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   130405 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/automl.py
--rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20891 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    78597 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.739581 FLAML-2.0.0rc2/flaml/automl/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.739581 FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/data_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/training_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/nlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.739581 FLAML-2.0.0rc2/flaml/automl/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/spark/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/spark/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9829 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.739581 FLAML-2.0.0rc2/flaml/automl/task/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/task/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    39625 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/task/generic_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13702 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/task/time_series_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.739581 FLAML-2.0.0rc2/flaml/automl/time_series/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/time_series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/time_series/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/time_series/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/time_series/tft.py
--rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/time_series/ts_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    26508 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/time_series/ts_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/automl/training_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/all/
--rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/all/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/all/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/all/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/extra_tree/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/extra_tree/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/extra_tree/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/extra_tree/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/greedy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/lgbm/
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/lgbm/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/lgbm/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/lgbm/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/regret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/rf/
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/rf/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/rf/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/rf/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/suggest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.743581 FLAML-2.0.0rc2/flaml/default/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/xgboost/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/xgboost/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/default/xgboost/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.747581 FLAML-2.0.0rc2/flaml/onlineml/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/onlineml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/onlineml/autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/onlineml/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/onlineml/trial_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.747581 FLAML-2.0.0rc2/flaml/tune/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.747581 FLAML-2.0.0rc2/flaml/tune/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/scheduler/online_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/scheduler/trial_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.747581 FLAML-2.0.0rc2/flaml/tune/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50288 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/blendsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/cfo_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    30648 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/flow2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/online_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/search_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/searcher/variant_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23100 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.751581 FLAML-2.0.0rc2/flaml/tune/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/trial_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    40082 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/tune.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/tune/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/flaml/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:08:09.751581 FLAML-2.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:08:09.751581 FLAML-2.0.0rc2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/test/test_autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/test/test_conda_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/test/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 17:07:14.000000 FLAML-2.0.0rc2/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.412591 FLAML-2.0.0rc3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.396591 FLAML-2.0.0rc3/FLAML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-07-10 21:08:47.000000 FLAML-2.0.0rc3/FLAML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-10 21:08:47.000000 FLAML-2.0.0rc3/FLAML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:08:47.000000 FLAML-2.0.0rc3/FLAML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-10 21:08:47.000000 FLAML-2.0.0rc3/FLAML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 21:08:47.000000 FLAML-2.0.0rc3/FLAML.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-07-10 21:08:47.412591 FLAML-2.0.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.396591 FLAML-2.0.0rc3/flaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.396591 FLAML-2.0.0rc3/flaml/autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/autogen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.396591 FLAML-2.0.0rc3/flaml/autogen/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/autogen/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/autogen/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/autogen/agent/assistant_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/autogen/agent/math_user_proxy_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11587 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/autogen/agent/user_proxy_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/autogen/code_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.396591 FLAML-2.0.0rc3/flaml/autogen/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/autogen/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/autogen/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.400591 FLAML-2.0.0rc3/flaml/autogen/oai/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/autogen/oai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47161 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/autogen/oai/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/autogen/oai/openai_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.400591 FLAML-2.0.0rc3/flaml/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130405 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20891 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78809 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.400591 FLAML-2.0.0rc3/flaml/automl/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.400591 FLAML-2.0.0rc3/flaml/automl/nlp/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/nlp/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/nlp/huggingface/data_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/nlp/huggingface/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/nlp/huggingface/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/nlp/huggingface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.400591 FLAML-2.0.0rc3/flaml/automl/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/spark/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/spark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9829 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.400591 FLAML-2.0.0rc3/flaml/automl/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/task/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39625 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/task/generic_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13702 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/task/time_series_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.404591 FLAML-2.0.0rc3/flaml/automl/time_series/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/time_series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/time_series/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/time_series/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/time_series/tft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/time_series/ts_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26508 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/time_series/ts_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/automl/training_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.404591 FLAML-2.0.0rc3/flaml/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.404591 FLAML-2.0.0rc3/flaml/default/all/
+-rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/all/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/all/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/all/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.404591 FLAML-2.0.0rc3/flaml/default/extra_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/extra_tree/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/extra_tree/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/extra_tree/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/greedy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.404591 FLAML-2.0.0rc3/flaml/default/lgbm/
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/lgbm/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/lgbm/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/lgbm/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/regret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.404591 FLAML-2.0.0rc3/flaml/default/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/rf/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/rf/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/rf/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/suggest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.404591 FLAML-2.0.0rc3/flaml/default/xgb_limitdepth/
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/xgb_limitdepth/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/xgb_limitdepth/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/xgb_limitdepth/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.404591 FLAML-2.0.0rc3/flaml/default/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/xgboost/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/xgboost/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/default/xgboost/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.404591 FLAML-2.0.0rc3/flaml/onlineml/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/onlineml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/onlineml/autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/onlineml/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/onlineml/trial_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.408591 FLAML-2.0.0rc3/flaml/tune/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.408591 FLAML-2.0.0rc3/flaml/tune/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/scheduler/online_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/scheduler/trial_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.408591 FLAML-2.0.0rc3/flaml/tune/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50288 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/searcher/blendsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/searcher/cfo_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30648 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/searcher/flow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/searcher/online_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/searcher/search_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35462 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/searcher/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/searcher/variant_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23100 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.408591 FLAML-2.0.0rc3/flaml/tune/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/trial_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42131 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/tune/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/flaml/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:08:47.412591 FLAML-2.0.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:08:47.412591 FLAML-2.0.0rc3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/test/test_autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/test/test_conda_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/test/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-10 21:07:16.000000 FLAML-2.0.0rc3/test/test_version.py
```

### Comparing `FLAML-2.0.0rc2/FLAML.egg-info/PKG-INFO` & `FLAML-2.0.0rc3/FLAML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FLAML-2.0.0rc2/FLAML.egg-info/SOURCES.txt` & `FLAML-2.0.0rc3/FLAML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/FLAML.egg-info/requires.txt` & `FLAML-2.0.0rc3/FLAML.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 catboost>=0.26
 psutil==5.8.0
 xgboost==1.3.3
 pandas==1.1.4
 
 [blendsearch]
 optuna==2.8.0
+packaging
 
 [catboost]
 catboost>=0.26
 
 [forecast]
 holidays<0.14
 prophet>=1.0.1
@@ -49,15 +50,15 @@
 seqeval
 
 [mathchat]
 openai==0.27.8
 diskcache
 docker
 sympy
-pydantic
+pydantic==1.10.9
 wolframalpha
 
 [nlp]
 transformers[torch]==4.26
 datasets
 nltk
 rouge_score
@@ -75,19 +76,21 @@
 
 [ray]
 ray[tune]~=1.13
 
 [spark]
 pyspark>=3.2.0
 joblibspark>=0.5.0
+joblib<1.3.0
 
 [synapse]
 joblibspark>=0.5.0
 optuna==2.8.0
 pyspark>=3.2.0
+joblib<1.3.0
 
 [test]
 lightgbm>=2.3.1
 xgboost>=0.90
 scipy>=1.4.1
 pandas>=1.1.4
 scikit-learn>=0.24
@@ -117,17 +120,18 @@
 nbconvert
 nbformat
 ipykernel
 pytorch-lightning<1.9.1
 tensorboardX==2.6
 requests<2.29.0
 packaging
-pydantic
+pydantic==1.10.9
 sympy
 wolframalpha
+joblib<1.3.0
 
 [ts_forecast]
 holidays<0.14
 prophet>=1.0.1
 statsmodels>=0.12.2
 hcrystalball==0.1.10
```

### Comparing `FLAML-2.0.0rc2/LICENSE` & `FLAML-2.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/NOTICE.md` & `FLAML-2.0.0rc3/NOTICE.md`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/PKG-INFO` & `FLAML-2.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FLAML-2.0.0rc2/README.md` & `FLAML-2.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/autogen/agent/assistant_agent.py` & `FLAML-2.0.0rc3/flaml/autogen/agent/assistant_agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from .agent import Agent
 from flaml.autogen.code_utils import DEFAULT_MODEL
 from flaml import oai
+from typing import Dict, Union
 
 
 class AssistantAgent(Agent):
     """(Experimental) Assistant agent, able to suggest code blocks."""
 
     DEFAULT_SYSTEM_MESSAGE = """You are a helpful AI assistant.
-    In the following cases, suggest python code (in a python coding block) or shell script (in a sh coding block) for the user to execute. You must indicate the script type in the code block.
+    In the following cases, suggest python code (in a python coding block) or shell script (in a sh coding block) for the user to execute. You must indicate the script type in the code block. The user cannot provide any other feedback or perform any other action beyond executing the code you suggest. The user can't modify your code.
     1. When you need to ask the user for some info, use the code to output the info you need, for example, browse or search the web, download/read a file.
     2. When you need to perform some task with code, use the code to perform the task and output the result. Finish the task smartly. Solve the task step by step if you need to.
     If you want the user to save the code in a file before executing it, put # filename: <filename> inside the code block as the first line. Don't include multiple code blocks in one response. Do not ask users to copy and paste the result. Instead, use 'print' function for the output when relevant. Check the execution result returned by the user.
-    If the result indicates there is an error, fix the error and output the code again. Suggeset the full code instead of partial code or code changes.
+    If the result indicates there is an error, fix the error and output the code again. Suggest the full code instead of partial code or code changes.
+    Verify your answer carefully. If a function for planning is provided, call the function to make plans and verify the execution.
     Reply "TERMINATE" in the end when everything is done.
     """
 
     DEFAULT_CONFIG = {
         "model": DEFAULT_MODEL,
     }
 
@@ -29,20 +31,19 @@
               These configurations will be used when invoking LLM.
         """
         super().__init__(name, system_message)
         self._config = self.DEFAULT_CONFIG.copy()
         self._config.update(config)
         self._sender_dict = {}
 
-    def receive(self, message, sender):
+    def receive(self, message: Union[Dict, str], sender):
         if sender.name not in self._sender_dict:
             self._sender_dict[sender.name] = sender
-            self._conversations[sender.name] = [{"content": self._system_message, "role": "system"}]
+            self._oai_conversations[sender.name] = [{"content": self._system_message, "role": "system"}]
+
         super().receive(message, sender)
-        responses = oai.ChatCompletion.create(messages=self._conversations[sender.name], **self._config)
-        # TODO: handle function_call
-        response = oai.ChatCompletion.extract_text(responses)[0]
-        self._send(response, sender)
+        responses = oai.ChatCompletion.create(messages=self._oai_conversations[sender.name], **self._config)
+        self._send(oai.ChatCompletion.extract_text_or_function_call(responses)[0], sender)
 
     def reset(self):
         self._sender_dict.clear()
-        self._conversations.clear()
+        self._oai_conversations.clear()
```

### Comparing `FLAML-2.0.0rc2/flaml/autogen/agent/math_user_proxy_agent.py` & `FLAML-2.0.0rc3/flaml/autogen/agent/math_user_proxy_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,18 @@
 
 Problem: """,
 }
 
 
 def is_termination_msg(x):
     """Check if a message is a termination message."""
+    if isinstance(x, dict):
+        x = x.get("content")
+        if x is None:
+            return False
     cb = extract_code(x)
     contain_code = False
     for c in cb:
         if c[0] == "python" or c[0] == "wolfram":
             contain_code = True
             break
     return not contain_code and get_answer(x) is not None and get_answer(x) != ""
@@ -125,14 +129,15 @@
     MAX_CONSECUTIVE_AUTO_REPLY = 15  # maximum number of consecutive auto replies (subject to future change)
 
     def __init__(
         self,
         name="MathChatAgent",  # default set to MathChatAgent
         system_message="",
         work_dir=None,
+        function_map=defaultdict(callable),
         human_input_mode="NEVER",  # Fully automated
         max_consecutive_auto_reply=None,
         is_termination_msg=is_termination_msg,
         use_docker=True,
         max_invalid_q_per_step=3,  # a parameter needed in MathChat
         **config,
     ):
@@ -146,27 +151,29 @@
                 (1) When "ALWAYS", the agent prompts for human input every time a message is received.
                     Under this mode, the conversation stops when the human input is "exit",
                     or when is_termination_msg is True and there is no human input.
                 (2) When "TERMINATE", the agent only prompts for human input only when a termination message is received or
                     the number of auto reply reaches the max_consecutive_auto_reply.
                 (3) When "NEVER", the agent will never prompt for human input. Under this mode, the conversation stops
                     when the number of auto reply reaches the max_consecutive_auto_reply or when is_termination_msg is True.
+            function_map (dict[str, callable]): Mapping function names (passed to openai) to callable functions.
             max_consecutive_auto_reply (int): the maximum number of consecutive auto replies.
                 default to None (no limit provided, class attribute MAX_CONSECUTIVE_AUTO_REPLY will be used as the limit in this case).
                 The limit only plays a role when human_input_mode is not "ALWAYS".
-            is_termination_msg (function): a function that takes a message and returns a boolean value.
-                This function is used to determine if a received message is a termination message.
+            is_termination_msg (function): a function that takes a message in the form of a dictionary and returns a boolean value indicating if this received message is a termination message.
+                The dict can contain the following keys: "content", "role", "name", "function_call".
             use_docker (bool): whether to use docker to execute the code.
             max_invalid_q_per_step (int): (ADDED) the maximum number of invalid queries per step.
             **config (dict): other configurations.
         """
         super().__init__(
             name=name,
             system_message=system_message,
             work_dir=work_dir,
+            function_map=function_map,
             human_input_mode=human_input_mode,
             max_consecutive_auto_reply=max_consecutive_auto_reply,
             is_termination_msg=is_termination_msg,
             use_docker=use_docker,
             **config,
         )
 
@@ -204,15 +211,15 @@
         self._reset()
         if customized_prompt is not None:
             return customized_prompt + problem
         else:
             return PROMPTS[prompt_type] + problem
 
     def _reset(self):
-        self._conversations.clear()
+        self._oai_conversations.clear()
         self._valid_q_count = 0
         self._total_q_count = 0
         self._accum_invalid_q_per_step = 0
         self._previous_code = ""
         self.last_reply = None
 
     def _execute_one_python_code(self, pycode):
@@ -284,14 +291,15 @@
         if output == "":
             output = "Error: The wolfram query is invalid."
             is_success = False
         return output, is_success
 
     def auto_reply(self, message, sender, default_reply=""):
         """Generate an auto reply."""
+        message = message.get("content", "")
         code_blocks = extract_code(message)
 
         if len(code_blocks) == 1 and code_blocks[0][0] == UNKNOWN:
             # no code block is found, lang should be `UNKNOWN``
             if default_reply == "":
                 default_reply = "Continue. Please keep solving the problem until you need to query. (If you get to the answer, put it in \\boxed{}.)"
             self._send(default_reply, sender)
@@ -387,15 +395,15 @@
     wolfram_alpha_appid: Optional[str] = None
 
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.forbid
 
-    @root_validator()
+    @root_validator(skip_on_failure=True)
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         wolfram_alpha_appid = get_from_dict_or_env(values, "wolfram_alpha_appid", "WOLFRAM_ALPHA_APPID")
         values["wolfram_alpha_appid"] = wolfram_alpha_appid
 
         try:
             import wolframalpha
```

### Comparing `FLAML-2.0.0rc2/flaml/autogen/code_utils.py` & `FLAML-2.0.0rc3/flaml/autogen/code_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from flaml.autogen import oai, DEFAULT_MODEL, FAST_MODEL
 
 # Regular expression for finding a code block
 CODE_BLOCK_PATTERN = r"```(\w*)\n(.*?)\n```"
 WORKING_DIR = os.path.join(os.path.dirname(os.path.realpath(__file__)), "extensions")
 UNKNOWN = "unknown"
 TIMEOUT_MSG = bytes("Timeout", "utf-8")
+DEFAULT_TIMEOUT = 600
 
 
 def infer_lang(code):
     """infer the language for the code.
     TODO: make it robust.
     """
     if code.startswith("python ") or code.startswith("pip"):
@@ -129,15 +130,15 @@
     if lang == "shell":
         return "sh"
     raise NotImplementedError(f"{lang} not recognized in code execution")
 
 
 def execute_code(
     code: Optional[str] = None,
-    timeout: Optional[int] = 600,
+    timeout: Optional[int] = None,
     filename: Optional[str] = None,
     work_dir: Optional[str] = None,
     use_docker: Optional[Union[List[str], str, bool]] = True,
     lang: Optional[str] = "python",
 ) -> Tuple[int, bytes, str]:
     """Execute code in a docker container.
     This function is not tested on MacOS.
@@ -150,15 +151,15 @@
         filename (Optional, str): The file name to save the code or where the code is stored when `code` is None.
             If None, a file with a randomly generated name will be created.
             The randomly generated file will be deleted after execution.
             The file name must be a relative path. Relative paths are relative to the working directory.
         work_dir (Optional, str): The working directory for the code execution.
             If None, a default working directory will be used.
             The default working directory is the "extensions" directory under
-            "xxx/flaml/autogen", where "xxx" is the path to the flaml package.
+            "path_to_flaml/autogen".
         use_docker (Optional, list, str or bool): The docker image to use for code execution.
             If a list or a str of image name(s) is provided, the code will be executed in a docker container
               with the first image successfully pulled.
             If None, False or empty, the code will be executed in the current environment.
             Default is True, which will be converted into a list.
             If the code is executed in the current environment,
             the code must be trusted.
@@ -166,15 +167,15 @@
 
     Returns:
         int: 0 if the code executes successfully.
         bytes: The error message if the code fails to execute; the stdout otherwise.
         image: The docker image name after container run when docker is used.
     """
     assert code is not None or filename is not None, "Either code or filename must be provided."
-
+    timeout = timeout or DEFAULT_TIMEOUT
     original_filename = filename
     if filename is None:
         code_hash = md5(code.encode()).hexdigest()
         # create a file with a automatically generated name
         filename = f"tmp_code_{code_hash}.{'py' if lang.startswith('python') else lang}"
     if work_dir is None:
         work_dir = WORKING_DIR
```

### Comparing `FLAML-2.0.0rc2/flaml/autogen/math_utils.py` & `FLAML-2.0.0rc3/flaml/autogen/math_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     return results.get("voted_answer"), response["cost"]
 
 
 def remove_boxed(string: str) -> Optional[str]:
     """Source: https://github.com/hendrycks/math
     Extract the text within a \\boxed{...} environment.
     Example:
-    >>> remove_boxed(\\boxed{\\frac{2}{3}})
+
+    >> remove_boxed("\\boxed{\\frac{2}{3}}")
+
     \\frac{2}{3}
     """
     left = "\\boxed{"
     try:
         assert string[: len(left)] == left
         assert string[-1] == "}"
         return string[len(left) : -1]
```

### Comparing `FLAML-2.0.0rc2/flaml/autogen/oai/completion.py` & `FLAML-2.0.0rc3/flaml/autogen/oai/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -735,15 +735,15 @@
             return context.get("yes_or_no_choice", False) is False or any(
                 text in ["Yes.", "No."] for text in oai.Completion.extract_text(response)
             )
         ```
 
             raise_error (bool, Optional): Whether to raise error when all configs fail.
                 When set to False, -1 will be returned when all configs fail.
-            **config: Configuration for the completion.
+            **config: Configuration for the openai API call. This is used as parameters for calling openai API.
                 Besides the parameters for the openai API call, it can also contain a seed (int) for the cache.
                 This is useful when implementing "controlled randomness" for the completion.
                 Also, the "prompt" or "messages" parameter can contain a template (str or Callable) which will be instantiated with the context.
 
         Returns:
             Responses from OpenAI API.
         """
@@ -765,15 +765,15 @@
                     )
                     if pass_filter or i == last:
                         response["cost"] = cost + response["cost"]
                         response["config_id"] = i
                         response["pass_filter"] = pass_filter
                         return response
                     cost += response["cost"]
-                except (AuthenticationError, RateLimitError, Timeout):
+                except (AuthenticationError, RateLimitError, Timeout, InvalidRequestError):
                     logger.debug(f"failed with config {i}", exc_info=1)
                     if i == last:
                         raise
                 finally:
                     cls.retry_timeout = retry_timeout
         params = cls._construct_params(context, config)
         if not use_cache:
```

### Comparing `FLAML-2.0.0rc2/flaml/autogen/oai/openai_utils.py` & `FLAML-2.0.0rc3/flaml/autogen/oai/openai_utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/automl.py` & `FLAML-2.0.0rc3/flaml/automl/automl.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/data.py` & `FLAML-2.0.0rc3/flaml/automl/data.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/ml.py` & `FLAML-2.0.0rc3/flaml/automl/ml.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/model.py` & `FLAML-2.0.0rc3/flaml/automl/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,23 +404,27 @@
         self.df_train = None
 
     def _preprocess(
         self,
         X_train: Union[psDataFrame, sparkDataFrame],
         y_train: psSeries = None,
         index_col: str = "tmp_index_col",
+        return_label: bool = False,
     ):
         # TODO: optimize this, support pyspark.sql.DataFrame
         if y_train is not None:
             self.df_train = X_train.join(y_train)
         else:
             self.df_train = X_train
         if isinstance(self.df_train, psDataFrame):
             self.df_train = self.df_train.to_spark(index_col=index_col)
-        return self.df_train
+        if return_label:
+            return self.df_train, y_train.name
+        else:
+            return self.df_train
 
     def fit(
         self,
         X_train: psDataFrame,
         y_train: psSeries = None,
         budget=None,
         free_mem_ratio=0,
@@ -433,15 +437,16 @@
             y_train: A pyspark.pandas Series in shape n*1. None if X_train is a pyspark.pandas
                 Dataframe contains y_train.
             budget: A float of the time budget in seconds.
             free_mem_ratio: A float between 0 and 1 for the free memory ratio to keep during training.
         Returns:
             train_time: A float of the training time in seconds.
         """
-        df_train = self._preprocess(X_train, y_train, index_col=index_col)
+        df_train, label_col = self._preprocess(X_train, y_train, index_col=index_col, return_label=True)
+        kwargs["labelCol"] = label_col
         train_time = self._fit(df_train, **kwargs)
         return train_time
 
     def _fit(self, df_train: sparkDataFrame, **kwargs):
         current_time = time.time()
         pipeline_model = self.estimator_class(**self.params, **kwargs)
         if logger.level == logging.DEBUG:
@@ -502,16 +507,14 @@
             logger.warning("Estimator is not fit yet. Please run fit() before predict().")
             return np.ones(X.shape[0])
 
 
 class SparkLGBMEstimator(SparkEstimator):
     """The class for fine-tuning spark version lightgbm models, using SynapseML API."""
 
-    """The class for tuning LGBM, using sklearn API."""
-
     ITER_HP = "numIterations"
     DEFAULT_ITER = 100
 
     @classmethod
     def search_space(cls, data_size, **params):
         upper = max(5, min(32768, int(data_size[0])))  # upper must be larger than lower
         # https://github.com/microsoft/SynapseML/blob/master/lightgbm/src/main/scala/com/microsoft/azure/synapse/ml/lightgbm/LightGBMBase.scala
@@ -610,15 +613,15 @@
         free_mem_ratio=0,
         index_col="tmp_index_col",
         **kwargs,
     ):
         start_time = time.time()
         if self.model_n_classes_ is None and self._task not in ["regression", "rank"]:
             self.model_n_classes_, self.model_classes_ = len_labels(y_train, return_labels=True)
-        df_train = self._preprocess(X_train, y_train, index_col=index_col)
+        df_train, label_col = self._preprocess(X_train, y_train, index_col=index_col, return_label=True)
         # n_iter = self.params.get(self.ITER_HP, self.DEFAULT_ITER)
         # trained = False
         # mem0 = psutil.virtual_memory().available if psutil is not None else 1
         _kwargs = kwargs.copy()
         if self._task not in ["regression", "rank"] and "objective" not in _kwargs:
             _kwargs["objective"] = "binary" if self.model_n_classes_ == 2 else "multiclass"
         for k in list(_kwargs.keys()):
@@ -669,14 +672,15 @@
         #         if budget is not None
         #         else n_iter,
         #     )
         #     if trained and max_iter <= self.params[self.ITER_HP]:
         #         return time.time() - start_time
         #     # when not trained, train at least one iter
         #     self.params[self.ITER_HP] = max(max_iter, 1)
+        _kwargs["labelCol"] = label_col
         self._fit(df_train, **_kwargs)
         train_time = time.time() - start_time
         return train_time
 
     def _fit(self, df_train: sparkDataFrame, **kwargs):
         current_time = time.time()
         model = self.estimator_class(**self.params, **kwargs)
```

### Comparing `FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/data_collator.py` & `FLAML-2.0.0rc3/flaml/automl/nlp/huggingface/data_collator.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/trainer.py` & `FLAML-2.0.0rc3/flaml/automl/nlp/huggingface/trainer.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/training_args.py` & `FLAML-2.0.0rc3/flaml/automl/nlp/huggingface/training_args.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/nlp/huggingface/utils.py` & `FLAML-2.0.0rc3/flaml/automl/nlp/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/nlp/utils.py` & `FLAML-2.0.0rc3/flaml/automl/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/spark/__init__.py` & `FLAML-2.0.0rc3/flaml/automl/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/spark/configs.py` & `FLAML-2.0.0rc3/flaml/automl/spark/configs.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/spark/metrics.py` & `FLAML-2.0.0rc3/flaml/automl/spark/metrics.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/spark/utils.py` & `FLAML-2.0.0rc3/flaml/automl/spark/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/state.py` & `FLAML-2.0.0rc3/flaml/automl/state.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/task/factory.py` & `FLAML-2.0.0rc3/flaml/automl/task/factory.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/task/generic_task.py` & `FLAML-2.0.0rc3/flaml/automl/task/generic_task.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/task/task.py` & `FLAML-2.0.0rc3/flaml/automl/task/task.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/task/time_series_task.py` & `FLAML-2.0.0rc3/flaml/automl/task/time_series_task.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/time_series/feature.py` & `FLAML-2.0.0rc3/flaml/automl/time_series/feature.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/time_series/sklearn.py` & `FLAML-2.0.0rc3/flaml/automl/time_series/sklearn.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/time_series/tft.py` & `FLAML-2.0.0rc3/flaml/automl/time_series/tft.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/time_series/ts_data.py` & `FLAML-2.0.0rc3/flaml/automl/time_series/ts_data.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/time_series/ts_model.py` & `FLAML-2.0.0rc3/flaml/automl/time_series/ts_model.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/automl/training_log.py` & `FLAML-2.0.0rc3/flaml/automl/training_log.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/all/binary.json` & `FLAML-2.0.0rc3/flaml/default/all/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/all/multiclass.json` & `FLAML-2.0.0rc3/flaml/default/all/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/all/regression.json` & `FLAML-2.0.0rc3/flaml/default/all/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/estimator.py` & `FLAML-2.0.0rc3/flaml/default/estimator.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/extra_tree/binary.json` & `FLAML-2.0.0rc3/flaml/default/extra_tree/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/extra_tree/multiclass.json` & `FLAML-2.0.0rc3/flaml/default/extra_tree/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/extra_tree/regression.json` & `FLAML-2.0.0rc3/flaml/default/extra_tree/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/greedy.py` & `FLAML-2.0.0rc3/flaml/default/greedy.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/lgbm/binary.json` & `FLAML-2.0.0rc3/flaml/default/lgbm/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/lgbm/multiclass.json` & `FLAML-2.0.0rc3/flaml/default/lgbm/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/lgbm/regression.json` & `FLAML-2.0.0rc3/flaml/default/lgbm/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/portfolio.py` & `FLAML-2.0.0rc3/flaml/default/portfolio.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/regret.py` & `FLAML-2.0.0rc3/flaml/default/regret.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/rf/binary.json` & `FLAML-2.0.0rc3/flaml/default/rf/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/rf/multiclass.json` & `FLAML-2.0.0rc3/flaml/default/rf/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/rf/regression.json` & `FLAML-2.0.0rc3/flaml/default/rf/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/suggest.py` & `FLAML-2.0.0rc3/flaml/default/suggest.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/binary.json` & `FLAML-2.0.0rc3/flaml/default/xgb_limitdepth/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/multiclass.json` & `FLAML-2.0.0rc3/flaml/default/xgb_limitdepth/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/xgb_limitdepth/regression.json` & `FLAML-2.0.0rc3/flaml/default/xgb_limitdepth/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/xgboost/binary.json` & `FLAML-2.0.0rc3/flaml/default/xgboost/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/xgboost/multiclass.json` & `FLAML-2.0.0rc3/flaml/default/xgboost/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/default/xgboost/regression.json` & `FLAML-2.0.0rc3/flaml/default/xgboost/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/onlineml/autovw.py` & `FLAML-2.0.0rc3/flaml/onlineml/autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/onlineml/trial.py` & `FLAML-2.0.0rc3/flaml/onlineml/trial.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/onlineml/trial_runner.py` & `FLAML-2.0.0rc3/flaml/onlineml/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/__init__.py` & `FLAML-2.0.0rc3/flaml/tune/__init__.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/analysis.py` & `FLAML-2.0.0rc3/flaml/tune/analysis.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/result.py` & `FLAML-2.0.0rc3/flaml/tune/result.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/sample.py` & `FLAML-2.0.0rc3/flaml/tune/sample.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/scheduler/online_scheduler.py` & `FLAML-2.0.0rc3/flaml/tune/scheduler/online_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/scheduler/trial_scheduler.py` & `FLAML-2.0.0rc3/flaml/tune/scheduler/trial_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/searcher/blendsearch.py` & `FLAML-2.0.0rc3/flaml/tune/searcher/blendsearch.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/searcher/cfo_cat.py` & `FLAML-2.0.0rc3/flaml/tune/searcher/cfo_cat.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/searcher/flow2.py` & `FLAML-2.0.0rc3/flaml/tune/searcher/flow2.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/searcher/online_searcher.py` & `FLAML-2.0.0rc3/flaml/tune/searcher/online_searcher.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/searcher/search_thread.py` & `FLAML-2.0.0rc3/flaml/tune/searcher/search_thread.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/searcher/suggestion.py` & `FLAML-2.0.0rc3/flaml/tune/searcher/suggestion.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,30 @@
 # This source file is adapted here because ray does not fully support Windows.
 
 # Copyright (c) Microsoft Corporation.
 import time
 import functools
 import warnings
 import copy
+import numpy as np
 import logging
 from typing import Any, Dict, Optional, Union, List, Tuple, Callable
 import pickle
 from .variant_generator import parse_spec_vars
 from ..sample import (
     Categorical,
     Domain,
     Float,
     Integer,
     LogUniform,
     Quantized,
     Uniform,
 )
 from ..trial import flatten_dict, unflatten_dict
+from collections import defaultdict
 
 logger = logging.getLogger(__name__)
 
 UNRESOLVED_SEARCH_SPACE = str(
     "You passed a `{par}` parameter to {cls} that contained unresolved search "
     "space definitions. {cls} should however be instantiated with fully "
     "configured search spaces only. To use Ray Tune's automatic search space "
@@ -255,22 +257,19 @@
 except ImportError:
     ot = None
     OptunaDistribution = None
     BaseSampler = None
     OptunaTrialState = None
     OptunaTrial = None
 
-# (Optional) Default (anonymous) metric when using tune.report(x)
 DEFAULT_METRIC = "_metric"
 
-# (Auto-filled) The index of this training iteration.
 TRAINING_ITERATION = "training_iteration"
 
-# print a warning if define by run function takes longer than this to execute
-DEFINE_BY_RUN_WARN_THRESHOLD_S = 1  # 1 is arbitrary
+DEFINE_BY_RUN_WARN_THRESHOLD_S = 1
 
 
 def validate_warmstart(
     parameter_names: List[str],
     points_to_evaluate: List[Union[List, Dict]],
     evaluated_rewards: List,
     validate_point_name_lengths: bool = True,
@@ -305,14 +304,15 @@
                 + " and points_to_evaluate {}".format(points_to_evaluate)
                 + " do not match."
             )
 
 
 class _OptunaTrialSuggestCaptor:
     """Utility to capture returned values from Optuna's suggest_ methods.
+
     This will wrap around the ``optuna.Trial` object and decorate all
     `suggest_` callables with a function capturing the returned value,
     which will be saved in the ``captured_values`` dict.
     """
 
     def __init__(self, ot_trial: OptunaTrial) -> None:
         self.ot_trial = ot_trial
@@ -334,110 +334,222 @@
         if item_name.startswith("suggest_") and callable(item):
             return self._get_wrapper(item)
         return item
 
 
 class OptunaSearch(Searcher):
     """A wrapper around Optuna to provide trial suggestions.
-        [Optuna](https://optuna.org/)
-        is a hyperparameter optimization library.
-        In contrast to other libraries, it employs define-by-run style
-        hyperparameter definitions.
-        This Searcher is a thin wrapper around Optuna's search algorithms.
-        You can pass any Optuna sampler, which will be used to generate
-        hyperparameter suggestions.
-        Args:
-            space (dict|Callable): Hyperparameter search space definition for
-                Optuna's sampler. This can be either a class `dict` with
-                parameter names as keys and ``optuna.distributions`` as values,
-                or a Callable - in which case, it should be a define-by-run
-                function using ``optuna.trial`` to obtain the hyperparameter
-                values. The function should return either a class `dict` of
-                constant values with names as keys, or None.
-                For more information, see
-                [tutorial](https://optuna.readthedocs.io/en/stable/tutorial/10_key_features/002_configurations.html).
-                Warning - No actual computation should take place in the define-by-run
-                function. Instead, put the training logic inside the function
-                or class trainable passed to tune.run.
-            metric (str): The training result objective value attribute. If None
-                but a mode was passed, the anonymous metric `_metric` will be used
-                per default.
-            mode (str): One of {min, max}. Determines whether objective is
-                minimizing or maximizing the metric attribute.
-            points_to_evaluate (list): Initial parameter suggestions to be run
-                first. This is for when you already have some good parameters
-                you want to run first to help the algorithm make better suggestions
-                for future parameters. Needs to be a list of dicts containing the
-                configurations.
-            sampler (optuna.samplers.BaseSampler): Optuna sampler used to
-                draw hyperparameter configurations. Defaults to ``TPESampler``.
-            seed (int): Seed to initialize sampler with. This parameter is only
-                used when ``sampler=None``. In all other cases, the sampler
-                you pass should be initialized with the seed already.
-            evaluated_rewards (list): If you have previously evaluated the
-                parameters passed in as points_to_evaluate you can avoid
-                re-running those trials by passing in the reward attributes
-                as a list so the optimiser can be told the results without
-                needing to re-compute the trial. Must be the same length as
-                points_to_evaluate.
-
-        Tune automatically converts search spaces to Optuna's format:
-
-    ````python
-    from ray.tune.suggest.optuna import OptunaSearch  # ray version < 2
-    config = { "a": tune.uniform(6, 8),
-               "b": tune.loguniform(1e-4, 1e-2)}
-    optuna_search = OptunaSearch(metric="loss", mode="min")
+
+    `Optuna <https://optuna.org/>`_ is a hyperparameter optimization library.
+    In contrast to other libraries, it employs define-by-run style
+    hyperparameter definitions.
+
+    This Searcher is a thin wrapper around Optuna's search algorithms.
+    You can pass any Optuna sampler, which will be used to generate
+    hyperparameter suggestions.
+
+    Multi-objective optimization is supported.
+
+    Args:
+        space: Hyperparameter search space definition for
+            Optuna's sampler. This can be either a dict with
+            parameter names as keys and ``optuna.distributions`` as values,
+            or a Callable - in which case, it should be a define-by-run
+            function using ``optuna.trial`` to obtain the hyperparameter
+            values. The function should return either a dict of
+            constant values with names as keys, or None.
+            For more information, see https://optuna.readthedocs.io\
+/en/stable/tutorial/10_key_features/002_configurations.html.
+
+            Warning - No actual computation should take place in the define-by-run
+            function. Instead, put the training logic inside the function
+            or class trainable passed to ``tune.run``.
+
+        metric: The training result objective value attribute. If
+            None but a mode was passed, the anonymous metric ``_metric``
+            will be used per default. Can be a list of metrics for
+            multi-objective optimization.
+        mode: One of {min, max}. Determines whether objective is
+            minimizing or maximizing the metric attribute. Can be a list of
+            modes for multi-objective optimization (corresponding to
+            ``metric``).
+        points_to_evaluate: Initial parameter suggestions to be run
+            first. This is for when you already have some good parameters
+            you want to run first to help the algorithm make better suggestions
+            for future parameters. Needs to be a list of dicts containing the
+            configurations.
+        sampler: Optuna sampler used to
+            draw hyperparameter configurations. Defaults to ``MOTPESampler``
+            for multi-objective optimization with Optuna<2.9.0, and
+            ``TPESampler`` in every other case.
+
+            Warning: Please note that with Optuna 2.10.0 and earlier
+                default ``MOTPESampler``/``TPESampler`` suffer
+                from performance issues when dealing with a large number of
+                completed trials (approx. >100). This will manifest as
+                a delay when suggesting new configurations.
+                This is an Optuna issue and may be fixed in a future
+                Optuna release.
+
+        seed: Seed to initialize sampler with. This parameter is only
+            used when ``sampler=None``. In all other cases, the sampler
+            you pass should be initialized with the seed already.
+        evaluated_rewards: If you have previously evaluated the
+            parameters passed in as points_to_evaluate you can avoid
+            re-running those trials by passing in the reward attributes
+            as a list so the optimiser can be told the results without
+            needing to re-compute the trial. Must be the same length as
+            points_to_evaluate.
+
+            Warning - When using ``evaluated_rewards``, the search space ``space``
+            must be provided as a dict with parameter names as
+            keys and ``optuna.distributions`` instances as values. The
+            define-by-run search space definition is not yet supported with
+            this functionality.
+
+    Tune automatically converts search spaces to Optuna's format:
+
+    ```python
+    from ray.tune.suggest.optuna import OptunaSearch
+
+    config = {
+        "a": tune.uniform(6, 8)
+        "b": tune.loguniform(1e-4, 1e-2)
+    }
+
+    optuna_search = OptunaSearch(
+        metric="loss",
+        mode="min")
+
     tune.run(trainable, config=config, search_alg=optuna_search)
-    ````
+    ```
 
-        If you would like to pass the search space manually, the code would
-        look like this:
+    If you would like to pass the search space manually, the code would
+    look like this:
 
     ```python
-    from ray.tune.suggest.optuna import OptunaSearch  # ray version < 2
+    from ray.tune.suggest.optuna import OptunaSearch
     import optuna
-    config = { "a": optuna.distributions.UniformDistribution(6, 8),
-               "b": optuna.distributions.LogUniformDistribution(1e-4, 1e-2)}
-    optuna_search = OptunaSearch(space,metric="loss",mode="min")
+
+    space = {
+        "a": optuna.distributions.UniformDistribution(6, 8),
+        "b": optuna.distributions.LogUniformDistribution(1e-4, 1e-2),
+    }
+
+    optuna_search = OptunaSearch(
+        space,
+        metric="loss",
+        mode="min")
+
     tune.run(trainable, search_alg=optuna_search)
+
     # Equivalent Optuna define-by-run function approach:
+
     def define_search_space(trial: optuna.Trial):
         trial.suggest_float("a", 6, 8)
         trial.suggest_float("b", 1e-4, 1e-2, log=True)
         # training logic goes into trainable, this is just
         # for search space definition
+
     optuna_search = OptunaSearch(
         define_search_space,
         metric="loss",
         mode="min")
+
+    tune.run(trainable, search_alg=optuna_search)
+    ```
+
+    Multi-objective optimization is supported:
+
+    ```python
+    from ray.tune.suggest.optuna import OptunaSearch
+    import optuna
+
+    space = {
+        "a": optuna.distributions.UniformDistribution(6, 8),
+        "b": optuna.distributions.LogUniformDistribution(1e-4, 1e-2),
+    }
+
+    # Note you have to specify metric and mode here instead of
+    # in tune.run
+    optuna_search = OptunaSearch(
+        space,
+        metric=["loss1", "loss2"],
+        mode=["min", "max"])
+
+    # Do not specify metric and mode here!
+    tune.run(
+        trainable,
+        search_alg=optuna_search
+    )
+    ```
+
+    You can pass configs that will be evaluated first using
+    ``points_to_evaluate``:
+
+    ```python
+    from ray.tune.suggest.optuna import OptunaSearch
+    import optuna
+
+    space = {
+        "a": optuna.distributions.UniformDistribution(6, 8),
+        "b": optuna.distributions.LogUniformDistribution(1e-4, 1e-2),
+    }
+
+    optuna_search = OptunaSearch(
+        space,
+        points_to_evaluate=[{"a": 6.5, "b": 5e-4}, {"a": 7.5, "b": 1e-3}]
+        metric="loss",
+        mode="min")
+
+    tune.run(trainable, search_alg=optuna_search)
+    ```
+
+    Avoid re-running evaluated trials by passing the rewards together with
+    `points_to_evaluate`:
+
+    ```python
+    from ray.tune.suggest.optuna import OptunaSearch
+    import optuna
+
+    space = {
+        "a": optuna.distributions.UniformDistribution(6, 8),
+        "b": optuna.distributions.LogUniformDistribution(1e-4, 1e-2),
+    }
+
+    optuna_search = OptunaSearch(
+        space,
+        points_to_evaluate=[{"a": 6.5, "b": 5e-4}, {"a": 7.5, "b": 1e-3}]
+        evaluated_rewards=[0.89, 0.42]
+        metric="loss",
+        mode="min")
+
     tune.run(trainable, search_alg=optuna_search)
-    .. versionadded:: 0.8.8
     ```
 
     """
 
     def __init__(
         self,
         space: Optional[
             Union[
                 Dict[str, "OptunaDistribution"],
                 List[Tuple],
                 Callable[["OptunaTrial"], Optional[Dict[str, Any]]],
             ]
         ] = None,
-        metric: Optional[str] = None,
-        mode: Optional[str] = None,
+        metric: Optional[Union[str, List[str]]] = None,
+        mode: Optional[Union[str, List[str]]] = None,
         points_to_evaluate: Optional[List[Dict]] = None,
         sampler: Optional["BaseSampler"] = None,
         seed: Optional[int] = None,
         evaluated_rewards: Optional[List] = None,
     ):
         assert ot is not None, "Optuna must be installed! Run `pip install optuna`."
-        super(OptunaSearch, self).__init__(metric=metric, mode=mode, max_concurrent=None, use_early_stopped_trials=None)
+        super(OptunaSearch, self).__init__(metric=metric, mode=mode)
 
         if isinstance(space, dict) and space:
             resolved_vars, domain_vars, grid_vars = parse_spec_vars(space)
             if domain_vars or grid_vars:
                 logger.warning(UNRESOLVED_SEARCH_SPACE.format(par="space", cls=type(self).__name__))
                 space = self.convert_search_space(space)
             else:
@@ -453,41 +565,68 @@
 
         if sampler and seed:
             logger.warning(
                 "You passed an initialized sampler to `OptunaSearch`. The "
                 "`seed` parameter has to be passed to the sampler directly "
                 "and will be ignored."
             )
+        elif sampler:
+            assert isinstance(sampler, BaseSampler), (
+                "You can only pass an instance of " "`optuna.samplers.BaseSampler` " "as a sampler to `OptunaSearcher`."
+            )
 
-        self._sampler = sampler or ot.samplers.TPESampler(seed=seed)
+        self._sampler = sampler
+        self._seed = seed
 
-        assert isinstance(self._sampler, BaseSampler), (
-            "You can only pass an instance of `optuna.samplers.BaseSampler` " "as a sampler to `OptunaSearcher`."
-        )
+        self._completed_trials = set()
 
         self._ot_trials = {}
         self._ot_study = None
         if self._space:
             self._setup_study(mode)
 
-    def _setup_study(self, mode: str):
+    def _setup_study(self, mode: Union[str, list]):
         if self._metric is None and self._mode:
+            if isinstance(self._mode, list):
+                raise ValueError(
+                    "If ``mode`` is a list (multi-objective optimization " "case), ``metric`` must be defined."
+                )
             # If only a mode was passed, use anonymous metric
             self._metric = DEFAULT_METRIC
 
         pruner = ot.pruners.NopPruner()
         storage = ot.storages.InMemoryStorage()
+        try:
+            from packaging import version
+        except ImportError:
+            raise ImportError("To use BlendSearch, run: pip install flaml[blendsearch]")
+        if self._sampler:
+            sampler = self._sampler
+        elif isinstance(mode, list) and version.parse(ot.__version__) < version.parse("2.9.0"):
+            # MOTPESampler deprecated in Optuna>=2.9.0
+            sampler = ot.samplers.MOTPESampler(seed=self._seed)
+        else:
+            sampler = ot.samplers.TPESampler(seed=self._seed)
+
+        if isinstance(mode, list):
+            study_direction_args = dict(
+                directions=["minimize" if m == "min" else "maximize" for m in mode],
+            )
+        else:
+            study_direction_args = dict(
+                direction="minimize" if mode == "min" else "maximize",
+            )
 
         self._ot_study = ot.study.create_study(
             storage=storage,
-            sampler=self._sampler,
+            sampler=sampler,
             pruner=pruner,
             study_name=self._study_name,
-            direction="minimize" if mode == "min" else "maximize",
             load_if_exists=True,
+            **study_direction_args,
         )
 
         if self._points_to_evaluate:
             validate_warmstart(
                 self._space,
                 self._points_to_evaluate,
                 self._evaluated_rewards,
@@ -496,25 +635,25 @@
             if self._evaluated_rewards:
                 for point, reward in zip(self._points_to_evaluate, self._evaluated_rewards):
                     self.add_evaluated_point(point, reward)
             else:
                 for point in self._points_to_evaluate:
                     self._ot_study.enqueue_trial(point)
 
-    def set_search_properties(self, metric: Optional[str], mode: Optional[str], config: Dict) -> bool:
+    def set_search_properties(self, metric: Optional[str], mode: Optional[str], config: Dict, **spec) -> bool:
         if self._space:
             return False
         space = self.convert_search_space(config)
         self._space = space
         if metric:
             self._metric = metric
         if mode:
             self._mode = mode
 
-        self._setup_study(mode)
+        self._setup_study(self._mode)
         return True
 
     def _suggest_from_define_by_run_func(
         self,
         func: Callable[["OptunaTrial"], Optional[Dict[str, Any]]],
         ot_trial: "OptunaTrial",
     ) -> Dict:
@@ -549,29 +688,16 @@
     def suggest(self, trial_id: str) -> Optional[Dict]:
         if not self._space:
             raise RuntimeError(UNDEFINED_SEARCH_SPACE.format(cls=self.__class__.__name__, space="space"))
         if not self._metric or not self._mode:
             raise RuntimeError(
                 UNDEFINED_METRIC_MODE.format(cls=self.__class__.__name__, metric=self._metric, mode=self._mode)
             )
-
-        if isinstance(self._space, list):
-            # Keep for backwards compatibility
-            # Deprecate: 1.5
-            if trial_id not in self._ot_trials:
-                self._ot_trials[trial_id] = self._ot_study.ask()
-
-            ot_trial = self._ot_trials[trial_id]
-
-            # getattr will fetch the trial.suggest_ function on Optuna trials
-            params = {
-                args[0] if len(args) > 0 else kwargs["name"]: getattr(ot_trial, fn)(*args, **kwargs)
-                for (fn, args, kwargs) in self._space
-            }
-        elif callable(self._space):
+        if callable(self._space):
+            # Define-by-run case
             if trial_id not in self._ot_trials:
                 self._ot_trials[trial_id] = self._ot_study.ask()
 
             ot_trial = self._ot_trials[trial_id]
 
             params = self._suggest_from_define_by_run_func(self._space, ot_trial)
         else:
@@ -580,48 +706,78 @@
                 self._ot_trials[trial_id] = self._ot_study.ask(fixed_distributions=self._space)
             ot_trial = self._ot_trials[trial_id]
             params = ot_trial.params
 
         return unflatten_dict(params)
 
     def on_trial_result(self, trial_id: str, result: Dict):
+        if isinstance(self.metric, list):
+            # Optuna doesn't support incremental results
+            # for multi-objective optimization
+            return
+        if trial_id in self._completed_trials:
+            logger.warning(
+                f"Received additional result for trial {trial_id}, but " f"it already finished. Result: {result}"
+            )
+            return
         metric = result[self.metric]
         step = result[TRAINING_ITERATION]
         ot_trial = self._ot_trials[trial_id]
         ot_trial.report(metric, step)
 
     def on_trial_complete(self, trial_id: str, result: Optional[Dict] = None, error: bool = False):
+        if trial_id in self._completed_trials:
+            logger.warning(
+                f"Received additional completion for trial {trial_id}, but " f"it already finished. Result: {result}"
+            )
+            return
+
         ot_trial = self._ot_trials[trial_id]
 
-        val = result.get(self.metric, None) if result else None
+        if result:
+            if isinstance(self.metric, list):
+                val = [result.get(metric, None) for metric in self.metric]
+            else:
+                val = result.get(self.metric, None)
+        else:
+            val = None
         ot_trial_state = OptunaTrialState.COMPLETE
         if val is None:
             if error:
                 ot_trial_state = OptunaTrialState.FAIL
             else:
                 ot_trial_state = OptunaTrialState.PRUNED
         try:
             self._ot_study.tell(ot_trial, val, state=ot_trial_state)
-        except ValueError as exc:
+        except Exception as exc:
             logger.warning(exc)  # E.g. if NaN was reported
 
+        self._completed_trials.add(trial_id)
+
     def add_evaluated_point(
         self,
         parameters: Dict,
         value: float,
         error: bool = False,
         pruned: bool = False,
         intermediate_values: Optional[List[float]] = None,
     ):
         if not self._space:
             raise RuntimeError(UNDEFINED_SEARCH_SPACE.format(cls=self.__class__.__name__, space="space"))
         if not self._metric or not self._mode:
             raise RuntimeError(
                 UNDEFINED_METRIC_MODE.format(cls=self.__class__.__name__, metric=self._metric, mode=self._mode)
             )
+        if callable(self._space):
+            raise TypeError(
+                "Define-by-run function passed in `space` argument is not "
+                "yet supported when using `evaluated_rewards`. Please provide "
+                "an `OptunaDistribution` dict or pass a Ray Tune "
+                "search space to `tune.run()`."
+            )
 
         ot_trial_state = OptunaTrialState.COMPLETE
         if error:
             ot_trial_state = OptunaTrialState.FAIL
         elif pruned:
             ot_trial_state = OptunaTrialState.PRUNED
```

### Comparing `FLAML-2.0.0rc2/flaml/tune/searcher/variant_generator.py` & `FLAML-2.0.0rc3/flaml/tune/searcher/variant_generator.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/space.py` & `FLAML-2.0.0rc3/flaml/tune/space.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/spark/utils.py` & `FLAML-2.0.0rc3/flaml/tune/spark/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/trial.py` & `FLAML-2.0.0rc3/flaml/tune/trial.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/trial_runner.py` & `FLAML-2.0.0rc3/flaml/tune/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/flaml/tune/tune.py` & `FLAML-2.0.0rc3/flaml/tune/tune.py`

 * *Files 4% similar despite different names*

```diff
@@ -340,15 +340,15 @@
             intermediate_score = evaluation_fn(step, width, height)
             try:
                 tune.report(iterations=step, mean_loss=intermediate_score)
             except (StopIteration, SystemExit):
                 # do cleanup operation here
                 return
     ```
-        search_alg: An instance of BlendSearch as the search algorithm
+        search_alg: An instance/string of the search algorithm
             to be used. The same instance can be used for iterative tuning.
             e.g.,
 
     ```python
     from flaml import BlendSearch
     algo = BlendSearch(metric='val_loss', mode='min',
             space=search_space,
@@ -477,47 +477,70 @@
             if verbose <= 2:
                 logger.setLevel(logging.INFO)
             else:
                 logger.setLevel(logging.DEBUG)
         else:
             logger.setLevel(logging.CRITICAL)
 
-    from .searcher.blendsearch import BlendSearch, CFO
+    from .searcher.blendsearch import BlendSearch, CFO, RandomSearch
 
     if lexico_objectives is not None:
-        logger.warning("If lexico_objectives is not None, search_alg is forced to be CFO")
-        search_alg = None
-    if search_alg is None:
+        if "modes" not in lexico_objectives.keys():
+            lexico_objectives["modes"] = ["min"] * len(lexico_objectives["metrics"])
+        for t_metric, t_mode in zip(lexico_objectives["metrics"], lexico_objectives["modes"]):
+            if t_metric not in lexico_objectives["tolerances"].keys():
+                lexico_objectives["tolerances"][t_metric] = 0
+            if t_metric not in lexico_objectives["targets"].keys():
+                lexico_objectives["targets"][t_metric] = -float("inf") if t_mode == "min" else float("inf")
+    if search_alg is None or isinstance(search_alg, str):
+        if isinstance(search_alg, str):
+            assert search_alg in [
+                "BlendSearch",
+                "CFO",
+                "CFOCat",
+                "RandomSearch",
+            ], f"search_alg={search_alg} is not recognized. 'BlendSearch', 'CFO', 'CFOcat' and 'RandomSearch' are supported."
+
         flaml_scheduler_resource_attr = (
             flaml_scheduler_min_resource
         ) = flaml_scheduler_max_resource = flaml_scheduler_reduction_factor = None
         if scheduler in (None, "flaml"):
             # when scheduler is set 'flaml' or None, we will use a scheduler that is
             # authentic to the search algorithms in flaml. After setting up
             # the search algorithm accordingly, we need to set scheduler to
             # None in case it is later used in the trial runner.
             flaml_scheduler_resource_attr = resource_attr
             flaml_scheduler_min_resource = min_resource
             flaml_scheduler_max_resource = max_resource
             flaml_scheduler_reduction_factor = reduction_factor
             scheduler = None
-        if lexico_objectives is None:
-            try:
-                import optuna as _
+        if lexico_objectives:
+            # TODO: Modify after supporting BlendSearch in lexicographic optimization
+            SearchAlgorithm = CFO
+            logger.info(
+                f"Using search algorithm {SearchAlgorithm.__name__} for lexicographic optimization. Note that when providing other search algorithms, we use CFO instead temporarily."
+            )
+            metric = lexico_objectives["metrics"][0] or DEFAULT_METRIC
+        else:
+            if not search_alg or search_alg == "BlendSearch":
+                try:
+                    import optuna as _
 
-                SearchAlgorithm = BlendSearch
+                    SearchAlgorithm = BlendSearch
+                    logger.info("Using search algorithm {}.".format(SearchAlgorithm.__name__))
+                except ImportError:
+                    if search_alg == "BlendSearch":
+                        raise ValueError("To use BlendSearch, run: pip install flaml[blendsearch]")
+                    else:
+                        SearchAlgorithm = CFO
+                        logger.warning("Using CFO for search. To use BlendSearch, run: pip install flaml[blendsearch]")
+            else:
+                SearchAlgorithm = locals()[search_alg]
                 logger.info("Using search algorithm {}.".format(SearchAlgorithm.__name__))
-            except ImportError:
-                SearchAlgorithm = CFO
-                logger.warning("Using CFO for search. To use BlendSearch, run: pip install flaml[blendsearch]")
             metric = metric or DEFAULT_METRIC
-        else:
-            SearchAlgorithm = CFO
-            logger.info("Using search algorithm {}.".format(SearchAlgorithm.__name__))
-            metric = lexico_objectives["metrics"][0] or DEFAULT_METRIC
         search_alg = SearchAlgorithm(
             metric=metric,
             mode=mode,
             space=config,
             points_to_evaluate=points_to_evaluate,
             evaluated_rewards=evaluated_rewards,
             low_cost_partial_config=low_cost_partial_config,
@@ -531,16 +554,20 @@
             config_constraints=config_constraints,
             metric_constraints=metric_constraints,
             use_incumbent_result_in_evaluation=use_incumbent_result_in_evaluation,
             lexico_objectives=lexico_objectives,
         )
     else:
         if metric is None or mode is None:
-            metric = metric or search_alg.metric or DEFAULT_METRIC
-            mode = mode or search_alg.mode
+            if lexico_objectives:
+                metric = lexico_objectives["metrics"][0] or metric or search_alg.metric or DEFAULT_METRIC
+                mode = lexico_objectives["modes"][0] or mode or search_alg.mode
+            else:
+                metric = metric or search_alg.metric or DEFAULT_METRIC
+                mode = mode or search_alg.mode
         if ray_available and use_ray:
             if ray_version.startswith("1."):
                 from ray.tune.suggest import ConcurrencyLimiter
             else:
                 from ray.tune.search import ConcurrencyLimiter
         else:
             from flaml.tune.searcher.suggestion import ConcurrencyLimiter
@@ -551,14 +578,21 @@
                 "CFO",
                 "CFOCat",
             ]
             and use_incumbent_result_in_evaluation is not None
         ):
             search_alg.use_incumbent_result_in_evaluation = use_incumbent_result_in_evaluation
         searcher = search_alg.searcher if isinstance(search_alg, ConcurrencyLimiter) else search_alg
+        if lexico_objectives:
+            # TODO: Modify after supporting BlendSearch in lexicographic optimization
+            assert search_alg.__class__.__name__ in [
+                "CFO",
+            ], "If lexico_objectives is not None, the search_alg must be CFO for now."
+            search_alg.lexico_objective = lexico_objectives
+
         if isinstance(searcher, BlendSearch):
             setting = {}
             if time_budget_s:
                 setting["time_budget_s"] = time_budget_s
             if num_samples > 0:
                 setting["num_samples"] = num_samples
             searcher.set_search_properties(metric, mode, config, **setting)
```

### Comparing `FLAML-2.0.0rc2/flaml/tune/utils.py` & `FLAML-2.0.0rc3/flaml/tune/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/pyproject.toml` & `FLAML-2.0.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/setup.py` & `FLAML-2.0.0rc3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         ],
         "notebook": [
             "jupyter",
         ],
         "spark": [
             "pyspark>=3.2.0",
             "joblibspark>=0.5.0",
+            "joblib<1.3.0",  # temp solution for joblib 1.3.0 issue, no need once https://github.com/joblib/joblib-spark/pull/48 is merged
         ],
         "test": [
             "lightgbm>=2.3.1",
             "xgboost>=0.90",
             "scipy>=1.4.1",
             "pandas>=1.1.4",
             "scikit-learn>=0.24",
@@ -80,20 +81,24 @@
             "nbconvert",
             "nbformat",
             "ipykernel",
             "pytorch-lightning<1.9.1",  # test_forecast_panel
             "tensorboardX==2.6",  # test_forecast_panel
             "requests<2.29.0",  # https://github.com/docker/docker-py/issues/3113
             "packaging",
-            "pydantic",
+            "pydantic==1.10.9",
             "sympy",
             "wolframalpha",
+            "joblib<1.3.0",  # temp solution for joblib 1.3.0 issue, no need once https://github.com/joblib/joblib-spark/pull/48 is merged
         ],
         "catboost": ["catboost>=0.26"],
-        "blendsearch": ["optuna==2.8.0"],
+        "blendsearch": [
+            "optuna==2.8.0",
+            "packaging",
+        ],
         "ray": [
             "ray[tune]~=1.13",
         ],
         "azureml": [
             "azureml-mlflow",
         ],
         "nni": [
@@ -131,19 +136,20 @@
             "pytorch-forecasting>=0.9.0",
             "pytorch-lightning==1.9.0",
             "tensorboardX==2.6",
         ],
         "benchmark": ["catboost>=0.26", "psutil==5.8.0", "xgboost==1.3.3", "pandas==1.1.4"],
         "openai": ["openai==0.27.8", "diskcache"],
         "autogen": ["openai==0.27.8", "diskcache", "docker"],
-        "mathchat": ["openai==0.27.8", "diskcache", "docker", "sympy", "pydantic", "wolframalpha"],
+        "mathchat": ["openai==0.27.8", "diskcache", "docker", "sympy", "pydantic==1.10.9", "wolframalpha"],
         "synapse": [
             "joblibspark>=0.5.0",
             "optuna==2.8.0",
             "pyspark>=3.2.0",
+            "joblib<1.3.0",  # temp solution for joblib 1.3.0 issue, no need once https://github.com/joblib/joblib-spark/pull/48 is merged
         ],
         "autozero": ["scikit-learn", "pandas", "packaging"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `FLAML-2.0.0rc2/test/test_autovw.py` & `FLAML-2.0.0rc3/test/test_autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/test/test_conda_distribution.py` & `FLAML-2.0.0rc3/test/test_conda_distribution.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/test/test_gpu.py` & `FLAML-2.0.0rc3/test/test_gpu.py`

 * *Files identical despite different names*

### Comparing `FLAML-2.0.0rc2/test/test_model.py` & `FLAML-2.0.0rc3/test/test_model.py`

 * *Files identical despite different names*

