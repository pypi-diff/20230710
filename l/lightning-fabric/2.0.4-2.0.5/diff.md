# Comparing `tmp/lightning-fabric-2.0.4.tar.gz` & `tmp/lightning-fabric-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-fabric-2.0.4.tar", last modified: Thu Jun 22 18:25:15 2023, max compression
+gzip compressed data, was "lightning-fabric-2.0.5.tar", last modified: Mon Jul 10 16:11:25 2023, max compression
```

## Comparing `lightning-fabric-2.0.4.tar` & `lightning-fabric-2.0.5.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.352394 lightning-fabric-2.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.340394 lightning-fabric-2.0.4/.actions/
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-22 18:25:15.352394 lightning-fabric-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.336394 lightning-fabric-2.0.4/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.340394 lightning-fabric-2.0.4/requirements/fabric/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/requirements/fabric/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/requirements/fabric/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/requirements/fabric/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/requirements/fabric/strategies.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/requirements/fabric/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 18:25:15.352394 lightning-fabric-2.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.340394 lightning-fabric-2.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.340394 lightning-fabric-2.0.4/src/lightning_fabric/
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-06-22 18:25:14.000000 lightning-fabric-2.0.4/src/lightning_fabric/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-22 18:25:14.000000 lightning-fabric-2.0.4/src/lightning_fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.344394 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/tpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-06-22 18:25:14.000000 lightning-fabric-2.0.4/src/lightning_fabric/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    27286 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    40477 2023-06-22 18:25:14.000000 lightning-fabric-2.0.4/src/lightning_fabric/fabric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.344394 lightning-fabric-2.0.4/src/lightning_fabric/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.344394 lightning-fabric-2.0.4/src/lightning_fabric/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.344394 lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/collective.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/single_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/torch_collective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.344394 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/cluster_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/kubeflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/torchelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.344394 lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/torch_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.348394 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/tpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/tpu_bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.348394 lightning-fabric-2.0.4/src/lightning_fabric/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)    36789 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/dp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.348394 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/single_tpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.352394 lightning-fabric-2.0.4/src/lightning_fabric/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/device_dtype_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/device_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/version.info
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.340394 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.099836 lightning-fabric-2.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/.actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-10 16:11:25.099836 lightning-fabric-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22065 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.087836 lightning-fabric-2.0.5/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/requirements/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/requirements/fabric/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/requirements/fabric/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/requirements/fabric/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/requirements/fabric/strategies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/requirements/fabric/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:11:25.099836 lightning-fabric-2.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/src/lightning_fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27201 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40477 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/src/lightning_fabric/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.095836 lightning-fabric-2.0.5/src/lightning_fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.095836 lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/torch_collective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.095836 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/cluster_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/kubeflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/torchelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.095836 lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/torch_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.095836 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/tpu_bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.095836 lightning-fabric-2.0.5/src/lightning_fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37574 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/dp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15834 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.099836 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/single_tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.099836 lightning-fabric-2.0.5/src/lightning_fabric/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/device_dtype_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/device_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/version.info
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-10 16:11:25.000000 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-07-10 16:11:25.000000 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:11:25.000000 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:11:25.000000 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-10 16:11:25.000000 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 16:11:25.000000 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/version.info
```

### Comparing `lightning-fabric-2.0.4/.actions/assistant.py` & `lightning-fabric-2.0.5/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/LICENSE` & `lightning-fabric-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/PKG-INFO` & `lightning-fabric-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-fabric
-Version: 2.0.4
+Version: 2.0.5
 Summary: UNKNOWN
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -21,17 +21,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: strategies
 Provides-Extra: examples
+Provides-Extra: test
 Provides-Extra: deepspeed
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
@@ -48,15 +48,15 @@
   <a href="#faq">FAQ</a> •
   <a href="#asking-for-help">Help</a> •
   <a href="https://discord.gg/VptPCZkGNa">Discord</a>
 </p>
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning_fabric)](https://pypi.org/project/lightning_fabric/)
 [![PyPI Status](https://badge.fury.io/py/lightning_fabric.svg)](https://badge.fury.io/py/lightning_fabric)
-[![PyPI Status](https://pepy.tech/badge/lightning_fabric)](https://pepy.tech/project/lightning_fabric)
+[![PyPI Status](https://pepy.tech/badge/lightning-fabric)](https://pepy.tech/project/lightning-fabric)
 [![Conda](https://img.shields.io/conda/v/conda-forge/lightning_fabric?label=conda&color=success)](https://anaconda.org/conda-forge/lightning_fabric)
 
 </div>
 
 # Lightning Fabric: Expert control.
 
 Run on any device at any scale with expert-level control over PyTorch training loop and scaling strategy. You can even write your own Trainer.
```

### Comparing `lightning-fabric-2.0.4/README.md` & `lightning-fabric-2.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 **The Deep Learning framework to train, deploy, and ship AI products Lightning fast.**
 
 **NEW- Lightning 2.0 is featuring a clean and stable API!!**
 
 ______________________________________________________________________
 
 <p align="center">
-  <a href="https://www.lightning.ai/">Lightning.ai</a> •
+  <a href="https://lightning.ai/">Lightning.ai</a> •
   <a href="https://lightning.ai/docs/pytorch/stable/">PyTorch Lightning</a> •
   <a href="https://lightning.ai/docs/fabric/stable/">Fabric</a> •
   <a href="https://lightning.ai/docs/app/stable/">Lightning Apps</a> •
   <a href="https://pytorch-lightning.readthedocs.io/en/stable/">Docs</a> •
   <a href="#community">Community</a> •
   <a href="https://lightning.ai/docs/pytorch/stable/generated/CONTRIBUTING.html">Contribute</a> •
 </p>
```

### Comparing `lightning-fabric-2.0.4/pyproject.toml` & `lightning-fabric-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [metadata]
-name = "pytorch-lightning"
+name = "lightning"
 author = "Lightning-AI et al."
 url = "https://github.com/Lightning-AI/lightning"
 
 [build-system]
 requires = [
     "setuptools",
     "wheel",
```

### Comparing `lightning-fabric-2.0.4/setup.py` & `lightning-fabric-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/CHANGELOG.md` & `lightning-fabric-2.0.5/src/lightning_fabric/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
 
+## [2.0.5] - 2023-07-07
+
+### Added
+
+- Added validation against misconfigured device selection when using the DeepSpeed strategy ([#17952](https://github.com/Lightning-AI/lightning/pull/17952))
+
+### Changed
+
+- Avoid info message when loading 0 entry point callbacks ([#17990](https://github.com/Lightning-AI/lightning/pull/17990))
+
+### Fixed
+
+- Fixed the emission of a false-positive warning when calling a method on the Fabric-wrapped module that accepts no arguments ([#17875](https://github.com/Lightning-AI/lightning/pull/17875))
+- Fixed check for FSDP's flat parameters in all parameter groups ([#17914](https://github.com/Lightning-AI/lightning/pull/17914))
+- Fixed automatic step tracking in Fabric's CSVLogger ([#17942](https://github.com/Lightning-AI/lightning/pull/17942))
+- Fixed an issue causing the `torch.set_float32_matmul_precision` info message to show multiple times ([#17960](https://github.com/Lightning-AI/lightning/pull/17960))
+- Fixed loading model state when `Fabric.load()` is called after `Fabric.setup()` ([#17997](https://github.com/Lightning-AI/lightning/pull/17997))
+
+
 ## [2.0.4] - 2023-06-22
 
 ### Fixed
 
 - Fixed validation of parameters of `plugins.precision.MixedPrecision` ([#17687](https://github.com/Lightning-AI/lightning/pull/17687))
 - Fixed an issue with hpu imports leading to performance degradation  ([#17788](https://github.com/Lightning-AI/lightning/pull/17788))
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/README.md` & `lightning-fabric-2.0.5/src/lightning_fabric/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   <a href="#faq">FAQ</a> •
   <a href="#asking-for-help">Help</a> •
   <a href="https://discord.gg/VptPCZkGNa">Discord</a>
 </p>
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning_fabric)](https://pypi.org/project/lightning_fabric/)
 [![PyPI Status](https://badge.fury.io/py/lightning_fabric.svg)](https://badge.fury.io/py/lightning_fabric)
-[![PyPI Status](https://pepy.tech/badge/lightning_fabric)](https://pepy.tech/project/lightning_fabric)
+[![PyPI Status](https://pepy.tech/badge/lightning-fabric)](https://pepy.tech/project/lightning-fabric)
 [![Conda](https://img.shields.io/conda/v/conda-forge/lightning_fabric?label=conda&color=success)](https://anaconda.org/conda-forge/lightning_fabric)
 
 </div>
 
 # Lightning Fabric: Expert control.
 
 Run on any device at any scale with expert-level control over PyTorch training loop and scaling strategy. You can even write your own Trainer.
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/__init__.py` & `lightning-fabric-2.0.5/src/lightning_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/__setup__.py` & `lightning-fabric-2.0.5/src/lightning_fabric/__setup__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/__init__.py` & `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/accelerator.py` & `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/cpu.py` & `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/cpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/cuda.py` & `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/cuda.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,14 +333,15 @@
                 if cast(int, val) >= raw_cnt:
                     return idx
     except (OSError, AttributeError):
         return -1
     return len(visible_devices)
 
 
+@lru_cache(1)  # show the warning only ever once
 def _check_cuda_matmul_precision(device: torch.device) -> None:
     if not _TORCH_GREATER_EQUAL_1_12:
         # before 1.12, tf32 was used by default
         return
     major, _ = torch.cuda.get_device_capability(device)
     ampere_or_later = major >= 8  # Ampere and later leverage tensor cores, where this setting becomes useful
     if not ampere_or_later:
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/mps.py` & `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/mps.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/registry.py` & `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/tpu.py` & `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/cli.py` & `lightning-fabric-2.0.5/src/lightning_fabric/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/connector.py` & `lightning-fabric-2.0.5/src/lightning_fabric/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,14 @@
             if self._parallel_devices and len(self._parallel_devices) > 1:
                 return "xla"
             # TODO: lazy initialized device, then here could be self._strategy_flag = "single_tpu_device"
             return SingleTPUStrategy(device=self._parallel_devices[0])  # type: ignore
         if self._num_nodes_flag > 1:
             return "ddp"
         if len(self._parallel_devices) <= 1:
-            # TODO: Change this once gpu accelerator was renamed to cuda accelerator
             if isinstance(self._accelerator_flag, (CUDAAccelerator, MPSAccelerator)) or (
                 isinstance(self._accelerator_flag, str) and self._accelerator_flag in ("cuda", "gpu", "mps")
             ):
                 device = _determine_root_gpu_device(self._parallel_devices)
             else:
                 device = "cpu"
             # TODO: lazy initialized device, then here could be self._strategy_flag = "single_device"
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/fabric.py` & `lightning-fabric-2.0.5/src/lightning_fabric/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/loggers/__init__.py` & `lightning-fabric-2.0.5/src/lightning_fabric/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/loggers/csv_logs.py` & `lightning-fabric-2.0.5/src/lightning_fabric/loggers/csv_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,22 +121,26 @@
             return self._experiment
 
         os.makedirs(self.root_dir, exist_ok=True)
         self._experiment = _ExperimentWriter(log_dir=self.log_dir)
         return self._experiment
 
     @rank_zero_only
-    def log_hyperparams(self, params: Union[Dict[str, Any], Namespace]) -> None:
+    def log_hyperparams(self, params: Union[Dict[str, Any], Namespace]) -> None:  # type: ignore[override]
         raise NotImplementedError("The `CSVLogger` does not yet support logging hyperparameters.")
 
     @rank_zero_only
-    def log_metrics(self, metrics: Dict[str, Union[Tensor, float]], step: Optional[int] = None) -> None:
+    def log_metrics(  # type: ignore[override]
+        self, metrics: Dict[str, Union[Tensor, float]], step: Optional[int] = None
+    ) -> None:
         metrics = _add_prefix(metrics, self._prefix, self.LOGGER_JOIN_CHAR)
+        if step is None:
+            step = len(self.experiment.metrics)
         self.experiment.log_metrics(metrics, step)
-        if step is not None and (step + 1) % self._flush_logs_every_n_steps == 0:
+        if (step + 1) % self._flush_logs_every_n_steps == 0:
             self.save()
 
     @rank_zero_only
     def save(self) -> None:
         super().save()
         self.experiment.save()
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/loggers/logger.py` & `lightning-fabric-2.0.5/src/lightning_fabric/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/loggers/tensorboard.py` & `lightning-fabric-2.0.5/src/lightning_fabric/loggers/tensorboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
                 # TODO(fabric): specify the possible exception
                 except Exception as ex:
                     raise ValueError(
                         f"\n you tried to log {v} which is currently not supported. Try a dict or a scalar/tensor."
                     ) from ex
 
     @rank_zero_only
-    def log_hyperparams(
+    def log_hyperparams(  # type: ignore[override]
         self, params: Union[Dict[str, Any], Namespace], metrics: Optional[Dict[str, Any]] = None
     ) -> None:
         """Record hyperparameters. TensorBoard logs with and without saved hyperparameters are incompatible, the
         hyperparameters are then not displayed in the TensorBoard. Please delete or move the previously saved logs
         to display the new ones with hyperparameters.
 
         Args:
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/__init__.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/collective.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/single_device.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/torch_collective.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/torch_collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/__init__.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/cluster_environment.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/cluster_environment.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/kubeflow.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/kubeflow.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/lightning.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/lightning.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/lsf.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/lsf.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/mpi.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/mpi.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/slurm.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/slurm.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/torchelastic.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/torchelastic.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/xla.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/__init__.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/checkpoint_io.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/torch_io.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/torch_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/xla.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/__init__.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/amp.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/amp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/deepspeed.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/double.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/double.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/fsdp.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/precision.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/tpu.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/tpu_bf16.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/tpu_bf16.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/utils.py` & `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/__init__.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/ddp.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/ddp.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,14 +156,21 @@
         return obj[0]
 
     def get_module_state_dict(self, module: Module) -> Dict[str, Union[Any, Tensor]]:
         if isinstance(module, DistributedDataParallel):
             module = module.module
         return super().get_module_state_dict(module)
 
+    def load_module_state_dict(
+        self, module: Module, state_dict: Dict[str, Union[Any, Tensor]], strict: bool = True
+    ) -> None:
+        if isinstance(module, DistributedDataParallel):
+            module = module.module
+        super().load_module_state_dict(module=module, state_dict=state_dict, strict=strict)
+
     @classmethod
     def register_strategies(cls, strategy_registry: _StrategyRegistry) -> None:
         entries = (
             ("ddp", "popen"),
             ("ddp_spawn", "spawn"),
             ("ddp_fork", "fork"),
             ("ddp_notebook", "fork"),
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/deepspeed.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/deepspeed.py`

 * *Files 2% similar despite different names*

```diff
@@ -564,14 +564,16 @@
 
     def _setup_distributed(self) -> None:
         if not isinstance(self.accelerator, CUDAAccelerator):
             raise RuntimeError(
                 f"The DeepSpeed strategy is only supported on CUDA GPUs but `{self.accelerator.__class__.__name__}`"
                 " is used."
             )
+        assert self.parallel_devices is not None
+        _validate_device_index_selection(self.parallel_devices)
         reset_seed()
         self._set_world_ranks()
         rank_zero_only.rank = self.global_rank
         self._init_deepspeed_distributed()
         if not self._config_initialized:
             self._format_config()
             self._config_initialized = True
@@ -798,7 +800,18 @@
     colliding_keys = deepspeed_internal_keys.intersection(state.keys())
     if colliding_keys:
         rank_zero_warn(
             "Your state has keys that collide with DeepSpeed's internal engine state. This could result in your"
             " values being overwritten by DeepSpeed. Consider changing the name of these keys to something else: "
             + ", ".join(colliding_keys)
         )
+
+
+def _validate_device_index_selection(parallel_devices: List[torch.device]) -> None:
+    selected_device_indices = [device.index for device in parallel_devices]
+    expected_device_indices = list(range(len(parallel_devices)))
+    if selected_device_indices != expected_device_indices:
+        raise RuntimeError(
+            f"The selected device indices {selected_device_indices!r} don't match the local rank values of processes."
+            " If you need to select GPUs at a specific index, set the `CUDA_VISIBLE_DEVICES` environment variable"
+            f" instead. For example: `CUDA_VISIBLE_DEVICES={','.join(str(i) for i in selected_device_indices)}`."
+        )
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/dp.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/dp.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,10 +85,17 @@
         return decision
 
     def get_module_state_dict(self, module: Module) -> Dict[str, Union[Any, Tensor]]:
         if isinstance(module, DataParallel):
             module = module.module
         return super().get_module_state_dict(module)
 
+    def load_module_state_dict(
+        self, module: Module, state_dict: Dict[str, Union[Any, Tensor]], strict: bool = True
+    ) -> None:
+        if isinstance(module, DataParallel):
+            module = module.module
+        super().load_module_state_dict(module=module, state_dict=state_dict, strict=strict)
+
     @classmethod
     def register_strategies(cls, strategy_registry: _StrategyRegistry) -> None:
         strategy_registry.register("dp", cls, description=cls.__class__.__name__)
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/fsdp.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/fsdp.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,12 +348,14 @@
 
     return cpu_offload if isinstance(cpu_offload, CPUOffload) else CPUOffload(offload_params=bool(cpu_offload))
 
 
 def _optimizer_has_flat_params(optimizer: Optimizer) -> bool:
     _FSDP_FLATTENED = "_fsdp_flattened"
     if _TORCH_GREATER_EQUAL_1_13:
-        return any(getattr(param, _FSDP_FLATTENED, False) for param in optimizer.param_groups[0]["params"])
+        return any(
+            getattr(param, _FSDP_FLATTENED, False) for group in optimizer.param_groups for param in group["params"]
+        )
 
     from torch.distributed.fsdp import FlatParameter
 
-    return any(isinstance(param, FlatParameter) for param in optimizer.param_groups[0]["params"])
+    return any(isinstance(param, FlatParameter) for group in optimizer.param_groups for param in group["params"])
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/__init__.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/base.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/base.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/launcher.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/multiprocessing.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/subprocess_script.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/subprocess_script.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/xla.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/parallel.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/registry.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/single_device.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/single_tpu.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/single_tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/strategy.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,20 @@
         if self.is_global_zero:
             self.checkpoint_io.save_checkpoint(checkpoint=state, path=path, storage_options=storage_options)
 
     def get_module_state_dict(self, module: Module) -> Dict[str, Union[Any, Tensor]]:
         """Returns model state."""
         return module.state_dict()
 
+    def load_module_state_dict(
+        self, module: Module, state_dict: Dict[str, Union[Any, Tensor]], strict: bool = True
+    ) -> None:
+        """Loads the given state into the model."""
+        module.load_state_dict(state_dict, strict=strict)
+
     def get_optimizer_state(self, optimizer: Optimizer) -> Dict[str, Tensor]:
         """Returns state of an optimizer.
 
         Allows for syncing/collating optimizer state from processes in custom plugins.
         """
         if hasattr(optimizer, "consolidate_state_dict"):
             # there are optimizers like PyTorch's ZeroRedundancyOptimizer that shard their
@@ -275,16 +281,15 @@
             )
 
         for name, obj in state.copy().items():
             if name not in checkpoint:
                 continue
             if isinstance(obj, _Stateful):
                 if isinstance(obj, Module):
-                    # TODO(fabric): Make strict loading configurable
-                    obj.load_state_dict(checkpoint.pop(name), strict=True)
+                    self.load_module_state_dict(module=obj, state_dict=checkpoint.pop(name), strict=True)
                 else:
                     obj.load_state_dict(checkpoint.pop(name))
             else:
                 state[name] = checkpoint.pop(name)
         return checkpoint
 
     def remove_checkpoint(self, filepath: _PATH) -> None:
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/strategies/xla.py` & `lightning-fabric-2.0.5/src/lightning_fabric/strategies/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/__init__.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/apply_func.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/apply_func.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/cloud_io.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/cloud_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/data.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/data.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/device_dtype_mixin.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/device_dtype_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/device_parser.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/device_parser.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/distributed.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/enums.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/exceptions.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/imports.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/logger.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/optimizer.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/optimizer.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/rank_zero.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/rank_zero.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/registry.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,13 +57,14 @@
         factories = iter_entry_points(group)  # type: ignore[assignment]
 
     external_callbacks: List[Any] = []
     for factory in factories:
         callback_factory = factory.load()
         callbacks_list: Union[List[Any], Any] = callback_factory()
         callbacks_list = [callbacks_list] if not isinstance(callbacks_list, list) else callbacks_list
-        _log.info(
-            f"Adding {len(callbacks_list)} callbacks from entry point '{factory.name}':"
-            f" {', '.join(type(cb).__name__ for cb in callbacks_list)}"
-        )
+        if callbacks_list:
+            _log.info(
+                f"Adding {len(callbacks_list)} callbacks from entry point '{factory.name}':"
+                f" {', '.join(type(cb).__name__ for cb in callbacks_list)}"
+            )
         external_callbacks.extend(callbacks_list)
     return external_callbacks
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/seed.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/seed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/types.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/utilities/warnings.py` & `lightning-fabric-2.0.5/src/lightning_fabric/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric/wrappers.py` & `lightning-fabric-2.0.5/src/lightning_fabric/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,19 @@
             # Patch the original_module's forward so we can redirect the arguments back to the real method
             self._original_module.forward = wrapped_forward
             return self.forward(*args, **kwargs)
 
         return call_forward_module
 
     def _validate_method_access(self, name: str, attribute: Any) -> None:
-        if inspect.ismethod(attribute) and self._forward_module != self._original_module:
+        if (
+            inspect.ismethod(attribute)
+            and inspect.signature(attribute).parameters
+            and self._forward_module != self._original_module
+        ):
             warning_cache.warn(
                 f"You are calling the method `{type(self._original_module).__name__}.{name}()` from outside the"
                 " model. This will bypass the wrapper from the strategy and result in incorrect behavior in"
                 f" `.backward()`. You should pass your inputs through `{type(self._original_module)}.forward()`.",
                 category=PossibleUserWarning,
             )
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric.egg-info/PKG-INFO` & `lightning-fabric-2.0.5/src/lightning_fabric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-fabric
-Version: 2.0.4
+Version: 2.0.5
 Summary: UNKNOWN
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -21,17 +21,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: strategies
 Provides-Extra: examples
+Provides-Extra: test
 Provides-Extra: deepspeed
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
@@ -48,15 +48,15 @@
   <a href="#faq">FAQ</a> •
   <a href="#asking-for-help">Help</a> •
   <a href="https://discord.gg/VptPCZkGNa">Discord</a>
 </p>
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning_fabric)](https://pypi.org/project/lightning_fabric/)
 [![PyPI Status](https://badge.fury.io/py/lightning_fabric.svg)](https://badge.fury.io/py/lightning_fabric)
-[![PyPI Status](https://pepy.tech/badge/lightning_fabric)](https://pepy.tech/project/lightning_fabric)
+[![PyPI Status](https://pepy.tech/badge/lightning-fabric)](https://pepy.tech/project/lightning-fabric)
 [![Conda](https://img.shields.io/conda/v/conda-forge/lightning_fabric?label=conda&color=success)](https://anaconda.org/conda-forge/lightning_fabric)
 
 </div>
 
 # Lightning Fabric: Expert control.
 
 Run on any device at any scale with expert-level control over PyTorch training loop and scaling strategy. You can even write your own Trainer.
```

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric.egg-info/SOURCES.txt` & `lightning-fabric-2.0.5/src/lightning_fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.4/src/lightning_fabric.egg-info/requires.txt` & `lightning-fabric-2.0.5/src/lightning_fabric.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [deepspeed:platform_system != "Windows"]
 deepspeed>=0.8.2
 
 [dev]
 torchvision>=0.12.0
 torchmetrics>=0.10.0
 lightning-utilities>=0.8.0
-coverage==7.2.5
+coverage==7.2.7
 pytest==7.3.1
 pytest-cov==4.0.0
 pytest-rerunfailures==10.3
 click==8.1.3
 tensorboardX>=2.2
 
 [dev:platform_system != "Windows"]
@@ -39,13 +39,13 @@
 
 [strategies]
 
 [strategies:platform_system != "Windows"]
 deepspeed>=0.8.2
 
 [test]
-coverage==7.2.5
+coverage==7.2.7
 pytest==7.3.1
 pytest-cov==4.0.0
 pytest-rerunfailures==10.3
 click==8.1.3
 tensorboardX>=2.2
```

