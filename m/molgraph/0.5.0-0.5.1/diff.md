# Comparing `tmp/molgraph-0.5.0.tar.gz` & `tmp/molgraph-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.5.0.tar", last modified: Fri Jul  7 16:19:32 2023, max compression
+gzip compressed data, was "molgraph-0.5.1.tar", last modified: Mon Jul 10 07:58:25 2023, max compression
```

## Comparing `molgraph-0.5.0.tar` & `molgraph-0.5.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.809165 molgraph-0.5.0/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.0/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     6608 2023-07-07 16:19:32.809165 molgraph-0.5.0/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     5888 2023-07-07 16:19:15.000000 molgraph-0.5.0/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.801165 molgraph-0.5.0/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1154 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-07 16:19:15.000000 molgraph-0.5.0/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.801165 molgraph-0.5.0/molgraph/applications/
--rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-07-04 19:57:47.000000 molgraph-0.5.0/molgraph/applications/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6644 2023-07-04 20:05:31.000000 molgraph-0.5.0/molgraph/applications/graph_transformer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.801165 molgraph-0.5.0/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.801165 molgraph-0.5.0/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.0/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.0/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.0/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.0/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-07-05 11:29:34.000000 molgraph-0.5.0/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.0/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.0/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-07-05 11:29:41.000000 molgraph-0.5.0/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.0/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.0/molgraph/chemistry/vis.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.0/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12879 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/attentional/attentive_fp_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11687 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9875 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11815 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10798 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17095 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/attentional/gt_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.0/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10194 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10144 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11216 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10507 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.0/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9933 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10823 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/geometric/gcf_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1585 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/geometric/radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    25884 2023-07-07 12:49:35.000000 molgraph-0.5.0/molgraph/layers/gnn_layer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/gnn_ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.0/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16270 2023-07-07 12:49:35.000000 molgraph-0.5.0/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14446 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/message_passing/mpnn_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.0/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10724 2023-07-07 13:13:35.000000 molgraph-0.5.0/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.0/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3407 2023-07-05 11:38:46.000000 molgraph-0.5.0/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2013 2023-07-05 11:38:48.000000 molgraph-0.5.0/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2023-07-05 11:38:49.000000 molgraph-0.5.0/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.0/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10911 2023-07-05 11:38:52.000000 molgraph-0.5.0/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4557 2023-07-05 11:38:54.000000 molgraph-0.5.0/molgraph/layers/preprocessing/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9713 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4234 2023-07-05 11:38:58.000000 molgraph-0.5.0/molgraph/layers/preprocessing/masking.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11737 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6665 2023-07-05 11:39:05.000000 molgraph-0.5.0/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20385 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.0/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6398 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/readout/attentive_fp_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4579 2023-07-07 12:49:35.000000 molgraph-0.5.0/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3285 2023-07-05 11:39:31.000000 molgraph-0.5.0/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6239 2023-07-05 11:39:33.000000 molgraph-0.5.0/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5347 2023-07-07 12:49:35.000000 molgraph-0.5.0/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.0/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2425 2023-06-14 11:03:03.000000 molgraph-0.5.0/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5371 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.0/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2023-07-05 14:45:34.000000 molgraph-0.5.0/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      518 2023-07-05 14:38:06.000000 molgraph-0.5.0/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      971 2023-07-07 12:52:08.000000 molgraph-0.5.0/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7774 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6952 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.809165 molgraph-0.5.0/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11059 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6857 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.809165 molgraph-0.5.0/molgraph/models/pretraining/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.0/molgraph/models/pretraining/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    23572 2023-07-07 12:52:08.000000 molgraph-0.5.0/molgraph/models/pretraining/autoencoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13013 2023-07-05 11:40:27.000000 molgraph-0.5.0/molgraph/models/pretraining/masked_modeling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.809165 molgraph-0.5.0/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.0/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.0/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1849 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    51923 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.801165 molgraph-0.5.0/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     6608 2023-07-07 16:19:32.000000 molgraph-0.5.0/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3308 2023-07-07 16:19:32.000000 molgraph-0.5.0/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-07 16:19:32.000000 molgraph-0.5.0/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       87 2023-07-07 16:19:32.000000 molgraph-0.5.0/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-07 16:19:32.000000 molgraph-0.5.0/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-07 16:19:32.809165 molgraph-0.5.0/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1448 2023-07-07 13:22:31.000000 molgraph-0.5.0/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.1/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6608 2023-07-10 07:58:25.397915 molgraph-0.5.1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5888 2023-07-07 16:19:15.000000 molgraph-0.5.1/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.389916 molgraph-0.5.1/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1154 2023-07-10 07:53:56.000000 molgraph-0.5.1/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/applications/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-07-04 19:57:47.000000 molgraph-0.5.1/molgraph/applications/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6644 2023-07-04 20:05:31.000000 molgraph-0.5.1/molgraph/applications/graph_transformer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.1/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.1/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.1/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.1/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-07-05 11:29:34.000000 molgraph-0.5.1/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.1/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.1/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-07-05 11:29:41.000000 molgraph-0.5.1/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.1/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.1/molgraph/chemistry/vis.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.1/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12880 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/attentional/attentive_fp_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11688 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9876 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11816 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10799 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17096 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/attentional/gt_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.1/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10195 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10145 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11217 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10508 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.1/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9934 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10824 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/geometric/gcf_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1586 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/geometric/radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    25885 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/gnn_layer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/layers/gnn_ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.1/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16271 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14447 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/message_passing/mpnn_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.1/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10725 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.1/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3408 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2014 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2984 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.1/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11134 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4559 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9716 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4237 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/masking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11954 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6668 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20608 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.1/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6399 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/readout/attentive_fp_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4640 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3286 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6241 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5348 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.1/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2428 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5375 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.1/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2075 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      519 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      971 2023-07-07 12:52:08.000000 molgraph-0.5.1/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7775 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6953 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11059 2023-07-07 12:40:08.000000 molgraph-0.5.1/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6858 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/models/pretraining/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.1/molgraph/models/pretraining/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    23576 2023-07-10 07:10:13.000000 molgraph-0.5.1/molgraph/models/pretraining/autoencoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13013 2023-07-05 11:40:27.000000 molgraph-0.5.1/molgraph/models/pretraining/masked_modeling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.397915 molgraph-0.5.1/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.1/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.1/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1991 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    52163 2023-07-10 07:57:12.000000 molgraph-0.5.1/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 07:58:25.393916 molgraph-0.5.1/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6608 2023-07-10 07:58:25.000000 molgraph-0.5.1/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3308 2023-07-10 07:58:25.000000 molgraph-0.5.1/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-10 07:58:25.000000 molgraph-0.5.1/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-07-10 07:58:25.000000 molgraph-0.5.1/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-10 07:58:25.000000 molgraph-0.5.1/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-10 07:58:25.397915 molgraph-0.5.1/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1438 2023-07-10 07:57:12.000000 molgraph-0.5.1/setup.py
```

### Comparing `molgraph-0.5.0/LICENSE` & `molgraph-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/PKG-INFO` & `molgraph-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.5.0
+Version: 0.5.1
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.5.0/README.md` & `molgraph-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/_filter_warnings.py` & `molgraph-0.5.1/molgraph/_filter_warnings.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/applications/graph_transformer.py` & `molgraph-0.5.1/molgraph/applications/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/chemistry/__init__.py` & `molgraph-0.5.1/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.5.1/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.5.1/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.5.1/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.5.1/molgraph/chemistry/benchmark/tf_records.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/chemistry/conformer_generator.py` & `molgraph-0.5.1/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/chemistry/conformer_utils.py` & `molgraph-0.5.1/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/chemistry/encoders.py` & `molgraph-0.5.1/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/chemistry/features.py` & `molgraph-0.5.1/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.5.1/molgraph/chemistry/molecular_encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/chemistry/ops.py` & `molgraph-0.5.1/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/chemistry/vis.py` & `molgraph-0.5.1/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/layers/__init__.py` & `molgraph-0.5.1/molgraph/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/layers/attentional/attentive_fp_conv.py` & `molgraph-0.5.1/molgraph/layers/attentional/attentive_fp_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers.attentional.gat_conv import GATConv
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class AttentiveFPConv(GATConv):
 
     '''Node message passing step ("Atom embedding") of AttentiveFP.
 
     `AttentiveFPConv` inherits from `GATConv` and adds a GRU update. Also
     performs a initial linear transformation on node features if needed or desired.
```

### Comparing `molgraph-0.5.0/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.5.1/molgraph/layers/attentional/gat_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 from molgraph.layers import gnn_ops 
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GATConv(gnn_layer.GNNLayer):
 
     '''Multi-head graph attention layer (GAT).
 
     The implementation is based on Velickovic et al. (2018) [#]_ and
     Dwivedi et al. (2022) [#]_.
```

### Comparing `molgraph-0.5.0/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.5.1/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GatedGCNConv(gnn_layer.GNNLayer):
 
     '''Gated graph convolutional layer (GatedGCN).
 
     Implementation is based on Dwivedi et al. (2022) [#]_, Bresson et al. (2019) [#]_,
     Joshi et al. (2019) [#]_, and Bresson et al. (2018) [#]_.
```

### Comparing `molgraph-0.5.0/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.5.1/molgraph/layers/attentional/gatv2_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 from molgraph.layers import gnn_ops
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GATv2Conv(gnn_layer.GNNLayer):
 
     '''Multi-head graph attention (v2) layer (GATv2).
 
     The implementation is based on Brody et al. (2021) [#]_.
 
     **Examples:**
```

### Comparing `molgraph-0.5.0/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.5.1/molgraph/layers/attentional/gmm_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GMMConv(gnn_layer.GNNLayer):
 
     '''Multi-head graph gaussian mixture layer (MoNet)
 
     Implementation is based on Dwivedi et al. (2022) [#]_ and 
     Monti et al. (2016) [#]_.
```

### Comparing `molgraph-0.5.0/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.5.1/molgraph/layers/attentional/gt_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 from molgraph.layers import gnn_layer
 from molgraph.layers import gnn_ops
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GTConv(gnn_layer.GNNLayer):
 
     '''Graph transformer layer
 
     Implementation is based on Dwivedi et al. (2021) [#]_.
 
     Alias: ``GraphTransformerConv``
```

### Comparing `molgraph-0.5.0/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.5.1/molgraph/layers/convolutional/gcn_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 from molgraph.layers import gnn_ops
 
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GCNConv(gnn_layer.GNNLayer):
 
     """Graph convolutional layer (GCN).
 
     Implementation is based on Kipf et al. (2017) [#]_, Dwivedi et al. (2022) [#]_,
     and, for RGCN, Schlichtkrull et al. (2017) [#]_.
```

### Comparing `molgraph-0.5.0/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.5.1/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 from molgraph.layers import gnn_ops
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GCNIIConv(gnn_layer.GNNLayer):
 
     '''Graph convolutional 'via Initial residual and Identity mapping' layer (GCNII).
 
     Implementation is based on Chen et al. (2020) [#]_.
 
     **Examples:**
```

### Comparing `molgraph-0.5.0/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.5.1/molgraph/layers/convolutional/gin_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 from molgraph.layers import gnn_layer
 from molgraph.layers import gnn_ops
 
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GINConv(gnn_layer.GNNLayer):
 
     '''Graph isomorphism convolution layer (GIN).
 
     Implementation based on Dwivedi et al. (2022) [#]_, Xu et al. (2019) [#]_, 
     and Hu et al. (2020) [#]_.
```

### Comparing `molgraph-0.5.0/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.5.1/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GraphSageConv(gnn_layer.GNNLayer):
 
     '''Graph sage convolution layer (GraphSage)
 
     Implementation is based on Hamilton et al. (2018) [#]_ and
     Dwivedi et al. (2022) [#]_.
```

### Comparing `molgraph-0.5.0/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.5.1/molgraph/layers/geometric/dtnn_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 
 from molgraph.layers.geometric import radial_basis
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class DTNNConv(gnn_layer.GNNLayer):
 
     """Deep Tensor Neural Network (DTNN).
 
     Implementation is based on Schütt et al. (2017a) [#]_.
 
     **Examples:**
```

### Comparing `molgraph-0.5.0/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.5.1/molgraph/layers/geometric/gcf_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 
 from molgraph.layers.geometric import radial_basis
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GCFConv(gnn_layer.GNNLayer):
 
     """(Graph) continuous filter convolution layer ((G)CFConv).
 
     Implementation is based on Schütt et al. (2017b) [#]_.
 
     Operates on 3D molecular graphs (encoding distance geometry).
```

### Comparing `molgraph-0.5.0/molgraph/layers/geometric/radial_basis.py` & `molgraph-0.5.1/molgraph/layers/geometric/radial_basis.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from typing import Optional
 from typing import Union
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class RadialBasis(keras.layers.Layer):
 
     def __init__(
         self,
         distance_min: float = -1.0,
         distance_max: float = 18.0,
         distance_granularity: float = 0.1,
```

### Comparing `molgraph-0.5.0/molgraph/layers/gnn_layer.py` & `molgraph-0.5.1/molgraph/layers/gnn_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_ops
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GNNLayer(layers.Layer, metaclass=abc.ABCMeta):
 
     '''Base layer for the built-in GNN layers. 
     
     Can also be used to create new GNN layers.
     
     **Example usage:**
```

### Comparing `molgraph-0.5.0/molgraph/layers/gnn_ops.py` & `molgraph-0.5.1/molgraph/layers/gnn_ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.5.1/molgraph/layers/message_passing/edge_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import Callable
 from typing import Union
 from typing import Type
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class EdgeConv(tf.keras.layers.Layer):
 
     '''Edge convolutional layer, used to build DMPNN [#]_ and DGIN [#]_ like models.
 
     **Important:**
 
     As of now, EdgeConv only works on (sub)graphs with at least one edge/bond. If your dataset consists
```

### Comparing `molgraph-0.5.0/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.5.1/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 
 from molgraph.layers import gnn_layer
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class MPNNConv(gnn_layer.GNNLayer):
 
     """Message passing neural network layer (MPNN)
 
     Implementation is based on Gilmer et al. (2017) [#]_. In contrast to Gilmer
     et al. this implementation does not use weight tying by default; for neither the 
     message function nor the update function. Furthermore, instead of the GRU-based
```

### Comparing `molgraph-0.5.0/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.5.1/molgraph/layers/positional_encoding/laplacian.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Union
 from typing import Callable
 from typing import Optional
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class LaplacianPositionalEncoding(layers.Layer):
 
     '''Laplacian positional encoding.
 
     Implementation based on Dwivedi et al. (2021) [#]_ and Belkin et al. (2003) [#]_.
 
     **Example:**
```

### Comparing `molgraph-0.5.0/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.5.1/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from tensorflow import keras
 
 from typing import Optional
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class DotProductIncident(keras.layers.Layer):
     '''Performs dot product on the incident node features.
 
     Useful for e.g., edge and link classification.
 
     **Example:**
```

### Comparing `molgraph-0.5.0/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.5.1/molgraph/layers/postprocessing/extract_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class ExtractField(keras.layers.Layer):
     '''Extract specific field of ``GraphTensor``.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
```

### Comparing `molgraph-0.5.0/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.5.1/molgraph/layers/postprocessing/gather_incident.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GatherIncident(keras.layers.Layer):
     '''Gathers incident node features.
 
     Useful for e.g., downstream edge and link classification.
 
     **Example:**
```

### Comparing `molgraph-0.5.0/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.5.1/molgraph/layers/preprocessing/center_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import tensorflow as tf
 from tensorflow import keras
 from keras import layers
-from keras.layers.preprocessing import preprocessing_utils as utils
 
 from typing import Optional
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
+try:
+    PreprocessingLayer = layers.experimental.preprocessing.PreprocessingLayer
+except AttributeError:
+    PreprocessingLayer = layers.PreprocessingLayer
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
-class CenterScaling(layers.PreprocessingLayer):
+
+@keras.saving.register_keras_serializable(package='molgraph')
+class CenterScaling(PreprocessingLayer):
 
     '''Centering.
 
     Specify, as keyword argument only,
     ``CenterScaling(feature='node_feature')`` to perform center scaling
     on the ``node_feature`` component of the ``GraphTensor``, or,
     ``CenterScaling(feature='edge_feature')`` to perform center scaling
@@ -303,22 +307,30 @@
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
 
     def get_config(self):
         config = {
-            'mean': utils.listify_tensors(self.mean),
+            'mean': _listify_tensors(self.mean),
             'feature': self.feature,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class NodeCenterScaling(CenterScaling):
     feature = 'node_feature'
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class EdgeCenterScaling(CenterScaling):
     feature = 'edge_feature'
+
+
+def _listify_tensors(x):
+    if tf.is_tensor(x):
+        x = x.numpy()
+    if isinstance(x, np.ndarray):
+        x = x.tolist()
+    return x
```

### Comparing `molgraph-0.5.0/molgraph/layers/preprocessing/dropout.py` & `molgraph-0.5.1/molgraph/layers/preprocessing/dropout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class NodeDropout(keras.layers.Layer):
     '''Randomly dropping nodes from the graph.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
@@ -74,15 +74,15 @@
 
     def get_config(self):
         config = {'rate': self.rate,}
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class EdgeDropout(NodeDropout):
     '''Randomly dropping edges from the graph.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
```

### Comparing `molgraph-0.5.0/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.5.1/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Optional
 from typing import Union
 from typing import List
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class EmbeddingLookup(layers.StringLookup):
 
     '''A loookup layer and embedding layer in combination.
 
     Specify, as keyword argument only,
     ``EmbeddingLookup(feature='node_feature', ...)`` to perform embedding lookup
     on the ``node_feature`` component of the ``GraphTensor``, or,
@@ -242,15 +242,15 @@
                 self.embeddings_regularizer),
             'embeddings_constraint': constraints.serialize(
                 self.embeddings_constraint),
         })
         return base_config
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class NodeEmbeddingLookup(EmbeddingLookup):
     feature = 'node_feature'
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class EdgeEmbeddingLookup(EmbeddingLookup):
     feature = 'edge_feature'
```

### Comparing `molgraph-0.5.0/molgraph/layers/preprocessing/masking.py` & `molgraph-0.5.1/molgraph/layers/preprocessing/masking.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class FeatureMasking(keras.layers.Layer):
     '''Randomly masking node or edge features from the graph.
 
     Important: Requires node (or edge) features to be tokenized. I.e., requires 
     the `GraphTensor` instance to be produced from `molgraph.chemistry.Tokenizer` 
     instead of `molgraph.chemistry.Tokenizer`.
 
@@ -112,15 +112,15 @@
             'rate': self.rate, 
             'mask_token': self.mask_token
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class NodeFeatureMasking(FeatureMasking):
     feature = 'node_feature'
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class EdgeFeatureMasking(FeatureMasking):
     feature = 'edge_feature'
```

### Comparing `molgraph-0.5.0/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.5.1/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import tensorflow as tf
 from tensorflow import keras
 from keras import layers
 from keras import initializers
-from keras.layers.preprocessing import preprocessing_utils as utils
 
 from typing import Tuple
 from typing import Optional
 from typing import Tuple
 
-
 from molgraph.tensors.graph_tensor import GraphTensor
 
+try:
+    PreprocessingLayer = layers.experimental.preprocessing.PreprocessingLayer
+except AttributeError:
+    PreprocessingLayer = layers.PreprocessingLayer
+
 
-@keras.utils.register_keras_serializable(package='molgraph')
-class MinMaxScaling(layers.PreprocessingLayer):
+@keras.saving.register_keras_serializable(package='molgraph')
+class MinMaxScaling(PreprocessingLayer):
 
     '''Min-max scaling between a specified range.
 
     Specify, as keyword argument only,
     ``MinMaxScaling(feature='node_feature')`` to perform min-max scaling
     on the ``node_feature`` component of the ``GraphTensor``, or,
     ``MinMaxScaling(feature='edge_feature')`` to perform min-max scaling
@@ -299,16 +302,16 @@
         if self.threshold:
             self.keep = tf.where(self.adapt_keep == True)[:, 0]
 
     def get_config(self):
         config = {
             'feature': self.feature,
             'feature_range': self.feature_range,
-            'minimum': utils.listify_tensors(self.minimum),
-            'maximum': utils.listify_tensors(self.maximum),
+            'minimum': _listify_tensors(self.minimum),
+            'maximum': _listify_tensors(self.maximum),
             'threshold': self.threshold
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
     def compute_output_shape(self, input_shape):
         if self.variance_threshold is not None:
@@ -319,15 +322,23 @@
         if self.variance_threshold is not None:
             shape = input_spec.shape[:-1]
             shape += (len(self.keep),)
             return tf.TensorSpec(shape, dtype=tf.float32)
         return input_spec
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class NodeMinMaxScaling(MinMaxScaling):
     feature = 'node_feature'
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class EdgeMinMaxScaling(MinMaxScaling):
     feature = 'edge_feature'
+
+
+def _listify_tensors(x):
+    if tf.is_tensor(x):
+        x = x.numpy()
+    if isinstance(x, np.ndarray):
+        x = x.tolist()
+    return x
```

### Comparing `molgraph-0.5.0/molgraph/layers/preprocessing/projection.py` & `molgraph-0.5.1/molgraph/layers/preprocessing/projection.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from keras import initializers
 from keras import regularizers
 from keras import constraints
 from keras import activations
 
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class FeatureProjection(layers.Layer):
 
     '''Feature projection via dense layer.
 
     Specify, as keyword argument only,
     ``FeatureProjection(feature='node_feature')`` to perform a projection
     of the ``node_feature`` component of the ``GraphTensor``, or,
@@ -154,15 +154,15 @@
             'kernel_constraint': constraints.serialize(self.kernel_constraint),
             'bias_constraint': constraints.serialize(self.bias_constraint),
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class NodeFeatureProjection(FeatureProjection):
     feature = 'node_feature'
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class EdgeFeatureProjection(FeatureProjection):
     feature = 'edge_feature'
```

### Comparing `molgraph-0.5.0/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.5.1/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import tensorflow as tf
 from tensorflow import keras
 from keras import layers
 from keras import initializers
-from keras.layers.preprocessing import preprocessing_utils as utils
 
 from typing import Optional
 from typing import Union
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
+try:
+    PreprocessingLayer = layers.experimental.preprocessing.PreprocessingLayer
+except AttributeError:
+    PreprocessingLayer = layers.PreprocessingLayer
 
-@keras.utils.register_keras_serializable(package='molgraph')
-class StandardScaling(layers.PreprocessingLayer):
+
+
+@keras.saving.register_keras_serializable(package='molgraph')
+class StandardScaling(PreprocessingLayer):
 
     '''Standard scaling, via centering and standardization.
 
     Specify, as keyword argument only,
     ``StandardScaling(feature='node_feature')`` to perform standard scaling
     on the ``node_feature`` component of the ``GraphTensor``, or,
     ``StandardScaling(feature='edge_feature')`` to perform standard scaling
@@ -376,23 +381,23 @@
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
 
     def get_config(self):
         config = {
-            'mean': utils.listify_tensors(self.mean),
-            'variance': utils.listify_tensors(self.variance),
+            'mean': _listify_tensors(self.mean),
+            'variance': _listify_tensors(self.variance),
             'feature': self.feature,
             'variance_threshold': self.variance_threshold}
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class VarianceThreshold(StandardScaling):
 
     '''Variance thresholding.
 
     Uses the ``StandardScaling`` layer but ignores the normalization when
     calling the layer.
 
@@ -556,25 +561,33 @@
 
         if self.variance_threshold is not None:
             feature = tf.gather(feature, self.keep, axis=gather_axis)
 
         return data.update({self.feature: feature})
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class NodeStandardScaling(StandardScaling):
     feature = 'node_feature'
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class EdgeStandardScaling(StandardScaling):
     feature = 'edge_feature'
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class NodeVarianceThreshold(VarianceThreshold):
     feature = 'node_feature'
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class EdgeVarianceThreshold(VarianceThreshold):
     feature = 'edge_feature'
+
+
+def _listify_tensors(x):
+    if tf.is_tensor(x):
+        x = x.numpy()
+    if isinstance(x, np.ndarray):
+        x = x.tolist()
+    return x
```

### Comparing `molgraph-0.5.0/molgraph/layers/readout/attentive_fp_readout.py` & `molgraph-0.5.1/molgraph/layers/readout/attentive_fp_readout.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from molgraph.layers.attentional.gat_conv import GATConv
 from molgraph.tensors.graph_tensor import GraphTensor
 
 Config = TypeVar('Config', bound=dict)
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class AttentiveFPReadout(tf.keras.layers.Layer):
 
     '''Readout step ("Molecule embedding") of AttentiveFP.
 
     For a complete implementation of AttentiveFP, add a number of `AttentiveFPConv` 
     steps before `AttentiveFPReadout` (see below).
```

### Comparing `molgraph-0.5.0/molgraph/layers/readout/node_readout.py` & `molgraph-0.5.1/molgraph/layers/readout/node_readout.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from tensorflow import keras
 
 from typing import Optional
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
-
+@keras.saving.register_keras_serializable(package='molgraph')
 class NodeReadout(keras.layers.Layer):
 
     '''Aggregates edge states to associated nodes.
 
     **Examples:**
 
     >>> graph_tensor = molgraph.GraphTensor(
```

### Comparing `molgraph-0.5.0/molgraph/layers/readout/segment_pool.py` & `molgraph-0.5.1/molgraph/layers/readout/segment_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from tensorflow import keras
 from keras import layers
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class SegmentPoolingReadout(layers.Layer):
 
     '''Segmentation pooling for graph readout.
 
     Alias: ``Readout``
 
     **Example:**
```

### Comparing `molgraph-0.5.0/molgraph/layers/readout/set_gather.py` & `molgraph-0.5.1/molgraph/layers/readout/set_gather.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class SetGatherReadout(layers.Layer):
 
     '''Set-to-set layer for graph readout.
 
     Implementation based on Gilmer et al. (2017) [#]_ and Vinyals et al. (2016) [#]_.
 
     **Example:**
@@ -127,15 +127,15 @@
         config = {
             'steps': self.steps,
         }
         base_config.update(config)
         return base_config
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class NoInputLSTMCell(layers.Layer):
 
     'Custom LSTM Cell that takes no input'
 
     def build(self, input_shape):
         memory_state_dim = input_shape[0][-1]
         carry_state_dim = input_shape[1][-1]
```

### Comparing `molgraph-0.5.0/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.5.1/molgraph/layers/readout/transformer_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Union
 from typing import Callable
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class TransformerEncoderReadout(layers.Layer):
 
     '''Transformer encoder layer for graph readout.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
```

### Comparing `molgraph-0.5.0/molgraph/losses/link_losses.py` & `molgraph-0.5.1/molgraph/losses/link_losses.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tensorflow as tf
 from tensorflow import keras
 
 
-@keras.utils.register_keras_serializable(package='molgraph.losses')
+@keras.saving.register_keras_serializable(package='molgraph.losses')
 class LinkBinaryCrossentropy(keras.losses.BinaryCrossentropy):
 
     def __init__(
         self,
         from_logits=True,
         label_smoothing=0.,
         axis=-1,
@@ -29,15 +29,15 @@
         y_pred = tf.concat([
             tf.ones_like(positive_score), tf.zeros_like(negative_score)
         ], axis=0)
         return super().call(y_pred, y_true)
 
 
 # TODO: Make it work for len(y_true) != len(y_pred)
-@keras.utils.register_keras_serializable(package='molgraph.losses')
+@keras.saving.register_keras_serializable(package='molgraph.losses')
 class LinkContrastiveMarginLoss(keras.losses.Loss):
 
     def __init__(
         self,
         margin=1.,
         reduction=keras.losses.Reduction.AUTO,
         name='link_contrastive_margin_loss',
@@ -51,15 +51,15 @@
     def get_config(self):
         base_config = super().get_config()
         base_config.update({'margin': self.margin})
         return base_config
 
 
 # TODO: Make it work for len(y_true) != len(y_pred)
-@keras.utils.register_keras_serializable(package='molgraph.losses')
+@keras.saving.register_keras_serializable(package='molgraph.losses')
 class LinkContrastiveBinaryCrossentropy(keras.losses.Loss):
 
     def __init__(
         self,
         reduction=keras.losses.Reduction.AUTO,
         name='link_contrastive_bce_loss',
     ):
```

### Comparing `molgraph-0.5.0/molgraph/losses/masked_losses.py` & `molgraph-0.5.1/molgraph/losses/masked_losses.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     def get_config(self):
         base_config = super().get_config()
         base_config.update({'reduction': self._reduction})
         return base_config
 
 
-@keras.utils.register_keras_serializable(package='molgraph.losses')
+@keras.saving.register_keras_serializable(package='molgraph.losses')
 class MaskedBinaryCrossentropy(MaskedLoss):
     
     '''Masked binary crossentropy loss. 
     
     Useful for multi-label classification with missing labels.
     '''
 
@@ -102,15 +102,15 @@
             'gamma': self._gamma,
             'from_logits': self._from_logits,
             'label_smoothing': self._label_smoothing,
         })
         return base_config
 
 
-@keras.utils.register_keras_serializable(package='molgraph.losses')
+@keras.saving.register_keras_serializable(package='molgraph.losses')
 class MaskedHuber(MaskedLoss):
 
     '''Masked huber loss. 
     
     Useful for multi-label regression with missing labels.
     '''
 
@@ -142,29 +142,29 @@
 
     def get_config(self):
         base_config = super().get_config()
         base_config.update({'delta': self._delta})
         return base_config
 
 
-@keras.utils.register_keras_serializable(package='molgraph.losses')
+@keras.saving.register_keras_serializable(package='molgraph.losses')
 class MaskedMeanSquaredError(MaskedLoss):
 
     '''Masked mean squared error loss. 
     
     Useful for multi-label regression with missing labels.
     '''
 
     def call(self, y_true: tf.Tensor, y_pred: tf.Tensor) -> tf.Tensor:
         y_pred = tf.convert_to_tensor(y_pred)
         y_true = tf.cast(y_true, y_pred.dtype)
         return tf.math.squared_difference(y_pred, y_true)
 
 
-@keras.utils.register_keras_serializable(package='molgraph.losses')
+@keras.saving.register_keras_serializable(package='molgraph.losses')
 class MaskedMeanAbsoluteError(MaskedLoss):
 
     '''Masked mean absolute error loss. 
     
     Useful for multi-label regression with missing labels.
     '''
```

### Comparing `molgraph-0.5.0/molgraph/metrics/masked_metrics.py` & `molgraph-0.5.1/molgraph/metrics/masked_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from molgraph.metrics.mean_relative_error import MeanRelativeError
 
 
-@keras.utils.register_keras_serializable(package='molgraph.metrics')
+@keras.saving.register_keras_serializable(package='molgraph.metrics')
 class MaskedMeanSquaredError(keras.metrics.MeanSquaredError):
 
     def update_state(self, y_true, y_pred, sample_weight=None):
         if sample_weight is not None:
             sample_weight = tf.cast(sample_weight, tf.bool)
             y_true = tf.ragged.boolean_mask(y_true, sample_weight)
             y_pred = tf.ragged.boolean_mask(y_pred, sample_weight)
         return super().update_state(y_true, y_pred, None)
 
 
-@keras.utils.register_keras_serializable(package='molgraph.metrics')
+@keras.saving.register_keras_serializable(package='molgraph.metrics')
 class MaskedMeanAbsoluteError(keras.metrics.MeanAbsoluteError):
 
     def update_state(self, y_true, y_pred, sample_weight=None):
         if sample_weight is not None:
             sample_weight = tf.cast(sample_weight, tf.bool)
             y_true = tf.ragged.boolean_mask(y_true, sample_weight)
             y_pred = tf.ragged.boolean_mask(y_pred, sample_weight)
         return super().update_state(y_true, y_pred, None)
 
 
-@keras.utils.register_keras_serializable(package='molgraph.metrics')
+@keras.saving.register_keras_serializable(package='molgraph.metrics')
 class MaskedMeanRelativeError(MeanRelativeError):
 
     def update_state(self, y_true, y_pred, sample_weight=None):
         if sample_weight is not None:
             sample_weight = tf.cast(sample_weight, tf.bool)
             y_true = tf.ragged.boolean_mask(y_true, sample_weight)
             y_pred = tf.ragged.boolean_mask(y_pred, sample_weight)
         return super().update_state(y_true, y_pred, None)
 
 
-@keras.utils.register_keras_serializable(package='molgraph.metrics')
+@keras.saving.register_keras_serializable(package='molgraph.metrics')
 class MaskedRootMeanSquaredError(keras.metrics.RootMeanSquaredError):
 
     def update_state(self, y_true, y_pred, sample_weight=None):
         if sample_weight is not None:
             sample_weight = tf.cast(sample_weight, tf.bool)
             y_true = tf.ragged.boolean_mask(y_true, sample_weight)
             y_pred = tf.ragged.boolean_mask(y_pred, sample_weight)
```

### Comparing `molgraph-0.5.0/molgraph/metrics/mean_relative_error.py` & `molgraph-0.5.1/molgraph/metrics/mean_relative_error.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tensorflow as tf
 from tensorflow import keras
 
 
-@keras.utils.register_keras_serializable(package='molgraph.metrics')
+@keras.saving.register_keras_serializable(package='molgraph.metrics')
 class MeanRelativeError(keras.metrics.Mean):
 
     def update_state(self, y_true, y_pred, sample_weight=None):
         y_true = tf.cast(y_true, self._dtype)
         y_pred = tf.cast(y_pred, self._dtype)
         abs_error = tf.abs(y_true - y_pred)
         mr_error = tf.math.divide_no_nan(abs_error, tf.math.abs(y_true))
```

### Comparing `molgraph-0.5.0/molgraph/models/__init__.py` & `molgraph-0.5.1/molgraph/models/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/models/dgin.py` & `molgraph-0.5.1/molgraph/models/dgin.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Callable
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.gnn_ops import propagate_node_features
 from molgraph.layers.message_passing.edge_conv import edge_message_step
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class DGIN(keras.models.Model):
 
     '''Directed graph isomorphism network (DGIN).
 
     Implementation is based on Wieder et al. (2021) [#]_. 
     
     **Important:**
```

### Comparing `molgraph-0.5.0/molgraph/models/dmpnn.py` & `molgraph-0.5.1/molgraph/models/dmpnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Union
 from typing import Callable
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.message_passing.edge_conv import edge_message_step
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class DMPNN(keras.models.Model):
 
     '''Directed message passing neural network (DMPNN).
 
     Implementation is based on Yang et al. (2019) [#]_.
 
     **Important:**
```

### Comparing `molgraph-0.5.0/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.5.1/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/models/interpretability/saliency.py` & `molgraph-0.5.1/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/models/mpnn.py` & `molgraph-0.5.1/molgraph/models/mpnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional
 from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.message_passing.mpnn_conv import message_step
 
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class MPNN(keras.layers.Layer):
 
     '''Message passing neural network (MPNN) with weight tying.
 
     Implementation is based on Gilmer et al. (2017) [#]_. In contrast to
     ``MPNNConv``, which performs a single step of message passing, ``MPNN``
     performs n-steps of message passing. Furthermore, the weights are shared
```

### Comparing `molgraph-0.5.0/molgraph/models/pretraining/autoencoders.py` & `molgraph-0.5.1/molgraph/models/pretraining/autoencoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.postprocessing.dot_product_incident import DotProductIncident
 from molgraph.losses.link_losses import LinkBinaryCrossentropy
 
     
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GraphAutoEncoder(keras.Model):
     '''Graph AutoEncoder (GAE) based on Kipf and Welling [#]_.
     
     Args:
         encoder (tf.keras.layers.Layer):
             The encoder part of the autoencoder. The encoder could be
             any of the graph neural neural network layers provided by
@@ -300,15 +300,15 @@
             `GraphTensor` as well as decoded `GraphTensor`s.
         '''
         return super().predict(
             x=x, batch_size=batch_size, *args, **kwargs)
 
       
 # TODO: instead of beta_initial/end/incr, pass a scheduler?
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class GraphVariationalAutoEncoder(GraphAutoEncoder):
     '''Graph Variational AutoEncoder (GAE) based on Kipf and Welling [#]_.
     
     Args:
         encoder (tf.keras.layers.Layer):
             The encoder part of the autoencoder. The encoder could be
             any of the graph neural neural network layers provided by
@@ -507,15 +507,15 @@
         config = super().get_config()
         config.update({
             'beta_initial': self.beta_initial,
             'beta_end': self.beta_end,
             'beta_incr': self.beta_incr
         })
 
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class NaiveNegativeGraphSampler(layers.Layer):
     
     '''Samples a negative graphs, or rather, a graph with negative edges.
     
     It is a "naive" implementation as it simply just shuffles `edge_dst` of
     the `GraphTensor` instance, without considering that the resulting
     `edge_dst` and `edge_src` pair could be a positive (correct) edge.
@@ -544,15 +544,15 @@
         return tensor.__class__(**data)
     
     def get_config(self):
         config = super().get_config()
         config.update({'k': self.k})
         return config
     
-@keras.utils.register_keras_serializable(package='molgraph')
+@keras.saving.register_keras_serializable(package='molgraph')
 class NegativeGraphSampler(NaiveNegativeGraphSampler):
     
     '''Samples a negative graphs, or rather, a graph with negative edges.
     
     This is a "non-naive" implementation as it makes sure that the original
     (positive) edges do not exist in the set of negative edges.
```

### Comparing `molgraph-0.5.0/molgraph/models/pretraining/masked_modeling.py` & `molgraph-0.5.1/molgraph/models/pretraining/masked_modeling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/tensors/_graph_tensor.py` & `molgraph-0.5.1/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.5.1/molgraph/tensors/graph_keras_tensor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,18 @@
-from keras.engine import keras_tensor
-from keras.layers import core
+try:
+    from keras.engine import keras_tensor
+except ImportError:
+    from keras.src.engine import keras_tensor
 
-from molgraph.tensors.graph_tensor import GraphTensor
+try:
+    from keras.layers import core
+except ImportError:
+    from keras.src.layers import core
 
+from molgraph.tensors.graph_tensor import GraphTensor
 
 
 class GraphKerasTensor(keras_tensor.KerasTensor):
 
     @property
     def dtype(self):
         return self.spec.dtype
```

### Comparing `molgraph-0.5.0/molgraph/tensors/graph_tensor.py` & `molgraph-0.5.1/molgraph/tensors/graph_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 import tensorflow as tf
 
 from tensorflow.python.framework import composite_tensor
 from tensorflow.python.framework import type_spec
 
+try:
+    from tensorflow.python.framework import type_spec_registry
+except ImportError:
+    type_spec_registry = None
+
 import numpy as np
 
 from typing import Optional
 from typing import Mapping
 from typing import List
 from typing import Tuple
 from typing import Union
 from typing import Any
 from typing import Type
 
 from molgraph.layers import gnn_ops
 
 
+type_spec_registry = (
+    type_spec_registry.register if type_spec_registry is not None 
+    else type_spec.register
+)
+
 _allowable_input_types = (
     tf.Tensor,
     tf.RaggedTensor,
     np.ndarray,
     list,
     tuple
 )
@@ -743,15 +753,15 @@
             else:
                 # Should not happen, but just in case.
                 fields.append('{}=<unknown>'.format(key))
 
         return f'GraphTensor(\n  ' + ',\n  '.join(fields) + ')'
 
 
-@type_spec.register('molgraph.tensors.graph_tensor.GraphTensorSpec')
+@type_spec_registry('molgraph.tensors.graph_tensor.GraphTensorSpec')
 class GraphTensorSpec(type_spec.BatchableTypeSpec):
 
     '''Spec of :class:`~GraphTensor`.
     '''
     __slots__ = ('_data_spec', '_shape', '_dtype')
 
     def __init__(
```

### Comparing `molgraph-0.5.0/molgraph.egg-info/PKG-INFO` & `molgraph-0.5.1/molgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.5.0
+Version: 0.5.1
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.5.0/molgraph.egg-info/SOURCES.txt` & `molgraph-0.5.1/molgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.0/setup.py` & `molgraph-0.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   from _version import __version__ as version
   return version
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 install_requires = [
-    "tensorflow>=2.7.0, <=2.12.0",
+    "tensorflow>=2.7.0",
     "numpy>=1.21.2",
     "rdkit>=2022.3.3",
     "pandas>=1.0.3",
     "ipython==8.12.0",
 ]
 
 setuptools.setup(
```

