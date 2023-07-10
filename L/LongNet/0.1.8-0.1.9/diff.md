# Comparing `tmp/LongNet-0.1.8.tar.gz` & `tmp/LongNet-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.1.8.tar", last modified: Mon Jul 10 18:17:20 2023, max compression
+gzip compressed data, was "LongNet-0.1.9.tar", last modified: Mon Jul 10 18:34:23 2023, max compression
```

## Comparing `LongNet-0.1.8.tar` & `LongNet-0.1.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:20.420567 LongNet-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 18:17:08.000000 LongNet-0.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:20.404566 LongNet-0.1.8/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 18:17:08.000000 LongNet-0.1.8/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-10 18:17:08.000000 LongNet-0.1.8/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-07-10 18:17:08.000000 LongNet-0.1.8/LongNet/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-10 18:17:08.000000 LongNet-0.1.8/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-10 18:17:08.000000 LongNet-0.1.8/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-10 18:17:08.000000 LongNet-0.1.8/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:20.404566 LongNet-0.1.8/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 18:17:20.000000 LongNet-0.1.8/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-10 18:17:20.000000 LongNet-0.1.8/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:17:20.000000 LongNet-0.1.8/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 18:17:20.000000 LongNet-0.1.8/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 18:17:20.000000 LongNet-0.1.8/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 18:17:20.420567 LongNet-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-07-10 18:17:08.000000 LongNet-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:20.408567 LongNet-0.1.8/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:20.412567 LongNet-0.1.8/flash_attn/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/bert_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/flash_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/flash_attn_triton.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/flash_attn_triton_og.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/flash_blocksparse_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/flash_blocksparse_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/fused_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:20.412567 LongNet-0.1.8/flash_attn/flash_attn/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/layers/patch_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/layers/rotary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:20.412567 LongNet-0.1.8/flash_attn/flash_attn/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/losses/cross_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:20.416567 LongNet-0.1.8/flash_attn/flash_attn/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/models/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/models/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/models/gpt_neox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/models/gptj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/models/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/models/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/models/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:20.416567 LongNet-0.1.8/flash_attn/flash_attn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/modules/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/modules/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/modules/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:20.416567 LongNet-0.1.8/flash_attn/flash_attn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/ops/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/ops/fused_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    19306 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/ops/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/ops/rms_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:20.420567 LongNet-0.1.8/flash_attn/flash_attn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/utils/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/utils/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/flash_attn/utils/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-10 18:17:08.000000 LongNet-0.1.8/flash_attn/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:17:20.420567 LongNet-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-10 18:17:08.000000 LongNet-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:17:20.420567 LongNet-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 18:17:08.000000 LongNet-0.1.8/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:23.951028 LongNet-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 18:34:14.000000 LongNet-0.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:23.943029 LongNet-0.1.9/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 18:34:14.000000 LongNet-0.1.9/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-07-10 18:34:14.000000 LongNet-0.1.9/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-07-10 18:34:14.000000 LongNet-0.1.9/LongNet/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-10 18:34:14.000000 LongNet-0.1.9/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-10 18:34:14.000000 LongNet-0.1.9/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-10 18:34:14.000000 LongNet-0.1.9/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:23.947028 LongNet-0.1.9/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 18:34:23.000000 LongNet-0.1.9/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-10 18:34:23.000000 LongNet-0.1.9/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:34:23.000000 LongNet-0.1.9/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 18:34:23.000000 LongNet-0.1.9/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 18:34:23.000000 LongNet-0.1.9/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 18:34:23.951028 LongNet-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-07-10 18:34:14.000000 LongNet-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:23.947028 LongNet-0.1.9/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:23.947028 LongNet-0.1.9/flash_attn/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/bert_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/flash_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/flash_attn_triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/flash_attn_triton_og.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/flash_blocksparse_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/flash_blocksparse_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/fused_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:23.947028 LongNet-0.1.9/flash_attn/flash_attn/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/layers/patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/layers/rotary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:23.947028 LongNet-0.1.9/flash_attn/flash_attn/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/losses/cross_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:23.947028 LongNet-0.1.9/flash_attn/flash_attn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/models/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/models/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/models/gpt_neox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/models/gptj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/models/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/models/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:23.947028 LongNet-0.1.9/flash_attn/flash_attn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/modules/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/modules/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/modules/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:23.951028 LongNet-0.1.9/flash_attn/flash_attn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/ops/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/ops/fused_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19306 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/ops/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/ops/rms_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:23.951028 LongNet-0.1.9/flash_attn/flash_attn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/utils/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/flash_attn/utils/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-10 18:34:14.000000 LongNet-0.1.9/flash_attn/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:34:23.951028 LongNet-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-10 18:34:14.000000 LongNet-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:34:23.951028 LongNet-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 18:34:14.000000 LongNet-0.1.9/test/test.py
```

### Comparing `LongNet-0.1.8/LICENSE` & `LongNet-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/LongNet/attend.py` & `LongNet-0.1.9/LongNet/attend.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,29 +45,31 @@
 # main class
 
 class FlashAttention(nn.Module):
     def __init__(
         self,
         *,
         dropout = 0.,
+        attention_dropout=0.,
         causal = False,
         heads = None,
         talking_heads = False,
         scale = None,
         qk_norm = True,
         flash = True,
     ):
         super().__init__()
         self.scale = scale
         self.qk_norm = qk_norm
         self.causal = causal
         self.attn_fn = partial(F.softmax, dtype = torch.float32) if not qk_norm else F.softmax
 
         self.dropout = dropout
-        self.attn_dropout = nn.Dropout(dropout)
+
+        self.attn_dropout = nn.Dropout(attention_dropout)   # modify this line
 
         # talking heads
 
         assert not (flash and talking_heads), 'talking heads not compatible with flash attention'
 
         self.talking_heads = talking_heads
         if talking_heads:
```

### Comparing `LongNet-0.1.8/LongNet/attention.py` & `LongNet-0.1.9/LongNet/attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
         if use_xpos:
             self.xpos = XPOS(head_dim=d_model//num_heads)
         if use_rel_pos_bias:
             self.relative_bias = RelativePositionBias(num_buckets=32, max_distance=128, n_heads=num_heads)
 
         #head offsets
-        self.head_offsets = nn.Parameer(torch.randn(num_heads, d_model))
+        self.head_offsets = nn.Parameter(torch.randn(num_heads, d_model))
 
     def get_mask(self, i, j):
         return torch.ones((i, j), device=device, dtype=torch.bool).triu(j - i + 2)
 
     def forward(self, x):
         batch_size, seq_len, _ = x.shape
```

### Comparing `LongNet-0.1.8/LongNet/model.py` & `LongNet-0.1.9/LongNet/model.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/LongNet/training.py` & `LongNet-0.1.9/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/LongNet/utils.py` & `LongNet-0.1.9/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/LongNet.egg-info/PKG-INFO` & `LongNet-0.1.9/LongNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.1.8
+Version: 0.1.9
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.1.8/LongNet.egg-info/SOURCES.txt` & `LongNet-0.1.9/LongNet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/PKG-INFO` & `LongNet-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.1.8
+Version: 0.1.9
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.1.8/README.md` & `LongNet-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/bert_padding.py` & `LongNet-0.1.9/flash_attn/flash_attn/bert_padding.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/flash_attention.py` & `LongNet-0.1.9/flash_attn/flash_attn/flash_attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/flash_attn_interface.py` & `LongNet-0.1.9/flash_attn/flash_attn/flash_attn_interface.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/flash_attn_triton.py` & `LongNet-0.1.9/flash_attn/flash_attn/flash_attn_triton.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/flash_attn_triton_og.py` & `LongNet-0.1.9/flash_attn/flash_attn/flash_attn_triton_og.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/flash_blocksparse_attention.py` & `LongNet-0.1.9/flash_attn/flash_attn/flash_blocksparse_attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/flash_blocksparse_attn_interface.py` & `LongNet-0.1.9/flash_attn/flash_attn/flash_blocksparse_attn_interface.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/fused_softmax.py` & `LongNet-0.1.9/flash_attn/flash_attn/fused_softmax.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/layers/patch_embed.py` & `LongNet-0.1.9/flash_attn/flash_attn/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/layers/rotary.py` & `LongNet-0.1.9/flash_attn/flash_attn/layers/rotary.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/losses/cross_entropy.py` & `LongNet-0.1.9/flash_attn/flash_attn/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/models/bert.py` & `LongNet-0.1.9/flash_attn/flash_attn/models/bert.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/models/gpt.py` & `LongNet-0.1.9/flash_attn/flash_attn/models/gpt.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/models/gpt_neox.py` & `LongNet-0.1.9/flash_attn/flash_attn/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/models/gptj.py` & `LongNet-0.1.9/flash_attn/flash_attn/models/gptj.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/models/llama.py` & `LongNet-0.1.9/flash_attn/flash_attn/models/llama.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/models/opt.py` & `LongNet-0.1.9/flash_attn/flash_attn/models/opt.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/models/vit.py` & `LongNet-0.1.9/flash_attn/flash_attn/models/vit.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/modules/block.py` & `LongNet-0.1.9/flash_attn/flash_attn/modules/block.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/modules/embedding.py` & `LongNet-0.1.9/flash_attn/flash_attn/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/modules/mha.py` & `LongNet-0.1.9/flash_attn/flash_attn/modules/mha.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/modules/mlp.py` & `LongNet-0.1.9/flash_attn/flash_attn/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/ops/activations.py` & `LongNet-0.1.9/flash_attn/flash_attn/ops/activations.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/ops/fused_dense.py` & `LongNet-0.1.9/flash_attn/flash_attn/ops/fused_dense.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/ops/layer_norm.py` & `LongNet-0.1.9/flash_attn/flash_attn/ops/layer_norm.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/ops/rms_norm.py` & `LongNet-0.1.9/flash_attn/flash_attn/ops/rms_norm.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/utils/benchmark.py` & `LongNet-0.1.9/flash_attn/flash_attn/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/utils/distributed.py` & `LongNet-0.1.9/flash_attn/flash_attn/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/utils/generation.py` & `LongNet-0.1.9/flash_attn/flash_attn/utils/generation.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/flash_attn/utils/pretrained.py` & `LongNet-0.1.9/flash_attn/flash_attn/utils/pretrained.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/flash_attn/setup.py` & `LongNet-0.1.9/flash_attn/setup.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.8/setup.py` & `LongNet-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.1.8',
+  version = '0.1.9',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

### Comparing `LongNet-0.1.8/test/test.py` & `LongNet-0.1.9/test/test.py`

 * *Files identical despite different names*

