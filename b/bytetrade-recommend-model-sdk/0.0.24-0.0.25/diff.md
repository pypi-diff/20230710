# Comparing `tmp/bytetrade-recommend-model-sdk-0.0.24.tar.gz` & `tmp/bytetrade-recommend-model-sdk-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.24.tar", last modified: Thu Jul  6 02:18:17 2023, max compression
+gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.25.tar", last modified: Mon Jul 10 21:46:10 2023, max compression
```

## Comparing `bytetrade-recommend-model-sdk-0.0.24.tar` & `bytetrade-recommend-model-sdk-0.0.25.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.359712 bytetrade-recommend-model-sdk-0.0.24/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-06 02:18:17.359712 bytetrade-recommend-model-sdk-0.0.24/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-06 02:18:17.000000 bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-07-06 02:18:17.000000 bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-06 02:18:17.000000 bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-07-06 02:18:17.000000 bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-06 02:18:17.000000 bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      489 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/bert_embedding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/embedding_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/word2vec_embedding.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/config/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/config/content_similar_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/config/mind_base_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/eval/__init_.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/eval/eval_operation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/exp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/exp/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/experiment_enum.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10528 2023-07-06 00:59:59.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/model/content_similar_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/proto_class/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/proto_class/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17830 2023-07-03 09:21:19.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/proto_class/embedding_pb2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.359712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3354 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/recommend_common_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/recommend_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/time_weight_decay_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.359712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/resources/model_management.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.359712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5147 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/aws_s3_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/common_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27513 2023-07-03 09:24:37.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/model_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-06 02:18:17.359712 bytetrade-recommend-model-sdk-0.0.24/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-07-06 02:12:13.000000 bytetrade-recommend-model-sdk-0.0.24/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.463279 bytetrade-recommend-model-sdk-0.0.25/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-10 21:46:10.463279 bytetrade-recommend-model-sdk-0.0.25/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-10 21:46:10.000000 bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-07-10 21:46:10.000000 bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 21:46:10.000000 bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-07-10 21:46:10.000000 bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-10 21:46:10.000000 bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      489 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/bert_embedding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/embedding_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/word2vec_embedding.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/config/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/config/content_similar_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/config/mind_base_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/eval/__init_.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/eval/eval_operation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/exp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/exp/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/experiment_enum.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10528 2023-07-06 00:59:59.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/model/content_similar_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/proto_class/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/proto_class/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17830 2023-07-03 09:21:19.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/proto_class/embedding_pb2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3354 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/recommend_common_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/recommend_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/time_weight_decay_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.459279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/resources/model_management.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:46:10.463279 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5147 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/aws_s3_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/common_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33393 2023-07-10 21:20:14.000000 bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/model_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-10 21:46:10.463279 bytetrade-recommend-model-sdk-0.0.25/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-07-10 21:25:29.000000 bytetrade-recommend-model-sdk-0.0.25/setup.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.24/README.md` & `bytetrade-recommend-model-sdk-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt` & `bytetrade-recommend-model-sdk-0.0.25/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/embedding_tool.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/embedding_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/word2vec_embedding.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/embeddings/word2vec_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/config/content_similar_config.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/config/content_similar_config.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/eval/eval_operation.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/eval/eval_operation.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/model/content_similar_model.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/model/content_similar_model.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/proto_class/embedding_pb2.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/proto_class/embedding_pb2.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/recommend_common_util.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/recommend_common_util.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/recommend_tool.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/recommend_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/time_weight_decay_tool.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/recommend/time_weight_decay_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/resources/model_management.json` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/resources/model_management.json`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/aws_s3_tool.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/aws_s3_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/common_tool.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/common_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/model_tool.py` & `bytetrade-recommend-model-sdk-0.0.25/recommend_model_sdk/tools/model_tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -297,15 +297,14 @@
             for current_field in feed_field_set:
                 if current_field not in current_feed:
                     current_feed[current_field] = None
             all_feed_id_to_feed[current_feed['id']] = current_feed
                 
         return all_feed_id_to_feed
         
-
     
     def download_latest_article_embedding_package(self,model_name,model_version,latest_number,publish_time=None):
         """_summary_
 
         Args:
             model_name (_type_): _description_
             model_version (_type_): _description_
@@ -515,8 +514,132 @@
                 response = self.__awss3tool.download(last_formt_dst_file,s3_bucket_name,file_name_key)
                 self.__logger.debug(f'download bucket {s3_bucket_name} file_name_key {file_name_key} response {response}')
             if os.path.exists(last_formt_dst_file) is False:
                 return False
         return True
                 
                 
-                
+    def download_increment_package(self,model_name,model_version,package_key,publish_time=None):
+        """_summary_
+
+        Args:
+            model_name (_type_): _description_
+            model_version (_type_): _description_
+            latest_number (_type_): _description_
+            start_time (_type_, optional): _description_. Defaults to None.
+
+        Raises:
+            ValueError: _description_
+            ValueError: _description_
+            ValueError: _description_
+            ValueError: _description_
+            ValueError: _description_
+
+        Returns:
+            _type_: _description_
+            url_to_article_dict 
+            {
+                "http...":{
+                    "url":
+                    "full_text":
+                    "created_at":
+                    "published_at":
+                    "title":
+                    "author":  may not exist
+                    "content":  may not exist
+                    "feed_id":
+                }
+                "http...":{
+                    
+                }
+            }
+            
+            url_to_embedding
+            {
+                "https://":{
+                    "url":
+                    "model_name":
+                    "model_version":
+                    "embeddings":[] list float
+                }
+            }
+        """
+        if isinstance(package_key,str) is False:
+            raise ValueError("package_key is not str")
+        article_field_set = set(['url', 'full_text', 'created_at', 'published_at', 'title', 'author', 'content', 'feed_id', 'hash','image_url'])
+        
+        self.valid_model_name_and_version(model_name,model_version)
+
+        latest_package_key = package_key
+        model_version_embedding_dir = os.path.join(os.path.join(os.path.join(self.__model_root_dir,model_name),model_version),'embedding')
+        if os.path.exists(model_version_embedding_dir) is False or os.path.isdir(model_version_embedding_dir) is False:
+            os.makedirs(model_version_embedding_dir)
+        current_embedding_path = os.path.join(model_version_embedding_dir,latest_package_key)
+                        
+        current_model_detail = self.__model_dict[model_name][model_version]
+        current_bucket_name = current_model_detail['s3_bucket']
+        
+        need_redownload = False
+        if os.path.exists(current_embedding_path) is False:
+            self.__logger.debug(f'current_embedding_path {current_embedding_path}  not exist')
+            need_redownload = True
+        else:
+            exist_protobuf_compress_hash = self.__common_tool.calculate_md5_for_big_file(current_embedding_path)
+            self.__logger.debug(f'current_embedding_path {current_embedding_path} does  exist ,exist file hash {exist_protobuf_compress_hash}')
+            response_header = self.__awss3tool.get_object_header(current_bucket_name, latest_package_key)
+            if ("ResponseMetadata" not in response_header or 
+                "HTTPStatusCode" not in response_header["ResponseMetadata"] or
+                response_header["ResponseMetadata"]["HTTPStatusCode"] != 200):
+                raise ValueError(f'current_bucket { current_bucket_name} key {latest_package_key} not exist')
+            if response_header["Metadata"]["md5_digest"] != exist_protobuf_compress_hash:
+                need_redownload = True
+                
+        if need_redownload:
+            result = self.__awss3tool.get_object_byte(current_bucket_name,latest_package_key)
+            if result["success"] is False:
+                raise ValueError(f"download embedding package fail result {result}")
+            current_package_compress_byte = result["bytes"]
+            with open(current_embedding_path,'wb') as f:
+                f.write(current_package_compress_byte)
+            self.__logger.debug(f'need_download {current_embedding_path}')
+        else:
+            with open(current_embedding_path,'rb') as f:
+                current_package_compress_byte = f.read()
+        
+        decompress_bytes = zlib.decompress(current_package_compress_byte)
+        current_latest_package = rec_proto_embebding.LatestPackage()
+        current_latest_package.ParseFromString(decompress_bytes)
+        
+        article_embedding_dict = MessageToDict(current_latest_package,preserving_proto_field_name=True)
+        article_list = article_embedding_dict["articles"]
+        embedding_list = article_embedding_dict["embeddings"]
+        url_to_article_dict = dict()
+        url_to_embedding_dict = dict()
+        for current_article in article_list:
+            current_article['published_at'] = int(current_article['published_at'])
+            current_article['created_at'] = int(current_article['created_at'])
+            for current_field in article_field_set:
+                if current_field not in current_article:
+                    current_article[current_field] = None
+                
+            url_to_article_dict[current_article["url"]] = current_article
+            
+        for current_embedding in embedding_list:
+            url_to_embedding_dict[current_embedding["url"]] = current_embedding    
+        
+        
+        if publish_time is not None: 
+            start_time_timestamp = int(round(publish_time.timestamp() * 1000))       
+            filter_url_to_article_dict = dict()
+            filter_url_to_embedding_dict = dict()
+            for current_url,current_article in url_to_article_dict.items():
+
+                if current_article['published_at'] > start_time_timestamp:
+                    filter_url_to_article_dict[current_url] = current_article
+                    filter_url_to_embedding_dict[current_url] = url_to_embedding_dict[current_url]
+            return filter_url_to_article_dict,filter_url_to_embedding_dict
+        else:
+            return url_to_article_dict,url_to_embedding_dict
+        
+            
+            
+
```

### Comparing `bytetrade-recommend-model-sdk-0.0.24/setup.py` & `bytetrade-recommend-model-sdk-0.0.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 sys.path.append(os.path.dirname(__file__) + "/recommend-model")
 
 
 
 
 setup(
     name="bytetrade-recommend-model-sdk",
-    version="0.0.24",
+    version="0.0.25",
     # packages=find_packages(exclude="unit_test"),
     install_requires=[
         "pandas==2.0.0",
         "gensim==4.3.1",
         "protobuf==3.20.1",
         "nltk==3.8.1",
         "boto3"
```

