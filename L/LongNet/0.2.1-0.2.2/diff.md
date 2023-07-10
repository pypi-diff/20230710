# Comparing `tmp/LongNet-0.2.1.tar.gz` & `tmp/LongNet-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.2.1.tar", last modified: Mon Jul 10 19:08:50 2023, max compression
+gzip compressed data, was "LongNet-0.2.2.tar", last modified: Mon Jul 10 19:21:21 2023, max compression
```

## Comparing `LongNet-0.2.1.tar` & `LongNet-0.2.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:50.121264 LongNet-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 19:08:36.000000 LongNet-0.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:50.113263 LongNet-0.2.1/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 19:08:36.000000 LongNet-0.2.1/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-10 19:08:36.000000 LongNet-0.2.1/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-07-10 19:08:36.000000 LongNet-0.2.1/LongNet/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-10 19:08:36.000000 LongNet-0.2.1/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-10 19:08:36.000000 LongNet-0.2.1/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-10 19:08:36.000000 LongNet-0.2.1/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:50.113263 LongNet-0.2.1/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 19:08:50.000000 LongNet-0.2.1/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-10 19:08:50.000000 LongNet-0.2.1/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:08:50.000000 LongNet-0.2.1/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 19:08:50.000000 LongNet-0.2.1/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 19:08:50.000000 LongNet-0.2.1/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 19:08:50.121264 LongNet-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-07-10 19:08:36.000000 LongNet-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:50.113263 LongNet-0.2.1/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:50.117263 LongNet-0.2.1/flash_attn/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/bert_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/flash_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/flash_attn_triton.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/flash_attn_triton_og.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/flash_blocksparse_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/flash_blocksparse_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/fused_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:50.117263 LongNet-0.2.1/flash_attn/flash_attn/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/layers/patch_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/layers/rotary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:50.117263 LongNet-0.2.1/flash_attn/flash_attn/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/losses/cross_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:50.117263 LongNet-0.2.1/flash_attn/flash_attn/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/models/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/models/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/models/gpt_neox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/models/gptj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/models/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/models/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/models/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:50.121264 LongNet-0.2.1/flash_attn/flash_attn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/modules/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/modules/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/modules/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:50.121264 LongNet-0.2.1/flash_attn/flash_attn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/ops/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/ops/fused_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    19306 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/ops/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/ops/rms_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:50.121264 LongNet-0.2.1/flash_attn/flash_attn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/utils/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/utils/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/flash_attn/utils/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-10 19:08:36.000000 LongNet-0.2.1/flash_attn/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:08:50.121264 LongNet-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-10 19:08:36.000000 LongNet-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:08:50.121264 LongNet-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 19:08:36.000000 LongNet-0.2.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:21.544830 LongNet-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 19:21:07.000000 LongNet-0.2.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:21.532830 LongNet-0.2.2/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 19:21:07.000000 LongNet-0.2.2/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12357 2023-07-10 19:21:07.000000 LongNet-0.2.2/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-07-10 19:21:07.000000 LongNet-0.2.2/LongNet/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-10 19:21:07.000000 LongNet-0.2.2/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-10 19:21:07.000000 LongNet-0.2.2/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-10 19:21:07.000000 LongNet-0.2.2/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:21.532830 LongNet-0.2.2/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 19:21:21.000000 LongNet-0.2.2/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-10 19:21:21.000000 LongNet-0.2.2/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:21:21.000000 LongNet-0.2.2/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 19:21:21.000000 LongNet-0.2.2/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 19:21:21.000000 LongNet-0.2.2/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 19:21:21.544830 LongNet-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-07-10 19:21:07.000000 LongNet-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:21.532830 LongNet-0.2.2/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:21.536830 LongNet-0.2.2/flash_attn/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/bert_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/flash_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/flash_attn_triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/flash_attn_triton_og.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/flash_blocksparse_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/flash_blocksparse_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/fused_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:21.536830 LongNet-0.2.2/flash_attn/flash_attn/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/layers/patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/layers/rotary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:21.536830 LongNet-0.2.2/flash_attn/flash_attn/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/losses/cross_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:21.540830 LongNet-0.2.2/flash_attn/flash_attn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/models/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/models/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/models/gpt_neox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/models/gptj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/models/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/models/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:21.540830 LongNet-0.2.2/flash_attn/flash_attn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/modules/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/modules/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/modules/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:21.540830 LongNet-0.2.2/flash_attn/flash_attn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/ops/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/ops/fused_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19306 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/ops/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/ops/rms_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:21.540830 LongNet-0.2.2/flash_attn/flash_attn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/utils/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/flash_attn/utils/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-10 19:21:07.000000 LongNet-0.2.2/flash_attn/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:21:21.544830 LongNet-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-10 19:21:07.000000 LongNet-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:21:21.544830 LongNet-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 19:21:07.000000 LongNet-0.2.2/test/test.py
```

### Comparing `LongNet-0.2.1/LICENSE` & `LongNet-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/LongNet/attend.py` & `LongNet-0.2.2/LongNet/attend.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,39 +286,36 @@
     def __init__(
             self,
             args,
             embed_dim,
             num_heads,
             dropout=0.0,
             self_attention=False,
-            flash_attention=False,
-            subln=False
+            flash_attention=False
         ):
-
             super().__init__()
-            self.args = args
             self.embed_dim = embed_dim
             self.num_heads = num_heads
-
-            self.head_dim = embed_dim // num_heads
-            self.scaling = self.head_dim**-0.5
-
             self.self_attention = self_attention
             self.flash_attention = flash_attention
             assert self.self_attention ^ self.flash_attention
 
+            self.head_dim = embed_dim // num_heads
+            self.scaling = self.head_dim**-0.5
+
             self.k_proj = nn.Linear(embed_dim, embed_dim, bias=True)
             self.v_proj = nn.Linear(embed_dim, embed_dim, bias=True)
             self.q_proj = nn.Linear(embed_dim, embed_dim, bias=True)
             self.outproj = nn.Linear(embed_dim, embed_dim, bias=True)
             
             self.dropout_module = torch.nn.Dropout(dropout)
 
-            #init flash attention
-            self.flash_attention = FlashAttention(dropout=dropout, causal=self_attention, heads=num_heads)
+            # init flash attention
+            if self.flash_attention:
+                self.flash_attention = FlashAttention(dropout=dropout, causal=self_attention, heads=num_heads)
     
     def reset_parameters(self):
         nn.init.xavier_uniform_(self.k_proj.weight, gain=1 / math.sqrt(2))
         nn.init.xavier_uniform_(self.v_proj.weight, gain=1 / math.sqrt(2))
         nn.init.xavier_uniform_(self.q_proj.weight, gain=1 / math.sqrt(2))
         nn.init.xavier_uniform_(self.out_proj.weight)
         nn.init.constant_(self.out_proj.bias, 0.0)
```

### Comparing `LongNet-0.2.1/LongNet/attention.py` & `LongNet-0.2.2/LongNet/attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,14 @@
 
 from LongNet.attend import FlashMHA
 
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
 
-
-
-
-
-
-
 #add alibi, qk layer norm, one write head, multihway, 
 class DilatedAttention(nn.Module):
     """
     Dilated Attention Module.
 
     Arguments:
         d_model: The dimension of the attention layers.
```

### Comparing `LongNet-0.2.1/LongNet/model.py` & `LongNet-0.2.2/LongNet/model.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/LongNet/training.py` & `LongNet-0.2.2/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/LongNet/utils.py` & `LongNet-0.2.2/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/LongNet.egg-info/PKG-INFO` & `LongNet-0.2.2/LongNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.2.1
+Version: 0.2.2
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.2.1/LongNet.egg-info/SOURCES.txt` & `LongNet-0.2.2/LongNet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/PKG-INFO` & `LongNet-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.2.1
+Version: 0.2.2
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.2.1/README.md` & `LongNet-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/bert_padding.py` & `LongNet-0.2.2/flash_attn/flash_attn/bert_padding.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/flash_attention.py` & `LongNet-0.2.2/flash_attn/flash_attn/flash_attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/flash_attn_interface.py` & `LongNet-0.2.2/flash_attn/flash_attn/flash_attn_interface.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/flash_attn_triton.py` & `LongNet-0.2.2/flash_attn/flash_attn/flash_attn_triton.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/flash_attn_triton_og.py` & `LongNet-0.2.2/flash_attn/flash_attn/flash_attn_triton_og.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/flash_blocksparse_attention.py` & `LongNet-0.2.2/flash_attn/flash_attn/flash_blocksparse_attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/flash_blocksparse_attn_interface.py` & `LongNet-0.2.2/flash_attn/flash_attn/flash_blocksparse_attn_interface.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/fused_softmax.py` & `LongNet-0.2.2/flash_attn/flash_attn/fused_softmax.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/layers/patch_embed.py` & `LongNet-0.2.2/flash_attn/flash_attn/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/layers/rotary.py` & `LongNet-0.2.2/flash_attn/flash_attn/layers/rotary.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/losses/cross_entropy.py` & `LongNet-0.2.2/flash_attn/flash_attn/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/models/bert.py` & `LongNet-0.2.2/flash_attn/flash_attn/models/bert.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/models/gpt.py` & `LongNet-0.2.2/flash_attn/flash_attn/models/gpt.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/models/gpt_neox.py` & `LongNet-0.2.2/flash_attn/flash_attn/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/models/gptj.py` & `LongNet-0.2.2/flash_attn/flash_attn/models/gptj.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/models/llama.py` & `LongNet-0.2.2/flash_attn/flash_attn/models/llama.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/models/opt.py` & `LongNet-0.2.2/flash_attn/flash_attn/models/opt.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/models/vit.py` & `LongNet-0.2.2/flash_attn/flash_attn/models/vit.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/modules/block.py` & `LongNet-0.2.2/flash_attn/flash_attn/modules/block.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/modules/embedding.py` & `LongNet-0.2.2/flash_attn/flash_attn/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/modules/mha.py` & `LongNet-0.2.2/flash_attn/flash_attn/modules/mha.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/modules/mlp.py` & `LongNet-0.2.2/flash_attn/flash_attn/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/ops/activations.py` & `LongNet-0.2.2/flash_attn/flash_attn/ops/activations.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/ops/fused_dense.py` & `LongNet-0.2.2/flash_attn/flash_attn/ops/fused_dense.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/ops/layer_norm.py` & `LongNet-0.2.2/flash_attn/flash_attn/ops/layer_norm.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/ops/rms_norm.py` & `LongNet-0.2.2/flash_attn/flash_attn/ops/rms_norm.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/utils/benchmark.py` & `LongNet-0.2.2/flash_attn/flash_attn/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/utils/distributed.py` & `LongNet-0.2.2/flash_attn/flash_attn/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/utils/generation.py` & `LongNet-0.2.2/flash_attn/flash_attn/utils/generation.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/flash_attn/utils/pretrained.py` & `LongNet-0.2.2/flash_attn/flash_attn/utils/pretrained.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/flash_attn/setup.py` & `LongNet-0.2.2/flash_attn/setup.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.1/setup.py` & `LongNet-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.2.1',
+  version = '0.2.2',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

### Comparing `LongNet-0.2.1/test/test.py` & `LongNet-0.2.2/test/test.py`

 * *Files identical despite different names*

