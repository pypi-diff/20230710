# Comparing `tmp/zetascale-0.0.2.tar.gz` & `tmp/zetascale-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zetascale-0.0.2.tar", last modified: Mon Jul 10 04:20:35 2023, max compression
+gzip compressed data, was "zetascale-0.2.0.tar", last modified: Mon Jul 10 03:07:06 2023, max compression
```

## Comparing `zetascale-0.0.2.tar` & `zetascale-0.2.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.166523 zetascale-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 04:20:25.000000 zetascale-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-10 04:20:35.166523 zetascale-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-10 04:20:25.000000 zetascale-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.158523 zetascale-0.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.158523 zetascale-0.0.2/examples/fairseq/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.158523 zetascale-0.0.2/examples/fairseq/criterions/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/criterions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/criterions/masked_lm_moe.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.158523 zetascale-0.0.2/examples/fairseq/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18546 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/models/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/models/language_modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/models/machine_translation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.158523 zetascale-0.0.2/examples/fairseq/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.158523 zetascale-0.0.2/examples/fairseq/tasks/data/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/tasks/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/tasks/data/basic_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/tasks/data/mlm_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/tasks/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/tasks/pretraining.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.158523 zetascale-0.0.2/examples/fairseq/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-10 04:20:25.000000 zetascale-0.0.2/examples/fairseq/utils/sparse_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 04:20:35.166523 zetascale-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-10 04:20:25.000000 zetascale-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.158523 zetascale-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-10 04:20:25.000000 zetascale-0.0.2/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-10 04:20:25.000000 zetascale-0.0.2/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-10 04:20:25.000000 zetascale-0.0.2/tests/test_encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.158523 zetascale-0.0.2/zeta/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.162523 zetascale-0.0.2/zeta/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/architecture/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15725 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/architecture/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/architecture/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/architecture/encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/architecture/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.162523 zetascale-0.0.2/zeta/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/models/BEiT3.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/models/GeneSplice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/models/KosmosX.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/models/LongNet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/models/Magneto.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.162523 zetascale-0.0.2/zeta/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.162523 zetascale-0.0.2/zeta/utils/attention/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/attention/dilated_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/attention/flash_multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    30365 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/attention/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/attention/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/droppath.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/feedforward_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.162523 zetascale-0.0.2/zeta/utils/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/module/alibi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/module/multiway_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/module/relative_position_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/module/xpos_relative_position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.162523 zetascale-0.0.2/zeta/utils/xmoe/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/xmoe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/xmoe/global_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/xmoe/moe_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-07-10 04:20:25.000000 zetascale-0.0.2/zeta/utils/xmoe/routing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:20:35.166523 zetascale-0.0.2/zetascale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-10 04:20:35.000000 zetascale-0.0.2/zetascale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-10 04:20:35.000000 zetascale-0.0.2/zetascale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 04:20:35.000000 zetascale-0.0.2/zetascale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 04:20:35.000000 zetascale-0.0.2/zetascale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 04:20:35.000000 zetascale-0.0.2/zetascale.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.862131 zetascale-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 03:06:55.000000 zetascale-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-10 03:07:06.862131 zetascale-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-10 03:06:55.000000 zetascale-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.850129 zetascale-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.854130 zetascale-0.2.0/examples/fairseq/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.854130 zetascale-0.2.0/examples/fairseq/criterions/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/criterions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/criterions/masked_lm_moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.854130 zetascale-0.2.0/examples/fairseq/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18546 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/models/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/models/language_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/models/machine_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.854130 zetascale-0.2.0/examples/fairseq/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.854130 zetascale-0.2.0/examples/fairseq/tasks/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/tasks/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/tasks/data/basic_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/tasks/data/mlm_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/tasks/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/tasks/pretraining.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.854130 zetascale-0.2.0/examples/fairseq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-10 03:06:55.000000 zetascale-0.2.0/examples/fairseq/utils/sparse_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 03:07:06.862131 zetascale-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-10 03:06:55.000000 zetascale-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.854130 zetascale-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-10 03:06:55.000000 zetascale-0.2.0/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-10 03:06:55.000000 zetascale-0.2.0/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-10 03:06:55.000000 zetascale-0.2.0/tests/test_encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.854130 zetascale-0.2.0/zeta/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.858130 zetascale-0.2.0/zeta/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/architecture/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15725 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/architecture/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/architecture/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/architecture/encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/architecture/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.858130 zetascale-0.2.0/zeta/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/models/BEiT3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/models/GeneSplice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/models/KosmosX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/models/LongNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/models/Magneto.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.858130 zetascale-0.2.0/zeta/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.862131 zetascale-0.2.0/zeta/utils/attention/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/attention/dilated_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/attention/flash_multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30365 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/attention/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/attention/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/droppath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/feedforward_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.862131 zetascale-0.2.0/zeta/utils/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/module/alibi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/module/multiway_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/module/relative_position_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/module/xpos_relative_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.862131 zetascale-0.2.0/zeta/utils/xmoe/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/xmoe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/xmoe/global_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/xmoe/moe_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-07-10 03:06:55.000000 zetascale-0.2.0/zeta/utils/xmoe/routing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 03:07:06.862131 zetascale-0.2.0/zetascale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-10 03:07:06.000000 zetascale-0.2.0/zetascale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-10 03:07:06.000000 zetascale-0.2.0/zetascale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 03:07:06.000000 zetascale-0.2.0/zetascale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 03:07:06.000000 zetascale-0.2.0/zetascale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 03:07:06.000000 zetascale-0.2.0/zetascale.egg-info/top_level.txt
```

### Comparing `zetascale-0.0.2/LICENSE` & `zetascale-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/PKG-INFO` & `zetascale-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 Metadata-Version: 2.1
 Name: zetascale
-Version: 0.0.2
+Version: 0.2.0
 Summary: Transformers at zeta scales
 Home-page: https://github.com/kyegomez/zeta
 Author: Zeta Team
 Author-email: kye@apac.ai
 License: MIT
 Keywords: Transformers at zeta scale
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Zeta - A Transgalactic Library for Scalable Transformations
 
 <p>
-  <a href="https://github.com/kyegomez/zeta/blob/main/LICENSE"><img alt="MIT License" src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>
+  <a href="https://github.com/KyGomez/zeta/blob/main/LICENSE"><img alt="MIT License" src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>
   <a href="https://pypi.org/project/zeta"><img alt="MIT License" src="https://badge.fury.io/py/zeta.svg" /></a>
 </p>
 
 Zeta is a PyTorch-powered library, forged in the heart of the Halo array, that empowers researchers and developers to scale up Transformers efficiently and effectively. It leverages seminal research advancements to enhance the generality, capability, and stability of scaling Transformers while optimizing training efficiency.
 
+- Stability - [**DeepNet**](https://arxiv.org/abs/2203.00555): Scaling Transformers beyond 1,000 layers 
+- Generality - [**Foundation Transformers (Magneto)**](https://arxiv.org/abs/2210.06423): Pioneering a path towards universal modeling across diverse tasks and modalities (including language, vision, speech, and multimodal)
+- Capability - The [**Length-Extrapolatable**](https://arxiv.org/abs/2212.10554) Transformer
+- Efficiency - [**X-MoE**](https://arxiv.org/abs/2204.09179): Scalable & finetunable sparse Mixture-of-Experts (MoE)
+
+## News
+
+- November, 2022: Zeta 0.1.1 released [[Paper](https://arxiv.org/abs/2211.13184)] [[PyPI](https://pypi.org/project/zeta/)]
+
 ## Installation
 
 To install:
 ```
-pip install zetascale
+pip install zeta
 ```
 
 To get hands-on and develop it locally:
 ```
 git clone https://github.com/kyegomez/zeta.git
 cd zeta
 pip install -e .
@@ -96,25 +105,25 @@
 
 - Vision
   * ViT/BEiT [In progress]
 
 - Speech
 
 - Multimodal
-  * [Multiway Transformers/BEiT-3](https://github.com/kyegomez/unilm/tree/master/beit3)
+  * [Multiway Transformers/BEiT-3](https://github.com/KyGomez/unilm/tree/master/beit3)
 
-We are working tirelessly to expand the collection of examples spanning various tasks (e.g., vision pretraining, speech recognition) and various deep learning frameworks (e.g., [DeepSpeed](https://github.com/kyegomez/DeepSpeed), [Megatron-LM](https://github.com/NVIDIA/Megatron-LM)). Your comments, suggestions, or contributions are welcome!
+We are working tirelessly to expand the collection of examples spanning various tasks (e.g., vision pretraining, speech recognition) and various deep learning frameworks (e.g., [DeepSpeed](https://github.com/KyGomez/DeepSpeed), [Megatron-LM](https://github.com/NVIDIA/Megatron-LM)). Your comments, suggestions, or contributions are welcome!
 
 ## Results
 
 Check out our [Results Page](results.md) to witness Zeta's exceptional performance in Stability Evaluations and Scaling-up Experiments.
 
 ## Acknowledgments
 
-Zeta is a masterpiece inspired by elements of [FairSeq](https://github.com/facebookresearch/fairseq) and [UniLM](https://github.com/kyegomez/unilm).
+Zeta is a masterpiece inspired by elements of [FairSeq](https://github.com/facebookresearch/fairseq) and [UniLM](https://github.com/KyGomez/unilm).
 
 ## Citations
 
 If our work here in Zeta has aided you in your journey, please consider acknowledging our efforts in your work. You can find relevant citation details in our [Citations Document](citations.md).
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,19 +1,28 @@
-Metadata-Version: 2.1 Name: zetascale Version: 0.0.2 Summary: Transformers at
+Metadata-Version: 2.1 Name: zetascale Version: 0.2.0 Summary: Transformers at
 zeta scales Home-page: https://github.com/kyegomez/zeta Author: Zeta Team
 Author-email: kye@apac.ai License: MIT Keywords: Transformers at zeta scale
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown License-File: LICENSE # Zeta - A
 Transgalactic Library for Scalable Transformations
 [MIT_License] [MIT_License]
 Zeta is a PyTorch-powered library, forged in the heart of the Halo array, that
 empowers researchers and developers to scale up Transformers efficiently and
 effectively. It leverages seminal research advancements to enhance the
 generality, capability, and stability of scaling Transformers while optimizing
-training efficiency. ## Installation To install: ``` pip install zetascale ```
+training efficiency. - Stability - [**DeepNet**](https://arxiv.org/abs/
+2203.00555): Scaling Transformers beyond 1,000 layers - Generality -
+[**Foundation Transformers (Magneto)**](https://arxiv.org/abs/2210.06423):
+Pioneering a path towards universal modeling across diverse tasks and
+modalities (including language, vision, speech, and multimodal) - Capability -
+The [**Length-Extrapolatable**](https://arxiv.org/abs/2212.10554) Transformer -
+Efficiency - [**X-MoE**](https://arxiv.org/abs/2204.09179): Scalable &
+finetunable sparse Mixture-of-Experts (MoE) ## News - November, 2022: Zeta
+0.1.1 released [[Paper](https://arxiv.org/abs/2211.13184)] [[PyPI](https://
+pypi.org/project/zeta/)] ## Installation To install: ``` pip install zeta ```
 To get hands-on and develop it locally: ``` git clone https://github.com/
 kyegomez/zeta.git cd zeta pip install -e . ``` ## Initiating Your Journey
 Creating a model empowered with the aforementioned breakthrough research
 features is a breeze. Here's how to quickly materialize a BERT-like encoder:
 ```python >>> from zeta import EncoderConfig >>> from zeta import Encoder >>>
 config = EncoderConfig(vocab_size=64000) >>> model = Encoder(config) >>> print
 (model) ``` Additionally, we support the `Decoder` and `EncoderDecoder`
@@ -30,24 +39,24 @@
 >>> print(model) ``` For a complete overview of our key features, refer to our
 [Feature Guide](features.md). ## Examples Discover how to wield Zeta in a
 multitude of scenarios/tasks, including but not limited to: - Language *
 [Decoder/GPT](examples/fairseq/README.md#example-gpt-pretraining) * [Encoder-
 Decoder/Neural Machine Translation](examples/fairseq/README.md#example-machine-
 translation) * [Encoder/BERT](examples/fairseq/README.md#example-bert-
 pretraining) - Vision * ViT/BEiT [In progress] - Speech - Multimodal *
-[Multiway Transformers/BEiT-3](https://github.com/kyegomez/unilm/tree/master/
+[Multiway Transformers/BEiT-3](https://github.com/KyGomez/unilm/tree/master/
 beit3) We are working tirelessly to expand the collection of examples spanning
 various tasks (e.g., vision pretraining, speech recognition) and various deep
-learning frameworks (e.g., [DeepSpeed](https://github.com/kyegomez/DeepSpeed),
+learning frameworks (e.g., [DeepSpeed](https://github.com/KyGomez/DeepSpeed),
 [Megatron-LM](https://github.com/NVIDIA/Megatron-LM)). Your comments,
 suggestions, or contributions are welcome! ## Results Check out our [Results
 Page](results.md) to witness Zeta's exceptional performance in Stability
 Evaluations and Scaling-up Experiments. ## Acknowledgments Zeta is a
 masterpiece inspired by elements of [FairSeq](https://github.com/
-facebookresearch/fairseq) and [UniLM](https://github.com/kyegomez/unilm). ##
+facebookresearch/fairseq) and [UniLM](https://github.com/KyGomez/unilm). ##
 Citations If our work here in Zeta has aided you in your journey, please
 consider acknowledging our efforts in your work. You can find relevant citation
 details in our [Citations Document](citations.md). ## Contributing We're always
 thrilled to welcome new ideas and improvements from the community. Please check
 our [Contributor's Guide](contributing.md) for more details about contributing.
 * Create an modular omni-universal Attention class with flash multihead
 attention or regular mh or dilated attention -> then integrate into Decoder/
```

### Comparing `zetascale-0.0.2/README.md` & `zetascale-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 # Zeta - A Transgalactic Library for Scalable Transformations
 
 <p>
-  <a href="https://github.com/kyegomez/zeta/blob/main/LICENSE"><img alt="MIT License" src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>
+  <a href="https://github.com/KyGomez/zeta/blob/main/LICENSE"><img alt="MIT License" src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>
   <a href="https://pypi.org/project/zeta"><img alt="MIT License" src="https://badge.fury.io/py/zeta.svg" /></a>
 </p>
 
 Zeta is a PyTorch-powered library, forged in the heart of the Halo array, that empowers researchers and developers to scale up Transformers efficiently and effectively. It leverages seminal research advancements to enhance the generality, capability, and stability of scaling Transformers while optimizing training efficiency.
 
+- Stability - [**DeepNet**](https://arxiv.org/abs/2203.00555): Scaling Transformers beyond 1,000 layers 
+- Generality - [**Foundation Transformers (Magneto)**](https://arxiv.org/abs/2210.06423): Pioneering a path towards universal modeling across diverse tasks and modalities (including language, vision, speech, and multimodal)
+- Capability - The [**Length-Extrapolatable**](https://arxiv.org/abs/2212.10554) Transformer
+- Efficiency - [**X-MoE**](https://arxiv.org/abs/2204.09179): Scalable & finetunable sparse Mixture-of-Experts (MoE)
+
+## News
+
+- November, 2022: Zeta 0.1.1 released [[Paper](https://arxiv.org/abs/2211.13184)] [[PyPI](https://pypi.org/project/zeta/)]
+
 ## Installation
 
 To install:
 ```
-pip install zetascale
+pip install zeta
 ```
 
 To get hands-on and develop it locally:
 ```
 git clone https://github.com/kyegomez/zeta.git
 cd zeta
 pip install -e .
@@ -82,25 +91,25 @@
 
 - Vision
   * ViT/BEiT [In progress]
 
 - Speech
 
 - Multimodal
-  * [Multiway Transformers/BEiT-3](https://github.com/kyegomez/unilm/tree/master/beit3)
+  * [Multiway Transformers/BEiT-3](https://github.com/KyGomez/unilm/tree/master/beit3)
 
-We are working tirelessly to expand the collection of examples spanning various tasks (e.g., vision pretraining, speech recognition) and various deep learning frameworks (e.g., [DeepSpeed](https://github.com/kyegomez/DeepSpeed), [Megatron-LM](https://github.com/NVIDIA/Megatron-LM)). Your comments, suggestions, or contributions are welcome!
+We are working tirelessly to expand the collection of examples spanning various tasks (e.g., vision pretraining, speech recognition) and various deep learning frameworks (e.g., [DeepSpeed](https://github.com/KyGomez/DeepSpeed), [Megatron-LM](https://github.com/NVIDIA/Megatron-LM)). Your comments, suggestions, or contributions are welcome!
 
 ## Results
 
 Check out our [Results Page](results.md) to witness Zeta's exceptional performance in Stability Evaluations and Scaling-up Experiments.
 
 ## Acknowledgments
 
-Zeta is a masterpiece inspired by elements of [FairSeq](https://github.com/facebookresearch/fairseq) and [UniLM](https://github.com/kyegomez/unilm).
+Zeta is a masterpiece inspired by elements of [FairSeq](https://github.com/facebookresearch/fairseq) and [UniLM](https://github.com/KyGomez/unilm).
 
 ## Citations
 
 If our work here in Zeta has aided you in your journey, please consider acknowledging our efforts in your work. You can find relevant citation details in our [Citations Document](citations.md).
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,14 +1,23 @@
 # Zeta - A Transgalactic Library for Scalable Transformations
 [MIT_License] [MIT_License]
 Zeta is a PyTorch-powered library, forged in the heart of the Halo array, that
 empowers researchers and developers to scale up Transformers efficiently and
 effectively. It leverages seminal research advancements to enhance the
 generality, capability, and stability of scaling Transformers while optimizing
-training efficiency. ## Installation To install: ``` pip install zetascale ```
+training efficiency. - Stability - [**DeepNet**](https://arxiv.org/abs/
+2203.00555): Scaling Transformers beyond 1,000 layers - Generality -
+[**Foundation Transformers (Magneto)**](https://arxiv.org/abs/2210.06423):
+Pioneering a path towards universal modeling across diverse tasks and
+modalities (including language, vision, speech, and multimodal) - Capability -
+The [**Length-Extrapolatable**](https://arxiv.org/abs/2212.10554) Transformer -
+Efficiency - [**X-MoE**](https://arxiv.org/abs/2204.09179): Scalable &
+finetunable sparse Mixture-of-Experts (MoE) ## News - November, 2022: Zeta
+0.1.1 released [[Paper](https://arxiv.org/abs/2211.13184)] [[PyPI](https://
+pypi.org/project/zeta/)] ## Installation To install: ``` pip install zeta ```
 To get hands-on and develop it locally: ``` git clone https://github.com/
 kyegomez/zeta.git cd zeta pip install -e . ``` ## Initiating Your Journey
 Creating a model empowered with the aforementioned breakthrough research
 features is a breeze. Here's how to quickly materialize a BERT-like encoder:
 ```python >>> from zeta import EncoderConfig >>> from zeta import Encoder >>>
 config = EncoderConfig(vocab_size=64000) >>> model = Encoder(config) >>> print
 (model) ``` Additionally, we support the `Decoder` and `EncoderDecoder`
@@ -25,24 +34,24 @@
 >>> print(model) ``` For a complete overview of our key features, refer to our
 [Feature Guide](features.md). ## Examples Discover how to wield Zeta in a
 multitude of scenarios/tasks, including but not limited to: - Language *
 [Decoder/GPT](examples/fairseq/README.md#example-gpt-pretraining) * [Encoder-
 Decoder/Neural Machine Translation](examples/fairseq/README.md#example-machine-
 translation) * [Encoder/BERT](examples/fairseq/README.md#example-bert-
 pretraining) - Vision * ViT/BEiT [In progress] - Speech - Multimodal *
-[Multiway Transformers/BEiT-3](https://github.com/kyegomez/unilm/tree/master/
+[Multiway Transformers/BEiT-3](https://github.com/KyGomez/unilm/tree/master/
 beit3) We are working tirelessly to expand the collection of examples spanning
 various tasks (e.g., vision pretraining, speech recognition) and various deep
-learning frameworks (e.g., [DeepSpeed](https://github.com/kyegomez/DeepSpeed),
+learning frameworks (e.g., [DeepSpeed](https://github.com/KyGomez/DeepSpeed),
 [Megatron-LM](https://github.com/NVIDIA/Megatron-LM)). Your comments,
 suggestions, or contributions are welcome! ## Results Check out our [Results
 Page](results.md) to witness Zeta's exceptional performance in Stability
 Evaluations and Scaling-up Experiments. ## Acknowledgments Zeta is a
 masterpiece inspired by elements of [FairSeq](https://github.com/
-facebookresearch/fairseq) and [UniLM](https://github.com/kyegomez/unilm). ##
+facebookresearch/fairseq) and [UniLM](https://github.com/KyGomez/unilm). ##
 Citations If our work here in Zeta has aided you in your journey, please
 consider acknowledging our efforts in your work. You can find relevant citation
 details in our [Citations Document](citations.md). ## Contributing We're always
 thrilled to welcome new ideas and improvements from the community. Please check
 our [Contributor's Guide](contributing.md) for more details about contributing.
 * Create an modular omni-universal Attention class with flash multihead
 attention or regular mh or dilated attention -> then integrate into Decoder/
```

### Comparing `zetascale-0.0.2/examples/fairseq/criterions/masked_lm_moe.py` & `zetascale-0.2.0/examples/fairseq/criterions/masked_lm_moe.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/examples/fairseq/models/__init__.py` & `zetascale-0.2.0/examples/fairseq/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/examples/fairseq/models/bert.py` & `zetascale-0.2.0/examples/fairseq/models/bert.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/examples/fairseq/models/language_modeling.py` & `zetascale-0.2.0/examples/fairseq/models/language_modeling.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/examples/fairseq/models/machine_translation.py` & `zetascale-0.2.0/examples/fairseq/models/machine_translation.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/examples/fairseq/tasks/__init__.py` & `zetascale-0.2.0/examples/fairseq/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/examples/fairseq/tasks/data/basic_loader.py` & `zetascale-0.2.0/examples/fairseq/tasks/data/basic_loader.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/examples/fairseq/tasks/data/mlm_loader.py` & `zetascale-0.2.0/examples/fairseq/tasks/data/mlm_loader.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/examples/fairseq/tasks/data/utils.py` & `zetascale-0.2.0/examples/fairseq/tasks/data/utils.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/examples/fairseq/tasks/pretraining.py` & `zetascale-0.2.0/examples/fairseq/tasks/pretraining.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/examples/fairseq/utils/sparse_clip.py` & `zetascale-0.2.0/examples/fairseq/utils/sparse_clip.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/setup.py` & `zetascale-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from io import open
 
 from setuptools import find_packages, setup
 
 setup(
     name="zetascale",
-    version="0.0.2",
+    version="0.2.0",
     author="Zeta Team",
     author_email="kye@apac.ai",
     description="Transformers at zeta scales",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="Transformers at zeta scale",
     license="MIT",
```

### Comparing `zetascale-0.0.2/tests/test_decoder.py` & `zetascale-0.2.0/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/tests/test_encoder.py` & `zetascale-0.2.0/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/tests/test_encoder_decoder.py` & `zetascale-0.2.0/tests/test_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/architecture/config.py` & `zetascale-0.2.0/zeta/architecture/config.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/architecture/decoder.py` & `zetascale-0.2.0/zeta/architecture/decoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/architecture/encoder.py` & `zetascale-0.2.0/zeta/architecture/encoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/architecture/encoder_decoder.py` & `zetascale-0.2.0/zeta/architecture/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/architecture/utils.py` & `zetascale-0.2.0/zeta/architecture/utils.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/models/BEiT3.py` & `zetascale-0.2.0/zeta/models/BEiT3.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/models/KosmosX.py` & `zetascale-0.2.0/zeta/models/KosmosX.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/models/LongNet.py` & `zetascale-0.2.0/zeta/models/LongNet.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/attention/attend.py` & `zetascale-0.2.0/zeta/utils/attention/attend.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/attention/dilated_attention.py` & `zetascale-0.2.0/zeta/utils/attention/dilated_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/attention/flash_multihead_attention.py` & `zetascale-0.2.0/zeta/utils/attention/flash_multihead_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/attention/main.py` & `zetascale-0.2.0/zeta/utils/attention/main.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/attention/multihead_attention.py` & `zetascale-0.2.0/zeta/utils/attention/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/droppath.py` & `zetascale-0.2.0/zeta/utils/droppath.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/embedding.py` & `zetascale-0.2.0/zeta/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/feedforward_network.py` & `zetascale-0.2.0/zeta/utils/feedforward_network.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/module/alibi.py` & `zetascale-0.2.0/zeta/utils/module/alibi.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/module/multiway_network.py` & `zetascale-0.2.0/zeta/utils/module/multiway_network.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/module/relative_position_bias.py` & `zetascale-0.2.0/zeta/utils/module/relative_position_bias.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/module/xpos_relative_position.py` & `zetascale-0.2.0/zeta/utils/module/xpos_relative_position.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/xmoe/global_groups.py` & `zetascale-0.2.0/zeta/utils/xmoe/global_groups.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/xmoe/moe_layer.py` & `zetascale-0.2.0/zeta/utils/xmoe/moe_layer.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zeta/utils/xmoe/routing.py` & `zetascale-0.2.0/zeta/utils/xmoe/routing.py`

 * *Files identical despite different names*

### Comparing `zetascale-0.0.2/zetascale.egg-info/PKG-INFO` & `zetascale-0.2.0/zetascale.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 Metadata-Version: 2.1
 Name: zetascale
-Version: 0.0.2
+Version: 0.2.0
 Summary: Transformers at zeta scales
 Home-page: https://github.com/kyegomez/zeta
 Author: Zeta Team
 Author-email: kye@apac.ai
 License: MIT
 Keywords: Transformers at zeta scale
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Zeta - A Transgalactic Library for Scalable Transformations
 
 <p>
-  <a href="https://github.com/kyegomez/zeta/blob/main/LICENSE"><img alt="MIT License" src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>
+  <a href="https://github.com/KyGomez/zeta/blob/main/LICENSE"><img alt="MIT License" src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>
   <a href="https://pypi.org/project/zeta"><img alt="MIT License" src="https://badge.fury.io/py/zeta.svg" /></a>
 </p>
 
 Zeta is a PyTorch-powered library, forged in the heart of the Halo array, that empowers researchers and developers to scale up Transformers efficiently and effectively. It leverages seminal research advancements to enhance the generality, capability, and stability of scaling Transformers while optimizing training efficiency.
 
+- Stability - [**DeepNet**](https://arxiv.org/abs/2203.00555): Scaling Transformers beyond 1,000 layers 
+- Generality - [**Foundation Transformers (Magneto)**](https://arxiv.org/abs/2210.06423): Pioneering a path towards universal modeling across diverse tasks and modalities (including language, vision, speech, and multimodal)
+- Capability - The [**Length-Extrapolatable**](https://arxiv.org/abs/2212.10554) Transformer
+- Efficiency - [**X-MoE**](https://arxiv.org/abs/2204.09179): Scalable & finetunable sparse Mixture-of-Experts (MoE)
+
+## News
+
+- November, 2022: Zeta 0.1.1 released [[Paper](https://arxiv.org/abs/2211.13184)] [[PyPI](https://pypi.org/project/zeta/)]
+
 ## Installation
 
 To install:
 ```
-pip install zetascale
+pip install zeta
 ```
 
 To get hands-on and develop it locally:
 ```
 git clone https://github.com/kyegomez/zeta.git
 cd zeta
 pip install -e .
@@ -96,25 +105,25 @@
 
 - Vision
   * ViT/BEiT [In progress]
 
 - Speech
 
 - Multimodal
-  * [Multiway Transformers/BEiT-3](https://github.com/kyegomez/unilm/tree/master/beit3)
+  * [Multiway Transformers/BEiT-3](https://github.com/KyGomez/unilm/tree/master/beit3)
 
-We are working tirelessly to expand the collection of examples spanning various tasks (e.g., vision pretraining, speech recognition) and various deep learning frameworks (e.g., [DeepSpeed](https://github.com/kyegomez/DeepSpeed), [Megatron-LM](https://github.com/NVIDIA/Megatron-LM)). Your comments, suggestions, or contributions are welcome!
+We are working tirelessly to expand the collection of examples spanning various tasks (e.g., vision pretraining, speech recognition) and various deep learning frameworks (e.g., [DeepSpeed](https://github.com/KyGomez/DeepSpeed), [Megatron-LM](https://github.com/NVIDIA/Megatron-LM)). Your comments, suggestions, or contributions are welcome!
 
 ## Results
 
 Check out our [Results Page](results.md) to witness Zeta's exceptional performance in Stability Evaluations and Scaling-up Experiments.
 
 ## Acknowledgments
 
-Zeta is a masterpiece inspired by elements of [FairSeq](https://github.com/facebookresearch/fairseq) and [UniLM](https://github.com/kyegomez/unilm).
+Zeta is a masterpiece inspired by elements of [FairSeq](https://github.com/facebookresearch/fairseq) and [UniLM](https://github.com/KyGomez/unilm).
 
 ## Citations
 
 If our work here in Zeta has aided you in your journey, please consider acknowledging our efforts in your work. You can find relevant citation details in our [Citations Document](citations.md).
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,19 +1,28 @@
-Metadata-Version: 2.1 Name: zetascale Version: 0.0.2 Summary: Transformers at
+Metadata-Version: 2.1 Name: zetascale Version: 0.2.0 Summary: Transformers at
 zeta scales Home-page: https://github.com/kyegomez/zeta Author: Zeta Team
 Author-email: kye@apac.ai License: MIT Keywords: Transformers at zeta scale
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown License-File: LICENSE # Zeta - A
 Transgalactic Library for Scalable Transformations
 [MIT_License] [MIT_License]
 Zeta is a PyTorch-powered library, forged in the heart of the Halo array, that
 empowers researchers and developers to scale up Transformers efficiently and
 effectively. It leverages seminal research advancements to enhance the
 generality, capability, and stability of scaling Transformers while optimizing
-training efficiency. ## Installation To install: ``` pip install zetascale ```
+training efficiency. - Stability - [**DeepNet**](https://arxiv.org/abs/
+2203.00555): Scaling Transformers beyond 1,000 layers - Generality -
+[**Foundation Transformers (Magneto)**](https://arxiv.org/abs/2210.06423):
+Pioneering a path towards universal modeling across diverse tasks and
+modalities (including language, vision, speech, and multimodal) - Capability -
+The [**Length-Extrapolatable**](https://arxiv.org/abs/2212.10554) Transformer -
+Efficiency - [**X-MoE**](https://arxiv.org/abs/2204.09179): Scalable &
+finetunable sparse Mixture-of-Experts (MoE) ## News - November, 2022: Zeta
+0.1.1 released [[Paper](https://arxiv.org/abs/2211.13184)] [[PyPI](https://
+pypi.org/project/zeta/)] ## Installation To install: ``` pip install zeta ```
 To get hands-on and develop it locally: ``` git clone https://github.com/
 kyegomez/zeta.git cd zeta pip install -e . ``` ## Initiating Your Journey
 Creating a model empowered with the aforementioned breakthrough research
 features is a breeze. Here's how to quickly materialize a BERT-like encoder:
 ```python >>> from zeta import EncoderConfig >>> from zeta import Encoder >>>
 config = EncoderConfig(vocab_size=64000) >>> model = Encoder(config) >>> print
 (model) ``` Additionally, we support the `Decoder` and `EncoderDecoder`
@@ -30,24 +39,24 @@
 >>> print(model) ``` For a complete overview of our key features, refer to our
 [Feature Guide](features.md). ## Examples Discover how to wield Zeta in a
 multitude of scenarios/tasks, including but not limited to: - Language *
 [Decoder/GPT](examples/fairseq/README.md#example-gpt-pretraining) * [Encoder-
 Decoder/Neural Machine Translation](examples/fairseq/README.md#example-machine-
 translation) * [Encoder/BERT](examples/fairseq/README.md#example-bert-
 pretraining) - Vision * ViT/BEiT [In progress] - Speech - Multimodal *
-[Multiway Transformers/BEiT-3](https://github.com/kyegomez/unilm/tree/master/
+[Multiway Transformers/BEiT-3](https://github.com/KyGomez/unilm/tree/master/
 beit3) We are working tirelessly to expand the collection of examples spanning
 various tasks (e.g., vision pretraining, speech recognition) and various deep
-learning frameworks (e.g., [DeepSpeed](https://github.com/kyegomez/DeepSpeed),
+learning frameworks (e.g., [DeepSpeed](https://github.com/KyGomez/DeepSpeed),
 [Megatron-LM](https://github.com/NVIDIA/Megatron-LM)). Your comments,
 suggestions, or contributions are welcome! ## Results Check out our [Results
 Page](results.md) to witness Zeta's exceptional performance in Stability
 Evaluations and Scaling-up Experiments. ## Acknowledgments Zeta is a
 masterpiece inspired by elements of [FairSeq](https://github.com/
-facebookresearch/fairseq) and [UniLM](https://github.com/kyegomez/unilm). ##
+facebookresearch/fairseq) and [UniLM](https://github.com/KyGomez/unilm). ##
 Citations If our work here in Zeta has aided you in your journey, please
 consider acknowledging our efforts in your work. You can find relevant citation
 details in our [Citations Document](citations.md). ## Contributing We're always
 thrilled to welcome new ideas and improvements from the community. Please check
 our [Contributor's Guide](contributing.md) for more details about contributing.
 * Create an modular omni-universal Attention class with flash multihead
 attention or regular mh or dilated attention -> then integrate into Decoder/
```

### Comparing `zetascale-0.0.2/zetascale.egg-info/SOURCES.txt` & `zetascale-0.2.0/zetascale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

