# Comparing `tmp/LongNet-0.1.6.tar.gz` & `tmp/LongNet-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.1.6.tar", last modified: Mon Jul 10 18:04:39 2023, max compression
+gzip compressed data, was "LongNet-0.1.7.tar", last modified: Mon Jul 10 18:11:58 2023, max compression
```

## Comparing `LongNet-0.1.6.tar` & `LongNet-0.1.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:39.217959 LongNet-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 18:04:27.000000 LongNet-0.1.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:39.201958 LongNet-0.1.6/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 18:04:27.000000 LongNet-0.1.6/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-10 18:04:27.000000 LongNet-0.1.6/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-07-10 18:04:27.000000 LongNet-0.1.6/LongNet/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-10 18:04:27.000000 LongNet-0.1.6/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-10 18:04:27.000000 LongNet-0.1.6/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-10 18:04:27.000000 LongNet-0.1.6/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:39.201958 LongNet-0.1.6/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 18:04:39.000000 LongNet-0.1.6/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-10 18:04:39.000000 LongNet-0.1.6/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:04:39.000000 LongNet-0.1.6/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 18:04:39.000000 LongNet-0.1.6/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 18:04:39.000000 LongNet-0.1.6/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 18:04:39.217959 LongNet-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-07-10 18:04:27.000000 LongNet-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:39.201958 LongNet-0.1.6/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:39.205958 LongNet-0.1.6/flash_attn/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/bert_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/flash_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/flash_attn_triton.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/flash_attn_triton_og.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/flash_blocksparse_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/flash_blocksparse_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/fused_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:39.205958 LongNet-0.1.6/flash_attn/flash_attn/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/layers/patch_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/layers/rotary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:39.209959 LongNet-0.1.6/flash_attn/flash_attn/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/losses/cross_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:39.209959 LongNet-0.1.6/flash_attn/flash_attn/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/models/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/models/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/models/gpt_neox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/models/gptj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/models/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/models/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/models/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:39.213959 LongNet-0.1.6/flash_attn/flash_attn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/modules/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/modules/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/modules/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:39.213959 LongNet-0.1.6/flash_attn/flash_attn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/ops/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/ops/fused_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    19306 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/ops/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/ops/rms_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:39.213959 LongNet-0.1.6/flash_attn/flash_attn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/utils/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/utils/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/flash_attn/utils/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-10 18:04:27.000000 LongNet-0.1.6/flash_attn/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:04:39.217959 LongNet-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-10 18:04:27.000000 LongNet-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:04:39.217959 LongNet-0.1.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 18:04:27.000000 LongNet-0.1.6/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:58.098079 LongNet-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 18:11:48.000000 LongNet-0.1.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:58.094079 LongNet-0.1.7/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 18:11:48.000000 LongNet-0.1.7/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-10 18:11:48.000000 LongNet-0.1.7/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-07-10 18:11:48.000000 LongNet-0.1.7/LongNet/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-10 18:11:48.000000 LongNet-0.1.7/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-10 18:11:48.000000 LongNet-0.1.7/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-10 18:11:48.000000 LongNet-0.1.7/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:58.094079 LongNet-0.1.7/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 18:11:58.000000 LongNet-0.1.7/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-10 18:11:58.000000 LongNet-0.1.7/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:11:58.000000 LongNet-0.1.7/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 18:11:58.000000 LongNet-0.1.7/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 18:11:58.000000 LongNet-0.1.7/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 18:11:58.098079 LongNet-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-07-10 18:11:48.000000 LongNet-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:58.094079 LongNet-0.1.7/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:58.094079 LongNet-0.1.7/flash_attn/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/bert_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/flash_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/flash_attn_triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/flash_attn_triton_og.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/flash_blocksparse_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/flash_blocksparse_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/fused_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:58.094079 LongNet-0.1.7/flash_attn/flash_attn/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/layers/patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/layers/rotary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:58.098079 LongNet-0.1.7/flash_attn/flash_attn/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/losses/cross_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:58.098079 LongNet-0.1.7/flash_attn/flash_attn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/models/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/models/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/models/gpt_neox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/models/gptj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/models/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/models/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:58.098079 LongNet-0.1.7/flash_attn/flash_attn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/modules/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/modules/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/modules/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:58.098079 LongNet-0.1.7/flash_attn/flash_attn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/ops/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/ops/fused_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19306 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/ops/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/ops/rms_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:58.098079 LongNet-0.1.7/flash_attn/flash_attn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/utils/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/flash_attn/utils/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-10 18:11:48.000000 LongNet-0.1.7/flash_attn/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:11:58.098079 LongNet-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-10 18:11:48.000000 LongNet-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:58.098079 LongNet-0.1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 18:11:48.000000 LongNet-0.1.7/test/test.py
```

### Comparing `LongNet-0.1.6/LICENSE` & `LongNet-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/LongNet/attend.py` & `LongNet-0.1.7/LongNet/attend.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/LongNet/attention.py` & `LongNet-0.1.7/LongNet/attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/LongNet/model.py` & `LongNet-0.1.7/LongNet/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import torch
 from torch.nn import Embedding, Module
 import bitsandbytes
 
-from torchscale import DecoderConfig, Decoder, PositionalEmbedding
 from transformers import AutoTokenizer
 
+
+from torchscale.architecture.config import DecoderConfig
+from torchscale.architecture.decoder import Decoder
+from torchscale.component.embedding import PositionalEmbedding
+
+
 class LongNetTokenizer:
     def __init__(self):
         self.tokenizer = AutoTokenizer.from_pretrained(
             "EleutherAI/gpt-neox-20b",
             eos_token="<eos>",
             pad_token="<pad>",
             extra_ids=0,
```

### Comparing `LongNet-0.1.6/LongNet/training.py` & `LongNet-0.1.7/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/LongNet/utils.py` & `LongNet-0.1.7/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/LongNet.egg-info/PKG-INFO` & `LongNet-0.1.7/LongNet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.1.6
+Version: 0.1.7
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.1.6/LongNet.egg-info/SOURCES.txt` & `LongNet-0.1.7/LongNet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/PKG-INFO` & `LongNet-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.1.6
+Version: 0.1.7
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.1.6/README.md` & `LongNet-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/bert_padding.py` & `LongNet-0.1.7/flash_attn/flash_attn/bert_padding.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/flash_attention.py` & `LongNet-0.1.7/flash_attn/flash_attn/flash_attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/flash_attn_interface.py` & `LongNet-0.1.7/flash_attn/flash_attn/flash_attn_interface.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/flash_attn_triton.py` & `LongNet-0.1.7/flash_attn/flash_attn/flash_attn_triton.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/flash_attn_triton_og.py` & `LongNet-0.1.7/flash_attn/flash_attn/flash_attn_triton_og.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/flash_blocksparse_attention.py` & `LongNet-0.1.7/flash_attn/flash_attn/flash_blocksparse_attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/flash_blocksparse_attn_interface.py` & `LongNet-0.1.7/flash_attn/flash_attn/flash_blocksparse_attn_interface.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/fused_softmax.py` & `LongNet-0.1.7/flash_attn/flash_attn/fused_softmax.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/layers/patch_embed.py` & `LongNet-0.1.7/flash_attn/flash_attn/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/layers/rotary.py` & `LongNet-0.1.7/flash_attn/flash_attn/layers/rotary.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/losses/cross_entropy.py` & `LongNet-0.1.7/flash_attn/flash_attn/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/models/bert.py` & `LongNet-0.1.7/flash_attn/flash_attn/models/bert.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/models/gpt.py` & `LongNet-0.1.7/flash_attn/flash_attn/models/gpt.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/models/gpt_neox.py` & `LongNet-0.1.7/flash_attn/flash_attn/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/models/gptj.py` & `LongNet-0.1.7/flash_attn/flash_attn/models/gptj.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/models/llama.py` & `LongNet-0.1.7/flash_attn/flash_attn/models/llama.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/models/opt.py` & `LongNet-0.1.7/flash_attn/flash_attn/models/opt.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/models/vit.py` & `LongNet-0.1.7/flash_attn/flash_attn/models/vit.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/modules/block.py` & `LongNet-0.1.7/flash_attn/flash_attn/modules/block.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/modules/embedding.py` & `LongNet-0.1.7/flash_attn/flash_attn/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/modules/mha.py` & `LongNet-0.1.7/flash_attn/flash_attn/modules/mha.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/modules/mlp.py` & `LongNet-0.1.7/flash_attn/flash_attn/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/ops/activations.py` & `LongNet-0.1.7/flash_attn/flash_attn/ops/activations.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/ops/fused_dense.py` & `LongNet-0.1.7/flash_attn/flash_attn/ops/fused_dense.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/ops/layer_norm.py` & `LongNet-0.1.7/flash_attn/flash_attn/ops/layer_norm.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/ops/rms_norm.py` & `LongNet-0.1.7/flash_attn/flash_attn/ops/rms_norm.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/utils/benchmark.py` & `LongNet-0.1.7/flash_attn/flash_attn/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/utils/distributed.py` & `LongNet-0.1.7/flash_attn/flash_attn/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/utils/generation.py` & `LongNet-0.1.7/flash_attn/flash_attn/utils/generation.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/flash_attn/utils/pretrained.py` & `LongNet-0.1.7/flash_attn/flash_attn/utils/pretrained.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/flash_attn/setup.py` & `LongNet-0.1.7/flash_attn/setup.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.6/setup.py` & `LongNet-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.1.6',
+  version = '0.1.7',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

### Comparing `LongNet-0.1.6/test/test.py` & `LongNet-0.1.7/test/test.py`

 * *Files identical despite different names*

