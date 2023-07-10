# Comparing `tmp/rl4co-0.0.5.tar.gz` & `tmp/rl4co-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl4co-0.0.5.tar", last modified: Thu Jul  6 13:47:23 2023, max compression
+gzip compressed data, was "rl4co-0.0.6.tar", last modified: Mon Jul 10 19:04:52 2023, max compression
```

## Comparing `rl4co-0.0.5.tar` & `rl4co-0.0.6.tar`

### file list

```diff
@@ -1,127 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.122796 rl4co-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-06 13:47:13.000000 rl4co-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-07-06 13:47:23.122796 rl4co-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-07-06 13:47:13.000000 rl4co-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-06 13:47:13.000000 rl4co-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.106796 rl4co-0.0.5/rl4co/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.110796 rl4co-0.0.5/rl4co/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/data/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.110796 rl4co-0.0.5/rl4co/envs/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/atsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.110796 rl4co-0.0.5/rl4co/envs/common/
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/common/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/cvrp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/dpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/ffsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/mdpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/mtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/op.py
--rw-r--r--   0 runner    (1001) docker     (123)    13562 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/pctsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/pdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/sdvrp.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/spctsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.110796 rl4co-0.0.5/rl4co/models/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.110796 rl4co-0.0.5/rl4co/models/nn/
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/env_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/env_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/flash_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.110796 rl4co-0.0.5/rl4co/models/nn/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/graph/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/graph/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/graph/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.106796 rl4co-0.0.5/rl4co/models/rl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/rl/ppo/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/rl/ppo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/rl/ppo/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/rl/reinforce/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/rl/reinforce/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/rl/reinforce/baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/rl/reinforce/critic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.106796 rl4co-0.0.5/rl4co/models/zoo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/zoo/am/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/am/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/am/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/am/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/am/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/zoo/amppo/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/amppo/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/amppo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/amppo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/zoo/ham/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ham/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ham/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ham/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ham/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ham/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/zoo/mdam/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/mdam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/mdam/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/mdam/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/mdam/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/mdam/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/zoo/pomo/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/pomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/pomo/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/pomo/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/pomo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/pomo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.118796 rl4co-0.0.5/rl4co/models/zoo/ptrnet/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ptrnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ptrnet/critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ptrnet/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ptrnet/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ptrnet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ptrnet/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.118796 rl4co-0.0.5/rl4co/models/zoo/symnco/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/symnco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/symnco/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/symnco/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/symnco/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/symnco/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/symnco/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.118796 rl4co-0.0.5/rl4co/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/tasks/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/tasks/rl4co.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.118796 rl4co-0.0.5/rl4co/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.118796 rl4co-0.0.5/rl4co/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/callbacks/speed_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.122796 rl4co-0.0.5/rl4co/utils/download/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/download/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/download/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/download/gdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/download/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/instantiators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/param_grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/pylogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.106796 rl4co-0.0.5/rl4co.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-07-06 13:47:23.000000 rl4co-0.0.5/rl4co.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-06 13:47:23.000000 rl4co-0.0.5/rl4co.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:47:23.000000 rl4co-0.0.5/rl4co.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-06 13:47:23.000000 rl4co-0.0.5/rl4co.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 13:47:23.000000 rl4co-0.0.5/rl4co.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 13:47:23.122796 rl4co-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.122796 rl4co-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-06 13:47:13.000000 rl4co-0.0.5/tests/test_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-06 13:47:13.000000 rl4co-0.0.5/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-06 13:47:13.000000 rl4co-0.0.5/tests/test_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.302782 rl4co-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-10 19:04:40.000000 rl4co-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-07-10 19:04:52.302782 rl4co-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-07-10 19:04:40.000000 rl4co-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-10 19:04:40.000000 rl4co-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.286781 rl4co-0.0.6/rl4co/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.286781 rl4co-0.0.6/rl4co/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/data/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/atsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/envs/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/cvrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/dpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/ffsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/mdpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/mtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16473 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/pctsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/pdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/sdvrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/spctsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/models/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/models/nn/env_embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/env_embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/env_embeddings/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/env_embeddings/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/env_embeddings/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/flash_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/models/nn/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/graph/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/graph/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/graph/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.282781 rl4co-0.0.6/rl4co/models/rl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/models/rl/ppo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/rl/ppo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/rl/ppo/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/models/rl/reinforce/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/rl/reinforce/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/rl/reinforce/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/rl/reinforce/critic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.282781 rl4co-0.0.6/rl4co/models/zoo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.294782 rl4co-0.0.6/rl4co/models/zoo/am/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/am/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/am/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/am/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/am/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.294782 rl4co-0.0.6/rl4co/models/zoo/amppo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/amppo/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/amppo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/amppo/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.294782 rl4co-0.0.6/rl4co/models/zoo/ham/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ham/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ham/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ham/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ham/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ham/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.294782 rl4co-0.0.6/rl4co/models/zoo/mdam/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/mdam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/mdam/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/mdam/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/mdam/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/mdam/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.294782 rl4co-0.0.6/rl4co/models/zoo/pomo/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/pomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/pomo/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/pomo/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/pomo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/pomo/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.298782 rl4co-0.0.6/rl4co/models/zoo/ptrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ptrnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ptrnet/critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ptrnet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ptrnet/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ptrnet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ptrnet/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.298782 rl4co-0.0.6/rl4co/models/zoo/symnco/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/symnco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/symnco/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/symnco/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/symnco/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/symnco/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/symnco/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.298782 rl4co-0.0.6/rl4co/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/tasks/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/tasks/rl4co.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.302782 rl4co-0.0.6/rl4co/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.302782 rl4co-0.0.6/rl4co/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/callbacks/speed_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.302782 rl4co-0.0.6/rl4co/utils/download/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/download/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/download/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/download/gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/download/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/param_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/pylogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.286781 rl4co-0.0.6/rl4co.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-07-10 19:04:52.000000 rl4co-0.0.6/rl4co.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-10 19:04:52.000000 rl4co-0.0.6/rl4co.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:04:52.000000 rl4co-0.0.6/rl4co.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-10 19:04:52.000000 rl4co-0.0.6/rl4co.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 19:04:52.000000 rl4co-0.0.6/rl4co.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:04:52.302782 rl4co-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.302782 rl4co-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-10 19:04:40.000000 rl4co-0.0.6/tests/test_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-10 19:04:40.000000 rl4co-0.0.6/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-10 19:04:40.000000 rl4co-0.0.6/tests/test_ops.py
```

### Comparing `rl4co-0.0.5/LICENSE` & `rl4co-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/PKG-INFO` & `rl4co-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.0.5
+Version: 0.0.6
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rl4co-0.0.5/README.md` & `rl4co-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/pyproject.toml` & `rl4co-0.0.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     "pyrootutils",
     "rich",
     "numpy",
     "einops",
     "wandb",
     "pre-commit>=3.3.3",
     "matplotlib",
-    "scipy"
+    "scipy",
+    "pydantic<2.0.0" # Temporary bugfix https://github.com/Lightning-AI/lightning/pull/18022
 ]
 
 [project.optional-dependencies]
 graph = ["torch_geometric"]
 testing = ["pytest"]
 linting = ["black", "ruff"]
```

### Comparing `rl4co-0.0.5/rl4co/data/dataset.py` & `rl4co-0.0.6/rl4co/data/dataset.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/data/generate_data.py` & `rl4co-0.0.6/rl4co/data/generate_data.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/data/utils.py` & `rl4co-0.0.6/rl4co/data/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/envs/atsp.py` & `rl4co-0.0.6/rl4co/envs/atsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/envs/common/base.py` & `rl4co-0.0.6/rl4co/envs/common/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,12 +132,20 @@
     def _set_seed(self, seed: Optional[int]):
         """Set the seed for the environment"""
         rng = torch.manual_seed(seed)
         self.rng = rng
 
     def __getstate__(self):
         """Return the state of the environment. By default, we want to avoid pickling
-        the random number generator as it is not allowed by deepcopy
+        the random number generator directly as it is not allowed by `deepcopy`
         """
         state = self.__dict__.copy()
-        del state["rng"]
+        state["rng"] = state["rng"].get_state()
         return state
+
+    def __setstate__(self, state):
+        """Set the state of the environment. By default, we want to avoid pickling
+        the random number generator directly as it is not allowed by `deepcopy`
+        """
+        self.__dict__.update(state)
+        self.rng = torch.manual_seed(0)
+        self.rng.set_state(state["rng"])
```

### Comparing `rl4co-0.0.5/rl4co/envs/common/utils.py` & `rl4co-0.0.6/rl4co/envs/common/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/envs/cvrp.py` & `rl4co-0.0.6/rl4co/envs/cvrp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/envs/dpp.py` & `rl4co-0.0.6/rl4co/envs/dpp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/envs/ffsp.py` & `rl4co-0.0.6/rl4co/envs/ffsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/envs/mdpp.py` & `rl4co-0.0.6/rl4co/envs/mdpp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/envs/mtsp.py` & `rl4co-0.0.6/rl4co/envs/mtsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/envs/op.py` & `rl4co-0.0.6/rl4co/envs/op.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,19 +15,15 @@
 from rl4co.utils.ops import gather_by_index, get_tour_length
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 # From Kool et al. 2019
-MAX_LENGTHS = {
-    20: 2.,
-    50: 3.,
-    100: 4.
-}
+MAX_LENGTHS = {20: 2.0, 50: 3.0, 100: 4.0}
 
 
 class OPEnv(RL4COEnvBase):
     """Orienteering Problem (OP) environment.
     At each step, the agent chooses a location to visit in order to maximize the collected prize.
     The total length of the path must not exceed a given threshold.
 
@@ -38,14 +34,15 @@
         max_length: maximum length of the path
         prize_type: type of prize to collect. Can be:
             - "dist": the prize is the distance from the previous location
             - "unif": the prize is a uniform random variable
             - "const": the prize is a constant
         td_params: parameters of the environment
     """
+
     name = "op"
 
     def __init__(
         self,
         num_loc: int = 20,
         min_loc: float = 0,
         max_loc: float = 1,
@@ -54,30 +51,42 @@
         td_params: TensorDict = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.num_loc = num_loc
         self.min_loc = min_loc
         self.max_loc = max_loc
-        self.max_length = MAX_LENGTHS.get(num_loc, None) if max_length is None else max_length
+        self.max_length = (
+            MAX_LENGTHS.get(num_loc, None) if max_length is None else max_length
+        )
         if self.max_length is None:
-            raise ValueError(f"`max_length` must be specified for num_loc={num_loc}. Please specify it manually.")
+            raise ValueError(
+                f"`max_length` must be specified for num_loc={num_loc}. Please specify it manually."
+            )
         self.prize_type = prize_type
-        assert self.prize_type in ["dist", "unif", "const"], f"Invalid prize_type: {self.prize_type}"
+        assert self.prize_type in [
+            "dist",
+            "unif",
+            "const",
+        ], f"Invalid prize_type: {self.prize_type}"
         self._make_spec(td_params)
 
     def _step(self, td: TensorDict) -> TensorDict:
-        current_node = td["action"][:, None] 
+        current_node = td["action"][:, None]
 
         # Update tour length
         current_loc = gather_by_index(td["locs"], current_node)
-        tour_length = td["tour_length"] + (current_loc - td["current_loc"]).norm(p=2, dim=-1)
+        tour_length = td["tour_length"] + (current_loc - td["current_loc"]).norm(
+            p=2, dim=-1
+        )
 
         # Update prize with collected prize
-        current_total_prize = td["current_total_prize"] + gather_by_index(td["prize"], current_node, dim=-1)
+        current_total_prize = td["current_total_prize"] + gather_by_index(
+            td["prize"], current_node, dim=-1
+        )
 
         # Set current node as visited
         visited = td["visited"].scatter(-1, current_node, 1)
 
         # Done if went back to depot (except if it's the first step, since we start at the depot)
         done = (current_node.squeeze(-1) == 0) & (td["i"] > 0)
 
@@ -99,15 +108,15 @@
                     "reward": reward,
                     "done": done,
                 }
             },
             td.shape,
         )
         td_step["next"].set("action_mask", self.get_action_mask(td_step["next"]))
-        return td_step     
+        return td_step
 
     def _reset(
         self,
         td: Optional[TensorDict] = None,
         batch_size: Optional[list] = None,
     ) -> TensorDict:
         # Initialize params
@@ -120,86 +129,113 @@
         # Add depot to locs
         locs_with_depot = torch.cat((td["depot"][:, None, :], td["locs"]), -2)
 
         # Create reset TensorDict
         td_reset = TensorDict(
             {
                 "locs": locs_with_depot,
-                "prize": F.pad(td["prize"], (1, 0), mode='constant', value=0),  # add 0 for depot
+                "prize": F.pad(
+                    td["prize"], (1, 0), mode="constant", value=0
+                ),  # add 0 for depot
                 "tour_length": torch.zeros(*batch_size, device=self.device),
                 "current_loc": td["depot"],
                 # max_length is max length allowed when arriving at node, so subtract distance to return to depot
                 # Additionally, substract epsilon margin for numeric stability
-                "max_length": td["max_length"][..., None] - (td["depot"][..., None, :] - locs_with_depot).norm(p=2, dim=-1) - 1e-6,
-                "current_node": torch.zeros(*batch_size, 1, dtype=torch.long, device=self.device),
-                "visited": torch.zeros((*batch_size, locs_with_depot.shape[-2]), dtype=torch.bool, device=self.device),
-                "current_total_prize": torch.zeros(*batch_size, 1, dtype=torch.float, device=self.device),
-                "i": torch.zeros((*batch_size,), dtype=torch.int64, device=self.device), # counter
+                "max_length": td["max_length"][..., None]
+                - (td["depot"][..., None, :] - locs_with_depot).norm(p=2, dim=-1)
+                - 1e-6,
+                "current_node": torch.zeros(
+                    *batch_size, 1, dtype=torch.long, device=self.device
+                ),
+                "visited": torch.zeros(
+                    (*batch_size, locs_with_depot.shape[-2]),
+                    dtype=torch.bool,
+                    device=self.device,
+                ),
+                "current_total_prize": torch.zeros(
+                    *batch_size, 1, dtype=torch.float, device=self.device
+                ),
+                "i": torch.zeros(
+                    (*batch_size,), dtype=torch.int64, device=self.device
+                ),  # counter
             },
             batch_size=batch_size,
         )
         td_reset.set("action_mask", self.get_action_mask(td_reset))
         return td_reset
-    
+
     @staticmethod
     def get_action_mask(td: TensorDict) -> torch.Tensor:
         """Get action mask with 1 = feasible action, 0 = infeasible action.
         Cannot visit if already visited, if depot has been visited, or if the length exceeds the maximum length.
         """
         exceeds_length = (
-            td["tour_length"][..., None] + (td["locs"] - td["current_loc"][..., None, :]).norm(p=2, dim=-1)
+            td["tour_length"][..., None]
+            + (td["locs"] - td["current_loc"][..., None, :]).norm(p=2, dim=-1)
             > td["max_length"]
         )
         mask = td["visited"] | td["visited"][..., 0:1] | exceeds_length
 
-        action_mask = ~mask # 1 = feasible action, 0 = infeasible action
+        action_mask = ~mask  # 1 = feasible action, 0 = infeasible action
 
         # Depot can always be visited: we do not hardcode knowledge that this is strictly suboptimal if other options are available
         action_mask[..., 0] = 1
-        return action_mask 
-    
-    def get_reward(self, td: TensorDict, actions: TensorDict) -> TensorDict: 
+        return action_mask
+
+    def get_reward(self, td: TensorDict, actions: TensorDict) -> TensorDict:
         """Reward is the sum of the prizes of visited nodes"""
 
         # In case all tours directly return to depot, prevent further problems
-        if actions.size(-1) == 1:  
+        if actions.size(-1) == 1:
             assert (actions == 0).all(), "If all length 1 tours, they should be zero"
             return torch.zeros(actions.size(0), dtype=torch.float, device=actions.device)
-               
+
         # Check that the solution is valid
         if self.check_solution:
             self.check_solution_validity(td, actions)
 
         # Prize is the sum of the prizes of the visited nodes. Note that prize is padded with 0 for depot at index 0
         collected_prize = td["prize"].gather(1, actions)
         return collected_prize.sum(-1)
-    
+
     @staticmethod
-    def check_solution_validity(td: TensorDict, actions: torch.Tensor, add_distance_to_depot: bool = True):
+    def check_solution_validity(
+        td: TensorDict, actions: torch.Tensor, add_distance_to_depot: bool = True
+    ):
         """Check that solution is valid: nodes are not visited twice except depot and capacity is not exceeded.
         If `add_distance_to_depot` if True, then the distance to the depot is added to max length since by default, the max length is
         modified in the reset function to account for the distance to the depot.
         """
 
         # Check that tours are valid, i.e. contain 0 to n -1
         sorted_actions = actions.data.sort(1)[0]
         # Make sure each node visited once at most (except for depot)
-        assert ((sorted_actions[:, 1:] == 0) | (sorted_actions[:, 1:] > sorted_actions[:, :-1])).all(), "Duplicates"
+        assert (
+            (sorted_actions[:, 1:] == 0)
+            | (sorted_actions[:, 1:] > sorted_actions[:, :-1])
+        ).all(), "Duplicates"
 
         # Gather locations in order of tour and get the length of tours
         locs_ordered = gather_by_index(td["locs"], actions)
         length = get_tour_length(locs_ordered)
-        
+
         max_length = td["max_length"]
         if add_distance_to_depot:
-            max_length = max_length + (td["locs"][..., 0:1, :] - td["locs"]).norm(p=2, dim=-1) + 1e-6
+            max_length = (
+                max_length
+                + (td["locs"][..., 0:1, :] - td["locs"]).norm(p=2, dim=-1)
+                + 1e-6
+            )
+
+        assert (
+            length[..., None] <= max_length + 1e-5
+        ).all(), "Max length exceeded by {}".format(
+            (length[..., None] - max_length).max()
+        )
 
-        assert (length[..., None] <= max_length + 1e-5).all(), \
-            "Max length exceeded by {}".format((length[..., None] - max_length).max())
-        
     def generate_data(self, batch_size, prize_type=None) -> TensorDict:
         # Batch size input check
         batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
 
         prize_type = self.prize_type if prize_type is None else prize_type
 
         # Initialize the locations (including the depot which is always the first node)
@@ -209,18 +245,27 @@
             .to(self.device)
         )
 
         # Methods taken from Fischetti et al. (1998) and Kool et al. (2019)
         if prize_type == "const":
             prize = torch.ones(*batch_size, self.num_loc, device=self.device)
         elif prize_type == "unif":
-            prize = (1 + torch.randint(0, 100, (*batch_size, self.num_loc), device=self.device).float()) / 100
-        elif prize_type == "dist": # based on the distance to the depot
-            prize = (locs_with_depot[..., 0:1, :] - locs_with_depot[..., 1:, :]).norm(p=2, dim=-1)
-            prize = (1 + (prize / prize.max(dim=-1, keepdim=True)[0] * 99).int()).float() / 100 
+            prize = (
+                1
+                + torch.randint(
+                    0, 100, (*batch_size, self.num_loc), device=self.device
+                ).float()
+            ) / 100
+        elif prize_type == "dist":  # based on the distance to the depot
+            prize = (locs_with_depot[..., 0:1, :] - locs_with_depot[..., 1:, :]).norm(
+                p=2, dim=-1
+            )
+            prize = (
+                1 + (prize / prize.max(dim=-1, keepdim=True)[0] * 99).int()
+            ).float() / 100
         else:
             raise ValueError(f"Invalid prize_type: {self.prize_type}")
 
         # Support for heterogeneous max length if provided
         if not isinstance(self.max_length, torch.Tensor):
             max_length = torch.full((*batch_size,), self.max_length, device=self.device)
         else:
@@ -285,8 +330,84 @@
             maximum=self.num_loc + 1,
         )
         self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
         self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
 
     @staticmethod
     def render(td: TensorDict, actions=None, ax=None):
-        raise NotImplementedError("TODO: render is not implemented yet")
+        import matplotlib.pyplot as plt
+        import numpy as np
+
+        # Create a plot of the nodes
+        if ax is None:
+            _, ax = plt.subplots()
+
+        td = td.detach().cpu()
+
+        # Actions
+        if actions is None:
+            actions = td.get("action", None)
+        actions = actions.detach().cpu() if actions is not None else None
+
+        # if batch_size greater than 0 , we need to select the first batch element
+        if td.batch_size != torch.Size([]):
+            td = td[0]
+            actions = actions[0] if actions is not None else None
+
+        # Variables
+        depot = td["locs"][0, :]
+        cities = td["locs"][1:, :]
+        prizes = td["prize"][1:]
+        normalized_prizes = (
+            200 * (prizes - torch.min(prizes)) / (torch.max(prizes) - torch.min(prizes))
+            + 10
+        )
+
+        # Plot depot and cities with prize
+        ax.scatter(
+            depot[0],
+            depot[1],
+            marker="s",
+            c="tab:green",
+            edgecolors="black",
+            zorder=5,
+            s=100,
+        )  # Plot depot as square
+        ax.scatter(
+            cities[:, 0],
+            cities[:, 1],
+            s=normalized_prizes,
+            c=normalized_prizes,
+            cmap="autumn_r",
+            alpha=0.6,
+            edgecolors="black",
+        )  # Plot all cities with size and color indicating the prize
+
+        # Gather locs in order of action if available
+        if actions is None:
+            log.warning("No action in TensorDict, rendering unsorted locs")
+        else:
+            # Reorder the cities and their corresponding prizes based on actions
+            tour = cities[actions - 1]  # subtract 1 to match Python's 0-indexing
+
+            # Append the depot at the beginning and the end of the tour
+            tour = np.vstack((depot, tour, depot))
+
+            # Use quiver to plot the tour
+            dx, dy = np.diff(tour[:, 0]), np.diff(tour[:, 1])
+            ax.quiver(
+                tour[:-1, 0],
+                tour[:-1, 1],
+                dx,
+                dy,
+                scale_units="xy",
+                angles="xy",
+                scale=1,
+                zorder=2,
+                color="black",
+                width=0.0035,
+            )
+
+        # Setup limits and show
+        ax.set_xlim(-0.05, 1.05)
+        ax.set_ylim(-0.05, 1.05)
+        plt.show()
```

### Comparing `rl4co-0.0.5/rl4co/envs/pctsp.py` & `rl4co-0.0.6/rl4co/envs/pctsp.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     UnboundedDiscreteTensorSpec,
 )
 
 from rl4co.envs.common.base import RL4COEnvBase
 from rl4co.utils.ops import gather_by_index, get_tour_length
 from rl4co.utils.pylogger import get_pylogger
 
-
 log = get_pylogger(__name__)
 
 # For the penalty to make sense it should be not too large (in which case all nodes will be visited) nor too small
 # so we want the objective term to be approximately equal to the length of the tour, which we estimate with half
 # of the nodes by half of the tour length (which is very rough but similar to op)
 # This means that the sum of penalties for all nodes will be approximately equal to the tour length (on average)
 # The expected total (uniform) penalty of half of the nodes (since approx half will be visited by the constraint)
@@ -38,15 +37,15 @@
         min_loc (float): Minimum location value
         max_loc (float): Maximum location value
         penalty_factor (float): Penalty factor
         prize_required (float): Minimum prize required to visit a node
         check_solution (bool): Set to False by default for small bug happening around 0.01% of the time (TODO: fix)
         td_params (TensorDict): Parameters of the environment
     """
-    
+
     name = "pctsp"
     _stochastic = False
 
     def __init__(
         self,
         num_loc: int = 10,
         min_loc: float = 0,
@@ -71,15 +70,15 @@
         # Get current coordinates, prize, and penalty
         cur_total_prize = td["cur_total_prize"] + gather_by_index(
             td["real_prize"], current_node
         )
         cur_total_penalty = td["cur_total_penalty"] + gather_by_index(
             td["penalty"], current_node
         )
-        
+
         # Update visited
         visited = td["visited"].scatter(-1, current_node[..., None], 1)
 
         # Done and reward. Calculation is done outside hence set -inf
         done = (td["i"] > 0) & (current_node == 0)
         reward = torch.ones_like(cur_total_prize) * float("-inf")
 
@@ -99,28 +98,30 @@
                     "reward": reward,
                     "done": done,
                 },
             },
             batch_size=td.batch_size,
         )
         td_step["next"].set("action_mask", self.get_action_mask(td_step["next"]))
-        return td_step 
+        return td_step
 
     def _reset(
         self, td: Optional[TensorDict] = None, batch_size: Optional[list] = None
     ) -> TensorDict:
         if batch_size is None:
             batch_size = self.batch_size if td is None else td["locs"].shape[:-2]
         if td is None or td.is_empty():
             td = self.generate_data(batch_size=batch_size)
         self.device = td.device
 
         locs = torch.cat([td["depot"][..., None, :], td["locs"]], dim=-2)
         expected_prize = td["deterministic_prize"]
-        real_prize = td["stochastic_prize"] if self.stochastic else td["deterministic_prize"]
+        real_prize = (
+            td["stochastic_prize"] if self.stochastic else td["deterministic_prize"]
+        )
         penalty = td["penalty"]
 
         # Concatenate depots
         real_prize_with_depot = torch.cat(
             [torch.zeros_like(real_prize[..., :1]), real_prize], dim=-1
         )
         penalty_with_depot = F.pad(penalty, (1, 0), mode="constant", value=0)
@@ -154,62 +155,68 @@
                 "prize_required": prize_required,
                 "i": i,
             },
             batch_size=batch_size,
         )
         td_reset.set("action_mask", self.get_action_mask(td_reset))
         return td_reset
-    
+
     @staticmethod
     def get_action_mask(td: TensorDict) -> torch.Tensor:
         """Cannot visit depot if not yet collected 1 total prize and there are unvisited nodes"""
         mask = td["visited"] | td["visited"][..., 0:1]
         mask[..., 0] = (td["cur_total_prize"] < 1.0) & (
             td["visited"][..., 1:].int().sum(-1) < td["visited"][..., 1:].size(-1)
         )
         return ~(mask > 0)  # Invert mask, since 1 means feasible action
 
     def get_reward(self, td: TensorDict, actions: torch.Tensor) -> torch.Tensor:
         """Reward is `saved penalties - (total length + penalty)`"""
 
         # In case all tours directly return to depot, prevent further problems
-        if actions.size(-1) == 1:  
+        if actions.size(-1) == 1:
             assert (actions == 0).all(), "If all length 1 tours, they should be zero"
             return torch.zeros(actions.size(0), dtype=torch.float, device=actions.device)
-        
+
         # Check that the solution is valid
         if self.check_solution:
             self.check_solution_validity(td, actions)
 
         # Gather locations in order of tour and get the length of tours
         locs_ordered = gather_by_index(td["locs"], actions)
         length = get_tour_length(locs_ordered)
-        
+
         # Reward is saved penalties - (total length + penalty)
         saved_penalty = td["penalty"].gather(1, actions)
         return saved_penalty.sum(-1) - (length + td["penalty"][..., 1:].sum(-1))
 
     @staticmethod
     def check_solution_validity(td: TensorDict, actions: torch.Tensor):
         """Check that the solution is valid, i.e. contains all nodes once at most, and either prize constraint is met or all nodes are visited"""
 
         # Check that tours are valid, i.e. contain 0 to n -1
         sorted_actions = actions.data.sort(1)[0]
 
         # Make sure each node visited once at most (except for depot)
-        assert ((sorted_actions[..., 1:] == 0) | (sorted_actions[..., 1:] > sorted_actions[..., :-1])).all(), "Duplicates"
+        assert (
+            (sorted_actions[..., 1:] == 0)
+            | (sorted_actions[..., 1:] > sorted_actions[..., :-1])
+        ).all(), "Duplicates"
 
         prize = td["real_prize"][..., 1:]  # Remove depot
         prize_with_depot = torch.cat((torch.zeros_like(prize[:, :1]), prize), 1)
         p = prize_with_depot.gather(1, actions)
 
         # Either prize constraint should be satisfied or all prizes should be visited
         assert (
-            (p.sum(-1) >= 1 - 1e-5) |
-            (sorted_actions.size(-1) - (sorted_actions == 0).int().sum(-1) == (td["locs"].size(-2) - 1)) # no depot
+            (p.sum(-1) >= 1 - 1e-5)
+            | (
+                sorted_actions.size(-1) - (sorted_actions == 0).int().sum(-1)
+                == (td["locs"].size(-2) - 1)
+            )  # no depot
         ).all(), "Total prize does not satisfy min total prize"
 
     def generate_data(self, batch_size) -> TensorDict:
         # Batch size input check
         batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
 
         depot = torch.rand((*batch_size, 2))
@@ -253,20 +260,22 @@
             },
             batch_size=batch_size,
         )
 
     @property
     def stochastic(self):
         return self._stochastic
-    
+
     @stochastic.setter
     def stochastic(self, state: bool):
-        if state == True:
-            log.warning('Stochastic mode should not be used for PCTSP. Use SPCTSP instead.')
-            
+        if state is True:
+            log.warning(
+                "Stochastic mode should not be used for PCTSP. Use SPCTSP instead."
+            )
+
     def _make_spec(self, td_params: TensorDict):
         """Make the locs and action specs from the parameters."""
         self.observation_spec = CompositeSpec(
             locs=BoundedTensorSpec(
                 minimum=self.min_loc,
                 maximum=self.max_loc,
                 shape=(self.num_loc, 2),
@@ -321,9 +330,98 @@
             minimum=0,
             maximum=self.num_loc,
         )
         self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
         self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
 
     @staticmethod
-    def render(td: TensorDict, actions=None, ax=None):
-        raise NotImplementedError("TODO: render is not implemented yet")
+    def render(td, actions=None, ax=None):
+        import matplotlib.pyplot as plt
+        import numpy as np
+
+        from matplotlib import colormaps
+
+        # Create a plot of the nodes
+        if ax is None:
+            _, ax = plt.subplots()
+
+        td = td.detach().cpu()
+
+        # Actions
+        if actions is None:
+            actions = td.get("action", None)
+        actions = actions.detach().cpu() if actions is not None else None
+
+        # if batch_size greater than 0 , we need to select the first batch element
+        if td.batch_size != torch.Size([]):
+            td = td[0]
+            actions = actions[0] if actions is not None else None
+
+        # Variables
+        depot = td["locs"][0, :]
+        cities = td["locs"][1:, :]
+        prizes = td["real_prize"][1:]
+        penalties = td["penalty"][1:]
+        normalized_prizes = (
+            200 * (prizes - torch.min(prizes)) / (torch.max(prizes) - torch.min(prizes))
+            + 10
+        )
+        normalized_penalties = (
+            3
+            * (penalties - torch.min(penalties))
+            / (torch.max(penalties) - torch.min(penalties))
+        )
+
+        # Represent penalty with colormap and size of edges
+        penalty_cmap = colormaps.get_cmap("BuPu")
+        penalty_colors = penalty_cmap(normalized_penalties)
+
+        # Plot depot and cities with prize (size of nodes) and penalties (size of borders)
+        ax.scatter(
+            depot[0],
+            depot[1],
+            marker="s",
+            c="tab:green",
+            edgecolors="black",
+            zorder=1,
+            s=100,
+        )  # Plot depot as square
+        ax.scatter(
+            cities[:, 0],
+            cities[:, 1],
+            s=normalized_prizes,
+            c=normalized_prizes,
+            cmap="autumn_r",
+            alpha=1,
+            edgecolors=penalty_colors,
+            linewidths=normalized_penalties,
+        )  # Plot all cities with size and color indicating the prize
+
+        # Gather locs in order of action if available
+        if actions is None:
+            print("No action in TensorDict, rendering unsorted locs")
+        else:
+            # Reorder the cities and their corresponding prizes based on actions
+            tour = cities[actions - 1]  # subtract 1 to match Python's 0-indexing
+
+            # Append the depot at the beginning and the end of the tour
+            tour = np.vstack((depot, tour, depot))
+
+            # Use quiver to plot the tour
+            dx, dy = np.diff(tour[:, 0]), np.diff(tour[:, 1])
+            ax.quiver(
+                tour[:-1, 0],
+                tour[:-1, 1],
+                dx,
+                dy,
+                scale_units="xy",
+                angles="xy",
+                scale=1,
+                zorder=2,
+                color="black",
+                width=0.0035,
+            )
+
+        # Setup limits and show
+        ax.set_xlim(-0.05, 1.05)
+        ax.set_ylim(-0.05, 1.05)
+        plt.show()
```

### Comparing `rl4co-0.0.5/rl4co/envs/pdp.py` & `rl4co-0.0.6/rl4co/envs/pdp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/envs/sdvrp.py` & `rl4co-0.0.6/rl4co/envs/sdvrp.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from torchrl.data import (
     BoundedTensorSpec,
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
-from rl4co.envs.cvrp import CVRPEnv, CAPACITIES
+from rl4co.envs.cvrp import CVRPEnv
 from rl4co.utils.ops import gather_by_index
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class SDVRPEnv(CVRPEnv):
@@ -57,30 +57,36 @@
             min_demand=min_demand,
             max_demand=max_demand,
             vehicle_capacity=vehicle_capacity,
             capacity=capacity,
             td_params=td_params,
             **kwargs,
         )
-    
+
     def _step(self, td: TensorDict) -> TensorDict:
         # Update the state
         current_node = td["action"][:, None]  # Add dimension for step
 
         # Not selected_demand is demand of first node (by clamp) so incorrect for nodes that visit depot!
         selected_demand = gather_by_index(
             td["demand_with_depot"], current_node, dim=-1, squeeze=False
         )[..., :1]
-        delivered_demand = torch.min(selected_demand, td["vehicle_capacity"] - td["used_capacity"])
+        delivered_demand = torch.min(
+            selected_demand, td["vehicle_capacity"] - td["used_capacity"]
+        )
 
         # Increase capacity if depot is not visited, otherwise set to 0
-        used_capacity = (td["used_capacity"] + delivered_demand) * (current_node != 0).float()
+        used_capacity = (td["used_capacity"] + delivered_demand) * (
+            current_node != 0
+        ).float()
 
         # Update demand
-        demand_with_depot = td["demand_with_depot"].scatter_add(-1, current_node, -delivered_demand)
+        demand_with_depot = td["demand_with_depot"].scatter_add(
+            -1, current_node, -delivered_demand
+        )
 
         # Get done and reward (-inf since we get it outside)
         done = ~(demand_with_depot > 0).any(-1)
         reward = torch.ones_like(done) * float("-inf")
 
         td_step = TensorDict(
             {
@@ -107,59 +113,64 @@
     ) -> TensorDict:
         if batch_size is None:
             batch_size = self.batch_size if td is None else td["locs"].shape[:-2]
 
         if td is None or td.is_empty():
             td = self.generate_data(batch_size=batch_size)
 
-        self.device = td.device
+        self.device = td["locs"].device
 
         # Create reset TensorDict
         reset_td = TensorDict(
             {
                 "locs": torch.cat((td["depot"][..., None, :], td["locs"]), -2),
                 "demand": td["demand"],
-                "demand_with_depot": torch.cat((torch.zeros_like(td["demand"][..., 0:1]), td["demand"]), -1),
-                "current_node": torch.zeros(*batch_size, 1, dtype=torch.long, device=self.device),
+                "demand_with_depot": torch.cat(
+                    (torch.zeros_like(td["demand"][..., 0:1]), td["demand"]), -1
+                ),
+                "current_node": torch.zeros(
+                    *batch_size, 1, dtype=torch.long, device=self.device
+                ),
                 "used_capacity": torch.zeros((*batch_size, 1), device=self.device),
-                "vehicle_capacity": torch.full((*batch_size, 1), self.vehicle_capacity, device=self.device),
+                "vehicle_capacity": torch.full(
+                    (*batch_size, 1), self.vehicle_capacity, device=self.device
+                ),
             },
             batch_size=batch_size,
         )
         reset_td.set("action_mask", self.get_action_mask(reset_td))
         return reset_td
-    
+
     @staticmethod
     def get_action_mask(td: TensorDict) -> torch.Tensor:
-        mask_loc = (td["demand_with_depot"][..., 1:] == 0) | (td["used_capacity"] >= td["vehicle_capacity"])
-        mask_depot = (td["current_node"] == 0).squeeze(-1) & ((mask_loc == 0).int().sum(-1) > 0)
+        mask_loc = (td["demand_with_depot"][..., 1:] == 0) | (
+            td["used_capacity"] >= td["vehicle_capacity"]
+        )
+        mask_depot = (td["current_node"] == 0).squeeze(-1) & (
+            (mask_loc == 0).int().sum(-1) > 0
+        )
         return ~torch.cat((mask_depot[..., None], mask_loc), -1)
 
     @staticmethod
     def check_solution_validity(td: TensorDict, actions: torch.Tensor):
         """Check that the solution is valid (all demand is satisfied)"""
-        
+
         batch_size, graph_size = td["demand"].size()
 
         # Each node can be visited multiple times, but we always deliver as much demand as possible
         # We check that at the end all demand has been satisfied
-        demands = torch.cat(
-            (
-                -td["vehicle_capacity"],
-                td['demand']
-            ),
-            1
-        )
+        demands = torch.cat((-td["vehicle_capacity"], td["demand"]), 1)
 
         rng = torch.arange(batch_size, out=demands.data.new().long())
-        used_cap = torch.zeros_like(td['demand'][..., 0])
+        used_cap = torch.zeros_like(td["demand"][..., 0])
         a_prev = None
         for a in actions.transpose(0, 1):
-            assert a_prev is None or (demands[((a_prev == 0) & (a == 0)), :] == 0).all(), \
-                "Cannot visit depot twice if any nonzero demand"
+            assert (
+                a_prev is None or (demands[((a_prev == 0) & (a == 0)), :] == 0).all()
+            ), "Cannot visit depot twice if any nonzero demand"
             d = torch.min(demands[rng, a], td["vehicle_capacity"].squeeze(-1) - used_cap)
             demands[rng, a] -= d
             used_cap += d
             used_cap[a == 0] = 0
             a_prev = a
         assert (demands == 0).all(), "All demand must be satisfied"
 
@@ -179,15 +190,15 @@
             demand=BoundedTensorSpec(
                 minimum=self.min_demand,
                 maximum=self.max_demand,
                 shape=(self.num_loc, 1),  # demand is only for customers
                 dtype=torch.float32,
             ),
             demand_with_depot=BoundedTensorSpec(
-                minimum=self.min_demand, 
+                minimum=self.min_demand,
                 maximum=self.max_demand,
                 shape=(self.num_loc + 1, 1),
                 dtype=torch.float32,
             ),
             used_capacity=BoundedTensorSpec(
                 minimum=0,
                 maximum=self.vehicle_capacity,
@@ -204,8 +215,8 @@
         self.action_spec = BoundedTensorSpec(
             shape=(1,),
             dtype=torch.int64,
             minimum=0,
             maximum=self.num_loc + 1,
         )
         self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
-        self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
+        self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
```

### Comparing `rl4co-0.0.5/rl4co/envs/spctsp.py` & `rl4co-0.0.6/rl4co/envs/spctsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/envs/tsp.py` & `rl4co-0.0.6/rl4co/envs/tsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/nn/attention.py` & `rl4co-0.0.6/rl4co/models/nn/attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/nn/env_context.py` & `rl4co-0.0.6/rl4co/models/nn/env_embeddings/context.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,80 @@
-from typing import Union
-
 import torch
 import torch.nn as nn
 
-from torchrl.envs import EnvBase
-
 from rl4co.utils.ops import gather_by_index
 
 
-def env_context(env: Union[str, EnvBase], config: dict) -> object:
-    """Get context object for given environment name"""
-    context_classes = {
+def env_context_embedding(env_name: str, config: dict) -> nn.Module:
+    """Get environment context embedding. The context embedding is used to modify the
+    query embedding of the problem node of the current partial solution.
+    Usually consists of a projection of gathered node embeddings and features to the embedding space.
+
+    Args:
+        env: Environment or its name.
+        config: A dictionary of configuration options for the environment.
+    """
+    embedding_registry = {
         "tsp": TSPContext,
         "atsp": TSPContext,
         "cvrp": VRPContext,
         "sdvrp": VRPContext,
         "pctsp": PCTSPContext,
         "spctsp": PCTSPContext,
         "op": OPContext,
         "dpp": DPPContext,
         "mdpp": DPPContext,
         "pdp": PDPContext,
         "mtsp": MTSPContext,
     }
 
-    env_name = env if isinstance(env, str) else env.name
-    context_class = context_classes.get(env_name, None)
-
-    if context_class is None:
-        raise ValueError(f"Unknown environment name '{env_name}'")
+    if env_name not in embedding_registry:
+        raise ValueError(
+            f"Unknown environment name '{env_name}'. Available context embeddings: {embedding_registry.keys()}"
+        )
 
-    return context_class(**config)
+    return embedding_registry[env_name](**config)
 
 
 class EnvContext(nn.Module):
+    """Base class for environment context embeddings. The context embedding is used to modify the
+    query embedding of the problem node of the current partial solution.
+    Consists of a linear layer that projects the node features to the embedding space."""
+
     def __init__(self, embedding_dim, step_context_dim=None):
-        """Get environment context and project it to embedding space"""
         super(EnvContext, self).__init__()
         self.embedding_dim = embedding_dim
         step_context_dim = (
             step_context_dim if step_context_dim is not None else embedding_dim
         )
         self.project_context = nn.Linear(step_context_dim, embedding_dim, bias=False)
 
     def _cur_node_embedding(self, embeddings, td):
+        """Get embedding of current node"""
         cur_node_embedding = gather_by_index(embeddings, td["current_node"])
         return cur_node_embedding
 
     def _state_embedding(self, embeddings, td):
+        """Get state embedding"""
         raise NotImplementedError("Implement for each environment")
 
     def forward(self, embeddings, td):
         cur_node_embedding = self._cur_node_embedding(embeddings, td)
         state_embedding = self._state_embedding(embeddings, td)
         context_embedding = torch.cat([cur_node_embedding, state_embedding], -1)
         return self.project_context(context_embedding)
 
 
 class TSPContext(EnvContext):
+    """Context embedding for the Traveling Salesman Problem (TSP).
+    Project the following to the embedding space:
+        - first node embedding
+        - current node embedding
+    """
+
     def __init__(self, embedding_dim):
         super(TSPContext, self).__init__(embedding_dim, 2 * embedding_dim)
         self.W_placeholder = nn.Parameter(
             torch.Tensor(2 * self.embedding_dim).uniform_(-1, 1)
         )
 
     def forward(self, embeddings, td):
@@ -80,72 +93,98 @@
                 ),
             ).view(batch_size, *node_dim)
 
         return self.project_context(context_embedding)
 
 
 class VRPContext(EnvContext):
+    """Context embedding for the Capacitated Vehicle Routing Problem (CVRP).
+    Project the following to the embedding space:
+        - current node embedding
+        - remaining capacity (vehicle_capacity - used_capacity)
+    """
+
     def __init__(self, embedding_dim):
         super(VRPContext, self).__init__(embedding_dim, embedding_dim + 1)
 
     def _state_embedding(self, embeddings, td):
         state_embedding = td["vehicle_capacity"] - td["used_capacity"]
         return state_embedding
 
 
 class PCTSPContext(EnvContext):
+    """Context embedding for the Prize Collecting TSP (PCTSP).
+    Project the following to the embedding space:
+        - current node embedding
+        - remaining prize (prize_required - cur_total_prize)
+    """
+
     def __init__(self, embedding_dim):
         super(PCTSPContext, self).__init__(embedding_dim, embedding_dim + 1)
 
     def _state_embedding(self, embeddings, td):
-        # Remaining prize to collect
         state_embedding = torch.clamp(
             td["prize_required"] - td["cur_total_prize"], min=0
         )[..., None]
         return state_embedding
 
 
 class OPContext(EnvContext):
+    """Context embedding for the Orienteering Problem (OP).
+    Project the following to the embedding space:
+        - current node embedding
+        - remaining distance (max_length - tour_length)
+    """
+
     def __init__(self, embedding_dim):
         super(OPContext, self).__init__(embedding_dim, embedding_dim + 1)
 
     def _state_embedding(self, embeddings, td):
         state_embedding = td["max_length"][..., 0] - td["tour_length"]
         return state_embedding[..., None]
 
 
 class DPPContext(EnvContext):
+    """Context embedding for the Decap Placement Problem (DPP), EDA (electronic design automation).
+    Project the following to the embedding space:
+        - current cell embedding
+    """
+
     def __init__(self, embedding_dim):
         super(DPPContext, self).__init__(embedding_dim)
 
     def forward(self, embeddings, td):
         """Context cannot be defined by a single node embedding for DPP, hence 0.
         We modify the dynamic embedding instead to capture placed items
         """
         return embeddings.new_zeros(embeddings.size(0), self.embedding_dim)
 
 
 class PDPContext(EnvContext):
-    """From https://arxiv.org/abs/2110.02634"""
+    """Context embedding for the Pickup and Delivery Problem (PDP).
+    Project the following to the embedding space:
+        - current node embedding
+    """
 
     def __init__(self, embedding_dim):
         super(PDPContext, self).__init__(embedding_dim, embedding_dim)
 
     def forward(self, embeddings, td):
         cur_node_embedding = self._cur_node_embedding(embeddings, td).squeeze()
         return self.project_context(cur_node_embedding)
 
 
 class MTSPContext(EnvContext):
-    """NOTE: new made by Fede in free style. May need to be checked
-    We use as features:
-        1. remaining number of agents
-        2. the current length of the tour
-        3. the max subtour length so far
-        4. the current distance from the depot
+    """Context embedding for the Multiple Traveling Salesman Problem (mTSP).
+    Project the following to the embedding space:
+        - current node embedding
+        - remaining_agents
+        - current_length
+        - max_subtour_length
+        - distance_from_depot
     """
 
     def __init__(self, embedding_dim):
         super(MTSPContext, self).__init__(embedding_dim, 2 * embedding_dim)
         proj_in_dim = (
             4  # remaining_agents, current_length, max_subtour_length, distance_from_depot
         )
```

### Comparing `rl4co-0.0.5/rl4co/models/nn/env_embedding.py` & `rl4co-0.0.6/rl4co/models/nn/env_embeddings/init.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,104 +1,65 @@
-from typing import Union
-
 import torch
 import torch.nn as nn
 
-from torchrl.envs import EnvBase
-
-
-def env_init_embedding(env: Union[str, EnvBase], config: dict) -> object:
-    return env_embedding(env, "init", config)
-
 
-def env_dynamic_embedding(env: Union[str, EnvBase], config: dict) -> object:
-    return env_embedding(env, "dynamic", config)
-
-
-def env_embedding(env: Union[str, EnvBase], embedding_type: str, config: dict) -> object:
-    """Create an embedding object for a given environment name and embedding type.
+def env_init_embedding(env_name: str, config: dict) -> nn.Module:
+    """Get environment initial embedding. The init embedding is used to initialize the
+    general embedding of the problem nodes without any solution information.
+    Consists of a linear layer that projects the node features to the embedding space.
 
     Args:
         env: Environment or its name.
         config: A dictionary of configuration options for the environment.
-        embedding_type: The type of embedding to create, either `init` or `dynamic`.
     """
-
-    embedding_classes = {
-        "tsp": {
-            "init": TSPInitEmbedding,
-            "dynamic": StaticEmbedding,
-        },
-        "atsp": {
-            "init": TSPInitEmbedding,
-            "dynamic": StaticEmbedding,
-        },
-        "cvrp": {
-            "init": VRPInitEmbedding,
-            "dynamic": StaticEmbedding,
-        },
-        "sdvrp": {
-            "init": VRPInitEmbedding,
-            "dynamic": SDVRPDynamicEmbedding,
-        },
-        "pctsp": {
-            "init": PCTSPInitEmbedding,
-            "dynamic": StaticEmbedding,
-        },
-        "spctsp": {
-            "init": PCTSPInitEmbedding,
-            "dynamic": StaticEmbedding,
-        },
-        "op": {
-            "init": OPInitEmbedding,
-            "dynamic": StaticEmbedding,
-        },
-        "dpp": {
-            "init": DPPInitEmbedding,
-            "dynamic": StaticEmbedding,
-        },
-        "mdpp": {
-            "init": MDPPInitEmbedding,
-            "dynamic": DPPDynamicEmbedding,
-        },
-        "pdp": {
-            "init": PDPInitEmbedding,
-            "dynamic": StaticEmbedding,
-        },
-        "mtsp": {
-            "init": MTSPInitEmbedding,
-            "dynamic": StaticEmbedding,
-        },
+    embedding_registry = {
+        "tsp": TSPInitEmbedding,
+        "atsp": TSPInitEmbedding,
+        "cvrp": VRPInitEmbedding,
+        "sdvrp": VRPInitEmbedding,
+        "pctsp": PCTSPInitEmbedding,
+        "spctsp": PCTSPInitEmbedding,
+        "op": OPInitEmbedding,
+        "dpp": DPPInitEmbedding,
+        "mdpp": MDPPInitEmbedding,
+        "pdp": PDPInitEmbedding,
+        "mtsp": MTSPInitEmbedding,
     }
 
-    assert embedding_type in [
-        "init",
-        "dynamic",
-    ], "Unknown embedding type. Must be one of 'init' or 'dynamic'"
-    env_name = env if isinstance(env, str) else env.name
-    embedding_class = embedding_classes.get(env_name, {}).get(embedding_type, None)
-
-    if embedding_class is None:
-        raise ValueError(f"Unknown environment name '{env_name}'")
+    if env_name not in embedding_registry:
+        raise ValueError(
+            f"Unknown environment name '{env_name}'. Available init embeddings: {embedding_registry.keys()}"
+        )
 
-    return embedding_class(**config)
+    return embedding_registry[env_name](**config)
 
 
 class TSPInitEmbedding(nn.Module):
+    """Initial embedding for the Traveling Salesman Problems (TSP).
+    Embed the following node features to the embedding space:
+        - locs: x, y coordinates of the cities
+    """
+
     def __init__(self, embedding_dim):
         super(TSPInitEmbedding, self).__init__()
         node_dim = 2  # x, y
         self.init_embed = nn.Linear(node_dim, embedding_dim)
 
     def forward(self, td):
         out = self.init_embed(td["locs"])
         return out
 
 
 class VRPInitEmbedding(nn.Module):
+    """Initial embedding for the Vehicle Routing Problems (VRP).
+    Embed the following node features to the embedding space:
+        - locs: x, y coordinates of the nodes (depot and customers separately)
+        - demand: demand of the customers
+    """
+
     def __init__(self, embedding_dim):
         super(VRPInitEmbedding, self).__init__()
         node_dim = 3  # x, y, demand
         self.init_embed = nn.Linear(node_dim, embedding_dim)
         self.init_embed_depot = nn.Linear(2, embedding_dim)  # depot embedding
 
     def forward(self, td):
@@ -111,14 +72,22 @@
         )
         # [batch, n_city+1, embedding_dim]
         out = torch.cat((depot_embedding, node_embeddings), -2)
         return out
 
 
 class PCTSPInitEmbedding(nn.Module):
+    """Initial embedding for the Prize Collecting Traveling Salesman Problems (PCTSP).
+    Embed the following node features to the embedding space:
+        - locs: x, y coordinates of the nodes (depot and customers separately)
+        - expected_prize: expected prize for visiting the customers.
+            In PCTSP, this is the actual prize. In SPCTSP, this is the expected prize.
+        - penalty: penalty for not visiting the customers
+    """
+
     def __init__(self, embedding_dim):
         super(PCTSPInitEmbedding, self).__init__()
         node_dim = 4  # x, y, prize, penalty
         self.init_embed = nn.Linear(node_dim, embedding_dim)
         self.init_embed_depot = nn.Linear(2, embedding_dim)
 
     def forward(self, td):
@@ -136,33 +105,49 @@
         )
         # batch, n_city+1, embedding_dim
         out = torch.cat((depot_embedding, node_embeddings), -2)
         return out
 
 
 class OPInitEmbedding(nn.Module):
+    """Initial embedding for the Orienteering Problems (OP).
+    Embed the following node features to the embedding space:
+        - locs: x, y coordinates of the nodes (depot and customers separately)
+        - prize: prize for visiting the customers
+    """
+
     def __init__(self, embedding_dim):
         super(OPInitEmbedding, self).__init__()
         node_dim = 3  # x, y, prize
         self.init_embed = nn.Linear(node_dim, embedding_dim)
         self.init_embed_depot = nn.Linear(2, embedding_dim)  # depot embedding
 
     def forward(self, td):
-        # batch, 1, 2 -> batch, 1, embedding_dim
-        depot_embedding = self.init_embed_depot(td["depot"])[:, None, :]
-        # [batch, n_city, 2, batch, n_city, 1, batch, n_city, 1]  -> batch, n_city, embedding_dim
+        depot, cities = td["locs"][:, :1, :], td["locs"][:, 1:, :]
+        depot_embedding = self.init_embed_depot(depot)
         node_embeddings = self.init_embed(
-            torch.cat((td["locs"], td["prize"][:, :, None]), -1)
+            torch.cat(
+                (
+                    cities,
+                    td["prize"][..., 1:, None],  # exclude depot
+                ),
+                -1,
+            )
         )
-        # batch, n_city+1, embedding_dim
-        out = torch.cat((depot_embedding, node_embeddings[..., 1:, :]), 1)
+        out = torch.cat((depot_embedding, node_embeddings), -2)
         return out
 
 
 class DPPInitEmbedding(nn.Module):
+    """Initial embedding for the Decap Placement Problem (DPP), EDA (electronic design automation).
+    Embed the following node features to the embedding space:
+        - locs: x, y coordinates of the nodes (cells)
+        - probe: index of the (single) probe cell. We embed the euclidean distance from the probe to all cells.
+    """
+
     def __init__(self, embedding_dim):
         super(DPPInitEmbedding, self).__init__()
         node_dim = 2  # x, y
         self.init_embed = nn.Linear(node_dim, embedding_dim // 2)  # locs
         self.init_embed_probe = nn.Linear(1, embedding_dim // 2)  # probe
 
     def forward(self, td):
@@ -175,14 +160,20 @@
     def _distance_probe(self, locs, probe):
         # Euclidean distance from probe to all locations
         probe_loc = torch.gather(locs, 1, probe.unsqueeze(-1).expand(-1, -1, 2))
         return torch.norm(locs - probe_loc, dim=-1).unsqueeze(-1)
 
 
 class MDPPInitEmbedding(nn.Module):
+    """Initial embedding for the Multi-port Placement Problem (MDPP), EDA (electronic design automation).
+    Embed the following node features to the embedding space:
+        - locs: x, y coordinates of the nodes (cells)
+        - probe: indexes of the probe cells (multiple). We embed the euclidean distance of each cell to the closest probe.
+    """
+
     def __init__(self, embedding_dim):
         super(MDPPInitEmbedding, self).__init__()
         node_dim = 2  # x, y
         self.init_embed = nn.Linear(node_dim, embedding_dim)  # locs
         self.init_embed_probe_distance = nn.Linear(1, embedding_dim)  # probe_distance
         self.project_out = nn.Linear(embedding_dim * 2, embedding_dim)
 
@@ -199,14 +190,20 @@
 
         return self.project_out(
             torch.cat([node_embeddings, min_probe_dist_embedding], -1)
         )
 
 
 class PDPInitEmbedding(nn.Module):
+    """Initial embedding for the Pickup and Delivery Problem (PDP).
+    Embed the following node features to the embedding space:
+        - locs: x, y coordinates of the nodes (depot, pickups and deliveries separately)
+           Note that pickups and deliveries are interleaved in the input.
+    """
+
     def __init__(self, embedding_dim):
         super(PDPInitEmbedding, self).__init__()
         node_dim = 2  # x, y
         self.init_embed_depot = nn.Linear(2, embedding_dim)
         self.init_embed_pick = nn.Linear(node_dim * 2, embedding_dim)
         self.init_embed_delivery = nn.Linear(node_dim, embedding_dim)
 
@@ -221,79 +218,23 @@
         pick_embeddings = self.init_embed_pick(pick_feats)
         delivery_embeddings = self.init_embed_delivery(delivery_feats)
         # concatenate on graph size dimension
         return torch.cat([depot_embeddings, pick_embeddings, delivery_embeddings], -2)
 
 
 class MTSPInitEmbedding(nn.Module):
+    """Initial embedding for the Multiple Traveling Salesman Problem (mTSP).
+    Embed the following node features to the embedding space:
+        - locs: x, y coordinates of the nodes (depot, cities)
+    """
+
     def __init__(self, embedding_dim):
         """NOTE: new made by Fede. May need to be checked"""
         super(MTSPInitEmbedding, self).__init__()
         node_dim = 2  # x, y
         self.init_embed = nn.Linear(node_dim, embedding_dim)
         self.init_embed_depot = nn.Linear(2, embedding_dim)  # depot embedding
 
     def forward(self, td):
         depot_embedding = self.init_embed_depot(td["locs"][..., 0:1, :])
         node_embedding = self.init_embed(td["locs"][..., 1:, :])
         return torch.cat([depot_embedding, node_embedding], -2)
-
-
-class SDVRPDynamicEmbedding(nn.Module):
-    def __init__(self, embedding_dim):
-        super(SDVRPDynamicEmbedding, self).__init__()
-        self.projection = nn.Linear(1, 3 * embedding_dim, bias=False)
-
-    def forward(self, td):
-        demands_with_depot = td["demand_with_depot"][..., None].clone()
-        demands_with_depot[..., 0, :] = 0
-        glimpse_key_dynamic, glimpse_val_dynamic, logit_key_dynamic = self.projection(
-            demands_with_depot
-        ).chunk(3, dim=-1)
-        return glimpse_key_dynamic, glimpse_val_dynamic, logit_key_dynamic
-
-
-class DPPDynamicEmbedding(nn.Module):
-    """Dynamic embedding for DPP. Features include:
-    1. location of placed decaps (to know where to place the next one)
-    2. decap density around each location (to know if an area has been covered)
-    """
-
-    def __init__(self, embedding_dim, radius=0.4, scale=20):
-        super(DPPDynamicEmbedding, self).__init__()
-        self.radius = radius
-        self.scale = scale
-        self.projection = nn.Linear(2, 3 * embedding_dim, bias=False)
-
-    def forward(self, td):
-        unavailable, keepouts, probes = (
-            ~td["action_mask"].clone(),
-            td["keepout"].clone(),
-            td["probe"].clone(),
-        )
-
-        placed_decaps = unavailable & ~(keepouts | probes)
-        decap_density = (
-            self._calculate_decap_density(td["locs"], placed_decaps, radius=self.radius)
-            / self.scale
-        )
-        glimpse_key_dynamic, glimpse_val_dynamic, logit_key_dynamic = self.projection(
-            torch.stack([placed_decaps.float(), decap_density.float()], dim=-1)
-        ).chunk(3, dim=-1)
-        return glimpse_key_dynamic, glimpse_val_dynamic, logit_key_dynamic
-
-    @staticmethod
-    def _calculate_decap_density(x, is_target, radius=0.4):
-        dists = torch.cdist(x, x, p=2)
-        infinity = torch.full_like(dists, float("inf"))
-        mask = ~is_target.unsqueeze(1).expand_as(dists)
-        dists_masked = torch.where(mask, infinity, dists)
-        density = (dists_masked < radius).sum(dim=-1)
-        return density
-
-
-class StaticEmbedding(nn.Module):
-    def __init__(self, embedding_dim):
-        super(StaticEmbedding, self).__init__()
-
-    def forward(self, td):
-        return 0, 0, 0
```

### Comparing `rl4co-0.0.5/rl4co/models/nn/flash_attention.py` & `rl4co-0.0.6/rl4co/models/nn/flash_attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/nn/graph/gat.py` & `rl4co-0.0.6/rl4co/models/nn/graph/gat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch.nn as nn
 
 from rl4co.models.nn.attention import MultiHeadAttention, NativeFlashMHA
-from rl4co.models.nn.env_embedding import env_init_embedding
+from rl4co.models.nn.env_embeddings import env_init_embedding
 from rl4co.models.nn.ops import Normalization, SkipConnection
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class MultiHeadAttentionLayer(nn.Sequential):
@@ -56,15 +56,15 @@
         disable_init_embedding=False,
     ):
         super(GraphAttentionEncoder, self).__init__()
 
         # To map input to embedding space
         if not disable_init_embedding:
             self.init_embedding = env_init_embedding(
-                env, {"embedding_dim": embedding_dim}
+                env.name, {"embedding_dim": embedding_dim}
             )
         else:
             log.warning("Disabling init embedding manually for GraphAttentionEncoder")
             self.init_embedding = nn.Identity()  # do nothing
 
         self.layers = nn.Sequential(
             *(
```

### Comparing `rl4co-0.0.5/rl4co/models/nn/graph/gcn.py` & `rl4co-0.0.6/rl4co/models/nn/graph/gcn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from torch_geometric.data import Batch, Data
 from torch_geometric.nn import GCNConv
 
-from rl4co.models.nn.env_embedding import env_init_embedding
+from rl4co.models.nn.env_embeddings import env_init_embedding
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class GCNEncoder(nn.Module):
     def __init__(
@@ -19,15 +19,17 @@
         num_nodes,
         num_gcn_layer,
         self_loop=False,
         residual=True,
     ):
         super(GCNEncoder, self).__init__()
         # Define the init embedding
-        self.init_embedding = env_init_embedding(env, {"embedding_dim": embedding_dim})
+        self.init_embedding = env_init_embedding(
+            env.name, {"embedding_dim": embedding_dim}
+        )
 
         # Generate edge index for a fully connected graph
         adj_matrix = torch.ones(num_nodes, num_nodes)
         if self_loop:
             adj_matrix.fill_diagonal_(0)  # No self-loops
         self.edge_index = torch.permute(torch.nonzero(adj_matrix), (1, 0))
```

### Comparing `rl4co-0.0.5/rl4co/models/nn/graph/mpnn.py` & `rl4co-0.0.6/rl4co/models/nn/graph/mpnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import torch.nn as nn
 
 from torch_geometric.data import Batch, Data
 from torch_geometric.nn import MessagePassing
 
-from rl4co.models.nn.env_embedding import env_init_embedding
+from rl4co.models.nn.env_embeddings import env_init_embedding
 from rl4co.models.nn.mlp import MLP
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class MessagePassingLayer(MessagePassing):
@@ -72,15 +72,17 @@
     ):
         """
         Note:
             - Support fully connected graph for now.
         """
         super(MessagePassingEncoder, self).__init__()
         # Define the init embedding
-        self.init_embedding = env_init_embedding(env, {"embedding_dim": embedding_dim})
+        self.init_embedding = env_init_embedding(
+            env.name, {"embedding_dim": embedding_dim}
+        )
 
         # Generate edge index for a fully connected graph
         adj_matrix = torch.ones(num_nodes, num_nodes)
         if self_loop:
             adj_matrix.fill_diagonal_(0)  # No self-loops
         self.edge_index = torch.permute(torch.nonzero(adj_matrix), (1, 0))
```

### Comparing `rl4co-0.0.5/rl4co/models/nn/mlp.py` & `rl4co-0.0.6/rl4co/models/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/nn/ops.py` & `rl4co-0.0.6/rl4co/models/nn/ops.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/nn/utils.py` & `rl4co-0.0.6/rl4co/models/nn/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/rl/ppo/model.py` & `rl4co-0.0.6/rl4co/models/rl/ppo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/rl/ppo/task.py` & `rl4co-0.0.6/rl4co/models/rl/ppo/task.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/rl/reinforce/base.py` & `rl4co-0.0.6/rl4co/models/rl/reinforce/base.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/rl/reinforce/baselines.py` & `rl4co-0.0.6/rl4co/models/rl/reinforce/baselines.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,19 +92,19 @@
         self.baseline.setup(*args, **kw)
 
     def eval(self, td, reward):
         if self.alpha == 1:
             return self.baseline.eval(td, reward)
         if self.alpha == 0:
             return self.warmup_baseline.eval(td, reward)
-        v, l = self.baseline.eval(td, reward)
-        vw, lw = self.warmup_baseline.eval(td, reward)
+        v_b, l_b = self.baseline.eval(td, reward)
+        v_wb, l_wb = self.warmup_baseline.eval(td, reward)
         # Return convex combination of baseline and of loss
-        return self.alpha * v + (1 - self.alpha) * vw, self.alpha * l + (
-            1 - self.alpha * lw
+        return self.alpha * v_b + (1 - self.alpha) * v_wb, self.alpha * l_b + (
+            1 - self.alpha * l_wb
         )
 
     def epoch_callback(self, *args, **kw):
         # Need to call epoch callback of inner model (also after first epoch if we have not used it)
         self.baseline.epoch_callback(*args, **kw)
         self.alpha = (kw["epoch"] + 1) / float(self.n_epochs)
         if kw["epoch"] < self.n_epochs:
@@ -199,7 +199,21 @@
         """Wrap the dataset in a baseline dataset"""
         rewards = (
             self.rollout(self.model, env, batch_size, device, dataset=dataset)
             .detach()
             .cpu()
         )
         return ExtraKeyDataset(dataset, rewards)
+
+    def __getstate__(self):
+        """Do not include datasets in state to avoid pickling issues"""
+        state = self.__dict__.copy()
+        try:
+            del state["dataset"]
+        except KeyError:
+            pass
+        return state
+
+    def __setstate__(self, state):
+        """Restore datasets after unpickling. Will be restored in setup"""
+        self.__dict__.update(state)
+        self.dataset = None
```

### Comparing `rl4co-0.0.5/rl4co/models/rl/reinforce/critic.py` & `rl4co-0.0.6/rl4co/models/rl/reinforce/critic.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/am/decoder.py` & `rl4co-0.0.6/rl4co/models/zoo/am/decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 import torch
 import torch.nn as nn
 
 from einops import rearrange
 
 from rl4co.models.nn.attention import LogitAttention
-from rl4co.models.nn.env_context import env_context
-from rl4co.models.nn.env_embedding import env_dynamic_embedding
+from rl4co.models.nn.env_embeddings import env_context_embedding, env_dynamic_embedding
 from rl4co.models.nn.utils import decode_probs
 from rl4co.utils.ops import batchify, select_start_nodes, unbatchify
 
 
 @dataclass
 class PrecomputedCache:
     node_embeddings: torch.Tensor
@@ -36,17 +35,19 @@
 
         self.env = env
         self.embedding_dim = embedding_dim
         self.num_heads = num_heads
 
         assert embedding_dim % num_heads == 0
 
-        self.context = env_context(self.env, {"embedding_dim": embedding_dim})
+        self.context = env_context_embedding(
+            self.env.name, {"embedding_dim": embedding_dim}
+        )
         self.dynamic_embedding = env_dynamic_embedding(
-            self.env, {"embedding_dim": embedding_dim}
+            self.env.name, {"embedding_dim": embedding_dim}
         )
 
         # For each node we compute (glimpse key, glimpse value, logit key) so 3 * embedding_dim
         self.project_node_embeddings = nn.Linear(
             embedding_dim, 3 * embedding_dim, bias=False
         )
         self.project_fixed_context = nn.Linear(embedding_dim, embedding_dim, bias=False)
```

### Comparing `rl4co-0.0.5/rl4co/models/zoo/am/model.py` & `rl4co-0.0.6/rl4co/models/zoo/am/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/am/policy.py` & `rl4co-0.0.6/rl4co/models/zoo/am/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/amppo/decoder.py` & `rl4co-0.0.6/rl4co/models/zoo/amppo/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/amppo/model.py` & `rl4co-0.0.6/rl4co/models/zoo/amppo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/amppo/policy.py` & `rl4co-0.0.6/rl4co/models/zoo/amppo/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/ham/attention.py` & `rl4co-0.0.6/rl4co/models/zoo/ham/attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/ham/encoder.py` & `rl4co-0.0.6/rl4co/models/zoo/ham/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch.nn as nn
 
-from rl4co.models.nn.env_embedding import env_init_embedding
+from rl4co.models.nn.env_embeddings import env_init_embedding
 from rl4co.models.nn.graph.gat import Normalization, SkipConnection
 from rl4co.models.zoo.ham.attention import HeterogenousMHA
 
 
 class HeterogeneuousMHALayer(nn.Sequential):
     def __init__(
         self,
@@ -39,15 +39,17 @@
         normalization="batch",
         feed_forward_hidden=512,
         force_flash_attn=False,
     ):
         super(GraphHeterogeneousAttentionEncoder, self).__init__()
 
         # Map input to embedding space
-        self.init_embedding = env_init_embedding(env, {"embedding_dim": embedding_dim})
+        self.init_embedding = env_init_embedding(
+            env.name, {"embedding_dim": embedding_dim}
+        )
 
         self.layers = nn.Sequential(
             *(
                 HeterogeneuousMHALayer(
                     num_heads,
                     embedding_dim,
                     feed_forward_hidden,
```

### Comparing `rl4co-0.0.5/rl4co/models/zoo/ham/model.py` & `rl4co-0.0.6/rl4co/models/zoo/ham/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/ham/policy.py` & `rl4co-0.0.6/rl4co/models/zoo/ham/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/mdam/decoder.py` & `rl4co-0.0.6/rl4co/models/zoo/mdam/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from dataclasses import dataclass
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from rl4co.models.nn.attention import LogitAttention
-from rl4co.models.nn.env_context import env_context
-from rl4co.models.nn.env_embedding import env_dynamic_embedding
+from rl4co.models.nn.env_embeddings import env_context_embedding, env_dynamic_embedding
 from rl4co.models.nn.utils import decode_probs, get_log_likelihood
 
 
 @dataclass
 class PrecomputedCache:
     node_embeddings: torch.Tensor
     graph_context: torch.Tensor
@@ -49,15 +48,15 @@
 
         self.W_placeholder = nn.Parameter(torch.Tensor(2 * embedding_dim))
         self.W_placeholder.data.uniform_(
             -1, 1
         )  # Placeholder should be in range of activations
 
         self.context = [
-            env_context(env.name, {"embedding_dim": embedding_dim})
+            env_context_embedding(env.name, {"embedding_dim": embedding_dim})
             for _ in range(num_paths)
         ]
 
         self.project_node_embeddings = [
             nn.Linear(embedding_dim, 3 * embedding_dim, device=env.device, bias=False)
             for _ in range(num_paths)
         ]
@@ -156,14 +155,15 @@
             _V = V.clone()
             _h_old = h_old.clone()
 
             outputs, actions = [], []
             fixed = self._precompute(_encoded_inputs, path_index=i)
 
             j = 0
+            mask, mask_first = None, None  # dummy, we get them during the steps
             while not (self.shrink_size is None and td_list[i]["done"].all()):
                 if j > 1 and j % self.eg_step_gap == 0:
                     if not self.is_vrp:
                         mask_attn = mask ^ mask_first
                     else:
                         mask_attn = mask
                     _encoded_inputs, _ = self.embedder.change(
```

### Comparing `rl4co-0.0.5/rl4co/models/zoo/mdam/encoder.py` & `rl4co-0.0.6/rl4co/models/zoo/mdam/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/mdam/model.py` & `rl4co-0.0.6/rl4co/models/zoo/mdam/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/mdam/policy.py` & `rl4co-0.0.6/rl4co/models/zoo/mdam/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch.nn as nn
 
 from tensordict import TensorDict
 from torchrl.envs import EnvBase
 
-from rl4co.models.nn.env_embedding import env_init_embedding
+from rl4co.models.nn.env_embeddings import env_init_embedding
 from rl4co.models.zoo.mdam.decoder import Decoder
 from rl4co.models.zoo.mdam.encoder import GraphAttentionEncoder
 
 
 class MDAMPolicy(nn.Module):
     """
     Args:
```

### Comparing `rl4co-0.0.5/rl4co/models/zoo/pomo/augmentations.py` & `rl4co-0.0.6/rl4co/models/zoo/pomo/augmentations.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/pomo/decoder.py` & `rl4co-0.0.6/rl4co/models/zoo/pomo/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 import torch
 import torch.nn as nn
 
 from einops import rearrange
 
 from rl4co.models.nn.attention import LogitAttention
-from rl4co.models.nn.env_context import env_context
-from rl4co.models.nn.env_embedding import env_dynamic_embedding
+from rl4co.models.nn.env_embeddings import env_context_embedding, env_dynamic_embedding
 from rl4co.models.nn.utils import decode_probs
 from rl4co.utils import get_pylogger
 from rl4co.utils.ops import batchify, select_start_nodes, unbatchify
 
 log = get_pylogger(__name__)
 
 
@@ -29,17 +28,19 @@
 
         self.env = env
         self.embedding_dim = embedding_dim
         self.num_heads = num_heads
 
         assert embedding_dim % num_heads == 0
 
-        self.context = env_context(self.env, {"embedding_dim": embedding_dim})
+        self.context = env_context_embedding(
+            self.env.name, {"embedding_dim": embedding_dim}
+        )
         self.dynamic_embedding = env_dynamic_embedding(
-            self.env, {"embedding_dim": embedding_dim}
+            self.env.name, {"embedding_dim": embedding_dim}
         )
 
         # For each node we compute (glimpse key, glimpse value, logit key) so 3 * embedding_dim
         self.project_node_embeddings = nn.Linear(
             embedding_dim, 3 * embedding_dim, bias=False
         )
         self.project_fixed_context = nn.Linear(embedding_dim, embedding_dim, bias=False)
```

### Comparing `rl4co-0.0.5/rl4co/models/zoo/pomo/model.py` & `rl4co-0.0.6/rl4co/models/zoo/pomo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/pomo/policy.py` & `rl4co-0.0.6/rl4co/models/zoo/pomo/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/ptrnet/critic.py` & `rl4co-0.0.6/rl4co/models/zoo/ptrnet/critic.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/ptrnet/decoder.py` & `rl4co-0.0.6/rl4co/models/zoo/ptrnet/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/ptrnet/encoder.py` & `rl4co-0.0.6/rl4co/models/zoo/ptrnet/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/ptrnet/model.py` & `rl4co-0.0.6/rl4co/models/zoo/ptrnet/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/ptrnet/policy.py` & `rl4co-0.0.6/rl4co/models/zoo/ptrnet/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/symnco/augmentations.py` & `rl4co-0.0.6/rl4co/models/zoo/symnco/augmentations.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/symnco/decoder.py` & `rl4co-0.0.6/rl4co/models/zoo/symnco/decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 import torch
 import torch.nn as nn
 
 from einops import rearrange
 
 from rl4co.models.nn.attention import LogitAttention
-from rl4co.models.nn.env_context import env_context
-from rl4co.models.nn.env_embedding import env_dynamic_embedding
+from rl4co.models.nn.env_embeddings import env_context_embedding, env_dynamic_embedding
 from rl4co.models.nn.utils import decode_probs
 from rl4co.utils import get_pylogger
 from rl4co.utils.ops import batchify, select_start_nodes, unbatchify
 
 log = get_pylogger(__name__)
 
 
@@ -38,17 +37,19 @@
 
         self.env = env
         self.embedding_dim = embedding_dim
         self.num_heads = num_heads
 
         assert embedding_dim % num_heads == 0
 
-        self.context = env_context(self.env, {"embedding_dim": embedding_dim})
+        self.context = env_context_embedding(
+            self.env.name, {"embedding_dim": embedding_dim}
+        )
         self.dynamic_embedding = env_dynamic_embedding(
-            self.env, {"embedding_dim": embedding_dim}
+            self.env.name, {"embedding_dim": embedding_dim}
         )
 
         # For each node we compute (glimpse key, glimpse value, logit key) so 3 * embedding_dim
         self.project_node_embeddings = nn.Linear(
             embedding_dim, 3 * embedding_dim, bias=False
         )
         self.project_fixed_context = nn.Linear(embedding_dim, embedding_dim, bias=False)
```

### Comparing `rl4co-0.0.5/rl4co/models/zoo/symnco/losses.py` & `rl4co-0.0.6/rl4co/models/zoo/symnco/losses.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/symnco/model.py` & `rl4co-0.0.6/rl4co/models/zoo/symnco/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/models/zoo/symnco/policy.py` & `rl4co-0.0.6/rl4co/models/zoo/symnco/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/tasks/eval.py` & `rl4co-0.0.6/rl4co/tasks/eval.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/tasks/rl4co.py` & `rl4co-0.0.6/rl4co/tasks/rl4co.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,34 @@
     Base LightningModule for Neural Combinatorial Optimization
     Args:
         cfg: Hydra config
         env: Environment to use overridding the config. If None, instantiate from config
         model: Model to use overridding the config. If None, instantiate from config
     """
 
-    def __init__(self, cfg: DictConfig, env: RL4COEnvBase = None, model: nn.Module = None):
+    def __init__(
+        self, cfg: DictConfig, env: RL4COEnvBase = None, model: nn.Module = None
+    ):
+        super().__init__()
+
+        # this line ensures params passed to LightningModule will be saved to ckpt
+        # it also allows to access params with 'self.hparams' attribute
+        # self.save_hyperparameters("env", "model", logger=False)
+        self.save_hyperparameters(logger=False)
+
         if cfg.get("train", {}).get("disable_profiling", True):
             # Disable profiling executor. This reduces memory and increases speed.
             # https://github.com/HazyResearch/safari/blob/111d2726e7e2b8d57726b7a8b932ad8a4b2ad660/train.py#LL124-L129C17
             try:
                 torch._C._jit_set_profiling_executor(False)
                 torch._C._jit_set_profiling_mode(False)
             except AttributeError:
                 pass
 
-        super().__init__()
-        # this line ensures params passed to LightningModule will be saved to ckpt
-        # it also allows to access params with 'self.hparams' attribute
         cfg = DictConfig(cfg) if not isinstance(cfg, DictConfig) else cfg
-        self.save_hyperparameters(cfg)
         self.cfg = cfg
 
         # Instantiate environment, model and metrics
         self.env = env if env is not None else self.instantiate_env()
         self.model = model if model is not None else self.instantiate_model()
         self.instantiate_metrics()
```

### Comparing `rl4co-0.0.5/rl4co/utils/callbacks/speed_monitor.py` & `rl4co-0.0.6/rl4co/utils/callbacks/speed_monitor.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/download/downloader.py` & `rl4co-0.0.6/rl4co/utils/download/downloader.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/download/gdrive.py` & `rl4co-0.0.6/rl4co/utils/download/gdrive.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/download/s3.py` & `rl4co-0.0.6/rl4co/utils/download/s3.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/helpers.py` & `rl4co-0.0.6/rl4co/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/instantiators.py` & `rl4co-0.0.6/rl4co/utils/instantiators.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/lightning.py` & `rl4co-0.0.6/rl4co/utils/lightning.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/logging_utils.py` & `rl4co-0.0.6/rl4co/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/ops.py` & `rl4co-0.0.6/rl4co/utils/ops.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/param_grouping.py` & `rl4co-0.0.6/rl4co/utils/param_grouping.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/pylogger.py` & `rl4co-0.0.6/rl4co/utils/pylogger.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/rich_utils.py` & `rl4co-0.0.6/rl4co/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/test_utils.py` & `rl4co-0.0.6/rl4co/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/transfer.py` & `rl4co-0.0.6/rl4co/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co/utils/utils.py` & `rl4co-0.0.6/rl4co/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/rl4co.egg-info/PKG-INFO` & `rl4co-0.0.6/rl4co.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.0.5
+Version: 0.0.6
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rl4co-0.0.5/rl4co.egg-info/SOURCES.txt` & `rl4co-0.0.6/rl4co.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,22 @@
 rl4co/envs/sdvrp.py
 rl4co/envs/spctsp.py
 rl4co/envs/tsp.py
 rl4co/envs/common/base.py
 rl4co/envs/common/utils.py
 rl4co/models/__init__.py
 rl4co/models/nn/attention.py
-rl4co/models/nn/env_context.py
-rl4co/models/nn/env_embedding.py
 rl4co/models/nn/flash_attention.py
 rl4co/models/nn/mlp.py
 rl4co/models/nn/ops.py
 rl4co/models/nn/utils.py
+rl4co/models/nn/env_embeddings/__init__.py
+rl4co/models/nn/env_embeddings/context.py
+rl4co/models/nn/env_embeddings/dynamic.py
+rl4co/models/nn/env_embeddings/init.py
 rl4co/models/nn/graph/gat.py
 rl4co/models/nn/graph/gcn.py
 rl4co/models/nn/graph/mpnn.py
 rl4co/models/rl/ppo/model.py
 rl4co/models/rl/ppo/task.py
 rl4co/models/rl/reinforce/base.py
 rl4co/models/rl/reinforce/baselines.py
```

### Comparing `rl4co-0.0.5/tests/test_envs.py` & `rl4co-0.0.6/tests/test_envs.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/tests/test_models.py` & `rl4co-0.0.6/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.5/tests/test_ops.py` & `rl4co-0.0.6/tests/test_ops.py`

 * *Files identical despite different names*

