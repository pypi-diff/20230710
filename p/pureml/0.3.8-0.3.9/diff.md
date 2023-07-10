# Comparing `tmp/pureml-0.3.8.tar.gz` & `tmp/pureml-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pureml-0.3.8.tar", max compression
+gzip compressed data, was "pureml-0.3.9.tar", max compression
```

## Comparing `pureml-0.3.8.tar` & `pureml-0.3.9.tar`

### file list

```diff
@@ -1,108 +1,109 @@
--rw-r--r--   0        0        0    11789 2023-04-27 08:45:08.465073 pureml-0.3.8/README.md
--rw-r--r--   0        0        0      735 2023-05-14 12:52:56.701682 pureml-0.3.8/pureml/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/cli/__init__.py
--rw-r--r--   0        0        0     9742 2023-05-14 12:52:56.705682 pureml-0.3.8/pureml/cli/auth.py
--rw-r--r--   0        0        0     2285 2023-05-14 12:52:56.717682 pureml-0.3.8/pureml/cli/helpers.py
--rw-r--r--   0        0        0     3255 2023-05-14 12:52:56.725683 pureml-0.3.8/pureml/cli/main.py
--rw-r--r--   0        0        0     3365 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/cli/orgs.py
--rw-r--r--   0        0        0      451 2023-01-10 08:50:07.936557 pureml-0.3.8/pureml/cli/public.pem
--rw-r--r--   0        0        0     1697 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/cli/puremlconfig.py
--rw-r--r--   0        0        0     7182 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/cli/secrets.py
--rw-r--r--   0        0        0     2754 2023-05-14 12:52:56.737684 pureml-0.3.8/pureml/components/__init__.py
--rw-r--r--   0        0        0     1829 2023-05-14 12:52:56.741684 pureml-0.3.8/pureml/components/auth.py
--rw-r--r--   0        0        0    15074 2023-05-07 10:40:19.558251 pureml-0.3.8/pureml/components/dataset.py
--rw-r--r--   0        0        0       88 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/__init__.py
--rw-r--r--   0        0        0     6866 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/arrays.py
--rw-r--r--   0        0        0     6634 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/artifacts.py
--rw-r--r--   0        0        0     6708 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/audio.py
--rw-r--r--   0        0        0     9603 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/figure.py
--rw-r--r--   0        0        0     6679 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/image.py
--rw-r--r--   0        0        0     2041 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/log.py
--rw-r--r--   0        0        0     5929 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/metrics.py
--rw-r--r--   0        0        0     5925 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/params.py
--rw-r--r--   0        0        0     6166 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/pip_requirement.py
--rw-r--r--   0        0        0     6181 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/predict.py
--rw-r--r--   0        0        0     6049 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/resources.py
--rw-r--r--   0        0        0     6776 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/tabular.py
--rw-r--r--   0        0        0     6168 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/components/log/video.py
--rw-r--r--   0        0        0    13508 2023-05-07 10:40:19.558251 pureml-0.3.8/pureml/components/model.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:07.988555 pureml-0.3.8/pureml/config/__init__.py
--rw-r--r--   0        0        0     3753 2023-01-10 08:50:07.988555 pureml-0.3.8/pureml/config/parser.py
--rw-r--r--   0        0        0      123 2023-04-06 11:08:21.812260 pureml-0.3.8/pureml/decorators/__init__.py
--rw-r--r--   0        0        0     2219 2023-04-06 11:08:21.812260 pureml-0.3.8/pureml/decorators/dataset.py
--rw-r--r--   0        0        0      856 2023-04-05 12:44:15.358475 pureml-0.3.8/pureml/decorators/load_data.py
--rw-r--r--   0        0        0     2720 2023-04-05 12:44:15.358475 pureml-0.3.8/pureml/decorators/model.py
--rw-r--r--   0        0        0      607 2023-01-10 08:50:07.992555 pureml-0.3.8/pureml/decorators/pip_requirements.py
--rw-r--r--   0        0        0      838 2023-01-10 08:50:08.012554 pureml-0.3.8/pureml/decorators/predict.py
--rw-r--r--   0        0        0      895 2023-04-05 12:44:15.362475 pureml-0.3.8/pureml/decorators/transformer.py
--rw-r--r--   0        0        0       49 2023-04-05 12:44:15.362475 pureml-0.3.8/pureml/evaluate/__init__.py
--rw-r--r--   0        0        0     1489 2023-04-05 12:44:15.362475 pureml-0.3.8/pureml/evaluate/classification.py
--rw-r--r--   0        0        0     1766 2023-04-05 12:44:15.362475 pureml-0.3.8/pureml/evaluate/eval.py
--rw-r--r--   0        0        0     1665 2023-04-05 12:44:15.370475 pureml-0.3.8/pureml/evaluate/grade.py
--rw-r--r--   0        0        0      227 2023-04-05 12:44:15.382475 pureml-0.3.8/pureml/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0      633 2023-04-05 12:44:15.398476 pureml-0.3.8/pureml/evaluate/metrics/accuracy.py
--rw-r--r--   0        0        0        0 2023-04-05 12:44:15.398476 pureml-0.3.8/pureml/evaluate/metrics/base.py
--rw-r--r--   0        0        0      673 2023-04-05 12:44:15.402476 pureml-0.3.8/pureml/evaluate/metrics/confusion_matrix.py
--rw-r--r--   0        0        0      699 2023-04-05 12:44:15.406476 pureml-0.3.8/pureml/evaluate/metrics/f1.py
--rw-r--r--   0        0        0      629 2023-04-05 12:44:15.406476 pureml-0.3.8/pureml/evaluate/metrics/mae.py
--rw-r--r--   0        0        0      686 2023-04-05 12:44:15.410476 pureml-0.3.8/pureml/evaluate/metrics/mse.py
--rw-r--r--   0        0        0      802 2023-04-05 12:44:15.418476 pureml-0.3.8/pureml/evaluate/metrics/precision.py
--rw-r--r--   0        0        0      787 2023-04-05 12:44:15.434476 pureml-0.3.8/pureml/evaluate/metrics/recall.py
--rw-r--r--   0        0        0     1225 2023-04-05 12:44:15.434476 pureml-0.3.8/pureml/evaluate/metrics/roc_auc.py
--rw-r--r--   0        0        0      654 2023-04-05 12:44:15.434476 pureml-0.3.8/pureml/evaluate/regression.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.8/pureml/lineage/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.8/pureml/lineage/data/__init__.py
--rw-r--r--   0        0        0     2852 2023-04-05 12:44:15.434476 pureml-0.3.8/pureml/lineage/data/create_lineage.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:07.345247 pureml-0.3.8/pureml/package/__init__.py
--rw-r--r--   0        0        0     6446 2023-04-30 20:33:34.175641 pureml-0.3.8/pureml/package/docker.py
--rw-r--r--   0        0        0     6189 2023-05-14 12:52:56.749684 pureml-0.3.8/pureml/package/fastapi.py
--rw-r--r--   0        0        0      876 2023-03-15 11:32:07.429247 pureml-0.3.8/pureml/packaging/__init__.py
--rw-r--r--   0        0        0      496 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/errors.py
--rw-r--r--   0        0        0     2245 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_framework.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/__init__.py
--rw-r--r--   0        0        0      973 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/catboost.py
--rw-r--r--   0        0        0     1103 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/custom.py
--rw-r--r--   0        0        0      965 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/keras.py
--rw-r--r--   0        0        0      976 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/lightgbm.py
--rw-r--r--   0        0        0     1075 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/pytorch.py
--rw-r--r--   0        0        0     1146 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/pytorch_tabnet.py
--rw-r--r--   0        0        0     2163 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/sklearn.py
--rw-r--r--   0        0        0     1028 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/tensorflow.py
--rw-r--r--   0        0        0     1021 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/model_packaging/xgboost.py
--rw-r--r--   0        0        0     4006 2023-03-15 11:32:07.457247 pureml-0.3.8/pureml/packaging/packaging.py
--rw-r--r--   0        0        0     1381 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/packaging/packaging_utils.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:07.457247 pureml-0.3.8/pureml/predictor/__init__.py
--rw-r--r--   0        0        0      778 2023-03-15 11:32:07.545248 pureml-0.3.8/pureml/predictor/predictor.py
--rw-r--r--   0        0        0      439 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/schema/__init__.py
--rw-r--r--   0        0        0     2580 2023-04-27 08:45:08.465073 pureml-0.3.8/pureml/schema/backend.py
--rw-r--r--   0        0        0      350 2023-04-05 12:44:15.486478 pureml-0.3.8/pureml/schema/config.py
--rw-r--r--   0        0        0      330 2023-03-15 11:32:07.669248 pureml-0.3.8/pureml/schema/dataset.py
--rw-r--r--   0        0        0      140 2023-05-14 12:52:56.749684 pureml-0.3.8/pureml/schema/env.py
--rw-r--r--   0        0        0      474 2023-04-05 12:44:15.510478 pureml-0.3.8/pureml/schema/log.py
--rw-r--r--   0        0        0      396 2023-05-14 12:52:47.673188 pureml-0.3.8/pureml/schema/model.py
--rw-r--r--   0        0        0     1007 2023-04-11 17:20:43.542513 pureml-0.3.8/pureml/schema/packaging.py
--rw-r--r--   0        0        0     2528 2023-03-15 11:32:07.685248 pureml-0.3.8/pureml/schema/paths.py
--rw-r--r--   0        0        0     1095 2023-04-11 17:20:43.542513 pureml-0.3.8/pureml/schema/predict.py
--rw-r--r--   0        0        0      308 2023-04-27 08:45:08.469073 pureml-0.3.8/pureml/schema/request.py
--rw-r--r--   0        0        0      385 2023-03-15 11:32:07.733248 pureml-0.3.8/pureml/schema/singleton.py
--rw-r--r--   0        0        0      243 2023-04-05 12:44:15.510478 pureml-0.3.8/pureml/schema/storage.py
--rw-r--r--   0        0        0      177 2023-03-15 11:32:07.789248 pureml-0.3.8/pureml/schema/types.py
--rw-r--r--   0        0        0       66 2023-04-05 12:44:15.510478 pureml-0.3.8/pureml/settings/__init__.py
--rw-r--r--   0        0        0      278 2023-04-05 12:44:15.510478 pureml-0.3.8/pureml/settings/backend.py
--rw-r--r--   0        0        0      376 2023-04-05 12:44:15.510478 pureml-0.3.8/pureml/settings/storage.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.8/pureml/utils/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-05 12:44:15.510478 pureml-0.3.8/pureml/utils/config.py
--rw-r--r--   0        0        0     2234 2023-03-15 11:32:07.789248 pureml-0.3.8/pureml/utils/constants.py
--rw-r--r--   0        0        0     1044 2023-05-14 12:52:56.761685 pureml-0.3.8/pureml/utils/env.py
--rw-r--r--   0        0        0     2942 2023-04-27 08:45:08.469073 pureml-0.3.8/pureml/utils/hash.py
--rw-r--r--   0        0        0      522 2023-02-10 14:59:51.046215 pureml-0.3.8/pureml/utils/log_utils.py
--rw-r--r--   0        0        0     1985 2023-03-15 11:32:07.865248 pureml-0.3.8/pureml/utils/package.py
--rw-r--r--   0        0        0    14445 2023-04-10 21:10:47.359606 pureml-0.3.8/pureml/utils/pipeline.py
--rw-r--r--   0        0        0     2868 2023-04-05 12:44:15.642481 pureml-0.3.8/pureml/utils/predict.py
--rw-r--r--   0        0        0      816 2023-04-27 08:45:08.469073 pureml-0.3.8/pureml/utils/readme.py
--rw-r--r--   0        0        0     1643 2023-04-11 17:20:43.542513 pureml-0.3.8/pureml/utils/resources.py
--rw-r--r--   0        0        0      137 2023-01-10 08:50:08.036553 pureml-0.3.8/pureml/utils/source_code.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:08.013249 pureml-0.3.8/pureml/utils/types.py
--rw-r--r--   0        0        0      698 2023-03-15 11:32:08.013249 pureml-0.3.8/pureml/utils/version_utils.py
--rw-r--r--   0        0        0     1927 2023-05-14 12:52:56.765685 pureml-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    13710 1970-01-01 00:00:00.000000 pureml-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     6690 2023-05-21 10:58:34.529091 pureml-0.3.9/README.md
+-rw-r--r--   0        0        0      735 2023-07-10 21:08:37.712025 pureml-0.3.9/pureml/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/cli/__init__.py
+-rw-r--r--   0        0        0     9766 2023-07-10 21:08:37.716024 pureml-0.3.9/pureml/cli/auth.py
+-rw-r--r--   0        0        0     2285 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/cli/helpers.py
+-rw-r--r--   0        0        0     3255 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/cli/main.py
+-rw-r--r--   0        0        0     3365 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/cli/orgs.py
+-rw-r--r--   0        0        0      451 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/cli/public.pem
+-rw-r--r--   0        0        0     1697 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/cli/puremlconfig.py
+-rw-r--r--   0        0        0     7182 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/cli/secrets.py
+-rw-r--r--   0        0        0     2754 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/__init__.py
+-rw-r--r--   0        0        0     1829 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/auth.py
+-rw-r--r--   0        0        0    15074 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/dataset.py
+-rw-r--r--   0        0        0       88 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/log/__init__.py
+-rw-r--r--   0        0        0     6866 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/log/arrays.py
+-rw-r--r--   0        0        0     6634 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/log/artifacts.py
+-rw-r--r--   0        0        0     6708 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/log/audio.py
+-rw-r--r--   0        0        0     9603 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/log/figure.py
+-rw-r--r--   0        0        0     6679 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/log/image.py
+-rw-r--r--   0        0        0     2041 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/log/log.py
+-rw-r--r--   0        0        0     5929 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/log/metrics.py
+-rw-r--r--   0        0        0     5925 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/log/params.py
+-rw-r--r--   0        0        0     6166 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/log/pip_requirement.py
+-rw-r--r--   0        0        0     6181 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/log/predict.py
+-rw-r--r--   0        0        0     6049 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/log/resources.py
+-rw-r--r--   0        0        0     6776 2023-05-21 10:58:34.529091 pureml-0.3.9/pureml/components/log/tabular.py
+-rw-r--r--   0        0        0     6168 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/components/log/video.py
+-rw-r--r--   0        0        0    13508 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/components/model.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/config/__init__.py
+-rw-r--r--   0        0        0     3753 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/config/parser.py
+-rw-r--r--   0        0        0      123 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/decorators/__init__.py
+-rw-r--r--   0        0        0     2219 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/decorators/dataset.py
+-rw-r--r--   0        0        0      856 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/decorators/load_data.py
+-rw-r--r--   0        0        0     2720 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/decorators/model.py
+-rw-r--r--   0        0        0      607 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/decorators/pip_requirements.py
+-rw-r--r--   0        0        0      838 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/decorators/predict.py
+-rw-r--r--   0        0        0      895 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/decorators/transformer.py
+-rw-r--r--   0        0        0       73 2023-07-10 21:08:37.716024 pureml-0.3.9/pureml/evaluate/__init__.py
+-rw-r--r--   0        0        0     1489 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/evaluate/classification.py
+-rw-r--r--   0        0        0     4959 2023-07-10 21:08:37.716024 pureml-0.3.9/pureml/evaluate/eval.py
+-rw-r--r--   0        0        0     2150 2023-07-10 21:08:37.716024 pureml-0.3.9/pureml/evaluate/eval_old.py
+-rw-r--r--   0        0        0     1665 2023-06-14 19:32:31.884622 pureml-0.3.9/pureml/evaluate/grade.py
+-rw-r--r--   0        0        0      227 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0      633 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/evaluate/metrics/accuracy.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/evaluate/metrics/base.py
+-rw-r--r--   0        0        0      673 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/evaluate/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0      699 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/evaluate/metrics/f1.py
+-rw-r--r--   0        0        0      629 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/evaluate/metrics/mae.py
+-rw-r--r--   0        0        0      686 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/evaluate/metrics/mse.py
+-rw-r--r--   0        0        0      802 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/evaluate/metrics/precision.py
+-rw-r--r--   0        0        0      787 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/evaluate/metrics/recall.py
+-rw-r--r--   0        0        0     1225 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/evaluate/metrics/roc_auc.py
+-rw-r--r--   0        0        0      654 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/evaluate/regression.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/lineage/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/lineage/data/__init__.py
+-rw-r--r--   0        0        0     2852 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/lineage/data/create_lineage.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/package/__init__.py
+-rw-r--r--   0        0        0     6446 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/package/docker.py
+-rw-r--r--   0        0        0     6192 2023-07-10 21:08:37.728025 pureml-0.3.9/pureml/package/fastapi.py
+-rw-r--r--   0        0        0      876 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/__init__.py
+-rw-r--r--   0        0        0      496 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/errors.py
+-rw-r--r--   0        0        0     2245 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/model_framework.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/model_packaging/__init__.py
+-rw-r--r--   0        0        0      973 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/model_packaging/catboost.py
+-rw-r--r--   0        0        0     1103 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/model_packaging/custom.py
+-rw-r--r--   0        0        0      965 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/model_packaging/keras.py
+-rw-r--r--   0        0        0      976 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/model_packaging/lightgbm.py
+-rw-r--r--   0        0        0     1075 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/model_packaging/pytorch.py
+-rw-r--r--   0        0        0     1146 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/model_packaging/pytorch_tabnet.py
+-rw-r--r--   0        0        0     2163 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/model_packaging/sklearn.py
+-rw-r--r--   0        0        0     1028 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/model_packaging/tensorflow.py
+-rw-r--r--   0        0        0     1021 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/model_packaging/xgboost.py
+-rw-r--r--   0        0        0     4006 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/packaging.py
+-rw-r--r--   0        0        0     1381 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/packaging/packaging_utils.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/predictor/__init__.py
+-rw-r--r--   0        0        0      778 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/predictor/predictor.py
+-rw-r--r--   0        0        0      439 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/schema/__init__.py
+-rw-r--r--   0        0        0     2675 2023-07-10 21:08:37.728025 pureml-0.3.9/pureml/schema/backend.py
+-rw-r--r--   0        0        0      350 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/schema/config.py
+-rw-r--r--   0        0        0      330 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/schema/dataset.py
+-rw-r--r--   0        0        0      140 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/schema/env.py
+-rw-r--r--   0        0        0      474 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/schema/log.py
+-rw-r--r--   0        0        0      396 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/schema/model.py
+-rw-r--r--   0        0        0     1007 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/schema/packaging.py
+-rw-r--r--   0        0        0     2528 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/schema/paths.py
+-rw-r--r--   0        0        0     1222 2023-07-10 21:08:37.728025 pureml-0.3.9/pureml/schema/predict.py
+-rw-r--r--   0        0        0      308 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/schema/request.py
+-rw-r--r--   0        0        0      385 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/schema/singleton.py
+-rw-r--r--   0        0        0      243 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/schema/storage.py
+-rw-r--r--   0        0        0      177 2023-05-21 10:58:34.533091 pureml-0.3.9/pureml/schema/types.py
+-rw-r--r--   0        0        0       66 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/settings/__init__.py
+-rw-r--r--   0        0        0      278 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/settings/backend.py
+-rw-r--r--   0        0        0      376 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/settings/storage.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/__init__.py
+-rw-r--r--   0        0        0     1751 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/config.py
+-rw-r--r--   0        0        0     2234 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/constants.py
+-rw-r--r--   0        0        0     1044 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/env.py
+-rw-r--r--   0        0        0     2942 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/hash.py
+-rw-r--r--   0        0        0      522 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/log_utils.py
+-rw-r--r--   0        0        0     1985 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/package.py
+-rw-r--r--   0        0        0    14445 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/pipeline.py
+-rw-r--r--   0        0        0     2868 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/predict.py
+-rw-r--r--   0        0        0      816 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/readme.py
+-rw-r--r--   0        0        0     1643 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/resources.py
+-rw-r--r--   0        0        0      137 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/source_code.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/types.py
+-rw-r--r--   0        0        0      698 2023-05-21 10:58:34.537091 pureml-0.3.9/pureml/utils/version_utils.py
+-rw-r--r--   0        0        0     1954 2023-07-10 21:08:37.728025 pureml-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     8659 1970-01-01 00:00:00.000000 pureml-0.3.9/PKG-INFO
```

### Comparing `pureml-0.3.8/pureml/__init__.py` & `pureml-0.3.9/pureml/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
 from .package import docker, fastapi
 
 from .schema import Input, Output
 from .predictor.predictor import BasePredictor
 
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
```

### Comparing `pureml-0.3.8/pureml/cli/auth.py` & `pureml-0.3.9/pureml/cli/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,15 @@
                 print(f"[red]Unable to create session! Please try again later")
                 return
 
             session_id = response.json()["data"][0]["session_id"]
 
             # Generater link & Open browser
             link = urljoin(frontend_base_url, f"verify-session/{session_id}")
+            print(link)
 
             if browserless:
                 print(
                     f"Please open the following link in your browser to login: [underline]{link}[/underline]"
                 )
             else:
                 # Open browser
```

### Comparing `pureml-0.3.8/pureml/cli/helpers.py` & `pureml-0.3.9/pureml/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/cli/main.py` & `pureml-0.3.9/pureml/cli/main.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/cli/orgs.py` & `pureml-0.3.9/pureml/cli/orgs.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/cli/puremlconfig.py` & `pureml-0.3.9/pureml/cli/puremlconfig.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/cli/secrets.py` & `pureml-0.3.9/pureml/cli/secrets.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/__init__.py` & `pureml-0.3.9/pureml/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/auth.py` & `pureml-0.3.9/pureml/components/auth.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/dataset.py` & `pureml-0.3.9/pureml/components/dataset.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/log/arrays.py` & `pureml-0.3.9/pureml/components/log/arrays.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/log/artifacts.py` & `pureml-0.3.9/pureml/components/log/artifacts.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/log/audio.py` & `pureml-0.3.9/pureml/components/log/audio.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/log/figure.py` & `pureml-0.3.9/pureml/components/log/figure.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/log/image.py` & `pureml-0.3.9/pureml/components/log/image.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/log/log.py` & `pureml-0.3.9/pureml/components/log/log.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/log/metrics.py` & `pureml-0.3.9/pureml/components/log/metrics.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/log/params.py` & `pureml-0.3.9/pureml/components/log/params.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/log/pip_requirement.py` & `pureml-0.3.9/pureml/components/log/pip_requirement.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/log/predict.py` & `pureml-0.3.9/pureml/components/log/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/log/resources.py` & `pureml-0.3.9/pureml/components/log/resources.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/log/tabular.py` & `pureml-0.3.9/pureml/components/log/tabular.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/log/video.py` & `pureml-0.3.9/pureml/components/log/video.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/components/model.py` & `pureml-0.3.9/pureml/components/model.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/config/parser.py` & `pureml-0.3.9/pureml/config/parser.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/decorators/dataset.py` & `pureml-0.3.9/pureml/decorators/dataset.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/decorators/load_data.py` & `pureml-0.3.9/pureml/decorators/load_data.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/decorators/model.py` & `pureml-0.3.9/pureml/decorators/model.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/decorators/pip_requirements.py` & `pureml-0.3.9/pureml/decorators/pip_requirements.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/decorators/predict.py` & `pureml-0.3.9/pureml/decorators/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/decorators/transformer.py` & `pureml-0.3.9/pureml/decorators/transformer.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/evaluate/classification.py` & `pureml-0.3.9/pureml/evaluate/classification.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/evaluate/eval.py` & `pureml-0.3.9/pureml/evaluate/eval_old.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 from pydantic import BaseModel
 from pureml.predictor.predictor import BasePredictor
 from .grade import Grader
 from pureml.components import dataset
 from typing import Any
 from importlib import import_module
 from rich import print
+from pureml.schema import FastAPISchema, PredictSchema, PathSchema
+from pureml.package.fastapi import get_predict_file
+import shutil
+
+prediction_schema = PredictSchema()
+
 
 
 class Evaluator(BaseModel):
     task_type: str
     label_model: str
     label_dataset: str
     predictor: BasePredictor = None
-    predictor_path: str = "predict.py"
+    predictor_path: str = prediction_schema.PREDICT_NAME_TEMP
     grader: Grader = None
     dataset: Any = None
 
     class Config:
         validate_assignment = True
         arbitrary_types_allowed = True
 
     def load_dataset(self):
         self.dataset = dataset.fetch(self.label_dataset)
         print("[bold green] Succesfully fetched the dataset")
 
     def load_predictor(self):
+        get_predict_file(self.label_model,None)
+        shutil.copy(prediction_schema.PATH_PREDICT, self.predictor_path)
         module_path = self.predictor_path.replace(".py", "")
+        print(f"Module Path{module_path} and {self.predictor_path}")
         module_import = import_module(module_path)
 
         predictor_class = getattr(module_import, "Predictor")
 
         self.predictor = predictor_class()
         print("[bold green] Succesfully fetched the predictor")
```

### Comparing `pureml-0.3.8/pureml/evaluate/grade.py` & `pureml-0.3.9/pureml/evaluate/grade.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/evaluate/metrics/accuracy.py` & `pureml-0.3.9/pureml/evaluate/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/evaluate/metrics/confusion_matrix.py` & `pureml-0.3.9/pureml/evaluate/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/evaluate/metrics/f1.py` & `pureml-0.3.9/pureml/evaluate/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/evaluate/metrics/mae.py` & `pureml-0.3.9/pureml/evaluate/metrics/mae.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/evaluate/metrics/mse.py` & `pureml-0.3.9/pureml/evaluate/metrics/mse.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/evaluate/metrics/precision.py` & `pureml-0.3.9/pureml/evaluate/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/evaluate/metrics/recall.py` & `pureml-0.3.9/pureml/evaluate/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/evaluate/metrics/roc_auc.py` & `pureml-0.3.9/pureml/evaluate/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/evaluate/regression.py` & `pureml-0.3.9/pureml/evaluate/regression.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/lineage/data/create_lineage.py` & `pureml-0.3.9/pureml/lineage/data/create_lineage.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/package/docker.py` & `pureml-0.3.9/pureml/package/docker.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/package/fastapi.py` & `pureml-0.3.9/pureml/package/fastapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 import json
 import shutil
 from pureml.utils.package import process_input, process_output
 from typing import Union, Optional
 from pureml.utils.predict import predict_request_with_json, predict_request_with_file
 
 import nest_asyncio
-from pyngrok import ngrok
+#from pyngrok import ngrok
 
 load_dotenv()
 
 org_id = os.getenv('ORG_ID')
 api_token = os.getenv('API_TOKEN')
 
 if api_token is not None and org_id is not None:
@@ -145,18 +145,18 @@
     if file is not None:
         print("Processing uploaded file")
         predictions = await predict_request_with_file(file=file, predictor=predictor)
         
     return predictions
 
 if __name__ == '__main__':
-    ngrok_tunnel = ngrok.connect({PORT})
+    #ngrok_tunnel = ngrok.connect({PORT})
 
     # Public URL for fastapi server
-    print('Public URL:', ngrok_tunnel.public_url)
+    #print('Public URL:', ngrok_tunnel.public_url)
 
     nest_asyncio.apply()
 
     uvicorn.run(app, host='{HOST}', port={PORT})""".format(
         HOST=fastapi_schema.API_IP_HOST, PORT=fastapi_schema.PORT_FASTAPI
     )
```

### Comparing `pureml-0.3.8/pureml/packaging/__init__.py` & `pureml-0.3.9/pureml/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/packaging/model_framework.py` & `pureml-0.3.9/pureml/packaging/model_framework.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/packaging/model_packaging/catboost.py` & `pureml-0.3.9/pureml/packaging/model_packaging/catboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/packaging/model_packaging/custom.py` & `pureml-0.3.9/pureml/packaging/model_packaging/custom.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/packaging/model_packaging/keras.py` & `pureml-0.3.9/pureml/packaging/model_packaging/keras.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/packaging/model_packaging/lightgbm.py` & `pureml-0.3.9/pureml/packaging/model_packaging/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/packaging/model_packaging/pytorch.py` & `pureml-0.3.9/pureml/packaging/model_packaging/pytorch.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/packaging/model_packaging/pytorch_tabnet.py` & `pureml-0.3.9/pureml/packaging/model_packaging/pytorch_tabnet.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/packaging/model_packaging/sklearn.py` & `pureml-0.3.9/pureml/packaging/model_packaging/sklearn.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/packaging/model_packaging/tensorflow.py` & `pureml-0.3.9/pureml/packaging/model_packaging/tensorflow.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/packaging/model_packaging/xgboost.py` & `pureml-0.3.9/pureml/packaging/model_packaging/xgboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/packaging/packaging.py` & `pureml-0.3.9/pureml/packaging/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/packaging/packaging_utils.py` & `pureml-0.3.9/pureml/packaging/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/predictor/predictor.py` & `pureml-0.3.9/pureml/predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/schema/backend.py` & `pureml-0.3.9/pureml/schema/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,19 +45,21 @@
         # override frontend url (command specific option)
         return frontend_url
     if puremlconfig is not None:
         # user configured frontend url (self-hosted or custom pureml frontend instance)
         frontend_url = (
             puremlconfig.data["frontend_url"]
             if "frontend_url" in puremlconfig.data
-            else "https://pureml.com/"
+            #else "https://pureml.com/"
+            else "https://app.pureml.com/"
         )
     else:
         # default frontend url (production cloud frontend)
-        frontend_url = "https://pureml.com/"
+        frontend_url =  "https://app.pureml.com/"
+        #frontend_url = "https://pureml.com/"
     return frontend_url
 
 
 class BackendSchema(Singleton_BaseModel):
 
     BASE_URL: str = get_backend_base_url()
     FRONTEND_BASE_URL: str = get_frontend_base_url()
```

### Comparing `pureml-0.3.8/pureml/schema/packaging.py` & `pureml-0.3.9/pureml/schema/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/schema/paths.py` & `pureml-0.3.9/pureml/schema/paths.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/schema/predict.py` & `pureml-0.3.9/pureml/schema/predict.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,19 +14,21 @@
     shape: tuple = None
 
 
 class PredictSchema(BaseModel):
     paths: PathSchema = PathSchema().get_instance()
 
     PREDICT_NAME: str = "predict.py"
+    PREDICT_NAME_TEMP : str = "predict_temp.py"
     REQUIREMENTS_NAME: str = "requirements.txt"
     RESOURCES_NAME: str = "resources.zip"
 
     PATH_PREDICT: str = os.path.join(paths.PATH_PREDICT_DIR, PREDICT_NAME)
     PATH_PREDICT_USER: str = os.path.join(os.getcwd(), PREDICT_NAME)
+    PATH_PREDICT_USER_TEMP: str = os.path.join(os.getcwd(), PREDICT_NAME_TEMP)
 
     PATH_PREDICT_REQUIREMENTS: str = os.path.join(
         paths.PATH_PREDICT_DIR, REQUIREMENTS_NAME
     )
     PATH_PREDICT_REQUIREMENTS_USER: str = os.path.join(os.getcwd(), REQUIREMENTS_NAME)
 
     PATH_RESOURCES: str = os.path.join(paths.PATH_PREDICT_DIR, RESOURCES_NAME)
```

### Comparing `pureml-0.3.8/pureml/utils/config.py` & `pureml-0.3.9/pureml/utils/config.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/utils/constants.py` & `pureml-0.3.9/pureml/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/utils/env.py` & `pureml-0.3.9/pureml/utils/env.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/utils/hash.py` & `pureml-0.3.9/pureml/utils/hash.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/utils/log_utils.py` & `pureml-0.3.9/pureml/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/utils/package.py` & `pureml-0.3.9/pureml/utils/package.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/utils/pipeline.py` & `pureml-0.3.9/pureml/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/utils/predict.py` & `pureml-0.3.9/pureml/utils/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/utils/readme.py` & `pureml-0.3.9/pureml/utils/readme.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/utils/resources.py` & `pureml-0.3.9/pureml/utils/resources.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pureml/utils/version_utils.py` & `pureml-0.3.9/pureml/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.8/pyproject.toml` & `pureml-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pureml"
-version = "0.3.8"
+version = "0.3.9"
 description = ""
 license = "Apache-2.0"
 authors = ["vamsidhar muthireddy <vamsi.muthireddy@gmail.com>"]
 readme = "README.md"
 homepage = "https://pureml.com/"
 repository = "https://github.com/engageml-github/Pure"
 documentation = "https://docs.pureml.com"
@@ -38,14 +38,15 @@
 uvicorn = "^0.20.0"
 docker = "^6.0.1"
 python-multipart = "^0.0.5"
 nest-asyncio = "^1.5.6"
 pyngrok = "^5.2.1"
 ipapi = "^1.0.4"
 scikit-learn = "^1.2.2"
+pureml_evaluate = "^0.0.1"
 
 [tool.poetry.dev-dependencies]
 ipykernel = "^6.19.2"
 lightgbm = "^3.3.2"
 xgboost = "^1.6.1"
 catboost = "^1.0.6"
 scikit-learn = "^1.1.1"
```

