# Comparing `tmp/trailmet-0.0.1rc0.tar.gz` & `tmp/trailmet-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trailmet-0.0.1rc0.tar", last modified: Sun Jul  2 18:22:57 2023, max compression
+gzip compressed data, was "dist/trailmet-0.0.1rc2.tar", last modified: Mon Jul 10 18:58:37 2023, max compression
```

## Comparing `trailmet-0.0.1rc0.tar` & `trailmet-0.0.1rc2.tar`

### file list

```diff
@@ -1,85 +1,81 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.177221 trailmet-0.0.1rc0/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1073 2023-07-02 14:54:23.000000 trailmet-0.0.1rc0/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4280 2023-07-02 18:22:57.177221 trailmet-0.0.1rc0/PKG-INFO
--rw-------   0 gitpod   (33333) gitpod   (33333)     3345 2023-07-02 17:25:14.000000 trailmet-0.0.1rc0/README.md
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-07-02 18:22:57.177221 trailmet-0.0.1rc0/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7209 2023-07-02 17:41:56.000000 trailmet-0.0.1rc0/setup.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.161222 trailmet-0.0.1rc0/tests/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1303 2023-07-02 17:22:42.000000 trailmet-0.0.1rc0/tests/test_general.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1817 2023-07-02 17:22:42.000000 trailmet-0.0.1rc0/tests/test_unwanted_files.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.161222 trailmet-0.0.1rc0/trailmet/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1332 2023-07-02 18:02:09.000000 trailmet-0.0.1rc0/trailmet/__init__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.165222 trailmet-0.0.1rc0/trailmet/algorithms/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1149 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8922 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/algorithms.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.169221 trailmet-0.0.1rc0/trailmet/algorithms/binarize/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    21870 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/binarize/BNNBN.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    21196 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/binarize/ReActNet.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1320 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/binarize/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1406 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/binarize/binarize.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    16590 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/binarize/birealnet.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4004 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/binarize/utils.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.169221 trailmet-0.0.1rc0/trailmet/algorithms/distill/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1362 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/distill/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    15480 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/distill/attention_transfer.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     9625 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/distill/distill.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    25723 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/distill/factor_transfer.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2767 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/distill/losses.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    12137 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/distill/response_kd.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    13377 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/distill/rkd.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.169221 trailmet-0.0.1rc0/trailmet/algorithms/prune/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1659 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/prune/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    26986 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/prune/chip.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    37595 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/prune/chipnet.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    16913 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/prune/growth_regularisation.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    13896 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/prune/network_slimming.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    18664 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/prune/pns.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1396 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/prune/prune.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.173221 trailmet-0.0.1rc0/trailmet/algorithms/prune/pruner/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1495 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/prune/pruner/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1875 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/prune/pruner/l1_pruner.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    20129 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/prune/pruner/meta_pruner.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    32016 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/prune/pruner/reg_pruner.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6489 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/prune/utils.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.173221 trailmet-0.0.1rc0/trailmet/algorithms/quantize/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2175 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/quantize/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    33267 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/quantize/bitsplit.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    19592 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/quantize/brecq.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    17327 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/algorithms/quantize/lapq.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    29579 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/quantize/methods.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    21093 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/quantize/qmodel.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7403 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/quantize/quantize.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    27516 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/algorithms/quantize/reconstruct.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.173221 trailmet-0.0.1rc0/trailmet/algorithms/utils/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    19208 2023-07-02 17:12:46.000000 trailmet-0.0.1rc0/trailmet/algorithms/utils/__init__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.173221 trailmet-0.0.1rc0/trailmet/datasets/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1154 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/datasets/__init__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.177221 trailmet-0.0.1rc0/trailmet/datasets/classification/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2743 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/datasets/classification/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     9974 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/datasets/classification/chest.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    10056 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/datasets/classification/cifar.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6333 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/datasets/classification/dataset.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4119 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/datasets/classification/imagenet.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11325 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/datasets/classification/tcga.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.177221 trailmet-0.0.1rc0/trailmet/models/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7865 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/models/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1880 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/models/base_model.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    10060 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/models/mobilenet.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    10153 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/models/mobilenetv2_bireal.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    17705 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/models/resnet.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    21882 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/models/resnet_bireal.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7078 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/models/resnet_chip.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6126 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/models/wideresnet.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.177221 trailmet-0.0.1rc0/trailmet/utils/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1455 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/utils/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7336 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/utils/benchmark.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7981 2023-07-02 17:12:27.000000 trailmet-0.0.1rc0/trailmet/utils/functions.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5761 2023-07-02 17:12:26.000000 trailmet-0.0.1rc0/trailmet/utils/tp_pruning.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      785 2023-07-02 18:21:28.000000 trailmet-0.0.1rc0/trailmet/version.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-02 18:22:57.161222 trailmet-0.0.1rc0/trailmet.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4280 2023-07-02 18:22:57.000000 trailmet-0.0.1rc0/trailmet.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2407 2023-07-02 18:22:57.000000 trailmet-0.0.1rc0/trailmet.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-07-02 18:22:57.000000 trailmet-0.0.1rc0/trailmet.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-07-02 18:20:00.000000 trailmet-0.0.1rc0/trailmet.egg-info/not-zip-safe
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      437 2023-07-02 18:22:57.000000 trailmet-0.0.1rc0/trailmet.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        9 2023-07-02 18:22:57.000000 trailmet-0.0.1rc0/trailmet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/algorithms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/
+-rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/BNNBN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21686 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/ReActNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/binarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17234 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/birealnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15922 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/attention_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26230 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/factor_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/response_kd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/rkd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27307 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37915 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/chipnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17230 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/growth_regularisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/network_slimming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19335 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/pns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/l1_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20535 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/meta_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32365 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/reg_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33476 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/bitsplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19698 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/brecq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/lapq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32027 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/qmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/quantize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29083 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19597 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/chest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/tcga.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/mobilenetv2_bireal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21882 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/resnet_bireal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/resnet_chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/wideresnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/utils/tp_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `trailmet-0.0.1rc0/LICENSE` & `trailmet-0.0.1rc2/trailmet/algorithms/prune/prune.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,33 @@
-MIT License
+# MIT License
+#
+# Copyright (c) 2023 Transmute AI Lab
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+from ..algorithms import BaseAlgorithm
 
-Copyright (c) 2021 Transmute AI Lab
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+class BasePruning(BaseAlgorithm):
+    """Base class for pruning algorithms."""
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+    def __init__(self, **kwargs):
+        super(BasePruning, self).__init__(**kwargs)
+        pass
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+    def prune(self, model, dataloaders, **kwargs):
+        pass
```

### Comparing `trailmet-0.0.1rc0/PKG-INFO` & `trailmet-0.0.1rc2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,135 +1,135 @@
 Metadata-Version: 2.1
 Name: trailmet
-Version: 0.0.1rc0
+Version: 0.0.1rc2
 Summary: Transmute AI Model Efficiency Toolkit
 Home-page: https://github.com/transmuteAI/trailmet
 Author: TrAILMET Contributors
 Author-email: transmute.ai@gmail.com
 License: MIT License
+Description: <p align="center">
+            <br>
+                <img src="docs/source/imgs/trailmet.png" width="500"/>
+            </br>
+            <br>
+                <strong> Transmute AI Model Efficiency Toolkit </strong>
+            </br>
+        </p>
+        <p align="center">
+            <a href="https://github.com/transmuteAI/trailmet/blob/dev/LICENSE">
+                <img alt="GitHub" src="https://img.shields.io/github/license/transmuteAI/trailmet?color=blue">
+            </a>
+            <a href="https://transmuteai-trailmet.readthedocs.io/en/latest/">
+                <img alt="Documentation" src="https://img.shields.io/badge/docs-passing-brightgreen">
+            </a>
+            <a href="https://github.com/transmuteAI/trailmet/actions/workflows/ci.yml">
+                <img alt="Run tests with pytest" src="https://github.com/transmuteAI/trailmet/actions/workflows/ci.yml/badge.svg">
+            </a>
+            <a href="#">
+                <img alt="GitHub Stars" src="https://img.shields.io/github/stars/transmuteAI/trailmet">
+            </a>
+            <a href="#">
+                <img alt="GitHub Forks" src="https://img.shields.io/github/forks/transmuteAI/trailmet">
+            </a>
+        </p>
+        <h3 align="justified">
+        <!-- <p>Transmute AI Lab Model Efficiency Toolkit -->
+        </h3>
+        
+        # Introduction
+        
+        Trailmet is a model efficiency toolkit for compressing deep learning models using state of the art compression techniques.
+        Today deep learning models are not deployable because of their huge memory footprint, TRAILMET is an effort to make deep learning models more efficient in their size to performance ratio. It is developed using Pytorch 1.13.
+        
+        ### Major features
+        
+        - State of the art compression algorithms implemented.
+        - Demo notebooks for training each algorithm.
+        - Modular Design: All alogithms are modular and can customized easily for any kind of model and dataset.
+        
+        # Installation
+        
+        Below are quick steps for installation:
+        
+        ```shell
+        git clone https://github.com/transmuteAI/trailmet.git
+        cd trailmet
+        conda create -n trailmet
+        conda activate trailmet
+        conda install pytorch=1.13 torchvision=0.14 pytorch-cuda=11.7 -c pytorch -c nvidia
+        pip install -r requirements.txt
+        ```
+        
+        # Algorithms Implemented
+        
+        Demo notebooks for each algorithm is added in [experiments](https://github.com/transmuteAI/trailmet/blob/dev/experiments) folder
+        
+        <details open>
+        <summary> Knowledge Distillation</summary>
+        
+        - [x] [Response KD](https://arxiv.org/abs/1503.02531)
+        - [x] [Factor Transfer](https://arxiv.org/abs/1802.04977)
+        - [x] [Attention Transfer](https://arxiv.org/abs/1612.03928)
+        
+        </details>
+        
+        <details open>
+        <summary> Pruning </summary>
+        
+        - [x] [Chipnet](https://arxiv.org/abs/2102.07156)
+        - [x] [Network slimming](https://arxiv.org/abs/1708.06519)
+        - [x] [Growth Regularization](https://arxiv.org/abs/2012.09243)
+        
+        </details>
+        
+        <details open>
+        <summary> Quantization</summary>
+        
+        - [x] [BitSplit](https://dl.acm.org/doi/abs/10.5555/3524938.3525851)
+        - [x] [BRECQ](https://arxiv.org/abs/2102.05426)
+        - [x] [LAPQ](https://arxiv.org/abs/1911.07190)
+        
+        </details>
+        
+        <details open>
+        <summary> Binarization</summary>
+        
+        - [x] [BiRealNet](https://arxiv.org/abs/1808.00278)
+        - [x] [ReActNet](https://arxiv.org/abs/2003.03488)
+        - [x] [BNN-BN](https://arxiv.org/abs/2104.08215v1)
+        
+        </details>
+        
+        # Acknowledgement
+        
+        # Citation
+        
+        If you find this project useful in your research, please consider cite:
+        
+        ```BibTeX
+        @misc{,
+            title={},
+            author={},
+            howpublished = {}},
+            year={2023}
+        }
+        ```
+        
+        # License
+        
+        This project is released under the [MIT license](LICENSE).
+        
 Keywords: computer vision,image classification,model efficiency
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
-License-File: LICENSE
-
-<p align="center">
-    <br>
-        <img src="docs/source/imgs/Group 13.png" width="500"/>
-    </br>
-    <br>
-        <strong> Transmute AI Model Efficiency Toolkit </strong>
-    </br>
-</p>
-<p align="center">
-    <a href="https://github.com/transmuteAI/trailmet/blob/dev/LICENSE">
-        <img alt="GitHub" src="https://img.shields.io/github/license/transmuteAI/trailmet?color=blue">
-    </a>
-    <a href="https://transmuteai-trailmet.readthedocs.io/en/latest/">
-        <img alt="Documentation" src="https://img.shields.io/badge/docs-passing-brightgreen">
-    </a>
-    <a href="https://github.com/transmuteAI/trailmet/actions/workflows/ci.yml">
-        <img alt="Run tests with pytest" src="https://github.com/transmuteAI/trailmet/actions/workflows/ci.yml/badge.svg">
-    </a>
-    <a href="#">
-        <img alt="GitHub Stars" src="https://img.shields.io/github/stars/transmuteAI/trailmet">
-    </a>
-    <a href="#">
-        <img alt="GitHub Forks" src="https://img.shields.io/github/forks/transmuteAI/trailmet">
-    </a>
-</p>
-<h3 align="justified">
-<!-- <p>Transmute AI Lab Model Efficiency Toolkit -->
-</h3>
-
-# Introduction
-
-Trailmet is a model efficiency toolkit for compressing deep learning models using state of the art compression techniques.
-Today deep learning models are not deployable because of their huge memory footprint, TRAILMET is an effort to make deep learning models more efficient in their size to performance ratio. It is developed using Pytorch 1.13.
-
-### Major features
-
-- State of the art compression algorithms implemented.
-- Demo notebooks for training each algorithm.
-- Modular Design: All alogithms are modular and can customized easily for any kind of model and dataset.
-
-# Installation
-
-Below are quick steps for installation:
-
-```shell
-git clone https://github.com/transmuteAI/trailmet.git
-cd trailmet
-conda create -n trailmet
-conda activate trailmet
-conda install pytorch=1.13 torchvision=0.14 pytorch-cuda=11.7 -c pytorch -c nvidia
-pip install -r requirements.txt
-```
-
-# Algorithms Implemented
-
-Demo notebooks for each algorithm is added in [experiments](https://github.com/transmuteAI/trailmet/blob/dev/experiments) folder
-
-<details open>
-<summary> Knowledge Distillation</summary>
-
-- [x] [Response KD](https://arxiv.org/abs/1503.02531)
-- [x] [Factor Transfer](https://arxiv.org/abs/1802.04977)
-- [x] [Attention Transfer](https://arxiv.org/abs/1612.03928)
-
-</details>
-
-<details open>
-<summary> Pruning </summary>
-
-- [x] [Chipnet](https://arxiv.org/abs/2102.07156)
-- [x] [Network slimming](https://arxiv.org/abs/1708.06519)
-- [x] [Growth Regularization](https://arxiv.org/abs/2012.09243)
-
-</details>
-
-<details open>
-<summary> Quantization</summary>
-
-- [x] [BitSplit](https://dl.acm.org/doi/abs/10.5555/3524938.3525851)
-- [x] [BRECQ](https://arxiv.org/abs/2102.05426)
-- [x] [LAPQ](https://arxiv.org/abs/1911.07190)
-
-</details>
-
-<details open>
-<summary> Binarization</summary>
-
-- [x] [BiRealNet](https://arxiv.org/abs/1808.00278)
-- [x] [ReActNet](https://arxiv.org/abs/2003.03488)
-- [x] [BNN-BN](https://arxiv.org/abs/2104.08215v1)
-
-</details>
-
-# Acknowledgement
-
-# Citation
-
-If you find this project useful in your research, please consider cite:
-
-```BibTeX
-@misc{,
-    title={},
-    author={},
-    howpublished = {}},
-    year={2023}
-}
-```
-
-# License
-
-This project is released under the [MIT license](LICENSE).
```

#### html2text {}

```diff
@@ -1,22 +1,13 @@
-Metadata-Version: 2.1 Name: trailmet Version: 0.0.1rc0 Summary: Transmute AI
+Metadata-Version: 2.1 Name: trailmet Version: 0.0.1rc2 Summary: Transmute AI
 Model Efficiency Toolkit Home-page: https://github.com/transmuteAI/trailmet
 Author: TrAILMET Contributors Author-email: transmute.ai@gmail.com License: MIT
-License Keywords: computer vision,image classification,model efficiency
-Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-all License-File: LICENSE
+License Description:
 
-                       [docs/source/imgs/Group 13.png]
+                       [docs/source/imgs/trailmet.png]
                     Transmute AI Model Efficiency Toolkit
 [GitHub] [Documentation] [Run_tests_with_pytest] [GitHub_Stars] [GitHub_Forks]
 # Introduction Trailmet is a model efficiency toolkit for compressing deep
 learning models using state of the art compression techniques. Today deep
 learning models are not deployable because of their huge memory footprint,
 TRAILMET is an effort to make deep learning models more efficient in their size
 to performance ratio. It is developed using Pytorch 1.13. ### Major features -
@@ -37,8 +28,18 @@
 Quantization - [x] [BitSplit](https://dl.acm.org/doi/abs/10.5555/
 3524938.3525851) - [x] [BRECQ](https://arxiv.org/abs/2102.05426) - [x] [LAPQ]
 (https://arxiv.org/abs/1911.07190)    Binarization - [x] [BiRealNet](https://
 arxiv.org/abs/1808.00278) - [x] [ReActNet](https://arxiv.org/abs/2003.03488) -
 [x] [BNN-BN](https://arxiv.org/abs/2104.08215v1)  # Acknowledgement # Citation
 If you find this project useful in your research, please consider cite:
 ```BibTeX @misc{, title={}, author={}, howpublished = {}}, year={2023} } ``` #
-License This project is released under the [MIT license](LICENSE).
+License This project is released under the [MIT license](LICENSE). Keywords:
+computer vision,image classification,model efficiency Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
+all
```

### Comparing `trailmet-0.0.1rc0/README.md` & `trailmet-0.0.1rc2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <p align="center">
     <br>
-        <img src="docs/source/imgs/Group 13.png" width="500"/>
+        <img src="docs/source/imgs/trailmet.png" width="500"/>
     </br>
     <br>
         <strong> Transmute AI Model Efficiency Toolkit </strong>
     </br>
 </p>
 <p align="center">
     <a href="https://github.com/transmuteAI/trailmet/blob/dev/LICENSE">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 
-                       [docs/source/imgs/Group 13.png]
+                       [docs/source/imgs/trailmet.png]
                     Transmute AI Model Efficiency Toolkit
 [GitHub] [Documentation] [Run_tests_with_pytest] [GitHub_Stars] [GitHub_Forks]
 # Introduction Trailmet is a model efficiency toolkit for compressing deep
 learning models using state of the art compression techniques. Today deep
 learning models are not deployable because of their huge memory footprint,
 TRAILMET is an effort to make deep learning models more efficient in their size
 to performance ratio. It is developed using Pytorch 1.13. ### Major features -
```

### Comparing `trailmet-0.0.1rc0/tests/test_general.py` & `trailmet-0.0.1rc2/trailmet/algorithms/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,17 +15,8 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-def test_sum():
-    assert sum([1, 2, 3]) == 6, 'Should be 6'
-
-
-def test_sum2():
-    assert sum([1, 2, 3]) == 6, 'Should be 6'
-
-
-def test_sum3():
-    assert sum([1, 2, 3]) == 6, 'Should be 6'
+from .algorithms import BaseAlgorithm
```

### Comparing `trailmet-0.0.1rc0/tests/test_unwanted_files.py` & `trailmet-0.0.1rc2/trailmet/algorithms/binarize/binarize.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,31 +15,19 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-import os
-import re
+from ..algorithms import BaseAlgorithm
 
-unwanted_extensions = [
-    '.DS_Store',
-    '.pyc',
-    '.pth',
-    '.gz',
-]  # Add any other unwanted file extensions
 
+class BaseBinarize(BaseAlgorithm):
+    """Base class for binarization algorithms."""
 
-def test_unwanted_files():
-    root_dir = '..'  # Replace with the root directory of your repository
-    for dirpath, dirnames, filenames in os.walk(root_dir):
-        print(filenames)
-        print(dirpath)
-        if 'tests' in re.split(r'[\\/]', dirpath):
-            print(dirpath)
-            continue  # Skip the current directory
-        for filename in filenames:
-            file_extension = os.path.splitext(filename)[1]
-            assert (
-                file_extension
-                not in unwanted_extensions), f'Unwanted file found: {filename}'
+    def __init__(self, **kwargs):
+        super(BaseBinarize, self).__init__(**kwargs)
+        pass
+
+    def Binarize(self, model, dataloaders, **kwargs):
+        pass
```

### Comparing `trailmet-0.0.1rc0/trailmet/__init__.py` & `trailmet-0.0.1rc2/trailmet/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from .algorithms import BaseAlgorithm
 from .datasets import DatasetFactory
 from .models import ModelsFactory
 from .version import __version__
 
-__all__ = ['BaseAlgorithm', "DatasetFactory", "ModelsFactory", '__version__']
+__all__ = ['BaseAlgorithm', 'DatasetFactory', 'ModelsFactory', '__version__']
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/__init__.py` & `trailmet-0.0.1rc2/trailmet/datasets/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from .algorithms import BaseAlgorithm
+from .classification import DatasetFactory
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/algorithms.py` & `trailmet-0.0.1rc2/trailmet/algorithms/algorithms.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,17 @@
     template function and use it as the first point of invoking the model
     compression process.
 
     For methods that require to perform pretraining and fine-tuning, the
     implementation of base_train() method can directly be used for both the
     tasks. In case of modifications, overwrite this function based on the
     needs.
+    Parameters
+    ----------
+        kwargs (object): A yaml safe loaded file with information like cuda_id, log_dir, device, etc.
     """
 
     def __init__(self, **kwargs):
         self.pretraining_epochs = 200
         self.cuda_id = kwargs.get('cuda_id', 0)
         self.device = torch.device(f'cuda:{str(self.cuda_id)}')
         self.log_name = kwargs.get('log_dir', 'abc')
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/binarize/BNNBN.py` & `trailmet-0.0.1rc2/trailmet/algorithms/binarize/BNNBN.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,24 @@
 import wandb
 import pandas as pd
 
 logger = logging.getLogger(__name__)
 
 
 class BNNBN:
+    """
+    References
+    ----------
+
+    Parameters
+    ----------
+        model (object): A pytorch model you want to use.
+        dataloaders (dict): Dictionary with dataloaders for train, val and test. Keys: 'train', 'val', 'test'.
+        kwargs (object): YAML safe loaded file with information like batch_size, optimizer, epochs, momentum, etc.
+    """
 
     def __init__(self, model, dataloaders, **kwargs):
         self.train_loader = dataloaders['train']
         self.val_loader = dataloaders['val']
         self.test_loader = dataloaders['test']
         self.model_student = model
         self.kwargs = kwargs
@@ -95,14 +105,15 @@
         logger.info(f'Experiment Arguments: {self.kwargs}')
 
         if self.wandb_monitor:
             wandb.init(project='Trailmet BNNBN', name=self.name)
             wandb.config.update(self.kwargs)
 
     def compress_model(self):
+        """Function for compressing the model."""
         if not torch.cuda.is_available():
             sys.exit(1)
         start_t = time.time()
 
         cudnn.benchmark = True
         cudnn.enabled = True
 
@@ -325,14 +336,15 @@
         train_loader,
         model_student,
         model_teacher,
         criterion,
         optimizer,
         scheduler,
     ):
+        """Function for training KD."""
         batch_time = AverageMeter('Time', ':6.3f')
         data_time = AverageMeter('Data', ':6.3f')
         losses = AverageMeter('Loss', ':.4e')
         top1 = AverageMeter('Acc@1', ':6.2f')
         top5 = AverageMeter('Acc@5', ':6.2f')
 
         model_student.train()
@@ -422,14 +434,15 @@
                     'train_top5_acc_KD': top5.val,
                 })
 
         return losses.avg, top1.avg, top5.avg
 
     def train(self, epoch, train_loader, model_student, criterion, optimizer,
               scheduler):
+        """Training Function."""
         batch_time = AverageMeter('Time', ':6.3f')
         data_time = AverageMeter('Data', ':6.3f')
         losses = AverageMeter('Loss', ':.4e')
         top1 = AverageMeter('Acc@1', ':6.2f')
         top5 = AverageMeter('Acc@5', ':6.2f')
 
         epoch_iterator = tqdm(
@@ -515,14 +528,15 @@
                     'train_top1_acc': top1.val,
                     'train_top5_acc': top5.val,
                 })
 
         return losses.avg, top1.avg, top5.avg
 
     def validate(self, epoch, val_loader, model, criterion):
+        """Validate Function."""
         batch_time = AverageMeter('Time', ':6.3f')
         losses = AverageMeter('Loss', ':.4e')
         top1 = AverageMeter('Acc@1', ':6.2f')
         top5 = AverageMeter('Acc@5', ':6.2f')
 
         epoch_iterator = tqdm(
             val_loader,
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/binarize/ReActNet.py` & `trailmet-0.0.1rc2/trailmet/algorithms/binarize/ReActNet.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
                      kernel_size=3,
                      stride=stride,
                      padding=1,
                      bias=False)
 
 
 class BinaryActivation(nn.Module):
+    """Class for BinaryActivation."""
 
     def __init__(self):
         super(BinaryActivation, self).__init__()
 
     def forward(self, x):
         out_forward = torch.sign(x)
         # out_e1 = (x^2 + 2*x)
@@ -71,14 +72,15 @@
             torch.float32) + 1 * (1 - mask3.type(torch.float32))
         out = out_forward.detach() - out3.detach() + out3
 
         return out
 
 
 class LearnableBias(nn.Module):
+    """Class for LearnableBias."""
 
     def __init__(self, out_chn):
         super(LearnableBias, self).__init__()
         self.bias = nn.Parameter(torch.zeros(1, out_chn, 1, 1),
                                  requires_grad=True)
 
     def forward(self, x):
@@ -192,14 +194,25 @@
         out = self.prelu(out)
         out = self.move2(out)
 
         return out
 
 
 class ReActNet(BaseBinarize):
+    """
+    References
+    ----------
+
+    Parameters
+    ----------
+        teacher (object): Teacher model you want to use.
+        model (object): A pytorch model you want to use.
+        dataloaders (dict): Dictionary with dataloaders for train, val and test. Keys: 'train', 'val', 'test'.
+        kwargs (object): YAML safe loaded file with information like batch_size, optimizer, epochs, momentum, etc.
+    """
 
     def __init__(self, teacher, model, dataloaders, **kwargs):
         super(ReActNet, self).__init__(**kwargs)
         self.teacher = teacher
         self.model = model
         self.layers = model.layers_size
         self.device = torch.device(
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/binarize/__init__.py` & `trailmet-0.0.1rc2/trailmet/algorithms/binarize/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/binarize/binarize.py` & `trailmet-0.0.1rc2/trailmet/algorithms/distill/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,19 +15,13 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from ..algorithms import BaseAlgorithm
-
-
-class BaseBinarize(BaseAlgorithm):
-    """Base class for binarization algorithms."""
-
-    def __init__(self, **kwargs):
-        super(BaseBinarize, self).__init__(**kwargs)
-        pass
-
-    def Binarize(self, model, dataloaders, **kwargs):
-        pass
+from .attention_transfer import AttentionTransfer
+from .distill import Distillation
+from .factor_transfer import FactorTransfer
+from .losses import KDTransferLoss, RkdDistance, RKdAngle
+from .response_kd import KDTransfer
+from .rkd import RKDTransfer
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/binarize/birealnet.py` & `trailmet-0.0.1rc2/trailmet/algorithms/binarize/birealnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,26 @@
 import pandas as pd
 import numpy as np
 
 logger = logging.getLogger(__name__)
 
 
 class BirealNet(BaseBinarize):
+    """
+    `BirealNet <https://openaccess.thecvf.com/content_ECCV_2018/papers/zechun_liu_Bi-Real_Net_Enhancing_ECCV_2018_paper.pdf>`_ Implementation.
+
+    References
+    ----------
+
+    Parameters
+    ----------
+        model (object): A pytorch model you want to use.
+        dataloaders (dict): Dictionary with dataloaders for train, val and test. Keys: 'train', 'val', 'test'.
+        CFG (object): YAML safe loaded file with information like batch_size, optimizer, epochs, momentum, etc.
+    """
 
     def __init__(self, model, dataloaders, **CFG):
         self.model = model
         self.dataloaders = dataloaders
         self.CFG = CFG
         self.batch_size = self.CFG['batch_size']
         self.optimizer = self.CFG['optimizer']
@@ -89,14 +101,15 @@
 
         if self.wandb_monitor:
             wandb.init(project='Trailmet BiRealNet', name=self.name)
             wandb.config.update(self.CFG)
 
     def train(self, epoch, train_loader, model, criterion, optimizer,
               scheduler):
+        """Train function."""
         batch_time = AverageMeter('Time', ':6.3f')
         data_time = AverageMeter('Data', ':6.3f')
         losses = AverageMeter('Loss', ':.4e')
         top1 = AverageMeter('Acc@1', ':6.2f')
         top5 = AverageMeter('Acc@5', ':6.2f')
 
         epoch_iterator = tqdm(
@@ -173,14 +186,15 @@
                     'train_top1_acc': top1.val,
                     'train_top5_acc': top5.val,
                 })
 
         return losses.avg, top1.avg, top5.avg
 
     def validate(self, epoch, val_loader, model, criterion, CFG):
+        """Validate Function."""
         batch_time = AverageMeter('Time', ':6.3f')
         losses = AverageMeter('Loss', ':.4e')
         top1 = AverageMeter('Acc@1', ':6.2f')
         top5 = AverageMeter('Acc@5', ':6.2f')
 
         epoch_iterator = tqdm(
             val_loader,
@@ -248,14 +262,15 @@
             print(
                 ' * Val acc@1 {top1.avg:.3f} Val acc@5 {top5.avg:.3f}'.format(
                     top1=top1, top5=top5))
 
         return losses.avg, top1.avg, top5.avg
 
     def test(self, epoch, test_loader, model, criterion, CFG):
+        """Test Function."""
         batch_time = AverageMeter('Time', ':6.3f')
         losses = AverageMeter('Loss', ':.4e')
         top1 = AverageMeter('Acc@1', ':6.2f')
         top5 = AverageMeter('Acc@5', ':6.2f')
 
         epoch_iterator = tqdm(
             test_loader,
@@ -322,14 +337,15 @@
 
             print(' * Test acc@1 {top1.avg:.3f} Test acc@5 {top5.avg:.3f}'.
                   format(top1=top1, top5=top5))
 
         return losses.avg, top1.avg, top5.avg
 
     def binarize(self):
+        """Function used to binarize the model."""
         if not torch.cuda.is_available():
             sys.exit(1)
         start_t = time.time()
 
         cudnn.benchmark = True
         cudnn.enabled = True
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/binarize/utils.py` & `trailmet-0.0.1rc2/trailmet/algorithms/binarize/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,21 @@
         [-0.5808, -0.0045, -0.8140],
         [-0.5836, -0.6948, 0.4203],
     ]),
 }
 
 
 class Lighting(object):
+    """
+    Parameters
+    ----------
+        alphastd ():
+        eigval (np.array): Eigen Value
+        eigvec (np.array): Eigen Vector
+    """
 
     def __init__(self,
                  alphastd,
                  eigval=imagenet_pca['eigval'],
                  eigvec=imagenet_pca['eigvec']):
         self.alphastd = alphastd
         assert eigval.shape == (3, )
@@ -83,14 +90,19 @@
 class DistributionLoss(loss._Loss):
     """The KL-Divergence loss for the binary student model and real teacher
     output.
 
     output must be a pair of (model_output, real_output), both NxC tensors. The
     rows of real_output must all add up to one (probability scores); however,
     model_output must be the pre-softmax output of the network.
+
+    Parameters
+    ----------
+        model_output (Tensor): Prediction from your model.
+        real_output (Tensor): Ground Truth.
     """
 
     def forward(self, model_output, real_output):
         self.size_average = True
 
         if real_output.requires_grad:
             raise ValueError(
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/distill/__init__.py` & `trailmet-0.0.1rc2/trailmet/algorithms/prune/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,13 +15,27 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from .attention_transfer import AttentionTransfer
-from .distill import Distillation
-from .factor_transfer import FactorTransfer
-from .losses import KDTransferLoss, RkdDistance, RKdAngle
-from .response_kd import KDTransfer
-from .rkd import RKDTransfer
+from .chip import Chip
+from .chipnet import ChipNet
+from .growth_regularisation import Growth_Regularisation
+from .network_slimming import Network_Slimming
+from .pns import ChannelRounding, Conv2dWrapper, LinearWrapper, BN2dWrapper, SlimPruner
+from .prune import BasePruning
+from .pruner import pruner_dict
+from .utils import (
+    update_bn_grad,
+    summary_model,
+    is_depthwise_conv2d,
+    prune_conv2d,
+    prune_bn2d,
+    prune_fc,
+    cal_threshold_by_bn2d_weights,
+    mask2idxes,
+    top_k_idxes,
+    ceil,
+    round_up_to_power_of_2,
+)
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/distill/attention_transfer.py` & `trailmet-0.0.1rc2/trailmet/algorithms/distill/attention_transfer.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
 from trailmet.algorithms.distill.distill import Distillation, ForwardHookManager
 
 # Paying More Attention to Attention: Improving the Performance of Convolutional Neural Networks via Attention Transfer
 
 
 class AttentionTransferLoss(nn.Module):
+    """Class for loss used."""
 
     def __init__(self):
         super().__init__()
 
     @staticmethod
     def attention_map(feature_map):
         """Compute the attention map from a feature map."""
@@ -65,15 +66,23 @@
         loss = 0
         for teacher_feature_map, student_feature_map in feature_map_pairs:
             loss += self.compute_loss(teacher_feature_map, student_feature_map)
         return loss
 
 
 class AttentionTransfer(Distillation):
-    """Class to compress model using distillation via attention transfer."""
+    """Class to compress model using distillation via attention transfer.
+
+    Parameters
+    ----------
+        teacher_model (object): Teacher model you want to use.
+        student_model (object): Student model you want to use.
+        dataloaders (dict): Dictionary with dataloaders for train, val and test. Keys: 'train', 'val', 'test'.
+        kwargs (object): YAML safe loaded file with information like device, distill_args(teacher_layer_names, student_layer_names, etc).
+    """
 
     def __init__(self, teacher_model, student_model, dataloaders, **kwargs):
         super(AttentionTransfer, self).__init__(**kwargs)
         self.teacher_model = teacher_model
         self.student_model = student_model
         self.dataloaders = dataloaders
         self.kwargs = kwargs
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/distill/distill.py` & `trailmet-0.0.1rc2/trailmet/algorithms/distill/distill.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from torch.nn.parallel import DistributedDataParallel
 from trailmet.algorithms.algorithms import BaseAlgorithm
 
 __all__ = ['Distillation']
 
 
 class Distillation(BaseAlgorithm):
+    """Base Class for Distillation."""
 
     def __init__(self, **kwargs):
         super(Distillation, self).__init__(**kwargs)
 
         pass
 
 
@@ -168,14 +169,17 @@
         >>> model = models.resnet18()
         >>> forward_hook_manager.add_hook(model, 'layer2')
         >>> x = torch.rand(16, 3, 224, 224)
         >>> y = model(x)
         >>> io_dict = forward_hook_manager.pop_io_dict()
         >>> layer2_input_tensor = io_dict['layer2']['input']
         >>> layer2_output_tensor = io_dict['layer2']['output']
+    Parameters
+    ----------
+        target_device (str): Target device
     """
 
     def __init__(self, target_device):
         self.target_device = (torch.device(target_device) if isinstance(
             target_device, str) else target_device)
         self.uses_cuda = self.target_device.type == 'cuda'
         self.io_dict = dict()
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/distill/factor_transfer.py` & `trailmet-0.0.1rc2/trailmet/algorithms/distill/factor_transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         loss = self.criterion_ce(logits, labels)
         loss += self.beta * self.criterion(self.FT(factor_student),
                                            self.FT(factor_teacher.detach()))
         return loss
 
 
 class Paraphraser(nn.Module):
+    """Paraphraser Class."""
 
     def __init__(self, in_planes, planes, stride=1):
         super(Paraphraser, self).__init__()
         self.leakyrelu = nn.LeakyReLU(0.1)
         #       self.bn0 = nn.BatchNorm2d(in_planes)
         self.conv0 = nn.Conv2d(in_planes,
                                in_planes,
@@ -132,14 +133,15 @@
             out = self.leakyrelu((self.deconv0(x)))
             out = self.leakyrelu((self.deconv1(out)))
             out = self.leakyrelu((self.deconv2(out)))
         return out
 
 
 class Translator(nn.Module):
+    """Translator Class."""
 
     def __init__(self, in_planes, planes, stride=1):
         super(Translator, self).__init__()
         self.leakyrelu = nn.LeakyReLU(0.1)
         #       self.bn0 = nn.BatchNorm2d(in_planes)
         self.conv0 = nn.Conv2d(in_planes,
                                in_planes,
@@ -166,15 +168,24 @@
         out = self.leakyrelu((self.conv0(x)))
         out = self.leakyrelu((self.conv1(out)))
         out = self.leakyrelu((self.conv2(out)))
         return out
 
 
 class FactorTransfer(Distillation):
-    """Class to compress model using distillation via factor transfer."""
+    """Class to compress model using distillation via factor transfer.
+
+    Parameters
+    ----------
+        teacher_model (object): Teacher model you want to use.
+        student_model (object): Student model you want to use.
+        dataloaders (dict): Dictionary with dataloaders for train, val and test. Keys: 'train', 'val', 'test'.
+        paraphraser (object): Paraphrase model
+        kwargs (object): YAML safe loaded file with information like distill_args(teacher_layer_names, student_layer_names, etc).
+    """
 
     def __init__(self,
                  teacher_model,
                  student_model,
                  dataloaders,
                  paraphraser=None,
                  **kwargs):
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/distill/losses.py` & `trailmet-0.0.1rc2/trailmet/algorithms/distill/losses.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import torch.nn.functional as F
 from trailmet.utils.functions import pdist
 
 __all__ = ['KDTransferLoss', 'RkdDistance', 'RKdAngle']
 
 
 class KDTransferLoss(nn.Module):
+    """Class for KD Transfer Loss."""
 
     def __init__(self, temperature, reduction):
         super().__init__()
         self.temperature = temperature
         self.reduction = reduction
         self.kd_fun = nn.KLDivLoss(reduction=self.reduction)
 
@@ -39,14 +40,15 @@
         s_max = F.log_softmax(out_s / self.temperature, dim=1)
         t_max = F.softmax(out_t / self.temperature, dim=1)
         loss_kd = self.kd_fun(s_max, t_max)
         return loss_kd
 
 
 class RkdDistance(nn.Module):
+    """Class for RKD Distance."""
 
     def forward(self, student, teacher):
         with torch.no_grad():
             t_d = pdist(teacher, squared=False)
             mean_td = t_d[t_d > 0].mean()
             t_d = t_d / mean_td
 
@@ -55,14 +57,15 @@
         d = d / mean_d
 
         loss = F.smooth_l1_loss(d, t_d, reduction='elementwise_mean')
         return loss
 
 
 class RKdAngle(nn.Module):
+    """Class for RKD Angle."""
 
     def forward(self, student, teacher):
         # N x C
         # N x N x C
 
         with torch.no_grad():
             td = teacher.unsqueeze(0) - teacher.unsqueeze(1)
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/distill/response_kd.py` & `trailmet-0.0.1rc2/trailmet/algorithms/distill/response_kd.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,24 @@
 logger = logging.getLogger(__name__)
 
 # Hinton's Knowledge Distillation
 seed_everything(43)
 
 
 class KDTransfer(Distillation):
-    """Class to compress model using distillation via kd transfer."""
+    """Class to compress model using distillation via KD transfer.
+
+    Parameters
+    ----------
+        teacher_model (object): Teacher model you want to use.
+        student_model (object): Student model you want to use.
+        dataloaders (dict): Dictionary with dataloaders for train, val and test. Keys: 'train', 'val', 'test'.
+        paraphraser (object): Paraphrase model
+        kwargs (object): YAML safe loaded file with information like distill_args(lambda, temperature, etc).
+    """
 
     def __init__(self, teacher_model, student_model, dataloaders, **kwargs):
         super(KDTransfer, self).__init__(**kwargs)
         self.teacher_model = teacher_model
         self.student_model = student_model
         self.dataloaders = dataloaders
         self.kwargs = kwargs
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/distill/rkd.py` & `trailmet-0.0.1rc2/trailmet/algorithms/distill/rkd.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,24 @@
 
 from trailmet.utils import AverageMeter, accuracy, save_checkpoint
 
 logger = logging.getLogger(__name__)
 
 
 class RKDTransfer(Distillation):
-    """Class to compress model using distillation via RKD transfer."""
+    """Class to compress model using distillation via RKD transfer.
+
+    Parameters
+    ----------
+        teacher_model (object): Teacher model you want to use.
+        student_model (object): Student model you want to use.
+        dataloaders (dict): Dictionary with dataloaders for train, val and test. Keys: 'train', 'val', 'test'.
+        paraphraser (object): Paraphrase model
+        kwargs (object): YAML safe loaded file with information like device, distill_args(beta, temperature, etc).
+    """
 
     def __init__(self, teacher_model, student_model, dataloaders, **kwargs):
         super(RKDTransfer, self).__init__(**kwargs)
         self.teacher_model = teacher_model
         self.student_model = student_model
         self.dataloaders = dataloaders
         self.kwargs = kwargs
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/prune/__init__.py` & `trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,27 +15,18 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from .chip import Chip
-from .chipnet import ChipNet
-from .growth_regularisation import Growth_Regularisation
-from .network_slimming import Network_Slimming
-from .pns import ChannelRounding, Conv2dWrapper, LinearWrapper, BN2dWrapper, SlimPruner
-from .prune import BasePruning
-from .pruner import pruner_dict
-from .utils import (
-    update_bn_grad,
-    summary_model,
-    is_depthwise_conv2d,
-    prune_conv2d,
-    prune_bn2d,
-    prune_fc,
-    cal_threshold_by_bn2d_weights,
-    mask2idxes,
-    top_k_idxes,
-    ceil,
-    round_up_to_power_of_2,
-)
+from .l1_pruner import Pruner as L1Pruner
+from .meta_pruner import MetaPruner
+from .reg_pruner import Pruner as RegPruner
+
+# when new pruner implementation is added in the 'pruner' dir, update this dict to maintain minimal code change.
+# key: pruning method name, value: the corresponding pruner
+pruner_dict = {
+    'GReg-1': RegPruner,
+    'GReg-2': RegPruner,
+    'L1': L1Pruner,
+}
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/prune/chip.py` & `trailmet-0.0.1rc2/trailmet/algorithms/prune/chip.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,21 @@
     chip_adjust_learning_rate,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class Chip(BasePruning):
+    """
+    Parameters
+    ----------
+        model (object): A pytorch model you want to use.
+        dataloaders (dict): Dictionary with dataloaders for train, val and test. Keys: 'train', 'val', 'test'.
+        CFG (object): YAML safe loaded file with information like batch_size, arch, epochs, momentum, etc.
+    """
 
     def __init__(self, model, dataloaders, **CFG):
         self.dataloaders = dataloaders
         self.model = model
         self.CFG = CFG
         self.batch_size = self.CFG['batch_size']
         self.arch = self.CFG['arch']
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/prune/chipnet.py` & `trailmet-0.0.1rc2/trailmet/algorithms/prune/chipnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,22 @@
         new_bn, conv_module = PrunableBatchNorm2d.from_batchnorm(
             bn_module, conv_module=conv_module)
         ModuleInjection.prunable_modules.append(new_bn)
         return conv_module, new_bn
 
 
 class ChipNet(BasePruning):
-    """Class to compress models using chipnet method."""
+    """Class to compress models using chipnet method.
+
+    Parameters
+    ----------
+        model (object): A pytorch model you want to use.
+        dataloaders (dict): Dictionary with dataloaders for train, val and test. Keys: 'train', 'val', 'test'.
+        kwargs (object): YAML safe loaded file with information like chipnet_args(budget_type, channel_ratio, etc.)
+    """
 
     def __init__(self, model, dataloaders, **kwargs):
         super(ChipNet, self).__init__(**kwargs)
         self.model = model
         self.dataloaders = dataloaders
         self.kwargs = kwargs
         self.budget_type = self.kwargs['CHIPNET_ARGS'].get(
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/prune/growth_regularisation.py` & `trailmet-0.0.1rc2/trailmet/algorithms/prune/growth_regularisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,20 @@
     functions defined below. The root command to invoke the compression of any
     model is .compress_model(). Thus, it is required that all algorithms
     complete this template function and use it as the first point of invoking
     the model compression process. For methods that require to perform
     pretraining and fine-tuning, the implementation of base_train() method can
     directly be used for both the tasks. In case of modifications, overwrite
     this function based on the needs.
+
+     Parameters
+    ----------
+        model (object): A pytorch model you want to use.
+        dataloaders (dict): Dictionary with dataloaders for train, val and test. Keys: 'train', 'val', 'test'.
+        kwargs (object): YAML safe loaded file with information like dataset, num_classes, epoch, weight_decay, etc.
     """
 
     def __init__(self, model, dataloaders, **kwargs):
         self.device = 'cuda'
         self.train_loader = dataloaders['train']
         self.val_loader = dataloaders['val']
         self.test_loader = dataloaders['test']
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/prune/network_slimming.py` & `trailmet-0.0.1rc2/trailmet/algorithms/prune/network_slimming.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,20 @@
     functions defined below. The root command to invoke the compression of any
     model is .compress_model(). Thus, it is required that all algorithms
     complete this template function and use it as the first point of invoking
     the model compression process. For methods that require to perform
     pretraining and fine-tuning, the implementation of base_train() method can
     directly be used for both the tasks. In case of modifications, overwrite
     this function based on the needs.
+
+    Parameters
+    ----------
+        model (object): A pytorch model you want to use.
+        dataloaders (dict): Dictionary with dataloaders for train, val and test. Keys: 'train', 'val', 'test'.
+        kwargs (object): YAML safe loaded file with information like num_classes, ft_only, dataset, etc.
     """
 
     def __init__(self, model, dataloaders, **kwargs):
         self.device = 'cuda'
         self.model = model
         self.num_classes = kwargs.get('num_classes', 100)
         self.dataloaders = dataloaders
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/prune/pns.py` & `trailmet-0.0.1rc2/trailmet/algorithms/prune/pns.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,14 +55,22 @@
 class ChannelRounding(Enum):
     NONE = 'none'
     EIGHT = 'eight'  # 8 的倍数
     TWO_POW = 'two_pow'  # 2^n
 
 
 class Conv2dWrapper:
+    """
+    Parameters
+    ----------
+        module (object): Module to be used.
+        name (str): Name of the layer.
+        prev_bn_name (str): Name of the previous BN layer.
+        next_bn_name (str): Name of the next BN layer.
+    """
 
     def __init__(self, module, name, prev_bn_name=None, next_bn_name=None):
         self.module: Conv2d = copy.deepcopy(module)
         self.pruned_module: Conv2d = module
         self.name = name
         self.prev_bn_name = prev_bn_name
         self.next_bn_name = next_bn_name
@@ -110,14 +118,21 @@
             'name': self.name,
             'in_channels_keep_idxes': self.in_channels_keep_idxes,
             'out_channels_keep_idxes': self.out_channels_keep_idxes,
         }
 
 
 class LinearWrapper:
+    """
+    Parameters
+    ----------
+        module (object): Module to be used.
+        name (str): Name of the layer.
+        prev_bn_name (str): Name of the previous BN layer.
+    """
 
     def __init__(self, module, name, prev_bn_name=None):
         self.module = copy.deepcopy(module)
         self.pruned_module: Linear = module
         self.name = name
         self.prev_bn_name = prev_bn_name
         self.is_pruned = False
@@ -149,14 +164,20 @@
         return {
             'name': self.name,
             'in_features_keep_idxes': self.in_features_keep_idxes,
         }
 
 
 class BN2dWrapper:
+    """
+    Parameters
+    ----------
+        module (object): Module to be used.
+        name (str): Name of the layer.
+    """
 
     def __init__(self, module: BatchNorm2d, name):
         self.module = copy.deepcopy(module)
         self.pruned_module = module
         self.name = name
         self.keep_idxes = None
         self.is_pruned = False
@@ -214,14 +235,21 @@
         return {'name': self.name, 'channels': str1, 'prune percent': str2}
 
     def prune_result(self):
         return {'name': self.name, 'keep_idxes': self.keep_idxes}
 
 
 class SlimPruner:
+    """
+    Parameters
+    ----------
+        model (object): Model to be used.
+        schema (str):
+    """
+
     PRUNING_RESULT_KEY = '_slim_pruning_result'
 
     def __init__(self, model, schema: str = None):
         """
 
         Args:
             model: Module will be modified inplace
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/prune/prune.py` & `trailmet-0.0.1rc2/trailmet/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,19 +15,23 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from ..algorithms import BaseAlgorithm
-
-
-class BasePruning(BaseAlgorithm):
-    """Base class for pruning algorithms."""
-
-    def __init__(self, **kwargs):
-        super(BasePruning, self).__init__(**kwargs)
-        pass
-
-    def prune(self, model, dataloaders, **kwargs):
-        pass
+from .functions import (
+    AverageMeter,
+    save_checkpoint,
+    accuracy,
+    seed_everything,
+    pdist,
+    CrossEntropyLabelSmooth,
+    adjust_learning_rate,
+    strlist_to_list,
+    get_optimizer,
+    lp_loss,
+    extract_sparsity,
+    chip_adjust_learning_rate,
+)
+from .benchmark import ModelBenchmark
+from .tp_pruning import TP_Prune
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/prune/pruner/__init__.py` & `trailmet-0.0.1rc2/trailmet/models/base_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,18 +15,30 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from .l1_pruner import Pruner as L1Pruner
-from .meta_pruner import MetaPruner
-from .reg_pruner import Pruner as RegPruner
+import torch.nn as nn
 
-# when new pruner implementation is added in the 'pruner' dir, update this dict to maintain minimal code change.
-# key: pruning method name, value: the corresponding pruner
-pruner_dict = {
-    'GReg-1': RegPruner,
-    'GReg-2': RegPruner,
-    'L1': L1Pruner,
-}
+
+class BaseModel(nn.Module):
+
+    def __init__(self):
+        super(BaseModel, self).__init__()
+        pass
+
+    def init_weights(self):
+        for m in self.modules():
+            if isinstance(m, nn.Conv2d):
+                nn.init.kaiming_normal_(m.weight,
+                                        mode='fan_out',
+                                        nonlinearity='relu')
+                if m.bias is not None:
+                    nn.init.constant_(m.bias, 0)
+            elif isinstance(m, nn.BatchNorm2d):
+                nn.init.constant_(m.weight, 1)
+                nn.init.constant_(m.bias, 0)
+            elif isinstance(m, nn.Linear):
+                nn.init.normal_(m.weight, 0, 0.01)
+                nn.init.constant_(m.bias, 0)
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/prune/pruner/l1_pruner.py` & `trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/l1_pruner.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,22 @@
 import time
 import numpy as np
 import logging
 from .meta_pruner import MetaPruner
 
 
 class Pruner(MetaPruner):
+    """
+    Parameters
+    ----------
+        model (object): A pytorch model you want to use.
+        args (object): Argument object
+        logger (object): Logger you want to use.
+        runner ():
+    """
 
     def __init__(self, model, args, logger, runner):
         super(Pruner, self).__init__(model, args, logger, runner)
         self.logger = logger
 
     def prune(self):
         self._get_kept_wg_L1()
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/prune/pruner/meta_pruner.py` & `trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/meta_pruner.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,22 @@
 from math import ceil
 from collections import OrderedDict
 import logging
 
 
 # +
 class Layer:
+    """
+    Parameters
+    ----------
+        name (str): Name of the layer
+        size (object): Argument object
+        layer_index (object): Logger you want to use.
+        runner ():
+    """
 
     def __init__(self, name, size, layer_index, res=False):
         self.name = name
         self.size = []
         for x in size:
             self.size.append(x)
         self.layer_index = layer_index
@@ -79,14 +87,22 @@
                 return stage, seq_ix, blk_ix
             except:
                 print('!Parsing the layer name failed: %s. Please check.' %
                       name)
 
 
 class MetaPruner:
+    """
+    Parameters
+    ----------
+        model (object): A pytorch model you want to use.
+        args (object): Argument object
+        logger (object): Logger you want to use.
+        passer ():
+    """
 
     def __init__(self, model, args, logger, passer):
         self.model = model
         self.args = args
         self.logger = logger
         self.test = lambda net: passer.test(passer.test_loader, net, passer.
                                             criterion, passer.args)
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/prune/pruner/reg_pruner.py` & `trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/reg_pruner.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,19 @@
 
 from ..pns import SlimPruner
 from ..utils import summary_model
 from trailmet.utils import save_checkpoint
 
 
 class LitModel(nn.Module):
+    """
+    Parameters
+    ----------
+        args (object): A yaml safe loaded file with information like arch, num_classes, etc.
+    """
 
     def __init__(self, args):
         super(LitModel, self).__init__()
         model = getattr(models, args['arch'])(num_classes=args['num_classes'])
         # to get better result on cifar10
         model.conv1 = torch.nn.Conv2d(3,
                                       64,
@@ -51,14 +56,22 @@
 
     def forward(self, x):
         return self.model(x)
 
 
 # +
 class Pruner(MetaPruner):
+    """
+    Parameters
+    ----------
+        model (object): A pytorch model you want to use.
+        args (object): Argument object
+        logger (object): Logger you want to use.
+        passer ():
+    """
 
     def __init__(self, model, args, logger, passer):
         super(Pruner, self).__init__(model, args, logger, passer)
 
         # Reg related variables
         self.reg = {}
         self.delta_reg = {}
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/prune/utils.py` & `trailmet-0.0.1rc2/trailmet/algorithms/prune/utils.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/quantize/__init__.py` & `trailmet-0.0.1rc2/trailmet/algorithms/quantize/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/quantize/bitsplit.py` & `trailmet-0.0.1rc2/trailmet/algorithms/quantize/bitsplit.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,20 @@
 
 def conv_hook(module, inputdata, outputdata):
     global conv_feat
     conv_feat = outputdata.data
 
 
 class QuantModel(nn.Module):
+    """
+    Parameters
+    ----------
+        model (nn.Module): Model to be used.
+        arch (str): Architecture to be used.
+    """
 
     def __init__(self, model: nn.Module, arch='ResNet50'):
         super().__init__()
         self.supported = {
             BasicBlock: QBasicBlock,
             Bottleneck: QBottleneck,
             InvertedResidual: QInvertedResidual,
@@ -100,24 +106,28 @@
 
 class BitSplit(BaseQuantization):
     """
     Class for post-training quantization using bit-split and stitching method
     based on - Towards accurate post-training network quantization via
     bit-split and stitching [https://dl.acm.org/doi/abs/10.5555/3524938.3525851]
 
-    :param W_BITS: bitwidth for weight quantization
-    :param A_BITS: bitwidth for activation quantization
-    :param CHANNEL_WISE: apply channel-wise quantization for weights
-    :param ACT_QUANT: apply activation quantization
-    :param HEAD_STEM_PRECISION: bitwidth for first and last layer
-    :param PREC_CONFIG: list of bitwidths of the body for mixed precision
-    :param CALIB_BATCHES: num of batches in calibration dataset
-    :param LOAD_ACT_SCALES: load precomputed weight scales
-    :param LOAD_WEIGHT_SCALES: load precomputed activation scales
-    :param SAVE_PATH: path for storing quantized weights and scales
+    Parameters
+    ----------
+    model (nn.Module): Model to be used
+    dataloaders (dict): Dictionary with dataloaders for train, test, val
+    W_BITS: bitwidth for weight quantization
+    A_BITS: bitwidth for activation quantization
+    CHANNEL_WISE: apply channel-wise quantization for weights
+    ACT_QUANT: apply activation quantization
+    HEAD_STEM_PRECISION: bitwidth for first and last layer
+    PREC_CONFIG: list of bitwidths of the body for mixed precision
+    CALIB_BATCHES: num of batches in calibration dataset
+    LOAD_ACT_SCALES: load precomputed weight scales
+    LOAD_WEIGHT_SCALES: load precomputed activation scales
+    SAVE_PATH: path for storing quantized weights and scales
     """
 
     def __init__(self, model: nn.Module, dataloaders, **kwargs):
         super(BitSplit, self).__init__(**kwargs)
         self.model = model
         self.train_loader = dataloaders['train']
         self.kwargs = kwargs
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/quantize/brecq.py` & `trailmet-0.0.1rc2/trailmet/algorithms/quantize/brecq.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,24 +65,28 @@
 
 class BRECQ(BaseQuantization):
     """
     Class for post-training quantization using block reconstruction method
     based on - BRECQ: PUSHING THE LIMIT OF POST-TRAINING QUANTIZATION
     BY BLOCK RECONSTRUCTION [https://arxiv.org/abs/2102.05426]
 
-    :param W_BITS: bitwidth for weight quantization
-    :param A_BITS: bitwidth for activation quantization
-    :param CHANNEL_WISE: apply channel_wise quantization for weights
-    :param ACT_QUANT: apply activation quantization
-    :param SET_8BIT_HEAD_STEM: Set the first and the last layer to 8-bit
-    :param NUM_SAMPLES: size of calibration dataset
-    :param WEIGHT: weight of rounding cost vs the reconstruction loss
-    :param ITERS_W: number of iteration for AdaRound
-    :param ITERS_A: number of iteration for LSQ
-    :param LR: learning rate for LSQ
+    Parameters
+    ----------
+    model (nn.Module): Model to be used
+    dataloaders (dict): Dictionary with dataloaders for train, test, val
+    W_BITS: bitwidth for weight quantization
+    A_BITS: bitwidth for activation quantization
+    CHANNEL_WISE: apply channel_wise quantization for weights
+    ACT_QUANT: apply activation quantization
+    SET_8BIT_HEAD_STEM: Set the first and the last layer to 8-bit
+    NUM_SAMPLES: size of calibration dataset
+    WEIGHT: weight of rounding cost vs the reconstruction loss
+    ITERS_W: number of iteration for AdaRound
+    ITERS_A: number of iteration for LSQ
+    LR: learning rate for LSQ
     """
 
     def __init__(self, model: nn.Module, dataloaders, **kwargs):
         super(BRECQ, self).__init__(**kwargs)
         self.model = copy.deepcopy(model)
         self.train_loader = dataloaders['train']
         self.test_loader = dataloaders['test']
@@ -348,18 +352,20 @@
         return losses.avg, top1.avg, top5.avg
 
 
 class QuantModel(nn.Module):
     """Recursively replace the normal conv2d and Linear layer to QuantModule,
     to enable calculating activation statistics and storing scaling factors.
 
-    :param module: nn.Module with nn.Conv2d or nn.Linear in its children
-    :param weight_quant_params: quantization parameters like n_bits for weight
+    Parameters
+    ----------
+    model (nn.Module): nn.Module with nn.Conv2d or nn.Linear in its children
+    weight_quant_params (dict): quantization parameters like n_bits for weight
         quantizer
-    :param act_quant_params: quantization parameters like n_bits for activation
+    act_quant_params(dict): quantization parameters like n_bits for activation
         quantizer
     """
 
     def __init__(
         self,
         model: nn.Module,
         weight_quant_params: dict = {},
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/quantize/lapq.py` & `trailmet-0.0.1rc2/trailmet/algorithms/quantize/lapq.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,14 +50,21 @@
 
 from trailmet.utils import AverageMeter, accuracy, save_checkpoint
 
 logger = logging.getLogger(__name__)
 
 
 class LAPQ(BaseQuantization):
+    """
+    Parameters
+    ----------
+    model (nn.Module): Model to be used
+    dataloaders (dict): Dictionary with dataloaders for train, test, val
+    kwargs (object): A yaml safe loaded file with information like W_BITS, A_BITS. CALIB_BATCHES, etc.
+    """
 
     def __init__(self, model: nn.Module, dataloaders, **kwargs):
         super(LAPQ, self).__init__(**kwargs)
         self.model = model
         self.train_loader = dataloaders['train']
         self.test_loader = dataloaders['test']
         self.kwargs = kwargs
@@ -337,14 +344,22 @@
                 output = model(images)
                 loss = criterion(output, target)
                 res += loss
             return res / len(self.cal_set)
 
 
 class QuantModel:
+    """
+    Parameters
+    ----------
+    model (nn.Module): Model to be used
+    args (object): A yaml safe loadec file with information like bit_weights, bit_act, etc.
+    quantizable_layers (list): A list of the quantizable layers.
+    optimizer_bridge ():
+    """
 
     def __init__(self, model, args, quantizable_layers, optimizer_bridge=None):
         self.model = model
         self.args = args
         self.bit_weights = args['bit_weights']
         self.bit_act = args['bit_act']
         self.post_relu = True
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/quantize/methods.py` & `trailmet-0.0.1rc2/trailmet/algorithms/quantize/methods.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,18 +63,20 @@
     """PyTorch Function that can be used for asymmetric quantization (uniform
     affine quantization).
 
     Quantizes its argument in the forward pass, passes the gradient 'straight
     through' on the backward pass, ignoring the quantization that occurred.
     Based on
     https://arxiv.org/abs/1806.08342.
-    :param n_bits: number of bit for quantization
-    :param symmetric: if True, the zero_point should always be 0
-    :param channel_wise: if True, compute scale and zero_point in each channel
-    :param scale_method: determines the quantization scale and zero point
+    Parameters
+    ----------
+    n_bits: number of bit for quantization
+    symmetric: if True, the zero_point should always be 0
+    channel_wise: if True, compute scale and zero_point in each channel
+    scale_method: determines the quantization scale and zero point
     """
 
     def __init__(
         self,
         n_bits: int = 8,
         symmetric: bool = False,
         channel_wise: bool = False,
@@ -201,19 +203,20 @@
 
 class AdaRoundQuantizer(nn.Module):
     """Adaptive Rounding Quantizer, used to optimize the rounding policy by
     reconstructing the intermediate output.
 
     Based on Up or Down? Adaptive Rounding for Post-Training Quantization:
     https://arxiv.org/abs/2004.10568
-    : https: //arxiv.org/abs/2004.10568
-    :param uaq: UniformAffineQuantizer, used to initialize quantization
-        parameters in this quantizer
-    :param round_mode: controls the forward pass in this quantizer
-    :param weight_tensor: initialize alpha
+    https: //arxiv.org/abs/2004.10568
+    Parameters
+    ----------
+    uaq: UniformAffineQuantizer, used to initialize quantization parameters in this quantizer
+    round_mode: controls the forward pass in this quantizer
+    weight_tensor: initialize alpha
     """
 
     def __init__(
         self,
         uaq: UniformAffineQuantizer,
         weight_tensor: torch.Tensor,
         round_mode='learned_round_sigmoid',
@@ -275,14 +278,20 @@
                 (rest - self.gamma) - 1)  # => sigmoid(alpha) = rest
             self.alpha = nn.Parameter(alpha)
         else:
             raise NotImplementedError
 
 
 class BitSplitQuantizer(object):
+    """
+    Parameters
+    ----------
+    W (np.ndarray): Weight vector
+    bitwidth (int): bitwidth to be used
+    """
 
     def __init__(self, W: np.ndarray, bitwidth):
         self.W = W
         self.bitwidth = bitwidth
 
     @staticmethod
     def splitWeightInteger(Q, bitwidth):
@@ -475,14 +484,20 @@
 
         B_sum = self.stitch(B_sav)
 
         return B_sum, alpha
 
 
 class ActQuantizer(nn.Module):
+    """
+    Parameters
+    ----------
+    islinear (bool):
+    bit_width (int): bit width to be used
+    """
 
     def __init__(self, islinear=False, bit_width=8):
         super(ActQuantizer, self).__init__()
         # self.scale = None
         self.in_scale = None
         self.out_scale = None
         self.signed = islinear
@@ -546,14 +561,20 @@
             self.out_scale = self.out_scale.to(x.device)
         # return torch.clamp(torch.round(x/self.in_scale), self.min_val, self.max_val) * self.out_scale
         return (torch.clamp(RoundSTE.apply(x / self.in_scale), self.min_val,
                             self.max_val) * self.out_scale)
 
 
 class QuantizationBase(object):
+    """
+    Parameters
+    ----------
+    module (object): Module to be used
+    num_bits (int): Number of bits to be used
+    """
 
     def __init__(self, module, num_bits):
         self.module = module
         self.num_bits = num_bits
         self.num_bins = int(2**num_bits)
         self.opt_params = {}
         self.named_params = []
@@ -591,14 +612,24 @@
 
     @staticmethod
     def learned_parameters():
         return []
 
 
 class UniformQuantization(QuantizationBase):
+    """
+    Parameters
+    ----------
+    module (object): Module to be used
+    num_bits (int): Number of bits to be used
+    symmetric (bool): Whether the distribution is symmetric or not
+    uint (bool):
+    stochastic (bool): if True, stochastic rounding will be done
+    tails (bool):
+    """
 
     def __init__(self,
                  module,
                  num_bits,
                  symmetric,
                  uint=False,
                  stochastic=False,
@@ -676,14 +707,25 @@
         s = '{} - ['.format(type(self).__name__)
         for name, value in self.__for_repr__():
             s += '{}: {}, '.format(name, value)
         return s + ']'
 
 
 class ClippedUniformQuantization(UniformQuantization):
+    """
+    Parameters
+    ----------
+    module (object): Module to be used
+    num_bits (int): Number of bits to be used
+    symmetric (bool): Whether the distribution is symmetric or not
+    uint (bool):
+    stochastic (bool): if True, stochastic rounding will be done
+    tails (bool):
+    """
+
     alpha_param_name = 'alpha'
 
     def __init__(self,
                  module,
                  num_bits,
                  symmetric,
                  uint=False,
@@ -702,14 +744,25 @@
         return [(
             self.alpha_param_name,
             '{:.4f}'.format(getattr(self, self.alpha_param_name).item()),
         )] + rpr
 
 
 class FixedClipValueQuantization(ClippedUniformQuantization):
+    """
+    Parameters
+    ----------
+    module (object): Module to be used
+    num_bits (int): Number of bits to be used
+    symmetric (bool): Whether the distribution is symmetric or not
+    uint (bool):
+    stochastic (bool): if True, stochastic rounding will be done
+    tails (bool):
+    kwargs (object): A yaml safe loaded file with information like clip_value, device.
+    """
 
     def __init__(self,
                  module,
                  num_bits,
                  symmetric,
                  uint=False,
                  stochastic=False,
@@ -723,14 +776,24 @@
                 self.alpha_param_name,
                 torch.tensor([self.clip_value],
                              dtype=torch.float32).to(self.device),
             )
 
 
 class MaxAbsStaticQuantization(ClippedUniformQuantization):
+    """
+    Parameters
+    ----------
+    module (object): Module to be used
+    tensor (torch.Tensor): Tensor which wpuld be quantized
+    num_bits (int): Number of bits to be used
+    symmetric (bool): Whether the distribution is symmetric or not
+    uint (bool):
+    stochastic (bool): if True, stochastic rounding will be done
+    """
 
     def __init__(
         self,
         module,
         tensor,
         num_bits,
         symmetric,
@@ -743,14 +806,24 @@
 
         with torch.no_grad():
             self.register_buffer(self.alpha_param_name,
                                  tensor.new_tensor([tensor.abs().max()]))
 
 
 class LearnedStepSizeQuantization(ClippedUniformQuantization):
+    """
+    Parameters
+    ----------
+    module (object): Module to be used
+    tensor (torch.Tensor): Tensor which wpuld be quantized
+    num_bits (int): Number of bits to be used
+    symmetric (bool): Whether the distribution is symmetric or not
+    uint (bool):
+    stochastic (bool): if True, stochastic rounding will be done
+    """
 
     def __init__(self,
                  module,
                  tensor,
                  num_bits,
                  symmetric,
                  uint=False,
@@ -798,14 +871,26 @@
 
     @staticmethod
     def learned_parameters():
         return [LearnedStepSizeQuantization.alpha_param_name]
 
 
 class LpNormQuantization(ClippedUniformQuantization):
+    """
+    Parameters
+    ----------
+    module (object): Module to be used
+    tensor (torch.Tensor): Tensor which wpuld be quantized
+    num_bits (int): Number of bits to be used
+    symmetric (bool): Whether the distribution is symmetric or not
+    uint (bool):
+    stochastic (bool): if True, stochastic rounding will be done
+    tails (bool):
+    kwargs (object): A yaml safe loaded file with information like lp
+    """
 
     def __init__(
         self,
         module,
         tensor,
         num_bits,
         symmetric,
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/quantize/qmodel.py` & `trailmet-0.0.1rc2/trailmet/algorithms/quantize/qmodel.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,14 +58,22 @@
 
 
 class QuantModule(nn.Module):
     """Quantized Module that can perform quantized convolution or normal
     convolution.
 
     To activate quantization, please use set_quant_state function.
+
+    Parameters
+    ----------
+    org_module (nn.Module): Module to be used
+    weight_quant_params (dict): Weight parameters
+    act_quant_params (dict): Activation Parameters
+    disable_act_quant (bool): if True, activation layer will be disabled
+    se_module (nn.Module): SE Module to be used
     """
 
     def __init__(
         self,
         org_module: Union[nn.Conv2d, nn.Linear],
         weight_quant_params: dict = {},
         act_quant_params: dict = {},
@@ -134,14 +142,18 @@
 
 class BaseQuantBlock(nn.Module):
     """Base implementation of block structures for all networks.
 
     Due to the branch architecture, we have to perform activation function and
     quantization after the elemental-wise add operation, therefore, we put this
     part in this class.
+
+    Parameters
+    ----------
+    act_quant_params (dict): Activation parameters
     """
 
     def __init__(self, act_quant_params: dict = {}):
         super().__init__()
         self.use_weight_quant = False
         self.use_act_quant = False
         # initialize quantizer
@@ -159,16 +171,22 @@
         self.use_act_quant = act_quant
         for m in self.modules():
             if isinstance(m, QuantModule):
                 m.set_quant_state(weight_quant, act_quant)
 
 
 class QuantBasicBlock(BaseQuantBlock):
-    """Implementation of Quantized BasicBlock used in ResNet-18 and
-    ResNet-34."""
+    """Implementation of Quantized BasicBlock used in ResNet-18 and ResNet-34.
+
+    Parameters
+    ----------
+    basic_block (object): BasicBlock which is to be used
+    weight_quant_params (dict): Weight parameters
+    act_quant_params (dict): Activation Parameters
+    """
 
     def __init__(
         self,
         basic_block: BasicBlock,
         weight_quant_params: dict = {},
         act_quant_params: dict = {},
     ):
@@ -206,16 +224,24 @@
         out = self.activation_function(out)
         if self.use_act_quant:
             out = self.act_quantizer(out)
         return out
 
 
 class QuantBottleneck(BaseQuantBlock):
-    """Implementation of Quantized Bottleneck Block used in ResNet-50, -101 and
-    -152."""
+    """
+    Implementation of Quantized Bottleneck Block used in ResNet-50, -101 and
+    -152.
+
+    Parameters
+    ----------
+    bottleneck (object): Bottleneck to be used
+    weight_quant_params (dict): Weight parameters
+    act_quant_params (dict): Activation Parameters
+    """
 
     def __init__(
         self,
         bottleneck: Bottleneck,
         weight_quant_params: dict = {},
         act_quant_params: dict = {},
     ):
@@ -260,14 +286,20 @@
         return out
 
 
 class QuantInvertedResidual(BaseQuantBlock):
     """Implementation of Quantized Inverted Residual Block used in MobileNetV2.
 
     Inverted Residual does not have activation function.
+
+    Parameters
+    ----------
+    inv_res (object): Inverted Residual block to be used
+    weight_quant_params (dict): Weight parameters
+    act_quant_params (dict): Activation Parameters
     """
 
     def __init__(
         self,
         inv_res: InvertedResidual,
         weight_quant_params: dict = {},
         act_quant_params: dict = {},
@@ -331,14 +363,20 @@
     - BasicBlock(nn.Module) -> QBasicBlock(nn.Module)
     - Bottleneck(nn.Module) -> QBottleneck(nn.Module)
     - InvertedResidual(nn.Module) -> QInvertedResidual(nn.Module)
 """
 
 
 class QBasicBlock(nn.Module):
+    """
+    Parameters
+    ----------
+    basic_block (object): BasicBlock which is to be used
+    """
+
     expansion = 1
 
     def __init__(self, basic_block: BasicBlock):
         super().__init__()
         self.quant1 = ActQuantizer()
         self.conv1 = basic_block.conv1
         self.bn1 = basic_block.bn1
@@ -359,14 +397,20 @@
             residual = self.downsample(x)
         out += residual
         out = self.active(out)
         return out
 
 
 class QBottleneck(nn.Module):
+    """
+    Parameters
+    ----------
+    bottleneck (object): Bottleneck to be used
+    """
+
     expansion = 4
 
     def __init__(self, bottleneck: Bottleneck):
         super().__init__()
         self.quant1 = ActQuantizer()
         self.conv1 = bottleneck.conv1
         self.bn1 = bottleneck.bn1
@@ -392,14 +436,19 @@
             residual = self.downsample(x)
         out += residual
         out = self.active(out)
         return out
 
 
 class QInvertedResidual(nn.Module):
+    """
+    Parameters
+    ----------
+    inv_res (object): Inverted Residual block to be used
+    """
 
     def __init__(self, inv_res: InvertedResidual):
         super().__init__()
         self.stride = inv_res.stride
         self.inp = inv_res.inp
         self.oup = inv_res.oup
         self.exp = inv_res.exp
@@ -441,14 +490,21 @@
 
 
 def is_positive(module):
     return isinstance(module, nn.ReLU) or isinstance(module, nn.ReLU6)
 
 
 class ActivationModuleWrapper(nn.Module):
+    """
+    Parameters
+    ----------
+    name (str): Name of the wrapped module
+    wrapped_module (object): Module to be used
+    kwargs (object): A yaml safe loaded file with information like bits_out and qtype
+    """
 
     def __init__(self, name, wrapped_module, **kwargs):
         super(ActivationModuleWrapper, self).__init__()
         self.name = name
         self.wrapped_module = wrapped_module
         self.bits_out = kwargs['bits_out']
         self.qtype = kwargs['qtype']
@@ -508,14 +564,21 @@
             symmetric=(not is_positive(self.wrapped_module)),
             uint=True,
             kwargs=kwargs,
         )
 
 
 class ParameterModuleWrapper(nn.Module):
+    """
+    Parameters
+    ----------
+    name (str): Name of the wrapped module
+    wrapped_module (object): Module to be used
+    kwargs (object): A yaml safe loaded file with information like bits_out, qtype, forward functor, bit_weight, etc.
+    """
 
     def __init__(self, name, wrapped_module, **kwargs):
         super(ParameterModuleWrapper, self).__init__()
         self.name = name
         self.wrapped_module = wrapped_module
         self.forward_functor = kwargs['forward_functor']
         self.bit_weights = kwargs['bit_weights']
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/quantize/quantize.py` & `trailmet-0.0.1rc2/trailmet/algorithms/quantize/quantize.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/quantize/reconstruct.py` & `trailmet-0.0.1rc2/trailmet/algorithms/quantize/reconstruct.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,15 +60,22 @@
 class StopForwardException(Exception):
     """Used to throw and catch an exception to stop traversing the graph."""
 
     pass
 
 
 class DataSaverHook:
-    """Forward hook that stores the input and output of a layer."""
+    """Forward hook that stores the input and output of a layer.
+
+    Parameters
+    ----------
+    store_input (bool): If True, input of a layer will be saved, default=False
+    store_output (bool): If True, output of a layer will be saved, default=False
+    stop_forward (bool): If True, forward prop will be stopped, default=False.
+    """
 
     def __init__(self,
                  store_input=False,
                  store_output=False,
                  stop_forward=False):
         self.store_input = store_input
         self.store_output = store_output
@@ -85,21 +92,19 @@
         if self.stop_forward:
             raise StopForwardException
 
 
 class GetLayerInpOut:
     """Get the input and output of a specified layer in a quantized model.
 
-    :param model: quantized model for which the input and output needs to be
-        extracted.
-    :param layer: the layer for which input and output needs to be extracted.
-    :param device: the device on which the computation needs to be performed.
-    :param asym: save quantized input and full precision output.
-        [default=False]
-    :param act_quant: use activation quantization. [default=False]
+    model: quantized model for which the input and output needs to be extracted.
+    layer: the layer for which input and output needs to be extracted.
+    device: the device on which the computation needs to be performed.
+    asym: save quantized input and full precision output. [default=False]
+    act_quant: use activation quantization. [default=False]
     """
 
     def __init__(
         self,
         model,
         layer: Union[QuantModule, BaseQuantBlock],
         device: torch.device,
@@ -113,16 +118,18 @@
         self.act_quant = act_quant
         self.data_saver = DataSaverHook(store_input=True,
                                         store_output=True,
                                         stop_forward=True)
 
     def __call__(self, model_input):
         """
-        :param model_input: calibration data samples
-        :return: tuple of layer input and output
+        Parameters
+        ----------
+        model_input: calibration data samples
+        return: tuple of layer input and output
         """
         self.model.eval()
         self.model.set_quant_state(False, False)
 
         handle = self.layer.register_forward_hook(self.data_saver)
         with torch.no_grad():
             try:
@@ -160,24 +167,23 @@
     act_quant: bool = False,
     batch_size: int = 32,
     keep_gpu: bool = True,
 ):
     """Function to save input data and output data of a particular layer/block
     over calibration dataset.
 
-    :param model: quantized model for which the input and output needs to be
-        extracted.
-    :param layer: the layer for which input and output needs to be extracted.
-    :param cali_data: calibration dataset
-    :param asym: save quantized input and full precision output.
-        [default=False]
-    :param act_quant: use activation quantization. [default=False]
-    :param batch_size: mini-batch size for calibration. [default=32]
-    :param keep_gpu: put saved data on GPU for faster optimization.
-        [default=True]
+    Parameters
+    ----------
+    model: quantized model for which the input and output needs to be extracted.
+    layer: the layer for which input and output needs to be extracted.
+    cali_data: calibration dataset
+    asym: save quantized input and full precision output. [default=False]
+    act_quant: use activation quantization. [default=False]
+    batch_size: mini-batch size for calibration. [default=32]
+    keep_gpu: put saved data on GPU for faster optimization. [default=True]
     :return: input and output data
     """
     device = next(model.parameters()).device
     get_inp_out = GetLayerInpOut(model,
                                  layer,
                                  device=device,
                                  asym=asym,
@@ -196,15 +202,20 @@
     if keep_gpu:
         cached_inps = cached_inps.to(device)
         cached_outs = cached_outs.to(device)
     return cached_inps, cached_outs
 
 
 class GradSaverHook:
-    """Backward hook that stores the gradients of a layer."""
+    """Backward hook that stores the gradients of a layer.
+
+    Parameters
+    ----------
+    store_grad (bool): if True, gradient of the layer will be stored
+    """
 
     def __init__(self, store_grad=True):
         self.store_grad = store_grad
         self.stop_backward = False
         self.grad_out = None
 
     def __call__(self, module, grad_input, grad_output):
@@ -213,21 +224,21 @@
         if self.stop_backward:
             raise StopForwardException
 
 
 class GetLayerGrad:
     """Get the gradient a specified layer in a quantized model.
 
-    :param model: quantized model for which the input and output needs to be
-        extracted.
-    :param layer: the layer for which input and output needs to be extracted.
-    :param device: the device on which the computation needs to be performed.
-    :param asym: if True, save quantized input and full precision output.
-        [default=False]
-    :param act_quant: use activation quantization. [default=False]
+    Parameters
+    ----------
+    model: quantized model for which the input and output needs to be extracted.
+    layer: the layer for which input and output needs to be extracted.
+    device: the device on which the computation needs to be performed.
+    asym: if True, save quantized input and full precision output. [default=False]
+    act_quant: use activation quantization. [default=False]
     """
 
     def __init__(
         self,
         model,
         layer: Union[QuantModule, BaseQuantBlock],
         device: torch.device,
@@ -239,15 +250,17 @@
         self.act_quant = act_quant
         self.data_saver = GradSaverHook(True)
 
     def __call__(self, model_input):
         """Compute the gradients of layer output, note that we compute the
         gradient by calculating the KL loss between fp model and quant model.
 
-        :param model_input: calibration data samples
+        Parameters
+        ----------
+        model_input: calibration data samples
         :return: gradients for the layer
         """
         self.model.eval()
 
         handle = self.layer.register_backward_hook(self.data_saver)
         with torch.enable_grad():
             try:
@@ -281,24 +294,23 @@
     act_quant: bool = False,
     batch_size: int = 32,
     keep_gpu: bool = True,
 ):
     """Function to save gradient data of a particular layer/block over
     calibration dataset.
 
-    :param model: quantized model for which the input and output needs to be
-        extracted.
-    :param layer: the layer for which input and output needs to be extracted.
-    :param cali_data: calibration dataset
-    :param damping: damping the second-order gradient by adding some constant
-        in the FIM diagonal
-    :param act_quant: use activation quantization. [default=False]
-    :param batch_size: mini-batch size for calibration. [default=32]
-    :param keep_gpu: put saved data on GPU for faster optimization.
-        [default=True]
+    Parameters
+    ----------
+    model: quantized model for which the input and output needs to be extracted.
+    layer: the layer for which input and output needs to be extracted.
+    cali_data: calibration dataset
+    damping: damping the second-order gradient by adding some constant in the FIM diagonal
+    act_quant: use activation quantization. [default=False]
+    batch_size: mini-batch size for calibration. [default=32]
+    keep_gpu: put saved data on GPU for faster optimization. [default=True]
     :return: gradient data
     """
     device = next(model.parameters()).device
     get_grad = GetLayerGrad(model, layer, device, act_quant=act_quant)
     cached_batches = []
     torch.cuda.empty_cache()
 
@@ -321,19 +333,20 @@
 # ================================
 
 
 class LinearTempDecay:
     """Class to implement a linear temperature decay scheduler for a given
     maximum time step.
 
-    :param t_max: maximum number of time steps to decay temperature over.
-    :param rel_start_decay: relative point in time to start the decay from the
-        maximum time step. [default=.2]
-    :param start_b: initial temperature value. [default=10]
-    :param end_b: final temperature value. [default=2]
+    Parameters
+    ----------
+    t_max: maximum number of time steps to decay temperature over.
+    rel_start_decay: relative point in time to start the decay from the maximum time step. [default=.2]
+    start_b: initial temperature value. [default=10]
+    end_b: final temperature value. [default=2]
     """
 
     def __init__(
         self,
         t_max: int,
         rel_start_decay: float = 0.2,
         start_b: int = 10,
@@ -343,26 +356,41 @@
         self.start_decay = rel_start_decay * t_max
         self.start_b = start_b
         self.end_b = end_b
 
     def __call__(self, t):
         """Cosine annealing scheduler for temperature b.
 
-        :param t: the current time step
+        Parameters
+        ----------
+        t: the current time step
         :return: scheduled temperature
         """
         if t < self.start_decay:
             return self.start_b
         else:
             rel_t = (t - self.start_decay) / (self.t_max - self.start_decay)
             return self.end_b + (self.start_b - self.end_b) * max(
                 0.0, (1 - rel_t))
 
 
 class LayerLossFunction:
+    """
+    Parameters
+    ----------
+    layer (object): layer to be quantized
+    Round_loss (str): type of regularization term used to optimize rounding policy (options: relaxation, none)
+    Weight (float): weight of rounding loss in total loss
+    Rec_loss (str): type of output reconstruction loss (options: mse, fisher_diag, fisher_full)
+    max_count (int): number of iterations
+    b_range (tuple): range of rounding relaxation factor (b) with linear temp decay scheduler
+    decay_start (float): starting point for temp decay of b
+    warmup (float): fraction of iterations used for warmup before applying rounding loss
+    p (float): power in lp-norm computation of reconstruction loss
+    """
 
     def __init__(
         self,
         layer: QuantModule,
         round_loss: str = 'relaxation',
         weight: float = 1.0,
         rec_loss: str = 'mse',
@@ -394,17 +422,20 @@
         )
 
     def __call__(self, pred, tgt, grad=None):
         """
         Compute the total loss for adaptive rounding:
         rec_loss is the quadratic output reconstruction loss, round_loss is
         a regularization term to optimize the rounding policy
-        :param pred: output from quantized model
-        :param tgt: output from FP model
-        :param grad: gradients to compute fisher information
+
+        Parameters
+        ----------
+        pred: output from quantized model
+        tgt: output from FP model
+        grad: gradients to compute fisher information
         :return: total loss function
         """
         self.count += 1
         if self.rec_loss == 'mse':
             rec_loss = lp_loss(pred, tgt, p=self.p)
         elif self.rec_loss == 'fisher_diag':
             rec_loss = ((pred - tgt).pow(2) * grad.pow(2)).sum(1).mean()
@@ -456,32 +487,31 @@
     lr: float = 4e-5,
     p: float = 2.0,
     multi_gpu: bool = False,
     optim='adam',
 ):
     """Block reconstruction to optimize the output from each layer.
 
-    :param model: QuantModel
-    :param layer: QuantModule that needs to be optimized
-    :param cali_data: data for calibration, typically 1024 training images, as
-        described in AdaRound
-    :param batch_size: mini-batch size for reconstruction
-    :param iters: optimization iterations for reconstruction,
-    :param weight: the weight of rounding regularization term
-    :param opt_mode: optimization mode
-    :param asym: asymmetric optimization designed in AdaRound, use quant input
-        to reconstruct fp output
-    :param include_act_func: optimize the output after activation function
-    :param b_range: temperature range
-    :param warmup: proportion of iterations that no scheduling for temperature
-    :param act_quant: use activation quantization or not.
-    :param lr: learning rate for act delta learning
-    :param p: L_p norm minimization
-    :param multi_gpu: use multi-GPU or not, if enabled, we should sync the
-        gradients
+    Parameters
+    ----------
+    model: QuantModel
+    layer: QuantModule that needs to be optimized
+    cali_data: data for calibration, typically 1024 training images, as described in AdaRound
+    batch_size: mini-batch size for reconstruction
+    iters: optimization iterations for reconstruction,
+    weight: the weight of rounding regularization term
+    opt_mode: optimization mode
+    asym: asymmetric optimization designed in AdaRound, use quant input to reconstruct fp output
+    include_act_func: optimize the output after activation function
+    b_range: temperature range
+    warmup: proportion of iterations that no scheduling for temperature
+    act_quant: use activation quantization or not.
+    lr: learning rate for act delta learning
+    p: L_p norm minimization
+    multi_gpu: use multi-GPU or not, if enabled, we should sync the gradients
     """
 
     model.set_quant_state(False, False)
     layer.set_quant_state(True, act_quant)
     round_mode = 'learned_hard_sigmoid'
 
     if not include_act_func:
@@ -566,14 +596,27 @@
 
 # =================================
 # ******* Reconstruct Block *******
 # =================================
 
 
 class BlockLossFunction:
+    """
+    Parameters
+    ----------
+    Module (object): module or block being quantized
+    Round_loss (str): type of regularization term used to optimize rounding policy (options: relaxation, none)
+    Weight (float): weight of rounding loss in total loss
+    Rec_loss (str): type of output reconstruction loss (options: mse, fisher_diag, fisher_full)
+    max_count (int): number of iterations
+    b_range (tuple): range of rounding relaxation factor (b) with linear temp decay scheduler
+    decay_start (float): starting point for temp decay of b
+    warmup (float): fraction of iterations used for warmup before applying rounding loss
+    p (float): power in lp-norm computation of reconstruction loss
+    """
 
     def __init__(
         self,
         block: BaseQuantBlock,
         round_loss: str = 'relaxation',
         weight: float = 1.0,
         rec_loss: str = 'mse',
@@ -605,17 +648,20 @@
         )
 
     def __call__(self, pred, tgt, grad=None):
         """
         Compute the total loss for adaptive rounding:
         rec_loss is the quadratic output reconstruction loss, round_loss is
         a regularization term to optimize the rounding policy
-        :param pred: output from quantized model
-        :param tgt: output from FP model
-        :param grad: gradients to compute fisher information
+
+        Parameters
+        ----------
+        pred: output from quantized model
+        tgt: output from FP model
+        grad: gradients to compute fisher information
         :return: total loss function
         """
         self.count += 1
         if self.rec_loss == 'mse':
             rec_loss = lp_loss(pred, tgt, p=self.p)
         elif self.rec_loss == 'fisher_diag':
             rec_loss = ((pred - tgt).pow(2) * grad.pow(2)).sum(1).mean()
@@ -668,32 +714,31 @@
     lr: float = 4e-5,
     p: float = 2.0,
     multi_gpu: bool = False,
     optim='adam',
 ):
     """Block reconstruction to optimize the output from each block.
 
-    :param model: QuantModel
-    :param block: BaseQuantBlock that needs to be optimized
-    :param cali_data: data for calibration, typically 1024 training images, as
-        described in AdaRound
-    :param batch_size: mini-batch size for reconstruction
-    :param iters: optimization iterations for reconstruction,
-    :param weight: the weight of rounding regularization term
-    :param opt_mode: optimization mode
-    :param asym: asymmetric optimization designed in AdaRound, use quant input
-        to reconstruct fp output
-    :param include_act_func: optimize the output after activation function
-    :param b_range: temperature range
-    :param warmup: proportion of iterations that no scheduling for temperature
-    :param act_quant: use activation quantization or not.
-    :param lr: learning rate for act delta learning
-    :param p: L_p norm minimization
-    :param multi_gpu: use multi-GPU or not, if enabled, we should sync the
-        gradients
+    Parameters
+    ----------
+    model: QuantModel
+    block: BaseQuantBlock that needs to be optimized
+    cali_data: data for calibration, typically 1024 training images, as described in AdaRound
+    batch_size: mini-batch size for reconstruction
+    iters: optimization iterations for reconstruction,
+    weight: the weight of rounding regularization term
+    opt_mode: optimization mode
+    asym: asymmetric optimization designed in AdaRound, use quant input to reconstruct fp output
+    include_act_func: optimize the output after activation function
+    b_range: temperature range
+    warmup: proportion of iterations that no scheduling for temperature
+    act_quant: use activation quantization or not.
+    lr: learning rate for act delta learning
+    p: L_p norm minimization
+    multi_gpu: use multi-GPU or not, if enabled, we should sync the gradients
     """
     model.set_quant_state(False, False)
     block.set_quant_state(True, act_quant)
     round_mode = 'learned_hard_sigmoid'
 
     if not include_act_func:
         org_act_func = block.activation_function
```

### Comparing `trailmet-0.0.1rc0/trailmet/algorithms/utils/__init__.py` & `trailmet-0.0.1rc2/trailmet/algorithms/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,21 @@
     full_path = glob.glob('Experiments/*%s*' % ExpID)
     assert (len(full_path) == 1
             )  # There should be only ONE folder with <ExpID> in its name.
     return full_path[0]
 
 
 class LogPrinter(object):
+    """
+    Parameters
+    ----------
+        file (object): .
+        ExpID (str): Experiment ID for the logger.
+        print_to_screen (bool): Whether to print to screen or not.
+    """
 
     def __init__(self, file, ExpID, print_to_screen=False):
         self.file = file
         self.ExpID = ExpID
         self.print_to_screen = print_to_screen
 
     def __call__(self, *in_str):
@@ -103,14 +110,19 @@
         for k_ in sorted(key_map.keys()):
             real_key = key_map[k_]
             logtmp += "('%s': %s) " % (real_key, args.__dict__[real_key])
         self.print(logtmp[:-1] + '\n')  # the last one is blank
 
 
 class LogTracker(object):
+    """
+    Parameters
+    ----------
+        momentum (float): Momentum to be used, default=0.9.
+    """
 
     def __init__(self, momentum=0.9):
         self.loss = OrderedDict()
         self.momentum = momentum
         self.show = OrderedDict()
 
     def __call__(self, name, value, step=-1, show=True):
@@ -510,15 +522,20 @@
     return args
 
 
 # -
 
 
 class PresetLRScheduler(object):
-    """Using a manually designed learning rate schedule rules."""
+    """Using a manually designed learning rate schedule rules.
+
+    Parameters
+    ----------
+        decay_schedule (dict): Decay schedule for the LR.
+    """
 
     def __init__(self, decay_schedule):
         # decay_schedule is a dictionary
         # which is for specifying iteration -> lr
         self.decay_schedule = {}
         for (
                 k,
```

### Comparing `trailmet-0.0.1rc0/trailmet/datasets/classification/__init__.py` & `trailmet-0.0.1rc2/trailmet/datasets/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/datasets/classification/chest.py` & `trailmet-0.0.1rc2/trailmet/datasets/classification/chest.py`

 * *Files 7% similar despite different names*

```diff
@@ -147,14 +147,45 @@
         elif self._mode == 'heatmap':
             return (image, path, label)
         else:
             raise Exception('Unknown mode : {}'.format(self._mode))
 
 
 class ChestDataset(BaseDataset):
+    """
+    `CheXpert <https://stanfordmlgroup.github.io/competitions/chexpert/>`_ Dataset.
+    The CheXpert dataset contains 224,316 chest radiographs of 65,240 patients with both frontal and lateral views available. The task is to do automated chest x-ray interpretation, featuring uncertainty labels and radiologist-labeled reference standard evaluation sets.
+
+    References
+    ----------
+    CheXpert: A Large Chest Radiograph Dataset with Uncertainty Labels and Expert Comparison,
+    Irvin et al, 2019.
+
+    Parameters
+    ----------
+        name (string): dataset name 'CHEST', default=None.
+        root (string): Root directory where ``train, train.csv`` exists or will be saved if download flag is set to
+        True (default is None).
+        train (bool, optional): If True, creates dataset from training set, otherwise
+            creates from test set, default=None.
+        transform (callable, optional): A function/transform that takes in an PIL image
+            and returns a transformed version. E.g, ``transforms.RandomCrop``. Default=None.
+        target_transform (callable, optional): A function/transform that takes in the
+            target and transforms it, default=None.
+        download (bool, optional): If true, downloads the dataset from the internet and
+            puts it in root directory. If dataset is already downloaded, it is not
+            downloaded again, default=True.
+        split_types (list): the possible values of this parameter are "train", "test" and "val".
+            If the split_type contains "val", then shuffle has to be True, default value is None.
+        val_fraction (float): If float, should be between 0.0 and 1.0 and represent
+        the proportion of the dataset to include in the val split.
+        shuffle (bool): Whether or not to shuffle the data before splitting into val from train,
+            default is True. If shuffle is true, there should be 'val' in split_types.
+        random_seed (int): RandomState instance, default=None.
+    """
 
     def __init__(
         self,
         name=None,
         root=None,
         transform=None,
         subname='atelectasis',
```

### Comparing `trailmet-0.0.1rc0/trailmet/datasets/classification/cifar.py` & `trailmet-0.0.1rc2/trailmet/datasets/classification/cifar.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/datasets/classification/dataset.py` & `trailmet-0.0.1rc2/trailmet/datasets/classification/dataset.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/datasets/classification/imagenet.py` & `trailmet-0.0.1rc2/trailmet/datasets/classification/imagenet.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/datasets/classification/tcga.py` & `trailmet-0.0.1rc2/trailmet/datasets/classification/tcga.py`

 * *Files 6% similar despite different names*

```diff
@@ -139,14 +139,43 @@
             img = Image.open(image_path).convert('RGB')
             img = self.target_transform(img)
             class_name = self.labels_dict[path]
             return img, torch.tensor([self.class_dict[class_name]])
 
 
 class TCGADataset(BaseDataset):
+    """
+    `TCGA <https://www.cancer.gov/ccg/research/structural-genomics/tcga/studied-cancers/lung-squamous-cell-carcinoma-study>`_ Dataset.
+
+    References
+    ----------
+
+
+    Parameters
+    ----------
+        name (string): dataset name 'TCGA', default=None.
+        root (string): Root directory where ``splits, images`` exists or will be saved if download flag is set to True (default is None).
+        train (bool, optional): If True, creates dataset from training set, otherwise
+            creates from test set, default=None.
+        transform (callable, optional): A function/transform that takes in an PIL image
+            and returns a transformed version. E.g, ``transforms.RandomCrop``. Default=None.
+        target_transform (callable, optional): A function/transform that takes in the
+            target and transforms it, default=None.
+        kfold (int): The fold which you want to use. Possible values are 0-9
+        download (bool, optional): If true, downloads the dataset from the internet and
+            puts it in root directory. If dataset is already downloaded, it is not
+            downloaded again, default=True.
+        split_types (list): the possible values of this parameter are "train", "test" and "val".
+            If the split_type contains "val", then shuffle has to be True, default value is None.
+        val_fraction (float): If float, should be between 0.0 and 1.0 and represent
+        the proportion of the dataset to include in the val split.
+        shuffle (bool): Whether or not to shuffle the data before splitting into val from train,
+            default is True. If shuffle is true, there should be 'val' in split_types.
+        random_seed (int): RandomState instance, default=None.
+    """
 
     def __init__(
         self,
         name=None,
         root=None,
         transform=None,
         target_transform=None,
```

### Comparing `trailmet-0.0.1rc0/trailmet/models/__init__.py` & `trailmet-0.0.1rc2/trailmet/models/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/models/mobilenet.py` & `trailmet-0.0.1rc2/trailmet/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/models/mobilenetv2_bireal.py` & `trailmet-0.0.1rc2/trailmet/models/mobilenetv2_bireal.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/models/resnet.py` & `trailmet-0.0.1rc2/trailmet/models/resnet.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/models/resnet_bireal.py` & `trailmet-0.0.1rc2/trailmet/models/resnet_bireal.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/models/resnet_chip.py` & `trailmet-0.0.1rc2/trailmet/models/resnet_chip.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/models/wideresnet.py` & `trailmet-0.0.1rc2/trailmet/models/wideresnet.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/utils/benchmark.py` & `trailmet-0.0.1rc2/trailmet/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/utils/functions.py` & `trailmet-0.0.1rc2/trailmet/utils/functions.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet/utils/tp_pruning.py` & `trailmet-0.0.1rc2/trailmet/utils/tp_pruning.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc0/trailmet.egg-info/PKG-INFO` & `trailmet-0.0.1rc2/trailmet.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,135 +1,135 @@
 Metadata-Version: 2.1
 Name: trailmet
-Version: 0.0.1rc0
+Version: 0.0.1rc2
 Summary: Transmute AI Model Efficiency Toolkit
 Home-page: https://github.com/transmuteAI/trailmet
 Author: TrAILMET Contributors
 Author-email: transmute.ai@gmail.com
 License: MIT License
+Description: <p align="center">
+            <br>
+                <img src="docs/source/imgs/trailmet.png" width="500"/>
+            </br>
+            <br>
+                <strong> Transmute AI Model Efficiency Toolkit </strong>
+            </br>
+        </p>
+        <p align="center">
+            <a href="https://github.com/transmuteAI/trailmet/blob/dev/LICENSE">
+                <img alt="GitHub" src="https://img.shields.io/github/license/transmuteAI/trailmet?color=blue">
+            </a>
+            <a href="https://transmuteai-trailmet.readthedocs.io/en/latest/">
+                <img alt="Documentation" src="https://img.shields.io/badge/docs-passing-brightgreen">
+            </a>
+            <a href="https://github.com/transmuteAI/trailmet/actions/workflows/ci.yml">
+                <img alt="Run tests with pytest" src="https://github.com/transmuteAI/trailmet/actions/workflows/ci.yml/badge.svg">
+            </a>
+            <a href="#">
+                <img alt="GitHub Stars" src="https://img.shields.io/github/stars/transmuteAI/trailmet">
+            </a>
+            <a href="#">
+                <img alt="GitHub Forks" src="https://img.shields.io/github/forks/transmuteAI/trailmet">
+            </a>
+        </p>
+        <h3 align="justified">
+        <!-- <p>Transmute AI Lab Model Efficiency Toolkit -->
+        </h3>
+        
+        # Introduction
+        
+        Trailmet is a model efficiency toolkit for compressing deep learning models using state of the art compression techniques.
+        Today deep learning models are not deployable because of their huge memory footprint, TRAILMET is an effort to make deep learning models more efficient in their size to performance ratio. It is developed using Pytorch 1.13.
+        
+        ### Major features
+        
+        - State of the art compression algorithms implemented.
+        - Demo notebooks for training each algorithm.
+        - Modular Design: All alogithms are modular and can customized easily for any kind of model and dataset.
+        
+        # Installation
+        
+        Below are quick steps for installation:
+        
+        ```shell
+        git clone https://github.com/transmuteAI/trailmet.git
+        cd trailmet
+        conda create -n trailmet
+        conda activate trailmet
+        conda install pytorch=1.13 torchvision=0.14 pytorch-cuda=11.7 -c pytorch -c nvidia
+        pip install -r requirements.txt
+        ```
+        
+        # Algorithms Implemented
+        
+        Demo notebooks for each algorithm is added in [experiments](https://github.com/transmuteAI/trailmet/blob/dev/experiments) folder
+        
+        <details open>
+        <summary> Knowledge Distillation</summary>
+        
+        - [x] [Response KD](https://arxiv.org/abs/1503.02531)
+        - [x] [Factor Transfer](https://arxiv.org/abs/1802.04977)
+        - [x] [Attention Transfer](https://arxiv.org/abs/1612.03928)
+        
+        </details>
+        
+        <details open>
+        <summary> Pruning </summary>
+        
+        - [x] [Chipnet](https://arxiv.org/abs/2102.07156)
+        - [x] [Network slimming](https://arxiv.org/abs/1708.06519)
+        - [x] [Growth Regularization](https://arxiv.org/abs/2012.09243)
+        
+        </details>
+        
+        <details open>
+        <summary> Quantization</summary>
+        
+        - [x] [BitSplit](https://dl.acm.org/doi/abs/10.5555/3524938.3525851)
+        - [x] [BRECQ](https://arxiv.org/abs/2102.05426)
+        - [x] [LAPQ](https://arxiv.org/abs/1911.07190)
+        
+        </details>
+        
+        <details open>
+        <summary> Binarization</summary>
+        
+        - [x] [BiRealNet](https://arxiv.org/abs/1808.00278)
+        - [x] [ReActNet](https://arxiv.org/abs/2003.03488)
+        - [x] [BNN-BN](https://arxiv.org/abs/2104.08215v1)
+        
+        </details>
+        
+        # Acknowledgement
+        
+        # Citation
+        
+        If you find this project useful in your research, please consider cite:
+        
+        ```BibTeX
+        @misc{,
+            title={},
+            author={},
+            howpublished = {}},
+            year={2023}
+        }
+        ```
+        
+        # License
+        
+        This project is released under the [MIT license](LICENSE).
+        
 Keywords: computer vision,image classification,model efficiency
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
-License-File: LICENSE
-
-<p align="center">
-    <br>
-        <img src="docs/source/imgs/Group 13.png" width="500"/>
-    </br>
-    <br>
-        <strong> Transmute AI Model Efficiency Toolkit </strong>
-    </br>
-</p>
-<p align="center">
-    <a href="https://github.com/transmuteAI/trailmet/blob/dev/LICENSE">
-        <img alt="GitHub" src="https://img.shields.io/github/license/transmuteAI/trailmet?color=blue">
-    </a>
-    <a href="https://transmuteai-trailmet.readthedocs.io/en/latest/">
-        <img alt="Documentation" src="https://img.shields.io/badge/docs-passing-brightgreen">
-    </a>
-    <a href="https://github.com/transmuteAI/trailmet/actions/workflows/ci.yml">
-        <img alt="Run tests with pytest" src="https://github.com/transmuteAI/trailmet/actions/workflows/ci.yml/badge.svg">
-    </a>
-    <a href="#">
-        <img alt="GitHub Stars" src="https://img.shields.io/github/stars/transmuteAI/trailmet">
-    </a>
-    <a href="#">
-        <img alt="GitHub Forks" src="https://img.shields.io/github/forks/transmuteAI/trailmet">
-    </a>
-</p>
-<h3 align="justified">
-<!-- <p>Transmute AI Lab Model Efficiency Toolkit -->
-</h3>
-
-# Introduction
-
-Trailmet is a model efficiency toolkit for compressing deep learning models using state of the art compression techniques.
-Today deep learning models are not deployable because of their huge memory footprint, TRAILMET is an effort to make deep learning models more efficient in their size to performance ratio. It is developed using Pytorch 1.13.
-
-### Major features
-
-- State of the art compression algorithms implemented.
-- Demo notebooks for training each algorithm.
-- Modular Design: All alogithms are modular and can customized easily for any kind of model and dataset.
-
-# Installation
-
-Below are quick steps for installation:
-
-```shell
-git clone https://github.com/transmuteAI/trailmet.git
-cd trailmet
-conda create -n trailmet
-conda activate trailmet
-conda install pytorch=1.13 torchvision=0.14 pytorch-cuda=11.7 -c pytorch -c nvidia
-pip install -r requirements.txt
-```
-
-# Algorithms Implemented
-
-Demo notebooks for each algorithm is added in [experiments](https://github.com/transmuteAI/trailmet/blob/dev/experiments) folder
-
-<details open>
-<summary> Knowledge Distillation</summary>
-
-- [x] [Response KD](https://arxiv.org/abs/1503.02531)
-- [x] [Factor Transfer](https://arxiv.org/abs/1802.04977)
-- [x] [Attention Transfer](https://arxiv.org/abs/1612.03928)
-
-</details>
-
-<details open>
-<summary> Pruning </summary>
-
-- [x] [Chipnet](https://arxiv.org/abs/2102.07156)
-- [x] [Network slimming](https://arxiv.org/abs/1708.06519)
-- [x] [Growth Regularization](https://arxiv.org/abs/2012.09243)
-
-</details>
-
-<details open>
-<summary> Quantization</summary>
-
-- [x] [BitSplit](https://dl.acm.org/doi/abs/10.5555/3524938.3525851)
-- [x] [BRECQ](https://arxiv.org/abs/2102.05426)
-- [x] [LAPQ](https://arxiv.org/abs/1911.07190)
-
-</details>
-
-<details open>
-<summary> Binarization</summary>
-
-- [x] [BiRealNet](https://arxiv.org/abs/1808.00278)
-- [x] [ReActNet](https://arxiv.org/abs/2003.03488)
-- [x] [BNN-BN](https://arxiv.org/abs/2104.08215v1)
-
-</details>
-
-# Acknowledgement
-
-# Citation
-
-If you find this project useful in your research, please consider cite:
-
-```BibTeX
-@misc{,
-    title={},
-    author={},
-    howpublished = {}},
-    year={2023}
-}
-```
-
-# License
-
-This project is released under the [MIT license](LICENSE).
```

#### html2text {}

```diff
@@ -1,22 +1,13 @@
-Metadata-Version: 2.1 Name: trailmet Version: 0.0.1rc0 Summary: Transmute AI
+Metadata-Version: 2.1 Name: trailmet Version: 0.0.1rc2 Summary: Transmute AI
 Model Efficiency Toolkit Home-page: https://github.com/transmuteAI/trailmet
 Author: TrAILMET Contributors Author-email: transmute.ai@gmail.com License: MIT
-License Keywords: computer vision,image classification,model efficiency
-Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-all License-File: LICENSE
+License Description:
 
-                       [docs/source/imgs/Group 13.png]
+                       [docs/source/imgs/trailmet.png]
                     Transmute AI Model Efficiency Toolkit
 [GitHub] [Documentation] [Run_tests_with_pytest] [GitHub_Stars] [GitHub_Forks]
 # Introduction Trailmet is a model efficiency toolkit for compressing deep
 learning models using state of the art compression techniques. Today deep
 learning models are not deployable because of their huge memory footprint,
 TRAILMET is an effort to make deep learning models more efficient in their size
 to performance ratio. It is developed using Pytorch 1.13. ### Major features -
@@ -37,8 +28,18 @@
 Quantization - [x] [BitSplit](https://dl.acm.org/doi/abs/10.5555/
 3524938.3525851) - [x] [BRECQ](https://arxiv.org/abs/2102.05426) - [x] [LAPQ]
 (https://arxiv.org/abs/1911.07190)    Binarization - [x] [BiRealNet](https://
 arxiv.org/abs/1808.00278) - [x] [ReActNet](https://arxiv.org/abs/2003.03488) -
 [x] [BNN-BN](https://arxiv.org/abs/2104.08215v1)  # Acknowledgement # Citation
 If you find this project useful in your research, please consider cite:
 ```BibTeX @misc{, title={}, author={}, howpublished = {}}, year={2023} } ``` #
-License This project is released under the [MIT license](LICENSE).
+License This project is released under the [MIT license](LICENSE). Keywords:
+computer vision,image classification,model efficiency Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
+all
```

### Comparing `trailmet-0.0.1rc0/trailmet.egg-info/SOURCES.txt` & `trailmet-0.0.1rc2/trailmet.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-LICENSE
 README.md
 setup.py
-tests/test_general.py
-tests/test_unwanted_files.py
 trailmet/__init__.py
 trailmet/version.py
 trailmet.egg-info/PKG-INFO
 trailmet.egg-info/SOURCES.txt
 trailmet.egg-info/dependency_links.txt
 trailmet.egg-info/not-zip-safe
 trailmet.egg-info/requires.txt
```

