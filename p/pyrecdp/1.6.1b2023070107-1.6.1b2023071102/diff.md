# Comparing `tmp/pyrecdp-1.6.1b2023070107.tar.gz` & `tmp/pyrecdp-1.6.1b2023071102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrecdp-1.6.1b2023070107.tar", last modified: Fri Jun 30 23:18:30 2023, max compression
+gzip compressed data, was "pyrecdp-1.6.1b2023071102.tar", last modified: Mon Jul 10 18:45:20 2023, max compression
```

## Comparing `pyrecdp-1.6.1b2023070107.tar` & `pyrecdp-1.6.1b2023071102.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/
--rw-r--r--   0 root         (0) root         (0)    94051 2023-06-02 20:11:31.000000 pyrecdp-1.6.1b2023070107/LICENSE
--rw-r--r--   0 root         (0) root         (0)      205 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8861 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8315 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-02 20:11:31.000000 pyrecdp-1.6.1b2023070107/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/spark-defaults.conf
--rw-r--r--   0 root         (0) root         (0)      559 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/spark-env.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/target/
--rw-r--r--   0 root         (0) root         (0)   114879 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-30 21:06:39.000000 pyrecdp-1.6.1b2023070107/pyrecdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/
--rw-r--r--   0 root         (0) root         (0)     4030 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/AutoFE.py
--rw-r--r--   0 root         (0) root         (0)    13999 2023-06-30 00:30:49.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/BasePipeline.py
--rw-r--r--   0 root         (0) root         (0)     4523 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/FeatureEstimator.py
--rw-r--r--   0 root         (0) root         (0)     3114 2023-06-29 21:19:32.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/FeatureProfiler.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-06-30 00:37:42.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/FeatureWrangler.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/RelationalBuilder.py
--rw-r--r--   0 root         (0) root         (0)      218 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/core/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      908 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/core/dataframe.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/core/di_graph.py
--rw-r--r--   0 root         (0) root         (0)      901 2023-06-30 17:24:14.000000 pyrecdp-1.6.1b2023070107/pyrecdp/core/parallel_iterator.py
--rw-r--r--   0 root         (0) root         (0)     5939 2023-06-29 22:50:40.000000 pyrecdp-1.6.1b2023070107/pyrecdp/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     7012 2023-06-30 18:42:09.000000 pyrecdp-1.6.1b2023070107/pyrecdp/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/
--rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/CESM_breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/amazon_product_review.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/base_api.py
--rw-r--r--   0 root         (0) root         (0)      288 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/download.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/ibm_fraud_detect.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/nyc_taxi.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/outbrain.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/pretrained.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/twitter_recsys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/estimators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/estimators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/estimators/base.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/estimators/lightgbm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-29 22:31:54.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/base.py
--rw-r--r--   0 root         (0) root         (0)      269 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/binned.py
--rw-r--r--   0 root         (0) root         (0)     1222 2023-06-30 15:52:33.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/category.py
--rw-r--r--   0 root         (0) root         (0)     1648 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/datetime.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-06-30 02:14:52.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/drop.py
--rw-r--r--   0 root         (0) root         (0)     5497 2023-06-29 22:51:31.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/encode.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/feature_transform.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/fillna.py
--rw-r--r--   0 root         (0) root         (0)     4666 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/name.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/nlp.py
--rw-r--r--   0 root         (0) root         (0)     4720 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/relation.py
--rw-r--r--   0 root         (0) root         (0)     2975 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6100 2023-06-29 20:57:59.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/base.py
--rw-r--r--   0 root         (0) root         (0)     2601 2023-06-30 20:29:52.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/category.py
--rw-r--r--   0 root         (0) root         (0)      351 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/custom.py
--rw-r--r--   0 root         (0) root         (0)     2293 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/data.py
--rw-r--r--   0 root         (0) root         (0)     3291 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/dataframe.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-06-30 17:44:38.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/drop.py
--rw-r--r--   0 root         (0) root         (0)     5272 2023-06-30 19:21:59.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/encode.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/fillna.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/merge.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/name.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/tuple.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/profilers/
--rw-r--r--   0 root         (0) root         (0)      157 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/profilers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5752 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/profilers/statics.py
--rw-r--r--   0 root         (0) root         (0)     4742 2023-06-29 22:28:23.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/profilers/type_infer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54072 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     8145 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/encoder.py
--rw-r--r--   0 root         (0) root         (0)     8699 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/
--rw-r--r--   0 root         (0) root         (0)     1092 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/BaseWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/PlotWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/ProfilerWidget.py
--rw-r--r--   0 root         (0) root         (0)      821 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/TabWidget.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/TableViewWidget.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/
--rw-r--r--   0 root         (0) root         (0)      989 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/base.html
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/error.html
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/interactions.html
--rw-r--r--   0 root         (0) root         (0)     1340 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/overview.html
--rw-r--r--   0 root         (0) root         (0)     7110 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/scripts.html
--rw-r--r--   0 root         (0) root         (0)    16515 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/styles.html
--rw-r--r--   0 root         (0) root         (0)     9250 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/variables.html
--rw-r--r--   0 root         (0) root         (0)      166 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8861 2023-06-30 23:18:30.000000 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3648 2023-06-30 23:18:30.000000 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 23:18:30.000000 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 20:27:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      196 2023-06-30 23:18:30.000000 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-30 23:18:30.000000 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1515 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_autofe.py
--rw-r--r--   0 root         (0) root         (0)     1856 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_feature_estimator.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_feature_profiler.py
--rw-r--r--   0 root         (0) root         (0)     2911 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_feature_wrangler.py
--rw-r--r--   0 root         (0) root         (0)     3808 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_pipeline_json.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_relational_builder.py
--rw-r--r--   0 root         (0) root         (0)     9017 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_spark_dataprocessor.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-30 23:18:24.000000 pyrecdp-1.6.1b2023070107/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.920409 pyrecdp-1.6.1b2023071102/
+-rw-r--r--   0 root         (0) root         (0)    94051 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      205 2023-06-28 06:07:34.000000 pyrecdp-1.6.1b2023071102/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8824 2023-07-10 18:45:20.920409 pyrecdp-1.6.1b2023071102/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.908408 pyrecdp-1.6.1b2023071102/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.908408 pyrecdp-1.6.1b2023071102/pyrecdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.908408 pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/spark-defaults.conf
+-rw-r--r--   0 root         (0) root         (0)      559 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/spark-env.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.908408 pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/target/
+-rw-r--r--   0 root         (0) root         (0)   114879 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.908408 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/
+-rw-r--r--   0 root         (0) root         (0)     4030 2023-07-07 08:53:54.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/AutoFE.py
+-rw-r--r--   0 root         (0) root         (0)    13999 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/BasePipeline.py
+-rw-r--r--   0 root         (0) root         (0)     4523 2023-07-07 08:53:54.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/FeatureEstimator.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/FeatureProfiler.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/FeatureWrangler.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-07 08:53:54.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/RelationalBuilder.py
+-rw-r--r--   0 root         (0) root         (0)      218 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.912408 pyrecdp-1.6.1b2023071102/pyrecdp/core/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      908 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/core/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/core/di_graph.py
+-rw-r--r--   0 root         (0) root         (0)      901 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/core/parallel_iterator.py
+-rw-r--r--   0 root         (0) root         (0)     5939 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     7012 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.912408 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/CESM_breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/amazon_product_review.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/base_api.py
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/download.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/ibm_fraud_detect.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/nyc_taxi.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/outbrain.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/pretrained.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/twitter_recsys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.912408 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.912408 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/estimators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/estimators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/estimators/base.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/estimators/lightgbm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.912408 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/base.py
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/binned.py
+-rw-r--r--   0 root         (0) root         (0)     1222 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/category.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/datetime.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/drop.py
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/encode.py
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/feature_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/fillna.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/name.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/nlp.py
+-rw-r--r--   0 root         (0) root         (0)     4720 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/relation.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.916408 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6100 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/base.py
+-rw-r--r--   0 root         (0) root         (0)     2601 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/category.py
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/custom.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/data.py
+-rw-r--r--   0 root         (0) root         (0)     3291 2023-07-07 22:06:49.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/drop.py
+-rw-r--r--   0 root         (0) root         (0)     5272 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/encode.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/fillna.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-07-07 08:53:54.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/merge.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/name.py
+-rw-r--r--   0 root         (0) root         (0)      712 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.916408 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/profilers/
+-rw-r--r--   0 root         (0) root         (0)      157 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/profilers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5752 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/profilers/statics.py
+-rw-r--r--   0 root         (0) root         (0)     4792 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/profilers/type_infer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.916408 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54072 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     8145 2023-07-07 22:06:49.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/encoder.py
+-rw-r--r--   0 root         (0) root         (0)     8699 2023-07-07 08:53:54.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.916408 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/BaseWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/PlotWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/ProfilerWidget.py
+-rw-r--r--   0 root         (0) root         (0)      821 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/TabWidget.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/TableViewWidget.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.916408 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/
+-rw-r--r--   0 root         (0) root         (0)      989 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/error.html
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/interactions.html
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/overview.html
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/scripts.html
+-rw-r--r--   0 root         (0) root         (0)    16515 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/styles.html
+-rw-r--r--   0 root         (0) root         (0)     9250 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/variables.html
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.908408 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8824 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3648 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 18:45:20.920409 pyrecdp-1.6.1b2023071102/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-06-28 06:07:34.000000 pyrecdp-1.6.1b2023071102/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.920409 pyrecdp-1.6.1b2023071102/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 06:07:34.000000 pyrecdp-1.6.1b2023071102/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/tests/test_autofe.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/tests/test_feature_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-06-27 23:05:53.000000 pyrecdp-1.6.1b2023071102/tests/test_feature_profiler.py
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/tests/test_feature_wrangler.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/tests/test_pipeline_json.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/tests/test_relational_builder.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/tests/test_spark_dataprocessor.py
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/version
```

### Comparing `pyrecdp-1.6.1b2023070107/LICENSE` & `pyrecdp-1.6.1b2023071102/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/PKG-INFO` & `pyrecdp-1.6.1b2023071102/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.6.1b2023070107
+Version: 1.6.1b2023071102
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -214,9 +212,7 @@
 
 ## LICENSE
 * Apache 2.0
 
 ## Dependency
 * Spark 3.x
 * python 3.*
-
-
```

### Comparing `pyrecdp-1.6.1b2023070107/README.md` & `pyrecdp-1.6.1b2023071102/README.md`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/spark-defaults.conf` & `pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/spark-env.sh` & `pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/spark-env.sh`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar` & `pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/__init__.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/autofe/AutoFE.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/autofe/AutoFE.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/autofe/BasePipeline.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/autofe/BasePipeline.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/autofe/FeatureEstimator.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/autofe/FeatureEstimator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/autofe/FeatureProfiler.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/autofe/FeatureProfiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/autofe/FeatureWrangler.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/autofe/FeatureWrangler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/autofe/RelationalBuilder.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/autofe/RelationalBuilder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/core/dataframe.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/core/di_graph.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/core/di_graph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/core/parallel_iterator.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/core/parallel_iterator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/core/schema.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/core/schema.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/core/utils.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/core/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/datasets/CESM_breast_cancer.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/datasets/CESM_breast_cancer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/datasets/amazon_product_review.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/datasets/amazon_product_review.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/datasets/base_api.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/datasets/base_api.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/datasets/ibm_fraud_detect.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/datasets/ibm_fraud_detect.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/datasets/nyc_taxi.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/datasets/nyc_taxi.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/datasets/outbrain.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/datasets/outbrain.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/estimators/base.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/estimators/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/estimators/lightgbm.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/estimators/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/__init__.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/category.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/datetime.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/datetime.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/drop.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/encode.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/feature_transform.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/feature_transform.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/featuretools_adaptor.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/fillna.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/geograph.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/name.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/nlp.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/nlp.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/relation.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/relation.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/type.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/base.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/category.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/data.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/data.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/dataframe.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/drop.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/encode.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/featuretools_adaptor.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/fillna.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/geograph.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/merge.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/merge.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/name.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/tuple.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/tuple.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/type.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/profilers/statics.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/profilers/statics.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/profilers/type_infer.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/profilers/type_infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 import copy
 from featuretools.primitives.base import TransformPrimitive
 from tqdm import tqdm
 
 def try_category(s):
     if pdt.is_categorical_dtype(s) and not pdt.is_bool_dtype(s):
         return False
+    if pdt.is_float_dtype(s):
+        return False
     n_unique = s.nunique()
     total_len = len(s)
     threshold = (total_len / 5)
-    if 1 <= n_unique <= threshold:
+    if 1 < n_unique <= threshold:
         return True     
     return False
 
 def try_onehot(s):
     n_unique = s.nunique()
     if n_unique < 10:
         return s.unique().tolist()
```

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/data_processor.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/data_processor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/encoder.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/encoder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/utils.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/BaseWidget.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/BaseWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/TabWidget.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/TabWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/TableViewWidget.py` & `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/TableViewWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/base.html` & `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/overview.html` & `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/overview.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/scripts.html` & `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/scripts.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/styles.html` & `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/styles.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/variables.html` & `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/variables.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/PKG-INFO` & `pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.6.1b2023070107
+Version: 1.6.1b2023071102
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -214,9 +212,7 @@
 
 ## LICENSE
 * Apache 2.0
 
 ## Dependency
 * Spark 3.x
 * python 3.*
-
-
```

### Comparing `pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/SOURCES.txt` & `pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/setup.py` & `pyrecdp-1.6.1b2023071102/setup.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/tests/test_autofe.py` & `pyrecdp-1.6.1b2023071102/tests/test_autofe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/tests/test_feature_estimator.py` & `pyrecdp-1.6.1b2023071102/tests/test_feature_estimator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/tests/test_feature_profiler.py` & `pyrecdp-1.6.1b2023071102/tests/test_feature_profiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/tests/test_feature_wrangler.py` & `pyrecdp-1.6.1b2023071102/tests/test_feature_wrangler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/tests/test_pipeline_json.py` & `pyrecdp-1.6.1b2023071102/tests/test_pipeline_json.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/tests/test_relational_builder.py` & `pyrecdp-1.6.1b2023071102/tests/test_relational_builder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023070107/tests/test_spark_dataprocessor.py` & `pyrecdp-1.6.1b2023071102/tests/test_spark_dataprocessor.py`

 * *Files identical despite different names*

