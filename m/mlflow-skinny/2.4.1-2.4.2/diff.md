# Comparing `tmp/mlflow-skinny-2.4.1.tar.gz` & `tmp/mlflow-skinny-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-skinny-2.4.1.tar", last modified: Sat Jun 10 01:34:27 2023, max compression
+gzip compressed data, was "mlflow-skinny-2.4.2.tar", last modified: Mon Jul 10 06:27:58 2023, max compression
```

## Comparing `mlflow-skinny-2.4.1.tar` & `mlflow-skinny-2.4.2.tar`

### file list

```diff
@@ -1,473 +1,476 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11382 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/LICENSE.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      608 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11500 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9817 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/README.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      949 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/README_SKINNY.rst
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.905476 mlflow-skinny-2.4.1/mlflow/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6490 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/__main__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3668 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/_doctor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9680 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/_spark_autologging.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.905476 mlflow-skinny-2.4.1/mlflow/artifacts/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6485 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/artifacts/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.905476 mlflow-skinny-2.4.1/mlflow/azure/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/azure/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11647 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/azure/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15140 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/catboost.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24024 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      407 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.905476 mlflow-skinny-2.4.1/mlflow/data/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2477 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7022 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/artifact_dataset_sources.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      946 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/code_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4333 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6297 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/dataset_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3534 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8270 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/dataset_source_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3734 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/delta_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4873 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/digest_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2598 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/filesystem_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3929 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/http_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10462 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/huggingface_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4008 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/huggingface_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7966 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/numpy_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6955 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/pandas_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      897 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/pyfunc_dataset_mixin.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2800 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/schema.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/sources.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15642 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/spark_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2196 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/spark_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3858 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/spark_delta_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11898 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/tensorflow_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      881 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/db.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.905476 mlflow-skinny-2.4.1/mlflow/deployments/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3797 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/deployments/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15582 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/deployments/base.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15078 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/deployments/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3825 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/deployments/interface.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5512 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/deployments/plugin_manager.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      556 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/deployments/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28178 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/diviner.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/entities/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1211 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1414 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/_mlflow_object.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2118 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1510 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/dataset_input.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3510 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/experiment.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      887 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/experiment_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1215 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/file_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      992 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/input_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1242 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/lifecycle_stage.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1418 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/metric.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/entities/model_registry/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      529 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      286 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/_model_registry_entity.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6435 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      831 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version_stages.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1533 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version_status.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      933 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4933 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/registered_model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/registered_model_alias.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/registered_model_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1133 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/param.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2134 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/run.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3032 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/run_data.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6182 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/run_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/run_inputs.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1550 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/run_status.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      890 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/run_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1212 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/source_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1826 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/view_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12114 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/environment_variables.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4881 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/exceptions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5080 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/experiments.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/fastai/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25449 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/fastai/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5660 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/fastai/callback.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/gluon/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19248 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/gluon/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2020 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/gluon/_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14185 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/h2o.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    36396 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/johnsnowlabs.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/keras.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/langchain/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21279 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/langchain/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4898 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/langchain/api_request_parallel_processor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38975 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/lightgbm.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      180 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/llm.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5786 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/ml_package_versions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13885 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/mleap.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/models/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3637 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9803 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/cli.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/models/container/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9387 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/container/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/models/container/scoring_server/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/container/scoring_server/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/container/scoring_server/wsgi.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9870 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/docker_utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/models/evaluation/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      491 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3105 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/_shap_patch.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6769 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/artifacts.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    64594 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/base.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52848 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/default_evaluator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2036 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/evaluator_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6223 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/lift_curve.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10946 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/validation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3420 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/flavor_backend.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2354 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/flavor_backend_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24997 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12595 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/signature.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    39843 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11707 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/wheeled_model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24919 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/onnx.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/openai/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23265 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/openai/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12309 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/openai/api_request_parallel_processor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2936 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/openai/retry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2088 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/openai/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/paddle/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23859 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/paddle/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4792 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/paddle/_paddle_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17616 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pmdarima.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/projects/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17396 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11532 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/_project_spec.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/projects/backend/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      271 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/backend/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2210 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/backend/abstract_backend.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1079 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/backend/loader.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17277 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/backend/local.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20212 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/databricks.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6402 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/docker.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       94 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/env_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6379 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/kubernetes.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3574 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/submitted_run.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12237 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14024 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/prophet.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/protos/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17261 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/databricks_artifacts_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14095 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/databricks_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    42316 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/databricks_uc_registry_messages_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12471 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/databricks_uc_registry_service_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16146 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/facet_feature_statistics_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1361 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/internal_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8552 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/mlflow_artifacts_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    54475 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/model_registry_pb2.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/protos/scalapb/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/scalapb/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3307 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/scalapb/scalapb_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    53666 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/service_pb2.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/pyfunc/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    81981 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16573 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/backend.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      901 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/mlserver.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15392 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/model.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/pyfunc/scoring_server/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13910 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/scoring_server/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4222 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/scoring_server/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      175 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/scoring_server/wsgi.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2124 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/spark_model_cache.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1001 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/stdin_server.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  7380252 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pypi_package_index.json
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/pyspark/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyspark/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/pyspark/ml/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    55602 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyspark/ml/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2908 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyspark/ml/_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1886 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyspark/ml/log_model_allowlist.txt
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/pytorch/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    45559 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pytorch/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17568 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pytorch/_lightning_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2654 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pytorch/_pytorch_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2090 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pytorch/pickle_module.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1330 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6092 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/artifacts.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/cards/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10189 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/cards/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4780 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/cards/histogram_generator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12548 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/cards/pandas_renderer.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/cards/templates/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/cards/templates/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/classification/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/classification/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/classification/v1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      122 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/classification/v1/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20462 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/classification/v1/recipe.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2917 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18431 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/dag_help_strings.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17933 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/recipe.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/regression/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/regression/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/regression/v1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      114 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/regression/v1/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22495 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/regression/v1/recipe.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14841 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/step.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/steps/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/steps/automl/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/automl/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6260 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/automl/flaml.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20666 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/evaluate.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/steps/ingest/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11137 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/ingest/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26390 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/ingest/datasets.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12140 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/predict.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7664 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/register.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19541 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/split.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    59735 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/train.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10602 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/transform.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/utils/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6355 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/utils/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28468 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/utils/execution.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8990 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/utils/metrics.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7680 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/utils/step.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12316 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/utils/tracking.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1748 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/utils/wrapped_recipe_model.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/rfunc/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1115 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/rfunc/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3639 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/rfunc/backend.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2519 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/runs.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/sagemaker/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   135083 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/sagemaker/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12986 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/sagemaker/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14450 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/sentence_transformers.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/server/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7077 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/server/auth/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28016 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      123 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/basic_auth.ini
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4689 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4217 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/entities.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2673 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/logo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1267 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/permissions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1111 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/routes.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12648 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/sqlalchemy_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    69738 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/handlers.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      481 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/server/prometheus_exporter.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26647 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/shap.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/sklearn/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    85689 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/sklearn/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    37469 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/sklearn/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14259 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/spacy.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    45175 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/spark.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24781 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/statsmodels.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      227 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/registry/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/registry/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28656 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/registry/rest_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5419 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/registry/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/artifact/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10481 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5836 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/artifact_repository_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8136 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/azure_blob_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5829 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/azure_data_lake_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5378 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35001 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/databricks_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9819 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/databricks_models_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10247 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/dbfs_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5234 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/ftp_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5873 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/gcs_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9684 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/hdfs_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3377 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/http_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5107 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/local_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3001 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/mlflow_artifacts_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6757 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/models_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6016 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/runs_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9433 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/s3_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5455 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/sftp_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5592 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/unity_catalog_models_artifact_repo.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/artifact/utils/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/utils/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3934 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/utils/models.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/db/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db/base_sql_model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      221 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db/db_types.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10567 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/db_migrations/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1634 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/alembic.ini
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2768 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/env.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1990 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      462 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/0c779009ac13_add_deleted_time_field_to_runs_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      924 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2624 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1375 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1201 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      940 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1014 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      476 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/84291f40a231_add_run_link_to_model_version.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5716 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1666 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      577 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      582 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2830 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/store/entities/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/entities/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      479 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/entities/paged_list.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/store/model_registry/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      605 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11022 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/abstract_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1440 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/base_rest_store.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/store/model_registry/dbmodels/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/dbmodels/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/dbmodels/models.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38833 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/file_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16920 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/rest_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50646 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/sqlalchemy_store.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/store/tracking/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1154 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13534 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/abstract_store.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/store/tracking/dbmodels/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/dbmodels/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8315 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/dbmodels/initial_models.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21085 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/dbmodels/models.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52631 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/file_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12822 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/rest_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    77913 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/sqlalchemy_store.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/tensorflow/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    60208 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tensorflow/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8442 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tensorflow/_autolog.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/tracking/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      995 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       41 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15534 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9641 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/fluent.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3152 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7008 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24289 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2335 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9517 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7540 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/artifact_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   142886 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.929476 mlflow-skinny-2.4.1/mlflow/tracking/context/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1076 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/abstract_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_cluster_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      561 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_command_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1965 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_job_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1713 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_notebook_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1952 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_repo_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/default_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      898 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/git_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3738 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      443 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/system_environment_context.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.929476 mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       28 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1703 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/abstract_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1718 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2300 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3173 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    78452 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/fluent.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3404 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/llm_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2248 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/metric_value_conversion_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3515 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/registry.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.929476 mlflow-skinny-2.4.1/mlflow/tracking/request_header/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/request_header/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1077 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/request_header/abstract_request_header_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1336 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/request_header/databricks_request_header_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      486 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/request_header/default_request_header_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2867 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/request_header/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   110231 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/transformers.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.929476 mlflow-skinny-2.4.1/mlflow/types/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      299 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/types/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15035 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/types/schema.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18044 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/types/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/mlflow/utils/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9365 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6589 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/_capture_modules.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2274 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/_capture_transformers_modules.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6387 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/_spark_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5009 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/annotations.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/arguments_utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27045 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16642 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10937 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13381 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/logging_and_warnings.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    47266 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/safety.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3570 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/versioning.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      215 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/class_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6431 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/cli_args.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13002 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/conda.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      432 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/data_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23803 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/databricks_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9138 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/docstring_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1669 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/download_cloud_file_chunk.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/env.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/env_manager.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22634 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/environment.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30464 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/file_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2306 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/git_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24178 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/gorilla.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/mlflow/utils/import_hooks/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13645 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/import_hooks/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2597 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/logging_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/mime_type_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4024 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/mlflow_tags.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8109 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/model_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5873 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/name_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2412 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/nfs_on_spark.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      139 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/os.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5799 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/process.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19909 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/proto_json_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5560 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/request_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20034 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/requirements_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11852 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/rest_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    59666 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/search_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2368 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/server_cli_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3805 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/string_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      512 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/time_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14271 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/uri.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19435 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/validation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16278 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/virtualenv.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      147 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/version.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/mlflow/xgboost/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    37317 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/xgboost/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2908 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/xgboost/_autolog.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11500 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14749 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/entry_points.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      618 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/top_level.txt
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/pylint_plugins/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      614 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2234 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/errors.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4556 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/import_checker.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      856 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/print_function.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/pylint_plugins/pytest_raises_checker/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1546 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/pytest_raises_checker/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      571 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/set_checker.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      878 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/string_checker.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      692 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/unittest_assert_raises.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/requirements/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      609 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/requirements/core-requirements.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      297 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/requirements/gateway-requirements.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      481 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/requirements/skinny-requirements.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7311 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.971708 mlflow-skinny-2.4.2/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11382 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/LICENSE.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      608 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11500 2023-07-10 06:27:58.971708 mlflow-skinny-2.4.2/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9817 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/README.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      949 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/README_SKINNY.rst
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.927708 mlflow-skinny-2.4.2/mlflow/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6490 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/__main__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3668 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/_doctor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9680 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/_spark_autologging.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.931708 mlflow-skinny-2.4.2/mlflow/artifacts/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6485 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/artifacts/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.931708 mlflow-skinny-2.4.2/mlflow/azure/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/azure/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11647 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/azure/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15140 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/catboost.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24024 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      407 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.931708 mlflow-skinny-2.4.2/mlflow/data/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2477 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7022 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/artifact_dataset_sources.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      946 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/code_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4333 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6297 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/dataset_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3534 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8270 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/dataset_source_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3734 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/delta_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4873 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/digest_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2598 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/filesystem_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3929 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/http_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10462 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/huggingface_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4008 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/huggingface_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7966 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/numpy_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6955 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/pandas_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      897 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/pyfunc_dataset_mixin.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2800 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/schema.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/sources.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15642 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/spark_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2196 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/spark_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3858 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/spark_delta_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11898 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/data/tensorflow_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      881 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/db.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.931708 mlflow-skinny-2.4.2/mlflow/deployments/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3797 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/deployments/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15582 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/deployments/base.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15078 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/deployments/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3825 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/deployments/interface.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5512 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/deployments/plugin_manager.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      556 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/deployments/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28178 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/diviner.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.935709 mlflow-skinny-2.4.2/mlflow/entities/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1211 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1414 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/_mlflow_object.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2118 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1510 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/dataset_input.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3510 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/experiment.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      887 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/experiment_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1215 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/file_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      992 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/input_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1242 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/lifecycle_stage.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1418 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/metric.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.935709 mlflow-skinny-2.4.2/mlflow/entities/model_registry/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      529 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/model_registry/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      286 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/model_registry/_model_registry_entity.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6435 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/model_registry/model_version.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      831 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/model_registry/model_version_stages.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1533 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/model_registry/model_version_status.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      933 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/model_registry/model_version_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4933 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/model_registry/registered_model.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/model_registry/registered_model_alias.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/model_registry/registered_model_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1133 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/param.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2134 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/run.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3032 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/run_data.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6182 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/run_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/run_inputs.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1550 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/run_status.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      890 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/run_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1212 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/source_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1826 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/entities/view_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12114 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/environment_variables.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4881 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/exceptions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5080 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/experiments.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.935709 mlflow-skinny-2.4.2/mlflow/fastai/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25449 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/fastai/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5660 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/fastai/callback.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.935709 mlflow-skinny-2.4.2/mlflow/gluon/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19248 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/gluon/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2020 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/gluon/_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14185 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/h2o.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    36269 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/johnsnowlabs.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/keras.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.939709 mlflow-skinny-2.4.2/mlflow/langchain/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21279 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/langchain/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4898 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/langchain/api_request_parallel_processor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38975 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/lightgbm.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      180 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/llm.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5786 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/ml_package_versions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13885 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/mleap.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.939709 mlflow-skinny-2.4.2/mlflow/models/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3637 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9803 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/cli.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.939709 mlflow-skinny-2.4.2/mlflow/models/container/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9387 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/container/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.939709 mlflow-skinny-2.4.2/mlflow/models/container/scoring_server/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/container/scoring_server/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/container/scoring_server/wsgi.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9870 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/docker_utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.939709 mlflow-skinny-2.4.2/mlflow/models/evaluation/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      491 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/evaluation/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3105 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/evaluation/_shap_patch.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6769 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/evaluation/artifacts.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    64594 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/evaluation/base.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52848 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/evaluation/default_evaluator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2036 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/evaluation/evaluator_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6223 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/evaluation/lift_curve.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10946 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/evaluation/validation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3420 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/flavor_backend.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2354 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/flavor_backend_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24997 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/model.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12595 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/signature.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    39843 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11707 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/models/wheeled_model.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24919 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/onnx.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.939709 mlflow-skinny-2.4.2/mlflow/openai/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23265 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/openai/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12309 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/openai/api_request_parallel_processor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2936 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/openai/retry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2088 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/openai/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.939709 mlflow-skinny-2.4.2/mlflow/paddle/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23859 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/paddle/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4792 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/paddle/_paddle_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17616 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pmdarima.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.943709 mlflow-skinny-2.4.2/mlflow/projects/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17396 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/projects/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11532 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/projects/_project_spec.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.943709 mlflow-skinny-2.4.2/mlflow/projects/backend/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      271 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/projects/backend/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2210 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/projects/backend/abstract_backend.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1079 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/projects/backend/loader.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17277 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/projects/backend/local.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20212 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/projects/databricks.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6402 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/projects/docker.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       94 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/projects/env_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6379 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/projects/kubernetes.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3574 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/projects/submitted_run.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12237 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/projects/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14024 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/prophet.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.943709 mlflow-skinny-2.4.2/mlflow/protos/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/protos/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17261 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/protos/databricks_artifacts_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14095 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/protos/databricks_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    42367 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/protos/databricks_uc_registry_messages_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12471 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/protos/databricks_uc_registry_service_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16146 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/protos/facet_feature_statistics_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1361 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/protos/internal_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8552 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/protos/mlflow_artifacts_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    54475 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/protos/model_registry_pb2.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.943709 mlflow-skinny-2.4.2/mlflow/protos/scalapb/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/protos/scalapb/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3307 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/protos/scalapb/scalapb_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    53666 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/protos/service_pb2.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.943709 mlflow-skinny-2.4.2/mlflow/pyfunc/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    81981 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pyfunc/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16573 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pyfunc/backend.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      901 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pyfunc/mlserver.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15392 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pyfunc/model.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.943709 mlflow-skinny-2.4.2/mlflow/pyfunc/scoring_server/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13910 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pyfunc/scoring_server/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4222 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pyfunc/scoring_server/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      175 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pyfunc/scoring_server/wsgi.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2124 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pyfunc/spark_model_cache.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1001 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pyfunc/stdin_server.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  7380252 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pypi_package_index.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.943709 mlflow-skinny-2.4.2/mlflow/pyspark/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pyspark/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.943709 mlflow-skinny-2.4.2/mlflow/pyspark/ml/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    55602 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pyspark/ml/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2908 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pyspark/ml/_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1886 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pyspark/ml/log_model_allowlist.txt
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.943709 mlflow-skinny-2.4.2/mlflow/pytorch/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    45559 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pytorch/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17568 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pytorch/_lightning_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2654 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pytorch/_pytorch_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2090 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/pytorch/pickle_module.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/recipes/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1330 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6092 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/artifacts.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/recipes/cards/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10189 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/cards/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4780 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/cards/histogram_generator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12548 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/cards/pandas_renderer.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/recipes/cards/templates/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/cards/templates/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3488 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/cards/templates/base.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/recipes/classification/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/classification/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/recipes/classification/v1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      122 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/classification/v1/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20462 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/classification/v1/recipe.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2917 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18431 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/dag_help_strings.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17933 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/recipe.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/recipes/regression/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/regression/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/recipes/regression/v1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      114 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/regression/v1/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22495 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/regression/v1/recipe.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/recipes/resources/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12211 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/resources/recipe_dag_template.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14841 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/step.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/recipes/steps/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/steps/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/recipes/steps/automl/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/steps/automl/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6260 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/steps/automl/flaml.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20666 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/steps/evaluate.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/recipes/steps/ingest/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11137 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/steps/ingest/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26390 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/steps/ingest/datasets.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12140 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/steps/predict.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7664 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/steps/register.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19541 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/steps/split.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    59735 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/steps/train.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10602 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/steps/transform.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/recipes/utils/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6355 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/utils/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28468 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/utils/execution.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8990 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/utils/metrics.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7680 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/utils/step.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12316 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/utils/tracking.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1748 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/recipes/utils/wrapped_recipe_model.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/rfunc/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1115 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/rfunc/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3639 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/rfunc/backend.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2519 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/runs.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.947708 mlflow-skinny-2.4.2/mlflow/sagemaker/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   135083 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/sagemaker/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12986 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/sagemaker/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14450 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/sentence_transformers.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.951708 mlflow-skinny-2.4.2/mlflow/server/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7077 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/server/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.951708 mlflow-skinny-2.4.2/mlflow/server/auth/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28016 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/server/auth/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      123 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/server/auth/basic_auth.ini
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4689 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/server/auth/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/server/auth/config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4217 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/server/auth/entities.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2673 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/server/auth/logo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1267 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/server/auth/permissions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1111 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/server/auth/routes.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12648 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/server/auth/sqlalchemy_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    69738 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/server/handlers.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      481 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/server/prometheus_exporter.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26647 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/shap.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.951708 mlflow-skinny-2.4.2/mlflow/sklearn/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    85689 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/sklearn/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    37469 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/sklearn/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14259 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/spacy.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    45175 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/spark.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24781 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/statsmodels.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.951708 mlflow-skinny-2.4.2/mlflow/store/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      227 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.951708 mlflow-skinny-2.4.2/mlflow/store/_unity_catalog/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/_unity_catalog/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.951708 mlflow-skinny-2.4.2/mlflow/store/_unity_catalog/registry/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/_unity_catalog/registry/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    29936 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/_unity_catalog/registry/rest_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5419 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/_unity_catalog/registry/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.951708 mlflow-skinny-2.4.2/mlflow/store/artifact/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10481 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5836 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/artifact_repository_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8136 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/azure_blob_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5829 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/azure_data_lake_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5378 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35169 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/databricks_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9819 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/databricks_models_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10247 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/dbfs_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5234 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/ftp_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5873 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/gcs_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9684 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/hdfs_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3377 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/http_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5107 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/local_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3001 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/mlflow_artifacts_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6757 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/models_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6016 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/runs_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9433 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/s3_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5455 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/sftp_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5744 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/unity_catalog_models_artifact_repo.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.951708 mlflow-skinny-2.4.2/mlflow/store/artifact/utils/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/utils/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3926 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/artifact/utils/models.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.955708 mlflow-skinny-2.4.2/mlflow/store/db/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db/base_sql_model.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      221 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db/db_types.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10567 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.955708 mlflow-skinny-2.4.2/mlflow/store/db_migrations/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1634 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/alembic.ini
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2768 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/env.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.955708 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1990 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      462 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/0c779009ac13_add_deleted_time_field_to_runs_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      924 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2624 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1375 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1201 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      940 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1014 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      476 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/84291f40a231_add_run_link_to_model_version.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5716 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1666 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      577 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      582 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2830 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.955708 mlflow-skinny-2.4.2/mlflow/store/entities/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/entities/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      479 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/entities/paged_list.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.955708 mlflow-skinny-2.4.2/mlflow/store/model_registry/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      605 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/model_registry/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11022 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/model_registry/abstract_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1440 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/model_registry/base_rest_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1339 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/model_registry/databricks_workspace_model_registry_rest_store.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.955708 mlflow-skinny-2.4.2/mlflow/store/model_registry/dbmodels/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/model_registry/dbmodels/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/model_registry/dbmodels/models.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38833 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/model_registry/file_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16920 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/model_registry/rest_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50646 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/model_registry/sqlalchemy_store.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.959708 mlflow-skinny-2.4.2/mlflow/store/tracking/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1154 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/tracking/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13534 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/tracking/abstract_store.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.959708 mlflow-skinny-2.4.2/mlflow/store/tracking/dbmodels/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/tracking/dbmodels/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8315 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/tracking/dbmodels/initial_models.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21085 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/tracking/dbmodels/models.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52631 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/tracking/file_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12822 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/tracking/rest_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    77913 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/store/tracking/sqlalchemy_store.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.959708 mlflow-skinny-2.4.2/mlflow/tensorflow/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    60208 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tensorflow/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8442 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tensorflow/_autolog.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.959708 mlflow-skinny-2.4.2/mlflow/tracking/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      995 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.959708 mlflow-skinny-2.4.2/mlflow/tracking/_model_registry/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       41 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/_model_registry/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15534 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/_model_registry/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9641 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/_model_registry/fluent.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3152 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/_model_registry/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7178 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/_model_registry/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.959708 mlflow-skinny-2.4.2/mlflow/tracking/_tracking_service/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/_tracking_service/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24289 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/_tracking_service/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2335 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/_tracking_service/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9517 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/_tracking_service/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7540 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/artifact_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   142886 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.959708 mlflow-skinny-2.4.2/mlflow/tracking/context/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/context/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1076 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/context/abstract_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/context/databricks_cluster_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      561 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/context/databricks_command_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1965 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/context/databricks_job_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1713 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/context/databricks_notebook_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1952 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/context/databricks_repo_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/context/default_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      898 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/context/git_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3738 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/context/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      443 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/context/system_environment_context.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.959708 mlflow-skinny-2.4.2/mlflow/tracking/default_experiment/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       28 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/default_experiment/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1703 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/default_experiment/abstract_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2300 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3013 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/default_experiment/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    78452 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/fluent.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3404 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/llm_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2248 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/metric_value_conversion_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3515 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/registry.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.963708 mlflow-skinny-2.4.2/mlflow/tracking/request_header/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/request_header/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1077 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/request_header/abstract_request_header_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1336 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/request_header/databricks_request_header_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      486 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/request_header/default_request_header_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2867 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/tracking/request_header/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   110655 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/transformers.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.963708 mlflow-skinny-2.4.2/mlflow/types/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      299 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/types/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15035 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/types/schema.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18044 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/types/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.967708 mlflow-skinny-2.4.2/mlflow/utils/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9365 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6589 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/_capture_modules.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2274 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/_capture_transformers_modules.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6387 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/_spark_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5009 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/annotations.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/arguments_utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.967708 mlflow-skinny-2.4.2/mlflow/utils/autologging_utils/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27045 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/autologging_utils/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16642 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/autologging_utils/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10937 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/autologging_utils/events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13381 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/autologging_utils/logging_and_warnings.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    47266 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/autologging_utils/safety.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3570 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/autologging_utils/versioning.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      215 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/class_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6431 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/cli_args.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13002 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/conda.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      432 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/data_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23727 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/databricks_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9138 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/docstring_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1669 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/download_cloud_file_chunk.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/env.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/env_manager.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22634 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/environment.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30464 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/file_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2306 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/git_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24178 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/gorilla.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.967708 mlflow-skinny-2.4.2/mlflow/utils/import_hooks/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13645 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/import_hooks/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2597 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/logging_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/mime_type_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4024 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/mlflow_tags.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8689 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/model_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5873 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/name_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2412 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/nfs_on_spark.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      139 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/os.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5799 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/process.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19909 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/proto_json_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6217 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/request_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20034 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/requirements_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11852 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/rest_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    59666 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/search_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2368 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/server_cli_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3805 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/string_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      512 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/time_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14271 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/uri.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19435 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/validation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16278 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/utils/virtualenv.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      147 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/version.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.967708 mlflow-skinny-2.4.2/mlflow/xgboost/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    37317 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/xgboost/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2908 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/mlflow/xgboost/_autolog.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.971708 mlflow-skinny-2.4.2/mlflow_skinny.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11500 2023-07-10 06:27:58.000000 mlflow-skinny-2.4.2/mlflow_skinny.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14845 2023-07-10 06:27:58.000000 mlflow-skinny-2.4.2/mlflow_skinny.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 06:27:58.000000 mlflow-skinny-2.4.2/mlflow_skinny.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-07-10 06:27:58.000000 mlflow-skinny-2.4.2/mlflow_skinny.egg-info/entry_points.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 06:27:58.000000 mlflow-skinny-2.4.2/mlflow_skinny.egg-info/not-zip-safe
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      618 2023-07-10 06:27:58.000000 mlflow-skinny-2.4.2/mlflow_skinny.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-07-10 06:27:58.000000 mlflow-skinny-2.4.2/mlflow_skinny.egg-info/top_level.txt
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.971708 mlflow-skinny-2.4.2/pylint_plugins/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      614 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/pylint_plugins/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2234 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/pylint_plugins/errors.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4556 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/pylint_plugins/import_checker.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      856 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/pylint_plugins/print_function.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.971708 mlflow-skinny-2.4.2/pylint_plugins/pytest_raises_checker/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1546 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/pylint_plugins/pytest_raises_checker/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      571 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/pylint_plugins/set_checker.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      878 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/pylint_plugins/string_checker.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      692 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/pylint_plugins/unittest_assert_raises.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:27:58.971708 mlflow-skinny-2.4.2/requirements/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      609 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/requirements/core-requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      297 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/requirements/gateway-requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      481 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/requirements/skinny-requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-10 06:27:58.971708 mlflow-skinny-2.4.2/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7377 2023-07-10 06:27:57.000000 mlflow-skinny-2.4.2/setup.py
```

### Comparing `mlflow-skinny-2.4.1/LICENSE.txt` & `mlflow-skinny-2.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/MANIFEST.in` & `mlflow-skinny-2.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/PKG-INFO` & `mlflow-skinny-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-skinny
-Version: 2.4.1
+Version: 2.4.2
 Summary: MLflow: A Platform for ML Development and Productionization
 Home-page: https://mlflow.org/
 Author: Databricks
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mlflow/mlflow/issues
 Project-URL: Documentation, https://mlflow.org/docs/latest/index.html
 Project-URL: Source Code, https://github.com/mlflow/mlflow
```

### Comparing `mlflow-skinny-2.4.1/README.rst` & `mlflow-skinny-2.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/README_SKINNY.rst` & `mlflow-skinny-2.4.2/README_SKINNY.rst`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/__init__.py` & `mlflow-skinny-2.4.2/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/_doctor.py` & `mlflow-skinny-2.4.2/mlflow/_doctor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/_spark_autologging.py` & `mlflow-skinny-2.4.2/mlflow/_spark_autologging.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/artifacts/__init__.py` & `mlflow-skinny-2.4.2/mlflow/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/azure/client.py` & `mlflow-skinny-2.4.2/mlflow/azure/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/catboost.py` & `mlflow-skinny-2.4.2/mlflow/catboost.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/cli.py` & `mlflow-skinny-2.4.2/mlflow/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/__init__.py` & `mlflow-skinny-2.4.2/mlflow/data/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/artifact_dataset_sources.py` & `mlflow-skinny-2.4.2/mlflow/data/artifact_dataset_sources.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/code_dataset_source.py` & `mlflow-skinny-2.4.2/mlflow/data/code_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/dataset.py` & `mlflow-skinny-2.4.2/mlflow/data/dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/dataset_registry.py` & `mlflow-skinny-2.4.2/mlflow/data/dataset_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/dataset_source.py` & `mlflow-skinny-2.4.2/mlflow/data/dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/dataset_source_registry.py` & `mlflow-skinny-2.4.2/mlflow/data/dataset_source_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/delta_dataset_source.py` & `mlflow-skinny-2.4.2/mlflow/data/delta_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/digest_utils.py` & `mlflow-skinny-2.4.2/mlflow/data/digest_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/filesystem_dataset_source.py` & `mlflow-skinny-2.4.2/mlflow/data/filesystem_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/http_dataset_source.py` & `mlflow-skinny-2.4.2/mlflow/data/http_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/huggingface_dataset.py` & `mlflow-skinny-2.4.2/mlflow/data/huggingface_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/huggingface_dataset_source.py` & `mlflow-skinny-2.4.2/mlflow/data/huggingface_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/numpy_dataset.py` & `mlflow-skinny-2.4.2/mlflow/data/numpy_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/pandas_dataset.py` & `mlflow-skinny-2.4.2/mlflow/data/pandas_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/pyfunc_dataset_mixin.py` & `mlflow-skinny-2.4.2/mlflow/data/pyfunc_dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/schema.py` & `mlflow-skinny-2.4.2/mlflow/data/schema.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/spark_dataset.py` & `mlflow-skinny-2.4.2/mlflow/data/spark_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/spark_dataset_source.py` & `mlflow-skinny-2.4.2/mlflow/data/spark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/spark_delta_utils.py` & `mlflow-skinny-2.4.2/mlflow/data/spark_delta_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/data/tensorflow_dataset.py` & `mlflow-skinny-2.4.2/mlflow/data/tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/db.py` & `mlflow-skinny-2.4.2/mlflow/db.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/deployments/__init__.py` & `mlflow-skinny-2.4.2/mlflow/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/deployments/base.py` & `mlflow-skinny-2.4.2/mlflow/deployments/base.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/deployments/cli.py` & `mlflow-skinny-2.4.2/mlflow/deployments/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/deployments/interface.py` & `mlflow-skinny-2.4.2/mlflow/deployments/interface.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/deployments/plugin_manager.py` & `mlflow-skinny-2.4.2/mlflow/deployments/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/deployments/utils.py` & `mlflow-skinny-2.4.2/mlflow/deployments/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/diviner.py` & `mlflow-skinny-2.4.2/mlflow/diviner.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/__init__.py` & `mlflow-skinny-2.4.2/mlflow/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/_mlflow_object.py` & `mlflow-skinny-2.4.2/mlflow/entities/_mlflow_object.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/dataset.py` & `mlflow-skinny-2.4.2/mlflow/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/dataset_input.py` & `mlflow-skinny-2.4.2/mlflow/entities/dataset_input.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/experiment.py` & `mlflow-skinny-2.4.2/mlflow/entities/experiment.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/experiment_tag.py` & `mlflow-skinny-2.4.2/mlflow/entities/experiment_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/file_info.py` & `mlflow-skinny-2.4.2/mlflow/entities/file_info.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/input_tag.py` & `mlflow-skinny-2.4.2/mlflow/entities/input_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/lifecycle_stage.py` & `mlflow-skinny-2.4.2/mlflow/entities/lifecycle_stage.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/metric.py` & `mlflow-skinny-2.4.2/mlflow/entities/metric.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/model_registry/__init__.py` & `mlflow-skinny-2.4.2/mlflow/entities/model_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version.py` & `mlflow-skinny-2.4.2/mlflow/entities/model_registry/model_version.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version_stages.py` & `mlflow-skinny-2.4.2/mlflow/entities/model_registry/model_version_stages.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version_status.py` & `mlflow-skinny-2.4.2/mlflow/entities/model_registry/model_version_status.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version_tag.py` & `mlflow-skinny-2.4.2/mlflow/entities/model_registry/model_version_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/model_registry/registered_model.py` & `mlflow-skinny-2.4.2/mlflow/entities/model_registry/registered_model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/model_registry/registered_model_alias.py` & `mlflow-skinny-2.4.2/mlflow/entities/model_registry/registered_model_alias.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/model_registry/registered_model_tag.py` & `mlflow-skinny-2.4.2/mlflow/entities/model_registry/registered_model_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/param.py` & `mlflow-skinny-2.4.2/mlflow/entities/param.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/run.py` & `mlflow-skinny-2.4.2/mlflow/entities/run.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/run_data.py` & `mlflow-skinny-2.4.2/mlflow/entities/run_data.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/run_info.py` & `mlflow-skinny-2.4.2/mlflow/entities/run_info.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/run_inputs.py` & `mlflow-skinny-2.4.2/mlflow/entities/run_inputs.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/run_status.py` & `mlflow-skinny-2.4.2/mlflow/entities/run_status.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/run_tag.py` & `mlflow-skinny-2.4.2/mlflow/entities/run_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/source_type.py` & `mlflow-skinny-2.4.2/mlflow/entities/source_type.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/entities/view_type.py` & `mlflow-skinny-2.4.2/mlflow/entities/view_type.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/environment_variables.py` & `mlflow-skinny-2.4.2/mlflow/environment_variables.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/exceptions.py` & `mlflow-skinny-2.4.2/mlflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/experiments.py` & `mlflow-skinny-2.4.2/mlflow/experiments.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/fastai/__init__.py` & `mlflow-skinny-2.4.2/mlflow/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/fastai/callback.py` & `mlflow-skinny-2.4.2/mlflow/fastai/callback.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/gluon/__init__.py` & `mlflow-skinny-2.4.2/mlflow/gluon/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/gluon/_autolog.py` & `mlflow-skinny-2.4.2/mlflow/gluon/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/h2o.py` & `mlflow-skinny-2.4.2/mlflow/h2o.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/johnsnowlabs.py` & `mlflow-skinny-2.4.2/mlflow/johnsnowlabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 """
 The ``mlflow.johnsnowlabs`` module provides an API for logging and loading Spark NLP and NLU models.
 This module exports the following flavors:
 
-The flavor gives you access to `20.000+ state-of-the-art enterprise NLP models in 200+ languages
+Johnsnowlabs (native) format
+    Allows models to be loaded as Spark Transformers for scoring in a Spark session.
+    Models with this flavor can be loaded as NluPipelines, with underlying Spark MLlib PipelineModel
+    This is the main flavor and is always produced.
+:py:mod:`mlflow.pyfunc`
+    Supports deployment outside of Spark by instantiating a SparkContext and reading
+    input data as a Spark DataFrame prior to scoring. Also supports deployment in Spark
+    as a Spark UDF. Models with this flavor can be loaded as Python functions
+    for performing inference. This flavor is always produced.
+
+This flavor gives you access to `20.000+ state-of-the-art enterprise NLP models in 200+ languages
 <https://nlp.johnsnowlabs.com/models>`_ for medical, finance, legal and many more domains.
 Features include: LLM's, Text Summarization, Question Answering, Named Entity Recognition, Relation
 Extration, Sentiment Analysis, Spell Checking, Image Classification, Automatic Speech Recognition
-powered by the latest Transformer Architectures. The models are provided by `John Snow Labs
-<https://www.johnsnowlabs.com/>`_ and requires a `John Snow Labs <https://www.johnsnowlabs.com/>`
-Enterprise NLP License. `You can reach out to us <https://www.johnsnowlabs.com/schedule-a-demo/>
-for a research or industry license.
-
-These keys must be present in your license json
-- ``SECRET``: The secret for the John Snow Labs Enterprise NLP Library
-- ``SPARK_NLP_LICENSE``: Your John Snow Labs Enterprise NLP License
-- ``AWS_ACCESS_KEY_ID``: Your AWS Secret ID for accessing John Snow Labs Enterprise Models
-- ``AWS_SECRET_ACCESS_KEY``: Your AWS Secret key for accessing John Snow Labs Enterprise Models
+and much more, powered by the latest Transformer Architectures. The models are provided by
+`John Snow Labs <https://www.johnsnowlabs.com/>`_ and requires a `John Snow Labs
+<https://www.johnsnowlabs.com/>`_ Enterprise NLP License. `You can reach out to us
+<https://www.johnsnowlabs.com/schedule-a-demo/>`_ for a research or industry license.
+
+These keys must be present in your license json:
+
+1. ``SECRET``: The secret for the John Snow Labs Enterprise NLP Library
+2. ``SPARK_NLP_LICENSE``: Your John Snow Labs Enterprise NLP License
+3. ``AWS_ACCESS_KEY_ID``: Your AWS Secret ID for accessing John Snow Labs Enterprise Models
+4. ``AWS_SECRET_ACCESS_KEY``: Your AWS Secret key for accessing John Snow Labs Enterprise Models
 
-You can set them like this in Python
+You can set them using the following code:
 
 .. code-block:: python
 
     import os
     import json
 
     # Write your raw license.json string into the 'JOHNSNOWLABS_LICENSE_JSON' env variable
     creds = {
         "AWS_ACCESS_KEY_ID": "...",
         "AWS_SECRET_ACCESS_KEY": "...",
         "SPARK_NLP_LICENSE": "...",
         "SECRET": "...",
     }
     os.environ["JOHNSNOWLABS_LICENSE_JSON"] = json.dumps(creds)
-
-Johnsnowlabs (native) format
-    Allows models to be loaded as Spark Transformers for scoring in a Spark session.
-    Models with this flavor can be loaded as NluPipelines, with underlying Spark MLlib PipelineModel
-    This is the main flavor and is always produced.
-:py:mod:`mlflow.pyfunc`
-    Supports deployment outside of Spark by instantiating a SparkContext and reading
-    input data as a Spark DataFrame prior to scoring. Also supports deployment in Spark
-    as a Spark UDF. Models with this flavor can be loaded as Python functions
-    for performing inference. This flavor is always produced.
-:py:mod:`mlflow.mleap`
-    Enables high-performance deployment outside of Spark by leveraging MLeap's
-    custom dataframe and pipeline representations. Models with this flavor *cannot* be loaded
-    back as Python objects. Rather, they must be deserialized in Java using the
-    ``mlflow/java`` package. This flavor is produced only if you specify
-    MLeap-compatible arguments.
 """
 import json
 import logging
 import os
 import posixpath
 import shutil
 import sys
@@ -178,38 +173,40 @@
     await_registration_for=DEFAULT_AWAIT_MAX_SLEEP_SECONDS,
     pip_requirements=None,
     extra_pip_requirements=None,
     metadata=None,
     store_license=False,
 ):
     """
-    Log a ``Johnsnowlabs NLUPipeline`` (created via ``nlp.load()``) model as an MLflow artifact for
-    the current run. This uses the MLlib persistence format and produces an MLflow Model with the
-    ``Johnsnowlabs`` flavor.
+    Log a ``Johnsnowlabs NLUPipeline`` created via `nlp.load()
+    <https://nlp.johnsnowlabs.com/docs/en/jsl/load_api>`_, as an MLflow artifact for the current
+    run. This uses the MLlib persistence format and produces an MLflow Model with the
+    ``johnsnowlabs`` flavor.
 
     Note: If no run is active, it will instantiate a run to obtain a run_id.
 
-    :param spark_model: NLUPipeline obtained via ``nlp.load()``
-    :param store_license: If True, the license will be stored with the model and used and
-                          re-loading it.
+    :param spark_model: NLUPipeline obtained via `nlp.load()
+                        <https://nlp.johnsnowlabs.com/docs/en/jsl/load_api>`_
+    :param store_license: If True, the license will be stored with the model and used and re-loading
+                          it.
     :param artifact_path: Run relative artifact path.
     :param conda_env: Either a dictionary representation of a Conda environment or the path to a
                       Conda environment yaml file. If provided, this describes the environment
                       this model should be run in. At minimum, it should specify the dependencies
                       contained in :func:`get_default_conda_env()`. If `None`, the default
                       :func:`get_default_conda_env()` environment is added to the model.
                       The following is an *example* dictionary representation of a Conda
                       environment::
 
                         {
                             'name': 'mlflow-env',
                             'channels': ['defaults'],
                             'dependencies': [
                                 'python=3.8.15',
-                                'johnsnowlabs=4.4.6'
+                                'johnsnowlabs'
                             ]
                         }
     :param dfs_tmpdir: Temporary directory path on Distributed (Hadoop) File System (DFS) or local
                        filesystem if running in local mode. The model is written in this
                        destination and then copied into the model's artifact directory. This is
                        necessary as Spark ML models read from and write to DFS if running on a
                        cluster. If this operation completes successfully, all temporary files
@@ -484,17 +481,17 @@
 
     By default, this function saves models using the Spark MLlib persistence mechanism.
     Additionally, if a sample input is specified using the ``sample_input`` parameter, the model
     is also serialized in MLeap format and the MLeap flavor is added.
 
     :param store_license: If True, the license will be stored with the model and used and
                           re-loading it.
-    :param spark_model: Spark model to be saved - MLflow can only save descendants of
-                        pyspark.ml.Model or pyspark.ml.Transformer which implement
-                        MLReadable and MLWritable.
+    :param spark_model: Either a pyspark.ml.pipeline.PipelineModel or nlu.NLUPipeline object to be
+                        saved. `Every johnsnowlabs model <https://nlp.johnsnowlabs.com/models>`_
+                        is a PipelineModel and loadable as nlu.NLUPipeline.
     :param path: Local path where the model is to be saved.
     :param mlflow_model: MLflow model config this flavor is being added to.
     :param conda_env: Either a dictionary representation of a Conda environment or the path to a
                       Conda environment yaml file. If provided, this describes the environment
                       this model should be run in. At minimum, it should specify the dependencies
                       contained in :func:`get_default_conda_env()`. If `None`, the default
                       :func:`get_default_conda_env()` environment is added to the model.
@@ -502,15 +499,15 @@
                       environment::
 
                         {
                             'name': 'mlflow-env',
                             'channels': ['defaults'],
                             'dependencies': [
                                 'python=3.8.15',
-                                'johnsnowlabs=4.4.6'
+                                'johnsnowlabs'
                             ]
                         }
     :param dfs_tmpdir: Temporary directory path on Distributed (Hadoop) File System (DFS) or local
                        filesystem if running in local mode. The model is be written in this
                        destination and then copied to the requested local path. This is necessary
                        as Spark ML models read from and write to DFS if running on a cluster. All
                        temporary files created on the DFS are removed if this operation
@@ -543,14 +540,15 @@
     :param metadata: Custom metadata dictionary passed to the model and stored in the MLmodel file.
 
                      .. Note:: Experimental: This parameter may change or be removed in a future
                                              release without warning.
 
     .. code-block:: python
         :caption: Example
+
         from johnsnowlabs import nlp
         import mlflow
         import os
 
         # Write your raw license.json string into the 'JOHNSNOWLABS_LICENSE_JSON' env variable
         creds = {
             "AWS_ACCESS_KEY_ID": "...",
@@ -665,18 +663,19 @@
                       artifact-locations>`_.
     :param dfs_tmpdir: Temporary directory path on Distributed (Hadoop) File System (DFS) or local
                        filesystem if running in local mode. The model is loaded from this
                        destination. Defaults to ``/tmp/mlflow``.
     :param dst_path: The local filesystem path to which to download the model artifact.
                      This directory must already exist. If unspecified, a local output
                      path will be created.
-    :return: nlu.NLUPipeline
+    :return: `nlu.NLUPipeline <https://nlp.johnsnowlabs.com/docs/en/jsl/predict_api>`_
 
     .. code-block:: python
         :caption: Example
+
         import mlflow
         from johnsnowlabs import nlp
         import os
 
         # Write your raw license.json string into the 'JOHNSNOWLABS_LICENSE_JSON' env variable
         creds = {
             "AWS_ACCESS_KEY_ID": "...",
```

### Comparing `mlflow-skinny-2.4.1/mlflow/langchain/__init__.py` & `mlflow-skinny-2.4.2/mlflow/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/langchain/api_request_parallel_processor.py` & `mlflow-skinny-2.4.2/mlflow/langchain/api_request_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/lightgbm.py` & `mlflow-skinny-2.4.2/mlflow/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/ml_package_versions.py` & `mlflow-skinny-2.4.2/mlflow/ml_package_versions.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/mleap.py` & `mlflow-skinny-2.4.2/mlflow/mleap.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/__init__.py` & `mlflow-skinny-2.4.2/mlflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/cli.py` & `mlflow-skinny-2.4.2/mlflow/models/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/container/__init__.py` & `mlflow-skinny-2.4.2/mlflow/models/container/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/docker_utils.py` & `mlflow-skinny-2.4.2/mlflow/models/docker_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/evaluation/_shap_patch.py` & `mlflow-skinny-2.4.2/mlflow/models/evaluation/_shap_patch.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/evaluation/artifacts.py` & `mlflow-skinny-2.4.2/mlflow/models/evaluation/artifacts.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/evaluation/base.py` & `mlflow-skinny-2.4.2/mlflow/models/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/evaluation/default_evaluator.py` & `mlflow-skinny-2.4.2/mlflow/models/evaluation/default_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/evaluation/evaluator_registry.py` & `mlflow-skinny-2.4.2/mlflow/models/evaluation/evaluator_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/evaluation/lift_curve.py` & `mlflow-skinny-2.4.2/mlflow/models/evaluation/lift_curve.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/evaluation/validation.py` & `mlflow-skinny-2.4.2/mlflow/models/evaluation/validation.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/flavor_backend.py` & `mlflow-skinny-2.4.2/mlflow/models/flavor_backend.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/flavor_backend_registry.py` & `mlflow-skinny-2.4.2/mlflow/models/flavor_backend_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/model.py` & `mlflow-skinny-2.4.2/mlflow/models/model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/signature.py` & `mlflow-skinny-2.4.2/mlflow/models/signature.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/utils.py` & `mlflow-skinny-2.4.2/mlflow/models/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/models/wheeled_model.py` & `mlflow-skinny-2.4.2/mlflow/models/wheeled_model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/onnx.py` & `mlflow-skinny-2.4.2/mlflow/onnx.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/openai/__init__.py` & `mlflow-skinny-2.4.2/mlflow/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/openai/api_request_parallel_processor.py` & `mlflow-skinny-2.4.2/mlflow/openai/api_request_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/openai/retry.py` & `mlflow-skinny-2.4.2/mlflow/openai/retry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/openai/utils.py` & `mlflow-skinny-2.4.2/mlflow/openai/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/paddle/__init__.py` & `mlflow-skinny-2.4.2/mlflow/paddle/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/paddle/_paddle_autolog.py` & `mlflow-skinny-2.4.2/mlflow/paddle/_paddle_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pmdarima.py` & `mlflow-skinny-2.4.2/mlflow/pmdarima.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/projects/__init__.py` & `mlflow-skinny-2.4.2/mlflow/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/projects/_project_spec.py` & `mlflow-skinny-2.4.2/mlflow/projects/_project_spec.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/projects/backend/abstract_backend.py` & `mlflow-skinny-2.4.2/mlflow/projects/backend/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/projects/backend/loader.py` & `mlflow-skinny-2.4.2/mlflow/projects/backend/loader.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/projects/backend/local.py` & `mlflow-skinny-2.4.2/mlflow/projects/backend/local.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/projects/databricks.py` & `mlflow-skinny-2.4.2/mlflow/projects/databricks.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/projects/docker.py` & `mlflow-skinny-2.4.2/mlflow/projects/docker.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/projects/kubernetes.py` & `mlflow-skinny-2.4.2/mlflow/projects/kubernetes.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/projects/submitted_run.py` & `mlflow-skinny-2.4.2/mlflow/projects/submitted_run.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/projects/utils.py` & `mlflow-skinny-2.4.2/mlflow/projects/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/prophet.py` & `mlflow-skinny-2.4.2/mlflow/prophet.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/protos/databricks_artifacts_pb2.py` & `mlflow-skinny-2.4.2/mlflow/protos/databricks_artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/protos/databricks_pb2.py` & `mlflow-skinny-2.4.2/mlflow/protos/databricks_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/protos/databricks_uc_registry_messages_pb2.py` & `mlflow-skinny-2.4.2/mlflow/protos/databricks_uc_registry_messages_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from .scalapb import scalapb_pb2 as scalapb_dot_scalapb__pb2
 from . import databricks_pb2 as databricks__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%databricks_uc_registry_messages.proto\x12\x16mlflow.ucmodelregistry\x1a\x15scalapb/scalapb.proto\x1a\x10\x64\x61tabricks.proto\"\xc0\x01\n\x0fRegisteredModel\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1a\n\x12\x63reation_timestamp\x18\x02 \x01(\x03\x12\x1e\n\x16last_updated_timestamp\x18\x03 \x01(\x03\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12=\n\x07\x61liases\x18\x06 \x03(\x0b\x32,.mlflow.ucmodelregistry.RegisteredModelAlias\"6\n\x14RegisteredModelAlias\x12\r\n\x05\x61lias\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"\x97\x03\n\x0cModelVersion\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x1a\n\x12\x63reation_timestamp\x18\x03 \x01(\x03\x12\x1e\n\x16last_updated_timestamp\x18\x04 \x01(\x03\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x0e\n\x06source\x18\x07 \x01(\t\x12\x0e\n\x06run_id\x18\x08 \x01(\t\x12\x19\n\x11run_experiment_id\x18\t \x01(\t\x12\x1e\n\x16run_tracking_server_id\x18\n \x01(\t\x12:\n\x06status\x18\x0b \x01(\x0e\x32*.mlflow.ucmodelregistry.ModelVersionStatus\x12\x16\n\x0estatus_message\x18\x0c \x01(\t\x12\x18\n\x10storage_location\x18\r \x01(\t\x12=\n\x07\x61liases\x18\x0e \x03(\x0b\x32,.mlflow.ucmodelregistry.RegisteredModelAlias\"\x9d\x02\n\x14TemporaryCredentials\x12\x46\n\x14\x61ws_temp_credentials\x18\x02 \x01(\x0b\x32&.mlflow.ucmodelregistry.AwsCredentialsH\x00\x12S\n\x19\x61zure_user_delegation_sas\x18\x03 \x01(\x0b\x32..mlflow.ucmodelregistry.AzureUserDelegationSASH\x00\x12@\n\x0fgcp_oauth_token\x18\x04 \x01(\x0b\x32%.mlflow.ucmodelregistry.GcpOauthTokenH\x00\x12\x17\n\x0f\x65xpiration_time\x18\x01 \x01(\x03\x42\r\n\x0b\x63redentials\"Y\n\x0e\x41wsCredentials\x12\x15\n\raccess_key_id\x18\x01 \x01(\t\x12\x19\n\x11secret_access_key\x18\x02 \x01(\t\x12\x15\n\rsession_token\x18\x03 \x01(\t\"+\n\x16\x41zureUserDelegationSAS\x12\x11\n\tsas_token\x18\x01 \x01(\t\"$\n\rGcpOauthToken\x12\x13\n\x0boauth_token\x18\x01 \x01(\t\"\x83\x01\n\x1c\x43reateRegisteredModelRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t::\xe2?7\n5com.databricks.rpc.RPC[CreateRegisteredModelResponse]\"b\n\x1d\x43reateRegisteredModelResponse\x12\x41\n\x10registered_model\x18\x01 \x01(\x0b\x32\'.mlflow.ucmodelregistry.RegisteredModel\"\x83\x01\n\x1cUpdateRegisteredModelRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t::\xe2?7\n5com.databricks.rpc.RPC[UpdateRegisteredModelResponse]\"b\n\x1dUpdateRegisteredModelResponse\x12\x41\n\x10registered_model\x18\x01 \x01(\x0b\x32\'.mlflow.ucmodelregistry.RegisteredModel\"n\n\x1c\x44\x65leteRegisteredModelRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01::\xe2?7\n5com.databricks.rpc.RPC[DeleteRegisteredModelResponse]\"\x1f\n\x1d\x44\x65leteRegisteredModelResponse\"h\n\x19GetRegisteredModelRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01:7\xe2?4\n2com.databricks.rpc.RPC[GetRegisteredModelResponse]\"_\n\x1aGetRegisteredModelResponse\x12\x41\n\x10registered_model\x18\x01 \x01(\x0b\x32\'.mlflow.ucmodelregistry.RegisteredModel\"\x8a\x01\n\x1dSearchRegisteredModelsRequest\x12\x18\n\x0bmax_results\x18\x01 \x01(\x03:\x03\x31\x30\x30\x12\x12\n\npage_token\x18\x02 \x01(\t:;\xe2?8\n6com.databricks.rpc.RPC[SearchRegisteredModelsResponse]\"}\n\x1eSearchRegisteredModelsResponse\x12\x42\n\x11registered_models\x18\x01 \x03(\x0b\x32\'.mlflow.ucmodelregistry.RegisteredModel\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xc3\x01\n\x19\x43reateModelVersionRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x14\n\x06source\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01\x12\x0e\n\x06run_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x1e\n\x16run_tracking_server_id\x18\x05 \x01(\t:7\xe2?4\n2com.databricks.rpc.RPC[CreateModelVersionResponse]\"Y\n\x1a\x43reateModelVersionResponse\x12;\n\rmodel_version\x18\x01 \x01(\x0b\x32$.mlflow.ucmodelregistry.ModelVersion\"\x94\x01\n\x19UpdateModelVersionRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t:7\xe2?4\n2com.databricks.rpc.RPC[UpdateModelVersionResponse]\"Y\n\x1aUpdateModelVersionResponse\x12;\n\rmodel_version\x18\x01 \x01(\x0b\x32$.mlflow.ucmodelregistry.ModelVersion\"\x7f\n\x19\x44\x65leteModelVersionRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01:7\xe2?4\n2com.databricks.rpc.RPC[DeleteModelVersionResponse]\"\x1c\n\x1a\x44\x65leteModelVersionResponse\"y\n\x16GetModelVersionRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01:4\xe2?1\n/com.databricks.rpc.RPC[GetModelVersionResponse]\"V\n\x17GetModelVersionResponse\x12;\n\rmodel_version\x18\x01 \x01(\x0b\x32$.mlflow.ucmodelregistry.ModelVersion\"\x96\x01\n\x1aSearchModelVersionsRequest\x12\x0e\n\x06\x66ilter\x18\x01 \x01(\t\x12\x1a\n\x0bmax_results\x18\x02 \x01(\x03:\x05\x31\x30\x30\x30\x30\x12\x12\n\npage_token\x18\x03 \x01(\t:8\xe2?5\n3com.databricks.rpc.RPC[SearchModelVersionsResponse]\"t\n\x1bSearchModelVersionsResponse\x12<\n\x0emodel_versions\x18\x01 \x03(\x0b\x32$.mlflow.ucmodelregistry.ModelVersion\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xf3\x01\n/GenerateTemporaryModelVersionCredentialsRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01\x12\x46\n\toperation\x18\x03 \x01(\x0e\x32-.mlflow.ucmodelregistry.ModelVersionOperationB\x04\xf8\x86\x19\x01:M\xe2?J\nHcom.databricks.rpc.RPC[GenerateTemporaryModelVersionCredentialsResponse]\"u\n0GenerateTemporaryModelVersionCredentialsResponse\x12\x41\n\x0b\x63redentials\x18\x01 \x01(\x0b\x32,.mlflow.ucmodelregistry.TemporaryCredentials\"\x8f\x01\n!GetModelVersionDownloadUriRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01:?\xe2?<\n:com.databricks.rpc.RPC[GetModelVersionDownloadUriResponse]\":\n\"GetModelVersionDownloadUriResponse\x12\x14\n\x0c\x61rtifact_uri\x18\x01 \x01(\t\"\x83\x01\n\x1b\x46inalizeModelVersionRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01:9\xe2?6\n4com.databricks.rpc.RPC[FinalizeModelVersionResponse]\"[\n\x1c\x46inalizeModelVersionResponse\x12;\n\rmodel_version\x18\x01 \x01(\x0b\x32$.mlflow.ucmodelregistry.ModelVersion\"\x9e\x01\n\x1eSetRegisteredModelAliasRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x13\n\x05\x61lias\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x03 \x01(\tB\x04\xf8\x86\x19\x01:<\xe2?9\n7com.databricks.rpc.RPC[SetRegisteredModelAliasResponse]\"!\n\x1fSetRegisteredModelAliasResponse\"\x8d\x01\n!DeleteRegisteredModelAliasRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x13\n\x05\x61lias\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01:?\xe2?<\n:com.databricks.rpc.RPC[DeleteRegisteredModelAliasResponse]\"$\n\"DeleteRegisteredModelAliasResponse\"\x85\x01\n\x1dGetModelVersionByAliasRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x13\n\x05\x61lias\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01:;\xe2?8\n6com.databricks.rpc.RPC[GetModelVersionByAliasResponse]\"]\n\x1eGetModelVersionByAliasResponse\x12;\n\rmodel_version\x18\x01 \x01(\x0b\x32$.mlflow.ucmodelregistry.ModelVersion\"\xa9\x01\n\x06\x45ntity\x12*\n\x03job\x18\x01 \x01(\x0b\x32\x1b.mlflow.ucmodelregistry.JobH\x00\x12\x34\n\x08notebook\x18\x02 \x01(\x0b\x32 .mlflow.ucmodelregistry.NotebookH\x00\x12\x34\n\x08pipeline\x18\x03 \x01(\x0b\x32 .mlflow.ucmodelregistry.PipelineH\x00\x42\x07\n\x05value\";\n\x08Pipeline\x12\x13\n\x0bpipeline_id\x18\x01 \x01(\t\x12\x1a\n\x12pipeline_update_id\x18\x02 \x01(\t\"L\n\x03Job\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08task_key\x18\x02 \x01(\t\x12\x12\n\njob_run_id\x18\x03 \x01(\t\x12\x13\n\x0btask_run_id\x18\x04 \x01(\t\"C\n\x08Notebook\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\ncommand_id\x18\x02 \x01(\t\x12\x17\n\x0fnotebook_run_id\x18\x03 \x01(\t\"E\n\x11LineageHeaderInfo\x12\x30\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x1e.mlflow.ucmodelregistry.Entity*c\n\x12ModelVersionStatus\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x18\n\x14PENDING_REGISTRATION\x10\x01\x12\x17\n\x13\x46\x41ILED_REGISTRATION\x10\x02\x12\t\n\x05READY\x10\x03*\x8a\x01\n\x15ModelVersionOperation\x12\'\n#MODEL_VERSION_OPERATION_UNSPECIFIED\x10\x00\x12 \n\x1cMODEL_VERSION_OPERATION_READ\x10\x01\x12&\n\"MODEL_VERSION_OPERATION_READ_WRITE\x10\x02\x42\x32\n(com.databricks.api.proto.ucmodelregistry\xa0\x01\x01\xe2?\x02\x10\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%databricks_uc_registry_messages.proto\x12\x16mlflow.ucmodelregistry\x1a\x15scalapb/scalapb.proto\x1a\x10\x64\x61tabricks.proto\"\xc0\x01\n\x0fRegisteredModel\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1a\n\x12\x63reation_timestamp\x18\x02 \x01(\x03\x12\x1e\n\x16last_updated_timestamp\x18\x03 \x01(\x03\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12=\n\x07\x61liases\x18\x06 \x03(\x0b\x32,.mlflow.ucmodelregistry.RegisteredModelAlias\"6\n\x14RegisteredModelAlias\x12\r\n\x05\x61lias\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"\x97\x03\n\x0cModelVersion\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x1a\n\x12\x63reation_timestamp\x18\x03 \x01(\x03\x12\x1e\n\x16last_updated_timestamp\x18\x04 \x01(\x03\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x0e\n\x06source\x18\x07 \x01(\t\x12\x0e\n\x06run_id\x18\x08 \x01(\t\x12\x19\n\x11run_experiment_id\x18\t \x01(\t\x12\x1e\n\x16run_tracking_server_id\x18\n \x01(\t\x12:\n\x06status\x18\x0b \x01(\x0e\x32*.mlflow.ucmodelregistry.ModelVersionStatus\x12\x16\n\x0estatus_message\x18\x0c \x01(\t\x12\x18\n\x10storage_location\x18\r \x01(\t\x12=\n\x07\x61liases\x18\x0e \x03(\x0b\x32,.mlflow.ucmodelregistry.RegisteredModelAlias\"\x9d\x02\n\x14TemporaryCredentials\x12\x46\n\x14\x61ws_temp_credentials\x18\x02 \x01(\x0b\x32&.mlflow.ucmodelregistry.AwsCredentialsH\x00\x12S\n\x19\x61zure_user_delegation_sas\x18\x03 \x01(\x0b\x32..mlflow.ucmodelregistry.AzureUserDelegationSASH\x00\x12@\n\x0fgcp_oauth_token\x18\x04 \x01(\x0b\x32%.mlflow.ucmodelregistry.GcpOauthTokenH\x00\x12\x17\n\x0f\x65xpiration_time\x18\x01 \x01(\x03\x42\r\n\x0b\x63redentials\"Y\n\x0e\x41wsCredentials\x12\x15\n\raccess_key_id\x18\x01 \x01(\t\x12\x19\n\x11secret_access_key\x18\x02 \x01(\t\x12\x15\n\rsession_token\x18\x03 \x01(\t\"+\n\x16\x41zureUserDelegationSAS\x12\x11\n\tsas_token\x18\x01 \x01(\t\"$\n\rGcpOauthToken\x12\x13\n\x0boauth_token\x18\x01 \x01(\t\"\x83\x01\n\x1c\x43reateRegisteredModelRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t::\xe2?7\n5com.databricks.rpc.RPC[CreateRegisteredModelResponse]\"b\n\x1d\x43reateRegisteredModelResponse\x12\x41\n\x10registered_model\x18\x01 \x01(\x0b\x32\'.mlflow.ucmodelregistry.RegisteredModel\"\x83\x01\n\x1cUpdateRegisteredModelRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t::\xe2?7\n5com.databricks.rpc.RPC[UpdateRegisteredModelResponse]\"b\n\x1dUpdateRegisteredModelResponse\x12\x41\n\x10registered_model\x18\x01 \x01(\x0b\x32\'.mlflow.ucmodelregistry.RegisteredModel\"n\n\x1c\x44\x65leteRegisteredModelRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01::\xe2?7\n5com.databricks.rpc.RPC[DeleteRegisteredModelResponse]\"\x1f\n\x1d\x44\x65leteRegisteredModelResponse\"h\n\x19GetRegisteredModelRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01:7\xe2?4\n2com.databricks.rpc.RPC[GetRegisteredModelResponse]\"_\n\x1aGetRegisteredModelResponse\x12\x41\n\x10registered_model\x18\x01 \x01(\x0b\x32\'.mlflow.ucmodelregistry.RegisteredModel\"\x8a\x01\n\x1dSearchRegisteredModelsRequest\x12\x18\n\x0bmax_results\x18\x01 \x01(\x03:\x03\x31\x30\x30\x12\x12\n\npage_token\x18\x02 \x01(\t:;\xe2?8\n6com.databricks.rpc.RPC[SearchRegisteredModelsResponse]\"}\n\x1eSearchRegisteredModelsResponse\x12\x42\n\x11registered_models\x18\x01 \x03(\x0b\x32\'.mlflow.ucmodelregistry.RegisteredModel\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xd9\x01\n\x19\x43reateModelVersionRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x14\n\x06source\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01\x12\x0e\n\x06run_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x1e\n\x16run_tracking_server_id\x18\x05 \x01(\t\x12\x14\n\x0c\x66\x65\x61ture_deps\x18\x06 \x01(\t:7\xe2?4\n2com.databricks.rpc.RPC[CreateModelVersionResponse]\"Y\n\x1a\x43reateModelVersionResponse\x12;\n\rmodel_version\x18\x01 \x01(\x0b\x32$.mlflow.ucmodelregistry.ModelVersion\"\x94\x01\n\x19UpdateModelVersionRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t:7\xe2?4\n2com.databricks.rpc.RPC[UpdateModelVersionResponse]\"Y\n\x1aUpdateModelVersionResponse\x12;\n\rmodel_version\x18\x01 \x01(\x0b\x32$.mlflow.ucmodelregistry.ModelVersion\"\x7f\n\x19\x44\x65leteModelVersionRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01:7\xe2?4\n2com.databricks.rpc.RPC[DeleteModelVersionResponse]\"\x1c\n\x1a\x44\x65leteModelVersionResponse\"y\n\x16GetModelVersionRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01:4\xe2?1\n/com.databricks.rpc.RPC[GetModelVersionResponse]\"V\n\x17GetModelVersionResponse\x12;\n\rmodel_version\x18\x01 \x01(\x0b\x32$.mlflow.ucmodelregistry.ModelVersion\"\x96\x01\n\x1aSearchModelVersionsRequest\x12\x0e\n\x06\x66ilter\x18\x01 \x01(\t\x12\x1a\n\x0bmax_results\x18\x02 \x01(\x03:\x05\x31\x30\x30\x30\x30\x12\x12\n\npage_token\x18\x03 \x01(\t:8\xe2?5\n3com.databricks.rpc.RPC[SearchModelVersionsResponse]\"t\n\x1bSearchModelVersionsResponse\x12<\n\x0emodel_versions\x18\x01 \x03(\x0b\x32$.mlflow.ucmodelregistry.ModelVersion\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xf3\x01\n/GenerateTemporaryModelVersionCredentialsRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01\x12\x46\n\toperation\x18\x03 \x01(\x0e\x32-.mlflow.ucmodelregistry.ModelVersionOperationB\x04\xf8\x86\x19\x01:M\xe2?J\nHcom.databricks.rpc.RPC[GenerateTemporaryModelVersionCredentialsResponse]\"u\n0GenerateTemporaryModelVersionCredentialsResponse\x12\x41\n\x0b\x63redentials\x18\x01 \x01(\x0b\x32,.mlflow.ucmodelregistry.TemporaryCredentials\"\x8f\x01\n!GetModelVersionDownloadUriRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01:?\xe2?<\n:com.databricks.rpc.RPC[GetModelVersionDownloadUriResponse]\":\n\"GetModelVersionDownloadUriResponse\x12\x14\n\x0c\x61rtifact_uri\x18\x01 \x01(\t\"\x83\x01\n\x1b\x46inalizeModelVersionRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01:9\xe2?6\n4com.databricks.rpc.RPC[FinalizeModelVersionResponse]\"[\n\x1c\x46inalizeModelVersionResponse\x12;\n\rmodel_version\x18\x01 \x01(\x0b\x32$.mlflow.ucmodelregistry.ModelVersion\"\x9e\x01\n\x1eSetRegisteredModelAliasRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x13\n\x05\x61lias\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01\x12\x15\n\x07version\x18\x03 \x01(\tB\x04\xf8\x86\x19\x01:<\xe2?9\n7com.databricks.rpc.RPC[SetRegisteredModelAliasResponse]\"!\n\x1fSetRegisteredModelAliasResponse\"\x8d\x01\n!DeleteRegisteredModelAliasRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x13\n\x05\x61lias\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01:?\xe2?<\n:com.databricks.rpc.RPC[DeleteRegisteredModelAliasResponse]\"$\n\"DeleteRegisteredModelAliasResponse\"\x85\x01\n\x1dGetModelVersionByAliasRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\xf8\x86\x19\x01\x12\x13\n\x05\x61lias\x18\x02 \x01(\tB\x04\xf8\x86\x19\x01:;\xe2?8\n6com.databricks.rpc.RPC[GetModelVersionByAliasResponse]\"]\n\x1eGetModelVersionByAliasResponse\x12;\n\rmodel_version\x18\x01 \x01(\x0b\x32$.mlflow.ucmodelregistry.ModelVersion\"\xa9\x01\n\x06\x45ntity\x12*\n\x03job\x18\x01 \x01(\x0b\x32\x1b.mlflow.ucmodelregistry.JobH\x00\x12\x34\n\x08notebook\x18\x02 \x01(\x0b\x32 .mlflow.ucmodelregistry.NotebookH\x00\x12\x34\n\x08pipeline\x18\x03 \x01(\x0b\x32 .mlflow.ucmodelregistry.PipelineH\x00\x42\x07\n\x05value\";\n\x08Pipeline\x12\x13\n\x0bpipeline_id\x18\x01 \x01(\t\x12\x1a\n\x12pipeline_update_id\x18\x02 \x01(\t\"L\n\x03Job\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08task_key\x18\x02 \x01(\t\x12\x12\n\njob_run_id\x18\x03 \x01(\t\x12\x13\n\x0btask_run_id\x18\x04 \x01(\t\"C\n\x08Notebook\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\ncommand_id\x18\x02 \x01(\t\x12\x17\n\x0fnotebook_run_id\x18\x03 \x01(\t\"E\n\x11LineageHeaderInfo\x12\x30\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x1e.mlflow.ucmodelregistry.Entity*c\n\x12ModelVersionStatus\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x18\n\x14PENDING_REGISTRATION\x10\x01\x12\x17\n\x13\x46\x41ILED_REGISTRATION\x10\x02\x12\t\n\x05READY\x10\x03*\x8a\x01\n\x15ModelVersionOperation\x12\'\n#MODEL_VERSION_OPERATION_UNSPECIFIED\x10\x00\x12 \n\x1cMODEL_VERSION_OPERATION_READ\x10\x01\x12&\n\"MODEL_VERSION_OPERATION_READ_WRITE\x10\x02\x42\x32\n(com.databricks.api.proto.ucmodelregistry\xa0\x01\x01\xe2?\x02\x10\x01')
 
 _MODELVERSIONSTATUS = DESCRIPTOR.enum_types_by_name['ModelVersionStatus']
 ModelVersionStatus = enum_type_wrapper.EnumTypeWrapper(_MODELVERSIONSTATUS)
 _MODELVERSIONOPERATION = DESCRIPTOR.enum_types_by_name['ModelVersionOperation']
 ModelVersionOperation = enum_type_wrapper.EnumTypeWrapper(_MODELVERSIONOPERATION)
 UNSPECIFIED = 0
 PENDING_REGISTRATION = 1
@@ -468,18 +468,18 @@
   _DELETEREGISTEREDMODELALIASREQUEST._serialized_options = b'\342?<\n:com.databricks.rpc.RPC[DeleteRegisteredModelAliasResponse]'
   _GETMODELVERSIONBYALIASREQUEST.fields_by_name['name']._options = None
   _GETMODELVERSIONBYALIASREQUEST.fields_by_name['name']._serialized_options = b'\370\206\031\001'
   _GETMODELVERSIONBYALIASREQUEST.fields_by_name['alias']._options = None
   _GETMODELVERSIONBYALIASREQUEST.fields_by_name['alias']._serialized_options = b'\370\206\031\001'
   _GETMODELVERSIONBYALIASREQUEST._options = None
   _GETMODELVERSIONBYALIASREQUEST._serialized_options = b'\342?8\n6com.databricks.rpc.RPC[GetModelVersionByAliasResponse]'
-  _MODELVERSIONSTATUS._serialized_start=5343
-  _MODELVERSIONSTATUS._serialized_end=5442
-  _MODELVERSIONOPERATION._serialized_start=5445
-  _MODELVERSIONOPERATION._serialized_end=5583
+  _MODELVERSIONSTATUS._serialized_start=5365
+  _MODELVERSIONSTATUS._serialized_end=5464
+  _MODELVERSIONOPERATION._serialized_start=5467
+  _MODELVERSIONOPERATION._serialized_end=5605
   _REGISTEREDMODEL._serialized_start=107
   _REGISTEREDMODEL._serialized_end=299
   _REGISTEREDMODELALIAS._serialized_start=301
   _REGISTEREDMODELALIAS._serialized_end=355
   _MODELVERSION._serialized_start=358
   _MODELVERSION._serialized_end=765
   _TEMPORARYCREDENTIALS._serialized_start=768
@@ -507,61 +507,61 @@
   _GETREGISTEREDMODELRESPONSE._serialized_start=1948
   _GETREGISTEREDMODELRESPONSE._serialized_end=2043
   _SEARCHREGISTEREDMODELSREQUEST._serialized_start=2046
   _SEARCHREGISTEREDMODELSREQUEST._serialized_end=2184
   _SEARCHREGISTEREDMODELSRESPONSE._serialized_start=2186
   _SEARCHREGISTEREDMODELSRESPONSE._serialized_end=2311
   _CREATEMODELVERSIONREQUEST._serialized_start=2314
-  _CREATEMODELVERSIONREQUEST._serialized_end=2509
-  _CREATEMODELVERSIONRESPONSE._serialized_start=2511
-  _CREATEMODELVERSIONRESPONSE._serialized_end=2600
-  _UPDATEMODELVERSIONREQUEST._serialized_start=2603
-  _UPDATEMODELVERSIONREQUEST._serialized_end=2751
-  _UPDATEMODELVERSIONRESPONSE._serialized_start=2753
-  _UPDATEMODELVERSIONRESPONSE._serialized_end=2842
-  _DELETEMODELVERSIONREQUEST._serialized_start=2844
-  _DELETEMODELVERSIONREQUEST._serialized_end=2971
-  _DELETEMODELVERSIONRESPONSE._serialized_start=2973
-  _DELETEMODELVERSIONRESPONSE._serialized_end=3001
-  _GETMODELVERSIONREQUEST._serialized_start=3003
-  _GETMODELVERSIONREQUEST._serialized_end=3124
-  _GETMODELVERSIONRESPONSE._serialized_start=3126
-  _GETMODELVERSIONRESPONSE._serialized_end=3212
-  _SEARCHMODELVERSIONSREQUEST._serialized_start=3215
-  _SEARCHMODELVERSIONSREQUEST._serialized_end=3365
-  _SEARCHMODELVERSIONSRESPONSE._serialized_start=3367
-  _SEARCHMODELVERSIONSRESPONSE._serialized_end=3483
-  _GENERATETEMPORARYMODELVERSIONCREDENTIALSREQUEST._serialized_start=3486
-  _GENERATETEMPORARYMODELVERSIONCREDENTIALSREQUEST._serialized_end=3729
-  _GENERATETEMPORARYMODELVERSIONCREDENTIALSRESPONSE._serialized_start=3731
-  _GENERATETEMPORARYMODELVERSIONCREDENTIALSRESPONSE._serialized_end=3848
-  _GETMODELVERSIONDOWNLOADURIREQUEST._serialized_start=3851
-  _GETMODELVERSIONDOWNLOADURIREQUEST._serialized_end=3994
-  _GETMODELVERSIONDOWNLOADURIRESPONSE._serialized_start=3996
-  _GETMODELVERSIONDOWNLOADURIRESPONSE._serialized_end=4054
-  _FINALIZEMODELVERSIONREQUEST._serialized_start=4057
-  _FINALIZEMODELVERSIONREQUEST._serialized_end=4188
-  _FINALIZEMODELVERSIONRESPONSE._serialized_start=4190
-  _FINALIZEMODELVERSIONRESPONSE._serialized_end=4281
-  _SETREGISTEREDMODELALIASREQUEST._serialized_start=4284
-  _SETREGISTEREDMODELALIASREQUEST._serialized_end=4442
-  _SETREGISTEREDMODELALIASRESPONSE._serialized_start=4444
-  _SETREGISTEREDMODELALIASRESPONSE._serialized_end=4477
-  _DELETEREGISTEREDMODELALIASREQUEST._serialized_start=4480
-  _DELETEREGISTEREDMODELALIASREQUEST._serialized_end=4621
-  _DELETEREGISTEREDMODELALIASRESPONSE._serialized_start=4623
-  _DELETEREGISTEREDMODELALIASRESPONSE._serialized_end=4659
-  _GETMODELVERSIONBYALIASREQUEST._serialized_start=4662
-  _GETMODELVERSIONBYALIASREQUEST._serialized_end=4795
-  _GETMODELVERSIONBYALIASRESPONSE._serialized_start=4797
-  _GETMODELVERSIONBYALIASRESPONSE._serialized_end=4890
-  _ENTITY._serialized_start=4893
-  _ENTITY._serialized_end=5062
-  _PIPELINE._serialized_start=5064
-  _PIPELINE._serialized_end=5123
-  _JOB._serialized_start=5125
-  _JOB._serialized_end=5201
-  _NOTEBOOK._serialized_start=5203
-  _NOTEBOOK._serialized_end=5270
-  _LINEAGEHEADERINFO._serialized_start=5272
-  _LINEAGEHEADERINFO._serialized_end=5341
+  _CREATEMODELVERSIONREQUEST._serialized_end=2531
+  _CREATEMODELVERSIONRESPONSE._serialized_start=2533
+  _CREATEMODELVERSIONRESPONSE._serialized_end=2622
+  _UPDATEMODELVERSIONREQUEST._serialized_start=2625
+  _UPDATEMODELVERSIONREQUEST._serialized_end=2773
+  _UPDATEMODELVERSIONRESPONSE._serialized_start=2775
+  _UPDATEMODELVERSIONRESPONSE._serialized_end=2864
+  _DELETEMODELVERSIONREQUEST._serialized_start=2866
+  _DELETEMODELVERSIONREQUEST._serialized_end=2993
+  _DELETEMODELVERSIONRESPONSE._serialized_start=2995
+  _DELETEMODELVERSIONRESPONSE._serialized_end=3023
+  _GETMODELVERSIONREQUEST._serialized_start=3025
+  _GETMODELVERSIONREQUEST._serialized_end=3146
+  _GETMODELVERSIONRESPONSE._serialized_start=3148
+  _GETMODELVERSIONRESPONSE._serialized_end=3234
+  _SEARCHMODELVERSIONSREQUEST._serialized_start=3237
+  _SEARCHMODELVERSIONSREQUEST._serialized_end=3387
+  _SEARCHMODELVERSIONSRESPONSE._serialized_start=3389
+  _SEARCHMODELVERSIONSRESPONSE._serialized_end=3505
+  _GENERATETEMPORARYMODELVERSIONCREDENTIALSREQUEST._serialized_start=3508
+  _GENERATETEMPORARYMODELVERSIONCREDENTIALSREQUEST._serialized_end=3751
+  _GENERATETEMPORARYMODELVERSIONCREDENTIALSRESPONSE._serialized_start=3753
+  _GENERATETEMPORARYMODELVERSIONCREDENTIALSRESPONSE._serialized_end=3870
+  _GETMODELVERSIONDOWNLOADURIREQUEST._serialized_start=3873
+  _GETMODELVERSIONDOWNLOADURIREQUEST._serialized_end=4016
+  _GETMODELVERSIONDOWNLOADURIRESPONSE._serialized_start=4018
+  _GETMODELVERSIONDOWNLOADURIRESPONSE._serialized_end=4076
+  _FINALIZEMODELVERSIONREQUEST._serialized_start=4079
+  _FINALIZEMODELVERSIONREQUEST._serialized_end=4210
+  _FINALIZEMODELVERSIONRESPONSE._serialized_start=4212
+  _FINALIZEMODELVERSIONRESPONSE._serialized_end=4303
+  _SETREGISTEREDMODELALIASREQUEST._serialized_start=4306
+  _SETREGISTEREDMODELALIASREQUEST._serialized_end=4464
+  _SETREGISTEREDMODELALIASRESPONSE._serialized_start=4466
+  _SETREGISTEREDMODELALIASRESPONSE._serialized_end=4499
+  _DELETEREGISTEREDMODELALIASREQUEST._serialized_start=4502
+  _DELETEREGISTEREDMODELALIASREQUEST._serialized_end=4643
+  _DELETEREGISTEREDMODELALIASRESPONSE._serialized_start=4645
+  _DELETEREGISTEREDMODELALIASRESPONSE._serialized_end=4681
+  _GETMODELVERSIONBYALIASREQUEST._serialized_start=4684
+  _GETMODELVERSIONBYALIASREQUEST._serialized_end=4817
+  _GETMODELVERSIONBYALIASRESPONSE._serialized_start=4819
+  _GETMODELVERSIONBYALIASRESPONSE._serialized_end=4912
+  _ENTITY._serialized_start=4915
+  _ENTITY._serialized_end=5084
+  _PIPELINE._serialized_start=5086
+  _PIPELINE._serialized_end=5145
+  _JOB._serialized_start=5147
+  _JOB._serialized_end=5223
+  _NOTEBOOK._serialized_start=5225
+  _NOTEBOOK._serialized_end=5292
+  _LINEAGEHEADERINFO._serialized_start=5294
+  _LINEAGEHEADERINFO._serialized_end=5363
 # @@protoc_insertion_point(module_scope)
```

### Comparing `mlflow-skinny-2.4.1/mlflow/protos/databricks_uc_registry_service_pb2.py` & `mlflow-skinny-2.4.2/mlflow/protos/databricks_uc_registry_service_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/protos/facet_feature_statistics_pb2.py` & `mlflow-skinny-2.4.2/mlflow/protos/facet_feature_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/protos/internal_pb2.py` & `mlflow-skinny-2.4.2/mlflow/protos/internal_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/protos/mlflow_artifacts_pb2.py` & `mlflow-skinny-2.4.2/mlflow/protos/mlflow_artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/protos/model_registry_pb2.py` & `mlflow-skinny-2.4.2/mlflow/protos/model_registry_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/protos/scalapb/scalapb_pb2.py` & `mlflow-skinny-2.4.2/mlflow/protos/scalapb/scalapb_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/protos/service_pb2.py` & `mlflow-skinny-2.4.2/mlflow/protos/service_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pyfunc/__init__.py` & `mlflow-skinny-2.4.2/mlflow/pyfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pyfunc/backend.py` & `mlflow-skinny-2.4.2/mlflow/pyfunc/backend.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pyfunc/mlserver.py` & `mlflow-skinny-2.4.2/mlflow/pyfunc/mlserver.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pyfunc/model.py` & `mlflow-skinny-2.4.2/mlflow/pyfunc/model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pyfunc/scoring_server/__init__.py` & `mlflow-skinny-2.4.2/mlflow/pyfunc/scoring_server/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pyfunc/scoring_server/client.py` & `mlflow-skinny-2.4.2/mlflow/pyfunc/scoring_server/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pyfunc/spark_model_cache.py` & `mlflow-skinny-2.4.2/mlflow/pyfunc/spark_model_cache.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pyfunc/stdin_server.py` & `mlflow-skinny-2.4.2/mlflow/pyfunc/stdin_server.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pypi_package_index.json` & `mlflow-skinny-2.4.2/mlflow/pypi_package_index.json`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pyspark/ml/__init__.py` & `mlflow-skinny-2.4.2/mlflow/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pyspark/ml/_autolog.py` & `mlflow-skinny-2.4.2/mlflow/pyspark/ml/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pyspark/ml/log_model_allowlist.txt` & `mlflow-skinny-2.4.2/mlflow/pyspark/ml/log_model_allowlist.txt`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pytorch/__init__.py` & `mlflow-skinny-2.4.2/mlflow/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pytorch/_lightning_autolog.py` & `mlflow-skinny-2.4.2/mlflow/pytorch/_lightning_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pytorch/_pytorch_autolog.py` & `mlflow-skinny-2.4.2/mlflow/pytorch/_pytorch_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/pytorch/pickle_module.py` & `mlflow-skinny-2.4.2/mlflow/pytorch/pickle_module.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/__init__.py` & `mlflow-skinny-2.4.2/mlflow/recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/artifacts.py` & `mlflow-skinny-2.4.2/mlflow/recipes/artifacts.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/cards/__init__.py` & `mlflow-skinny-2.4.2/mlflow/recipes/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/cards/histogram_generator.py` & `mlflow-skinny-2.4.2/mlflow/recipes/cards/histogram_generator.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/cards/pandas_renderer.py` & `mlflow-skinny-2.4.2/mlflow/recipes/cards/pandas_renderer.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/classification/v1/recipe.py` & `mlflow-skinny-2.4.2/mlflow/recipes/classification/v1/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/cli.py` & `mlflow-skinny-2.4.2/mlflow/recipes/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/dag_help_strings.py` & `mlflow-skinny-2.4.2/mlflow/recipes/dag_help_strings.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/recipe.py` & `mlflow-skinny-2.4.2/mlflow/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/regression/v1/recipe.py` & `mlflow-skinny-2.4.2/mlflow/recipes/regression/v1/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/step.py` & `mlflow-skinny-2.4.2/mlflow/recipes/step.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/steps/automl/flaml.py` & `mlflow-skinny-2.4.2/mlflow/recipes/steps/automl/flaml.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/steps/evaluate.py` & `mlflow-skinny-2.4.2/mlflow/recipes/steps/evaluate.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/steps/ingest/__init__.py` & `mlflow-skinny-2.4.2/mlflow/recipes/steps/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/steps/ingest/datasets.py` & `mlflow-skinny-2.4.2/mlflow/recipes/steps/ingest/datasets.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/steps/predict.py` & `mlflow-skinny-2.4.2/mlflow/recipes/steps/predict.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/steps/register.py` & `mlflow-skinny-2.4.2/mlflow/recipes/steps/register.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/steps/split.py` & `mlflow-skinny-2.4.2/mlflow/recipes/steps/split.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/steps/train.py` & `mlflow-skinny-2.4.2/mlflow/recipes/steps/train.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/steps/transform.py` & `mlflow-skinny-2.4.2/mlflow/recipes/steps/transform.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/utils/__init__.py` & `mlflow-skinny-2.4.2/mlflow/recipes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/utils/execution.py` & `mlflow-skinny-2.4.2/mlflow/recipes/utils/execution.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/utils/metrics.py` & `mlflow-skinny-2.4.2/mlflow/recipes/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/utils/step.py` & `mlflow-skinny-2.4.2/mlflow/recipes/utils/step.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/utils/tracking.py` & `mlflow-skinny-2.4.2/mlflow/recipes/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/recipes/utils/wrapped_recipe_model.py` & `mlflow-skinny-2.4.2/mlflow/recipes/utils/wrapped_recipe_model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/rfunc/__init__.py` & `mlflow-skinny-2.4.2/mlflow/rfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/rfunc/backend.py` & `mlflow-skinny-2.4.2/mlflow/rfunc/backend.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/runs.py` & `mlflow-skinny-2.4.2/mlflow/runs.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/sagemaker/__init__.py` & `mlflow-skinny-2.4.2/mlflow/sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/sagemaker/cli.py` & `mlflow-skinny-2.4.2/mlflow/sagemaker/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/sentence_transformers.py` & `mlflow-skinny-2.4.2/mlflow/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/server/__init__.py` & `mlflow-skinny-2.4.2/mlflow/server/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/server/auth/__init__.py` & `mlflow-skinny-2.4.2/mlflow/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/server/auth/client.py` & `mlflow-skinny-2.4.2/mlflow/server/auth/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/server/auth/config.py` & `mlflow-skinny-2.4.2/mlflow/server/auth/config.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/server/auth/entities.py` & `mlflow-skinny-2.4.2/mlflow/server/auth/entities.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/server/auth/logo.py` & `mlflow-skinny-2.4.2/mlflow/server/auth/logo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/server/auth/permissions.py` & `mlflow-skinny-2.4.2/mlflow/server/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/server/auth/routes.py` & `mlflow-skinny-2.4.2/mlflow/server/auth/routes.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/server/auth/sqlalchemy_store.py` & `mlflow-skinny-2.4.2/mlflow/server/auth/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/server/handlers.py` & `mlflow-skinny-2.4.2/mlflow/server/handlers.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/shap.py` & `mlflow-skinny-2.4.2/mlflow/shap.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/sklearn/__init__.py` & `mlflow-skinny-2.4.2/mlflow/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/sklearn/utils.py` & `mlflow-skinny-2.4.2/mlflow/sklearn/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/spacy.py` & `mlflow-skinny-2.4.2/mlflow/spacy.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/spark.py` & `mlflow-skinny-2.4.2/mlflow/spark.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/statsmodels.py` & `mlflow-skinny-2.4.2/mlflow/statsmodels.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/registry/rest_store.py` & `mlflow-skinny-2.4.2/mlflow/store/_unity_catalog/registry/rest_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 _DATABRICKS_ORG_ID_HEADER = "x-databricks-org-id"
 _DATABRICKS_LINEAGE_ID_HEADER = "X-Databricks-Lineage-Identifier"
 _TRACKING_METHOD_TO_INFO = extract_api_info_for_service(MlflowService, _REST_API_PATH_PREFIX)
 _METHOD_TO_INFO = extract_api_info_for_service(UcModelRegistryService, _REST_API_PATH_PREFIX)
 _METHOD_TO_ALL_INFO = extract_all_api_info_for_service(
     UcModelRegistryService, _REST_API_PATH_PREFIX
 )
+_DATABRICKS_FS_LOADER_MODULE = "databricks.feature_store.mlflow_model"
 
 _logger = logging.getLogger(__name__)
 
 
 def _require_arg_unspecified(arg_name, arg_value, default_values=None, message=None):
     default_values = [None] if default_values is None else default_values
     if arg_value not in default_values:
@@ -102,14 +103,46 @@
     ]
     if message is not None:
         messages.append(message)
     messages.append("See the user guide for more information")
     raise MlflowException(" ".join(messages))
 
 
+def _load_model(local_model_dir):
+    # Import Model here instead of in the top level, to avoid circular import; the
+    # mlflow.models.model module imports from MLflow tracking, which triggers an import of
+    # this file during store registry initialization
+    from mlflow.models.model import Model
+
+    try:
+        return Model.load(local_model_dir)
+    except Exception as e:
+        raise MlflowException(
+            "Unable to load model metadata. Ensure the source path of the model "
+            "being registered points to a valid MLflow model directory "
+            "(see https://mlflow.org/docs/latest/models.html#storage-format) containing a "
+            "model signature (https://mlflow.org/docs/latest/models.html#model-signature) "
+            "specifying both input and output type specifications."
+        ) from e
+
+
+def get_feature_dependencies(model_dir):
+    model = _load_model(model_dir)
+    model_info = model.get_model_info()
+    if (
+        model_info.flavors.get("python_function", {}).get("loader_module")
+        == _DATABRICKS_FS_LOADER_MODULE
+    ):
+        raise MlflowException(
+            "This model was packaged by Databricks Feature Store and can only be registered on a "
+            "Databricks cluster."
+        )
+    return ""
+
+
 @experimental
 class UcModelRegistryStore(BaseRestStore):
     """
     Client for a remote model registry server accessed via REST API calls
 
     :param store_uri: URI with scheme 'databricks-uc'
     :param tracking_uri: URI of the Databricks MLflow tracking server from which to fetch
@@ -268,19 +301,20 @@
         :param stages: List of desired stages. If input list is None, return latest versions for
                        each stage.
         :return: List of :py:class:`mlflow.entities.model_registry.ModelVersion` objects.
         """
         _raise_unsupported_method(
             method="get_latest_versions",
             message="If seeing this error while attempting to "
-            "load a models:/ URI of the form models:/<name>/<stage>, note that "
-            "staged-based model URIs are unsupported for models in UC. Future "
-            "MLflow Python client versions will include support for model "
-            "aliases and alias-based 'models:/' URIs "
-            "of the form models:/<name>@<alias> as an alternative.",
+            "load a model version by stage, note that setting stages and loading model versions "
+            "by stage is unsupported in Unity Catalog. Instead, we recommend using aliases for "
+            "flexible model deployment. If trying to load a model version by alias, use the "
+            "syntax 'models:/your_model_name@your_alias_name'. "
+            "To set aliases, you can use the "
+            "`MlflowClient().set_registered_model_alias(name, alias, version)` API.",
         )
 
     def set_registered_model_tag(self, name, tag):
         """
         Set a tag for the registered model.
 
         :param name: Registered model name.
@@ -363,29 +397,15 @@
 
     def _get_notebook_id(self, run):
         if run is None:
             return None
         return run.data.tags.get(MLFLOW_DATABRICKS_NOTEBOOK_ID, None)
 
     def _validate_model_signature(self, local_model_dir):
-        # Import Model here instead of in the top level, to avoid circular import; the
-        # mlflow.models.model module imports from MLflow tracking, which triggers an import of
-        # this file during store registry initialization
-        from mlflow.models.model import Model
-
-        try:
-            model = Model.load(local_model_dir)
-        except Exception as e:
-            raise MlflowException(
-                "Unable to load model metadata. Ensure the source path of the model "
-                "being registered points to a valid MLflow model directory "
-                "(see https://mlflow.org/docs/latest/models.html#storage-format) containing a "
-                "model signature (https://mlflow.org/docs/latest/models.html#model-signature) "
-                "specifying both input and output type specifications."
-            ) from e
+        model = _load_model(local_model_dir)
         signature_required_explanation = (
             "All models in the Unity Catalog must be logged with a "
             "model signature containing both input and output "
             "type specifications. See "
             "https://mlflow.org/docs/latest/models.html#model-signature "
             "for details on how to log a model with a signature"
         )
@@ -428,36 +448,38 @@
             lineage_header_info = LineageHeaderInfo(entities=[entity])
             # Base64-encode the header value to ensure it's valid ASCII,
             # similar to JWT (see https://stackoverflow.com/a/40347926)
             header_json = message_to_json(lineage_header_info)
             header_base64 = base64.b64encode(header_json.encode())
             extra_headers = {_DATABRICKS_LINEAGE_ID_HEADER: header_base64}
         full_name = get_full_name_from_sc(name, self.spark)
-        req_body = message_to_json(
-            CreateModelVersionRequest(
-                name=full_name,
-                source=source,
-                run_id=run_id,
-                description=description,
-                run_tracking_server_id=source_workspace_id,
-            )
-        )
         with tempfile.TemporaryDirectory() as tmpdir:
             try:
                 local_model_dir = mlflow.artifacts.download_artifacts(
                     artifact_uri=source, dst_path=tmpdir, tracking_uri=self.tracking_uri
                 )
             except Exception as e:
                 raise MlflowException(
                     f"Unable to download model artifacts from source artifact location "
                     f"'{source}' in order to upload them to Unity Catalog. Please ensure "
                     f"the source artifact location exists and that you can download from "
                     f"it via mlflow.artifacts.download_artifacts()"
                 ) from e
             self._validate_model_signature(local_model_dir)
+            feature_deps = get_feature_dependencies(local_model_dir)
+            req_body = message_to_json(
+                CreateModelVersionRequest(
+                    name=full_name,
+                    source=source,
+                    run_id=run_id,
+                    description=description,
+                    run_tracking_server_id=source_workspace_id,
+                    feature_deps=feature_deps,
+                )
+            )
             model_version = self._call_endpoint(
                 CreateModelVersionRequest, req_body, extra_headers=extra_headers
             ).model_version
             version_number = model_version.version
             scoped_token = self._get_temporary_model_version_write_credentials(
                 name=full_name, version=version_number
             )
@@ -476,15 +498,22 @@
         :param version: Registered model version.
         :param stage: New desired stage for this model version.
         :param archive_existing_versions: If this flag is set to ``True``, all existing model
             versions in the stage will be automatically moved to the "archived" stage. Only valid
             when ``stage`` is ``"staging"`` or ``"production"`` otherwise an error will be raised.
 
         """
-        _raise_unsupported_method(method="transition_model_version_stage")
+        _raise_unsupported_method(
+            method="transition_model_version_stage",
+            message="We recommend using aliases instead of stages for more flexible model "
+            "deployment management. You can set an alias on a registered model using "
+            "`MlflowClient().set_registered_model_alias(name, alias, version)` and load a model "
+            "version by alias using the URI 'models:/your_model_name@your_alias', e.g. "
+            "`mlflow.pyfunc.load_model('models:/your_model_name@your_alias')`.",
+        )
 
     def update_model_version(self, name, version, description):
         """
         Update metadata associated with a model version in backend.
 
         :param name: Registered model name.
         :param version: Registered model version.
```

### Comparing `mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/registry/utils.py` & `mlflow-skinny-2.4.2/mlflow/store/_unity_catalog/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/artifact_repository_registry.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/artifact_repository_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/azure_blob_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/azure_blob_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/azure_data_lake_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/azure_data_lake_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/cli.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/databricks_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/databricks_artifact_repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 from mlflow.utils.uri import (
     extract_and_normalize_path,
     get_databricks_profile_uri_from_artifact_uri,
     is_databricks_acled_artifacts_uri,
     is_valid_dbfs_uri,
     remove_databricks_profile_info_from_artifact_uri,
 )
+from mlflow.environment_variables import MLFLOW_ENABLE_MULTIPART_DOWNLOAD
 
 _logger = logging.getLogger(__name__)
 _DOWNLOAD_CHUNK_SIZE = 100_000_000  # 100 MB
 _MULTIPART_DOWNLOAD_MINIMUM_FILE_SIZE = 500_000_000  # 500 MB
 _MULTIPART_UPLOAD_CHUNK_SIZE = 10_000_000  # 10 MB
 _MAX_CREDENTIALS_REQUEST_SIZE = 2000  # Max number of artifact paths in a single credentials request
 _SERVICE_AND_METHOD_TO_INFO = {
@@ -779,15 +780,19 @@
         # contained by the parent directory. A bad path could result in there being
         # no matching FileInfos (by path), so fall back to None size to prevent
         # parallelized download.
         parent_dir = posixpath.dirname(remote_file_path)
         file_infos = self.list_artifacts(parent_dir)
         file_info = [info for info in file_infos if info.path == remote_file_path]
         file_size = file_info[0].file_size if len(file_info) == 1 else None
-        if not file_size or file_size < _MULTIPART_DOWNLOAD_MINIMUM_FILE_SIZE:
+        if (
+            not file_size
+            or file_size < _MULTIPART_DOWNLOAD_MINIMUM_FILE_SIZE
+            or not MLFLOW_ENABLE_MULTIPART_DOWNLOAD.get()
+        ):
             self._download_from_cloud(
                 cloud_credential_info=read_credentials[0], dst_local_file_path=local_path
             )
         else:
             self._parallelized_download_from_cloud(
                 read_credentials[0], file_size, local_path, remote_file_path
             )
```

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/databricks_models_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/databricks_models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/dbfs_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/dbfs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/ftp_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/ftp_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/gcs_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/gcs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/hdfs_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/hdfs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/http_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/http_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/local_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/local_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/mlflow_artifacts_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/mlflow_artifacts_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/models_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/runs_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/runs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/s3_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/s3_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/sftp_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/sftp_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/unity_catalog_models_artifact_repo.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/unity_catalog_models_artifact_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,24 +100,30 @@
             host_creds=db_creds,
             endpoint=endpoint,
             method=method,
             json_body=req_body,
             response_proto=response_proto,
         ).credentials
 
-    def list_artifacts(self, path=None):
-        raise MlflowException("This repository does not support listing artifacts.")
-
-    def download_artifacts(self, artifact_path, dst_path=None):
+    def _get_artifact_repo(self):
+        """
+        Get underlying ArtifactRepository instance for model version blob
+        storage
+        """
         scoped_token = self._get_scoped_token()
         blob_storage_path = self._get_blob_storage_path()
-        repo = get_artifact_repo_from_storage_info(
+        return get_artifact_repo_from_storage_info(
             storage_location=blob_storage_path, scoped_token=scoped_token
         )
-        return repo.download_artifacts(artifact_path, dst_path)
+
+    def list_artifacts(self, path=None):
+        return self._get_artifact_repo().list_artifacts(path=path)
+
+    def download_artifacts(self, artifact_path, dst_path=None):
+        return self._get_artifact_repo().download_artifacts(artifact_path, dst_path)
 
     def log_artifact(self, local_file, artifact_path=None):
         raise MlflowException("This repository does not support logging artifacts.")
 
     def log_artifacts(self, local_dir, artifact_path=None):
         raise MlflowException("This repository does not support logging artifacts.")
```

### Comparing `mlflow-skinny-2.4.1/mlflow/store/artifact/utils/models.py` & `mlflow-skinny-2.4.2/mlflow/store/artifact/utils/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     profile_uri = get_databricks_profile_uri_from_artifact_uri(uri) or mlflow.get_registry_uri()
     return is_databricks_uri(profile_uri)
 
 
 def _improper_model_uri_msg(uri):
     return (
         "Not a proper models:/ URI: %s. " % uri
-        + "Models URIs must be of the form 'models:/<model_name>/<suffix>' "
-        + "or 'models:/<model_name>@<alias>' where suffix is a model version, stage, "
+        + "Models URIs must be of the form 'models:/model_name/suffix' "
+        + "or 'models:/model_name@alias' where suffix is a model version, stage, "
         + "or the string '%s' and where alias is a registered model alias. "
         % _MODELS_URI_SUFFIX_LATEST
         + "Only one of suffix or alias can be defined at a time."
     )
 
 
 def _get_latest_model_version(client, name, stage):
```

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db/utils.py` & `mlflow-skinny-2.4.2/mlflow/store/db/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/alembic.ini` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/env.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/env.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py` & `mlflow-skinny-2.4.2/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/model_registry/__init__.py` & `mlflow-skinny-2.4.2/mlflow/store/model_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/model_registry/abstract_store.py` & `mlflow-skinny-2.4.2/mlflow/store/model_registry/abstract_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/model_registry/base_rest_store.py` & `mlflow-skinny-2.4.2/mlflow/store/model_registry/base_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/model_registry/dbmodels/models.py` & `mlflow-skinny-2.4.2/mlflow/store/model_registry/dbmodels/models.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/model_registry/file_store.py` & `mlflow-skinny-2.4.2/mlflow/store/model_registry/file_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/model_registry/rest_store.py` & `mlflow-skinny-2.4.2/mlflow/store/model_registry/rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/model_registry/sqlalchemy_store.py` & `mlflow-skinny-2.4.2/mlflow/store/model_registry/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/tracking/__init__.py` & `mlflow-skinny-2.4.2/mlflow/store/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/tracking/abstract_store.py` & `mlflow-skinny-2.4.2/mlflow/store/tracking/abstract_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/tracking/dbmodels/initial_models.py` & `mlflow-skinny-2.4.2/mlflow/store/tracking/dbmodels/initial_models.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/tracking/dbmodels/models.py` & `mlflow-skinny-2.4.2/mlflow/store/tracking/dbmodels/models.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/tracking/file_store.py` & `mlflow-skinny-2.4.2/mlflow/store/tracking/file_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/tracking/rest_store.py` & `mlflow-skinny-2.4.2/mlflow/store/tracking/rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/store/tracking/sqlalchemy_store.py` & `mlflow-skinny-2.4.2/mlflow/store/tracking/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tensorflow/__init__.py` & `mlflow-skinny-2.4.2/mlflow/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tensorflow/_autolog.py` & `mlflow-skinny-2.4.2/mlflow/tensorflow/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/__init__.py` & `mlflow-skinny-2.4.2/mlflow/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/client.py` & `mlflow-skinny-2.4.2/mlflow/tracking/_model_registry/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/fluent.py` & `mlflow-skinny-2.4.2/mlflow/tracking/_model_registry/fluent.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/registry.py` & `mlflow-skinny-2.4.2/mlflow/tracking/_model_registry/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/utils.py` & `mlflow-skinny-2.4.2/mlflow/tracking/_model_registry/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
 from functools import partial
 
 from mlflow.environment_variables import MLFLOW_TRACKING_AWS_SIGV4
 from mlflow.store.db.db_types import DATABASE_ENGINES
 from mlflow.store.model_registry.file_store import FileStore
 from mlflow.store.model_registry.rest_store import RestStore
+from mlflow.store.model_registry.databricks_workspace_model_registry_rest_store import (
+    DatabricksWorkspaceModelRegistryRestStore,
+)
 from mlflow.store._unity_catalog.registry.rest_store import UcModelRegistryStore
 from mlflow.tracking._model_registry.registry import ModelRegistryStoreRegistry
 from mlflow.tracking._tracking_service.utils import (
     _TRACKING_USERNAME_ENV_VAR,
     _TRACKING_PASSWORD_ENV_VAR,
     _TRACKING_TOKEN_ENV_VAR,
     _TRACKING_INSECURE_TLS_ENV_VAR,
@@ -145,15 +148,15 @@
 
 
 def _get_rest_store(store_uri, **_):
     return RestStore(partial(get_default_host_creds, store_uri))
 
 
 def _get_databricks_rest_store(store_uri, **_):
-    return RestStore(partial(get_databricks_host_creds, store_uri))
+    return DatabricksWorkspaceModelRegistryRestStore(partial(get_databricks_host_creds, store_uri))
 
 
 # We define the global variable as `None` so that instantiating the store does not lead to circular
 # dependency issues.
 _model_registry_store_registry = None
```

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/client.py` & `mlflow-skinny-2.4.2/mlflow/tracking/_tracking_service/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/registry.py` & `mlflow-skinny-2.4.2/mlflow/tracking/_tracking_service/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/utils.py` & `mlflow-skinny-2.4.2/mlflow/tracking/_tracking_service/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/artifact_utils.py` & `mlflow-skinny-2.4.2/mlflow/tracking/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/client.py` & `mlflow-skinny-2.4.2/mlflow/tracking/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/context/abstract_context.py` & `mlflow-skinny-2.4.2/mlflow/tracking/context/abstract_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_cluster_context.py` & `mlflow-skinny-2.4.2/mlflow/tracking/context/databricks_cluster_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_command_context.py` & `mlflow-skinny-2.4.2/mlflow/tracking/context/databricks_command_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_job_context.py` & `mlflow-skinny-2.4.2/mlflow/tracking/context/databricks_job_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_notebook_context.py` & `mlflow-skinny-2.4.2/mlflow/tracking/context/databricks_notebook_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_repo_context.py` & `mlflow-skinny-2.4.2/mlflow/tracking/context/databricks_repo_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/context/default_context.py` & `mlflow-skinny-2.4.2/mlflow/tracking/context/default_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/context/git_context.py` & `mlflow-skinny-2.4.2/mlflow/tracking/context/git_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/context/registry.py` & `mlflow-skinny-2.4.2/mlflow/tracking/context/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/abstract_context.py` & `mlflow-skinny-2.4.2/mlflow/tracking/default_experiment/abstract_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py` & `mlflow-skinny-2.4.2/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,57 @@
-import logging
-from mlflow.tracking.default_experiment.abstract_context import DefaultExperimentProvider
+from mlflow.exceptions import MlflowException
+from mlflow.protos import databricks_pb2
 from mlflow.tracking.client import MlflowClient
+from mlflow.tracking.default_experiment.abstract_context import DefaultExperimentProvider
 from mlflow.utils import databricks_utils
 from mlflow.utils.mlflow_tags import (
-    MLFLOW_DATABRICKS_JOB_TYPE_INFO,
     MLFLOW_EXPERIMENT_SOURCE_TYPE,
     MLFLOW_EXPERIMENT_SOURCE_ID,
 )
 
-_logger = logging.getLogger(__name__)
-_resolved_job_experiment_id = None
 
+class DatabricksNotebookExperimentProvider(DefaultExperimentProvider):
+    def in_context(self):
+        return databricks_utils.is_in_databricks_notebook()
+
+    def get_experiment_id(self):
+        return databricks_utils.get_notebook_id()
+
+
+class DatabricksRepoNotebookExperimentProvider(DefaultExperimentProvider):
+    _resolved_repo_notebook_experiment_id = None
 
-class DatabricksJobExperimentProvider(DefaultExperimentProvider):
     def in_context(self):
-        return (
-            databricks_utils.is_in_databricks_job()
-            and databricks_utils.get_job_type_info() == "NORMAL"
-        )
+        return databricks_utils.is_in_databricks_repo_notebook()
 
     def get_experiment_id(self):
-        global _resolved_job_experiment_id
-        if _resolved_job_experiment_id:
-            return _resolved_job_experiment_id
-
-        job_id = databricks_utils.get_job_id()
-        tags = {}
-        tags[MLFLOW_DATABRICKS_JOB_TYPE_INFO] = databricks_utils.get_job_type_info()
-        tags[MLFLOW_EXPERIMENT_SOURCE_TYPE] = "JOB"
-        tags[MLFLOW_EXPERIMENT_SOURCE_ID] = job_id
+        if DatabricksRepoNotebookExperimentProvider._resolved_repo_notebook_experiment_id:
+            return DatabricksRepoNotebookExperimentProvider._resolved_repo_notebook_experiment_id
+
+        source_notebook_id = databricks_utils.get_notebook_id()
+        source_notebook_name = databricks_utils.get_notebook_path()
+        tags = {
+            MLFLOW_EXPERIMENT_SOURCE_TYPE: "REPO_NOTEBOOK",
+            MLFLOW_EXPERIMENT_SOURCE_ID: source_notebook_id,
+        }
 
-        # The create_experiment is a get or create experiment function where it will
-        # return the corresponding experiment if one exists for the job.
+        # With the presence of the above tags, the following is a get or create in which it will
+        # return the corresponding experiment if one exists for the repo notebook.
         # If no corresponding experiment exist, it will create a new one and return
-        # the newly created experiment
-        experiment_id = MlflowClient().create_experiment(
-            databricks_utils.get_experiment_name_from_job_id(job_id), None, tags
-        )
-        _logger.debug(
-            "Job experiment with experiment ID '%s' fetched or created",
-            experiment_id,
-        )
+        # the newly created experiment ID.
+        try:
+            experiment_id = MlflowClient().create_experiment(source_notebook_name, None, tags)
+        except MlflowException as e:
+            if e.error_code == databricks_pb2.ErrorCode.Name(
+                databricks_pb2.INVALID_PARAMETER_VALUE
+            ):
+                # If repo notebook experiment creation isn't enabled, fall back to
+                # using the notebook ID
+                experiment_id = source_notebook_id
+            else:
+                raise e
 
-        _resolved_job_experiment_id = experiment_id
+        DatabricksRepoNotebookExperimentProvider._resolved_repo_notebook_experiment_id = (
+            experiment_id
+        )
 
         return experiment_id
```

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/registry.py` & `mlflow-skinny-2.4.2/mlflow/tracking/default_experiment/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,21 @@
 import logging
 
 from mlflow.tracking.default_experiment import DEFAULT_EXPERIMENT_ID
 from mlflow.tracking.default_experiment.databricks_notebook_experiment_provider import (
     DatabricksNotebookExperimentProvider,
     DatabricksRepoNotebookExperimentProvider,
 )
-from mlflow.tracking.default_experiment.databricks_job_experiment_provider import (
-    DatabricksJobExperimentProvider,
-)
 
 
 _logger = logging.getLogger(__name__)
 # Listed below are the list of providers, which are used to provide MLflow Experiment IDs based on
 # the current context where the MLflow client is running when the user has not explicitly set
 # an experiment. The order below is the order in which the these providers are registered.
 _EXPERIMENT_PROVIDERS = (
-    DatabricksJobExperimentProvider,
     DatabricksRepoNotebookExperimentProvider,
     DatabricksNotebookExperimentProvider,
 )
 
 
 class DefaultExperimentProviderRegistry:
     """Registry for default experiment provider implementations
```

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/fluent.py` & `mlflow-skinny-2.4.2/mlflow/tracking/fluent.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/llm_utils.py` & `mlflow-skinny-2.4.2/mlflow/tracking/llm_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/metric_value_conversion_utils.py` & `mlflow-skinny-2.4.2/mlflow/tracking/metric_value_conversion_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/registry.py` & `mlflow-skinny-2.4.2/mlflow/tracking/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/request_header/abstract_request_header_provider.py` & `mlflow-skinny-2.4.2/mlflow/tracking/request_header/abstract_request_header_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/request_header/databricks_request_header_provider.py` & `mlflow-skinny-2.4.2/mlflow/tracking/request_header/databricks_request_header_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/tracking/request_header/registry.py` & `mlflow-skinny-2.4.2/mlflow/tracking/request_header/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/transformers.py` & `mlflow-skinny-2.4.2/mlflow/transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import numpy as np
 import os
 import pathlib
 import pandas as pd
 import re
 from typing import Union, List, Optional, Dict, Any, NamedTuple
 from urllib.parse import urlparse
-
 import yaml
 
 import mlflow
 from mlflow import pyfunc
 from mlflow.exceptions import MlflowException
 from mlflow.models import ModelInputExample, Model, infer_pip_requirements
 from mlflow.models.model import MLMODEL_FILE_NAME
@@ -865,15 +864,21 @@
     """
     Loads components from a locally serialized ``Pipeline`` object.
     """
     import transformers
 
     model_instance = getattr(transformers, flavor_config[_PIPELINE_MODEL_TYPE_KEY])
     local_path = pathlib.Path(path)
-    model_path = local_path.joinpath(flavor_config.get(_MODEL_BINARY_KEY, _MODEL_BINARY_FILE_NAME))
+    # NB: Path resolution for models that were saved prior to 2.4.1 release when the pathing for
+    #     the saved pipeline or component artifacts was handled by duplicate entries for components
+    #     (artifacts/pipeline/* and artifacts/components/*) and pipelines were saved via the
+    #     "artifacts/pipeline/*" path. In order to load the older formats after the change, the
+    #     presence of the new path key is checked.
+    model_path = local_path.joinpath(flavor_config.get(_MODEL_BINARY_KEY, "pipeline"))
+
     conf = {
         "task": flavor_config[_TASK_KEY],
     }
 
     if device is None:
         if MLFLOW_DEFAULT_PREDICTION_DEVICE.get():
             try:
```

### Comparing `mlflow-skinny-2.4.1/mlflow/types/schema.py` & `mlflow-skinny-2.4.2/mlflow/types/schema.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/types/utils.py` & `mlflow-skinny-2.4.2/mlflow/types/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/__init__.py` & `mlflow-skinny-2.4.2/mlflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/_capture_modules.py` & `mlflow-skinny-2.4.2/mlflow/utils/_capture_modules.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/_capture_transformers_modules.py` & `mlflow-skinny-2.4.2/mlflow/utils/_capture_transformers_modules.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/_spark_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/_spark_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/annotations.py` & `mlflow-skinny-2.4.2/mlflow/utils/annotations.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/__init__.py` & `mlflow-skinny-2.4.2/mlflow/utils/autologging_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/client.py` & `mlflow-skinny-2.4.2/mlflow/utils/autologging_utils/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/events.py` & `mlflow-skinny-2.4.2/mlflow/utils/autologging_utils/events.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/logging_and_warnings.py` & `mlflow-skinny-2.4.2/mlflow/utils/autologging_utils/logging_and_warnings.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/safety.py` & `mlflow-skinny-2.4.2/mlflow/utils/autologging_utils/safety.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/versioning.py` & `mlflow-skinny-2.4.2/mlflow/utils/autologging_utils/versioning.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/cli_args.py` & `mlflow-skinny-2.4.2/mlflow/utils/cli_args.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/conda.py` & `mlflow-skinny-2.4.2/mlflow/utils/conda.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/databricks_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/databricks_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,18 +309,14 @@
 def get_job_type_info():
     try:
         return _get_context_tag("jobType")
     except Exception:
         return None
 
 
-def get_experiment_name_from_job_id(job_id):
-    return "jobs:/" + job_id
-
-
 @_use_repl_context_if_available("commandRunId")
 def get_command_run_id():
     try:
         return _get_command_context().commandRunId().get()
     except Exception:
         # Older runtimes may not have the commandRunId available
         return None
```

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/docstring_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/docstring_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/download_cloud_file_chunk.py` & `mlflow-skinny-2.4.2/mlflow/utils/download_cloud_file_chunk.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/environment.py` & `mlflow-skinny-2.4.2/mlflow/utils/environment.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/file_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/git_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/gorilla.py` & `mlflow-skinny-2.4.2/mlflow/utils/gorilla.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/import_hooks/__init__.py` & `mlflow-skinny-2.4.2/mlflow/utils/import_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/logging_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/mime_type_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/mime_type_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/mlflow_tags.py` & `mlflow-skinny-2.4.2/mlflow/utils/mlflow_tags.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/model_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/model_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 from pathlib import Path
 
 from mlflow.exceptions import MlflowException
 from mlflow.models import Model
 from mlflow.models.model import MLMODEL_FILE_NAME
 from mlflow.protos.databricks_pb2 import RESOURCE_DOES_NOT_EXIST, RESOURCE_ALREADY_EXISTS
+from mlflow.store.artifact.artifact_repository_registry import get_artifact_repository
 from mlflow.store.artifact.runs_artifact_repo import RunsArtifactRepository
 from mlflow.store.artifact.models_artifact_repo import ModelsArtifactRepository
 from mlflow.tracking.artifact_utils import _download_artifact_from_uri
 from mlflow.utils.uri import append_to_uri_path
 from mlflow.utils.file_utils import _copy_file_or_tree
 
 FLAVOR_CONFIG_CODE = "code"
@@ -60,17 +61,28 @@
         if RunsArtifactRepository.is_runs_uri(model_uri):
             resolved_uri = RunsArtifactRepository.get_underlying_uri(model_uri)
             logger.info("'%s' resolved as '%s'", model_uri, resolved_uri)
         elif ModelsArtifactRepository.is_models_uri(model_uri):
             resolved_uri = ModelsArtifactRepository.get_underlying_uri(model_uri)
             logger.info("'%s' resolved as '%s'", model_uri, resolved_uri)
 
-        ml_model_file = _download_artifact_from_uri(
-            artifact_uri=append_to_uri_path(resolved_uri, MLMODEL_FILE_NAME)
-        )
+        try:
+            ml_model_file = _download_artifact_from_uri(
+                artifact_uri=append_to_uri_path(resolved_uri, MLMODEL_FILE_NAME)
+            )
+        except Exception:
+            logger.debug(
+                f'Failed to download an "{MLMODEL_FILE_NAME}" model file from '
+                f"resolved URI {resolved_uri}. "
+                f"Falling back to downloading from original model URI {model_uri}",
+                exc_info=True,
+            )
+            ml_model_file = get_artifact_repository(artifact_uri=model_uri).download_artifacts(
+                artifact_path=MLMODEL_FILE_NAME
+            )
     except Exception as ex:
         raise MlflowException(
             f'Failed to download an "{MLMODEL_FILE_NAME}" model file from "{model_uri}"',
             RESOURCE_DOES_NOT_EXIST,
         ) from ex
     return _get_flavor_configuration_from_ml_model_file(ml_model_file, flavor_name)
```

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/name_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/name_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/nfs_on_spark.py` & `mlflow-skinny-2.4.2/mlflow/utils/nfs_on_spark.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/process.py` & `mlflow-skinny-2.4.2/mlflow/utils/process.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/proto_json_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/proto_json_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/request_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/request_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # DO NO IMPORT MLFLOW IN THIS FILE.
 # This file is imported by download_cloud_file_chunk.py.
 # Importing mlflow is time-consuming and we want to avoid that in artifact download subprocesses.
+import os
 import requests
 import urllib3
 
+from functools import lru_cache
 from packaging.version import Version
 from requests.adapters import HTTPAdapter
 from requests.exceptions import HTTPError
 from urllib3.util import Retry
 
 # Response codes that generally indicate transient network failures and merit client retries,
 # based on guidance from cloud service providers
@@ -47,24 +49,26 @@
         # don't overwrite the entire file.
         augmented_raise_for_status(response)
         with open(download_path, "r+b") as f:
             f.seek(range_start)
             f.write(response.content)
 
 
-def _get_request_session(max_retries, backoff_factor, retry_codes):
+@lru_cache(maxsize=64)
+def _cached_get_request_session(
+    max_retries,
+    backoff_factor,
+    retry_codes,
+    # To create a new Session object for each process, we use the process id as the cache key.
+    # This is to avoid sharing the same Session object across processes, which can lead to issues
+    # such as https://stackoverflow.com/q/3724900.
+    _pid,
+):
     """
-    Returns a `Requests.Session` object for making an HTTP request.
-
-    :param max_retries: Maximum total number of retries.
-    :param backoff_factor: a time factor for exponential backoff. e.g. value 5 means the HTTP
-      request will be retried with interval 5, 10, 20... seconds. A value of 0 turns off the
-      exponential backoff.
-    :param retry_codes: a list of HTTP response error codes that qualifies for retry.
-    :return: requests.Session object.
+    This function should not be called directly. Instead, use `_get_request_session` below.
     """
     assert 0 <= max_retries < 10
     assert 0 <= backoff_factor < 120
 
     retry_kwargs = {
         "total": max_retries,
         "connect": max_retries,
@@ -83,14 +87,33 @@
     adapter = HTTPAdapter(max_retries=retry)
     session = requests.Session()
     session.mount("https://", adapter)
     session.mount("http://", adapter)
     return session
 
 
+def _get_request_session(max_retries, backoff_factor, retry_codes):
+    """
+    Returns a `Requests.Session` object for making an HTTP request.
+
+    :param max_retries: Maximum total number of retries.
+    :param backoff_factor: a time factor for exponential backoff. e.g. value 5 means the HTTP
+      request will be retried with interval 5, 10, 20... seconds. A value of 0 turns off the
+      exponential backoff.
+    :param retry_codes: a list of HTTP response error codes that qualifies for retry.
+    :return: requests.Session object.
+    """
+    return _cached_get_request_session(
+        max_retries,
+        backoff_factor,
+        retry_codes,
+        _pid=os.getpid(),
+    )
+
+
 def _get_http_response_with_retries(
     method, url, max_retries, backoff_factor, retry_codes, **kwargs
 ):
     """
     Performs an HTTP request using Python's `requests` module with an automatic retry policy.
 
     :param method: a string indicating the method to use, e.g. "GET", "POST", "PUT".
```

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/requirements_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/requirements_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/rest_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/rest_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/search_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/server_cli_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/server_cli_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/string_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/time_utils.py` & `mlflow-skinny-2.4.2/mlflow/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/uri.py` & `mlflow-skinny-2.4.2/mlflow/utils/uri.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/validation.py` & `mlflow-skinny-2.4.2/mlflow/utils/validation.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/utils/virtualenv.py` & `mlflow-skinny-2.4.2/mlflow/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/xgboost/__init__.py` & `mlflow-skinny-2.4.2/mlflow/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow/xgboost/_autolog.py` & `mlflow-skinny-2.4.2/mlflow/xgboost/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/mlflow_skinny.egg-info/PKG-INFO` & `mlflow-skinny-2.4.2/mlflow_skinny.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-skinny
-Version: 2.4.1
+Version: 2.4.2
 Summary: MLflow: A Platform for ML Development and Productionization
 Home-page: https://mlflow.org/
 Author: Databricks
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mlflow/mlflow/issues
 Project-URL: Documentation, https://mlflow.org/docs/latest/index.html
 Project-URL: Source Code, https://github.com/mlflow/mlflow
```

### Comparing `mlflow-skinny-2.4.1/mlflow_skinny.egg-info/SOURCES.txt` & `mlflow-skinny-2.4.2/mlflow_skinny.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -172,20 +172,22 @@
 mlflow/recipes/dag_help_strings.py
 mlflow/recipes/recipe.py
 mlflow/recipes/step.py
 mlflow/recipes/cards/__init__.py
 mlflow/recipes/cards/histogram_generator.py
 mlflow/recipes/cards/pandas_renderer.py
 mlflow/recipes/cards/templates/__init__.py
+mlflow/recipes/cards/templates/base.html
 mlflow/recipes/classification/__init__.py
 mlflow/recipes/classification/v1/__init__.py
 mlflow/recipes/classification/v1/recipe.py
 mlflow/recipes/regression/__init__.py
 mlflow/recipes/regression/v1/__init__.py
 mlflow/recipes/regression/v1/recipe.py
+mlflow/recipes/resources/recipe_dag_template.html
 mlflow/recipes/steps/__init__.py
 mlflow/recipes/steps/evaluate.py
 mlflow/recipes/steps/predict.py
 mlflow/recipes/steps/register.py
 mlflow/recipes/steps/split.py
 mlflow/recipes/steps/train.py
 mlflow/recipes/steps/transform.py
@@ -274,14 +276,15 @@
 mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py
 mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py
 mlflow/store/entities/__init__.py
 mlflow/store/entities/paged_list.py
 mlflow/store/model_registry/__init__.py
 mlflow/store/model_registry/abstract_store.py
 mlflow/store/model_registry/base_rest_store.py
+mlflow/store/model_registry/databricks_workspace_model_registry_rest_store.py
 mlflow/store/model_registry/file_store.py
 mlflow/store/model_registry/rest_store.py
 mlflow/store/model_registry/sqlalchemy_store.py
 mlflow/store/model_registry/dbmodels/__init__.py
 mlflow/store/model_registry/dbmodels/models.py
 mlflow/store/tracking/__init__.py
 mlflow/store/tracking/abstract_store.py
@@ -318,15 +321,14 @@
 mlflow/tracking/context/databricks_repo_context.py
 mlflow/tracking/context/default_context.py
 mlflow/tracking/context/git_context.py
 mlflow/tracking/context/registry.py
 mlflow/tracking/context/system_environment_context.py
 mlflow/tracking/default_experiment/__init__.py
 mlflow/tracking/default_experiment/abstract_context.py
-mlflow/tracking/default_experiment/databricks_job_experiment_provider.py
 mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py
 mlflow/tracking/default_experiment/registry.py
 mlflow/tracking/request_header/__init__.py
 mlflow/tracking/request_header/abstract_request_header_provider.py
 mlflow/tracking/request_header/databricks_request_header_provider.py
 mlflow/tracking/request_header/default_request_header_provider.py
 mlflow/tracking/request_header/registry.py
```

### Comparing `mlflow-skinny-2.4.1/mlflow_skinny.egg-info/requires.txt` & `mlflow-skinny-2.4.2/mlflow_skinny.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/pylint_plugins/__init__.py` & `mlflow-skinny-2.4.2/pylint_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/pylint_plugins/errors.py` & `mlflow-skinny-2.4.2/pylint_plugins/errors.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/pylint_plugins/import_checker.py` & `mlflow-skinny-2.4.2/pylint_plugins/import_checker.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/pylint_plugins/print_function.py` & `mlflow-skinny-2.4.2/pylint_plugins/print_function.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/pylint_plugins/pytest_raises_checker/__init__.py` & `mlflow-skinny-2.4.2/pylint_plugins/pytest_raises_checker/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/pylint_plugins/set_checker.py` & `mlflow-skinny-2.4.2/pylint_plugins/set_checker.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/pylint_plugins/string_checker.py` & `mlflow-skinny-2.4.2/pylint_plugins/string_checker.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/pylint_plugins/unittest_assert_raises.py` & `mlflow-skinny-2.4.2/pylint_plugins/unittest_assert_raises.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/requirements/core-requirements.txt` & `mlflow-skinny-2.4.2/requirements/core-requirements.txt`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.1/setup.py` & `mlflow-skinny-2.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,32 +108,38 @@
     def finalize_options(self):
         pass
 
     def run(self):
         print(MINIMUM_SUPPORTED_PYTHON_VERSION)
 
 
+skinny_package_data = [
+    # include alembic files to enable usage of the skinny client with SQL databases
+    # if users install sqlalchemy and alembic independently
+    *alembic_files,
+    *extra_files,
+    *recipes_template_files,
+    *recipes_files,
+]
+
 setup(
     name="mlflow" if not _is_mlflow_skinny else "mlflow-skinny",
     version=version,
     packages=find_packages(exclude=["tests", "tests.*"]),
-    package_data={
-        "mlflow": (
-            js_files
-            + models_container_server_files
-            + alembic_files
-            + extra_files
-            + recipes_template_files
-            + recipes_files
-        ),
-    }
-    if not _is_mlflow_skinny
-    # include alembic files to enable usage of the skinny client with SQL databases
-    # if users install sqlalchemy and alembic independently
-    else {"mlflow": alembic_files + extra_files},
+    package_data=(
+        {"mlflow": skinny_package_data}
+        if _is_mlflow_skinny
+        else {
+            "mlflow": [
+                *skinny_package_data,
+                *js_files,
+                *models_container_server_files,
+            ]
+        }
+    ),
     install_requires=CORE_REQUIREMENTS if not _is_mlflow_skinny else SKINNY_REQUIREMENTS,
     extras_require={
         "extras": [
             # Required to log artifacts and models to HDFS artifact locations
             "pyarrow",
             # Required to sign outgoing request with SigV4 signature
             "requests-auth-aws-sigv4",
```

