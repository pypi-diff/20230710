# Comparing `tmp/deep_pipe-0.2.3.tar.gz` & `tmp/deep_pipe-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_pipe-0.2.3.tar", last modified: Tue May  9 14:43:41 2023, max compression
+gzip compressed data, was "deep_pipe-0.2.4.tar", last modified: Mon Jul 10 21:49:26 2023, max compression
```

## Comparing `deep_pipe-0.2.3.tar` & `deep_pipe-0.2.4.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.157978 deep_pipe-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-09 14:43:41.157978 deep_pipe-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.149978 deep_pipe-0.2.3/deep_pipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-09 14:43:41.000000 deep_pipe-0.2.3/deep_pipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-09 14:43:41.000000 deep_pipe-0.2.3/deep_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:43:41.000000 deep_pipe-0.2.3/deep_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-09 14:43:41.000000 deep_pipe-0.2.3/deep_pipe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-09 14:43:41.000000 deep_pipe-0.2.3/deep_pipe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 14:43:41.000000 deep_pipe-0.2.3/deep_pipe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.149978 deep_pipe-0.2.3/dpipe/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.153978 deep_pipe-0.2.3/dpipe/batch_iter/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/batch_iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/batch_iter/_pdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/batch_iter/expiration_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/batch_iter/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/batch_iter/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/batch_iter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.153978 deep_pipe-0.2.3/dpipe/config/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/config/commands_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/config/test_locker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.153978 deep_pipe-0.2.3/dpipe/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/dataset/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/dataset/dicom.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/dataset/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/dataset/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.153978 deep_pipe-0.2.3/dpipe/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/experiment/flat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.153978 deep_pipe-0.2.3/dpipe/im/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/hsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/shape_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/shape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/im/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.153978 deep_pipe-0.2.3/dpipe/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/layers/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/layers/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/layers/resblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/layers/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/layers/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.153978 deep_pipe-0.2.3/dpipe/layout/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/layout/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/layout/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.153978 deep_pipe-0.2.3/dpipe/predict/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/predict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/predict/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/predict/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.153978 deep_pipe-0.2.3/dpipe/prototypes/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/prototypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.153978 deep_pipe-0.2.3/dpipe/prototypes/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/prototypes/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/prototypes/strategy/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/prototypes/strategy/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.153978 deep_pipe-0.2.3/dpipe/prototypes/strategy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/prototypes/strategy/tests/optimization_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/prototypes/strategy/tests/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/prototypes/strategy/tests/test_single_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/prototypes/strategy/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.157978 deep_pipe-0.2.3/dpipe/split/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/split/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/split/cv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.157978 deep_pipe-0.2.3/dpipe/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/torch/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/torch/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/torch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:41.157978 deep_pipe-0.2.3/dpipe/train/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/train/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/train/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/train/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/train/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/train/test_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/train/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/dpipe/train/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:43:41.157978 deep_pipe-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-09 14:43:35.000000 deep_pipe-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.410862 deep_pipe-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-10 21:49:26.410862 deep_pipe-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.398862 deep_pipe-0.2.4/deep_pipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-10 21:49:26.000000 deep_pipe-0.2.4/deep_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-10 21:49:26.000000 deep_pipe-0.2.4/deep_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:49:26.000000 deep_pipe-0.2.4/deep_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 21:49:26.000000 deep_pipe-0.2.4/deep_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 21:49:26.000000 deep_pipe-0.2.4/deep_pipe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 21:49:26.000000 deep_pipe-0.2.4/deep_pipe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.402862 deep_pipe-0.2.4/dpipe/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.402862 deep_pipe-0.2.4/dpipe/batch_iter/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/batch_iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/batch_iter/_pdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/batch_iter/expiration_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/batch_iter/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/batch_iter/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/batch_iter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.402862 deep_pipe-0.2.4/dpipe/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/config/commands_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/config/test_locker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.406862 deep_pipe-0.2.4/dpipe/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/dataset/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/dataset/dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/dataset/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/dataset/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.406862 deep_pipe-0.2.4/dpipe/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/experiment/flat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.406862 deep_pipe-0.2.4/dpipe/im/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/hsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/shape_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/shape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/im/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.406862 deep_pipe-0.2.4/dpipe/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/layers/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/layers/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/layers/resblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/layers/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/layers/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.410862 deep_pipe-0.2.4/dpipe/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/layout/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/layout/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.410862 deep_pipe-0.2.4/dpipe/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/predict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/predict/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/predict/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.410862 deep_pipe-0.2.4/dpipe/prototypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/prototypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.410862 deep_pipe-0.2.4/dpipe/prototypes/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/prototypes/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/prototypes/strategy/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/prototypes/strategy/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.410862 deep_pipe-0.2.4/dpipe/prototypes/strategy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/prototypes/strategy/tests/optimization_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/prototypes/strategy/tests/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/prototypes/strategy/tests/test_single_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/prototypes/strategy/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.410862 deep_pipe-0.2.4/dpipe/split/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/split/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/split/cv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.410862 deep_pipe-0.2.4/dpipe/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10107 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/torch/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/torch/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/torch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:49:26.410862 deep_pipe-0.2.4/dpipe/train/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/train/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/train/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/train/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/train/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/train/test_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/train/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/dpipe/train/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:49:26.410862 deep_pipe-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-10 21:49:23.000000 deep_pipe-0.2.4/setup.py
```

### Comparing `deep_pipe-0.2.3/LICENSE` & `deep_pipe-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/PKG-INFO` & `deep_pipe-0.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: deep_pipe
-Version: 0.2.3
+Version: 0.2.4
 Summary: A collection of tools for deep learning experiments
 Home-page: https://github.com/neuro-ml/deep_pipe
 Author: NeuroML Group
 License: MIT
-Download-URL: https://github.com/neuro-ml/deep_pipe/v0.2.3.tar.gz
+Download-URL: https://github.com/neuro-ml/deep_pipe/v0.2.4.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `deep_pipe-0.2.3/deep_pipe.egg-info/PKG-INFO` & `deep_pipe-0.2.4/deep_pipe.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: deep-pipe
-Version: 0.2.3
+Version: 0.2.4
 Summary: A collection of tools for deep learning experiments
 Home-page: https://github.com/neuro-ml/deep_pipe
 Author: NeuroML Group
 License: MIT
-Download-URL: https://github.com/neuro-ml/deep_pipe/v0.2.3.tar.gz
+Download-URL: https://github.com/neuro-ml/deep_pipe/v0.2.4.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `deep_pipe-0.2.3/deep_pipe.egg-info/SOURCES.txt` & `deep_pipe-0.2.4/deep_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/batch_iter/_pdp.py` & `deep_pipe-0.2.4/dpipe/batch_iter/_pdp.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/batch_iter/expiration_pool.py` & `deep_pipe-0.2.4/dpipe/batch_iter/expiration_pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,23 +18,25 @@
         ExpirationPool(pool_size, repetitions),
         # ... here are the values from pool
         # ... other lightweight operations
         # ...
     )
     """
 
-    def __init__(self, pool_size: int, repetitions: int):
-        super().__init__(partial(expiration_pool, pool_size=pool_size, repetitions=repetitions), )
+    def __init__(self, pool_size: int, repetitions: int, iterations: int = 1):
+        super().__init__(partial(expiration_pool, pool_size=pool_size, repetitions=repetitions, iterations=iterations))
 
 
-def expiration_pool(iterable: Iterable, pool_size: int, repetitions: int):
+def expiration_pool(iterable: Iterable, pool_size: int, repetitions: int, iterations: int = 1):
     """
     Caches ``pool_size`` items from ``iterable``.
     The item is removed from cache after it was generated ``repetitions`` times.
     After an item is removed, a new one is extracted from the ``iterable``.
+    Finally, ``iterations`` controls how many values are generated after a new value is added,
+    thus speeding up the pipeline at early stages.
     """
 
     assert pool_size > 0
     assert repetitions > 0
     iterable = enumerate(iterable)
 
     def sample_value():
@@ -47,14 +49,17 @@
         else:
             value_frequency[idx] = [value, frequency]
         return value
 
     value_frequency = {}  # i -> [value, frequency]
     for idx, value in iterable:
         value_frequency[idx] = [value, 0]
-        yield sample_value()
+
+        for _ in range(iterations):
+            if value_frequency:
+                yield sample_value()
 
         while len(value_frequency) >= pool_size:
             yield sample_value()
 
     while len(value_frequency):
         yield sample_value()
```

### Comparing `deep_pipe-0.2.3/dpipe/batch_iter/pipeline.py` & `deep_pipe-0.2.4/dpipe/batch_iter/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,17 @@
 
         return Iterator(stacker)
 
     def close(self):
         """Stop all background processes."""
         self.__exit__(None, None, None)
 
+    def __iter__(self):
+        return self()
+
     def __call__(self):
         if not self.pipeline.pipeline_active:
             self.__enter__()
         return islice(self.pipeline, self.batches_per_epoch)
 
     def __enter__(self):
         self.pipeline.__enter__()
```

### Comparing `deep_pipe-0.2.3/dpipe/batch_iter/sources.py` & `deep_pipe-0.2.4/dpipe/batch_iter/sources.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/batch_iter/utils.py` & `deep_pipe-0.2.4/dpipe/batch_iter/utils.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/checks.py` & `deep_pipe-0.2.4/dpipe/checks.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/commands.py` & `deep_pipe-0.2.4/dpipe/commands.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/config/commands_runner.py` & `deep_pipe-0.2.4/dpipe/config/commands_runner.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/config/test_locker.py` & `deep_pipe-0.2.4/dpipe/config/test_locker.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/dataset/base.py` & `deep_pipe-0.2.4/dpipe/dataset/base.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/dataset/csv.py` & `deep_pipe-0.2.4/dpipe/dataset/csv.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/dataset/dicom.py` & `deep_pipe-0.2.4/dpipe/dataset/dicom.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/dataset/segmentation.py` & `deep_pipe-0.2.4/dpipe/dataset/segmentation.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/dataset/wrappers.py` & `deep_pipe-0.2.4/dpipe/dataset/wrappers.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/experiment/flat.py` & `deep_pipe-0.2.4/dpipe/experiment/flat.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/im/augmentation.py` & `deep_pipe-0.2.4/dpipe/im/augmentation.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/im/axes.py` & `deep_pipe-0.2.4/dpipe/im/axes.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/im/box.py` & `deep_pipe-0.2.4/dpipe/im/box.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/im/dist.py` & `deep_pipe-0.2.4/dpipe/im/dist.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/im/grid.py` & `deep_pipe-0.2.4/dpipe/im/grid.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/im/hsv.py` & `deep_pipe-0.2.4/dpipe/im/hsv.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/im/metrics.py` & `deep_pipe-0.2.4/dpipe/im/metrics.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/im/patch.py` & `deep_pipe-0.2.4/dpipe/im/patch.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/im/preprocessing.py` & `deep_pipe-0.2.4/dpipe/im/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/im/shape_ops.py` & `deep_pipe-0.2.4/dpipe/im/shape_ops.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/im/shape_utils.py` & `deep_pipe-0.2.4/dpipe/im/shape_utils.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/im/utils.py` & `deep_pipe-0.2.4/dpipe/im/utils.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/im/visualize.py` & `deep_pipe-0.2.4/dpipe/im/visualize.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/io.py` & `deep_pipe-0.2.4/dpipe/io.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/itertools.py` & `deep_pipe-0.2.4/dpipe/itertools.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/layers/conv.py` & `deep_pipe-0.2.4/dpipe/layers/conv.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/layers/fpn.py` & `deep_pipe-0.2.4/dpipe/layers/fpn.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/layers/resblock.py` & `deep_pipe-0.2.4/dpipe/layers/resblock.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/layers/shape.py` & `deep_pipe-0.2.4/dpipe/layers/shape.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/layers/structure.py` & `deep_pipe-0.2.4/dpipe/layers/structure.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/layout/base.py` & `deep_pipe-0.2.4/dpipe/layout/base.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/layout/scripts.py` & `deep_pipe-0.2.4/dpipe/layout/scripts.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/predict/functional.py` & `deep_pipe-0.2.4/dpipe/predict/functional.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/predict/shape.py` & `deep_pipe-0.2.4/dpipe/predict/shape.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/prototypes/strategy/optimization.py` & `deep_pipe-0.2.4/dpipe/prototypes/strategy/optimization.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/prototypes/strategy/policy.py` & `deep_pipe-0.2.4/dpipe/prototypes/strategy/policy.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/prototypes/strategy/tests/optimization_fixtures.py` & `deep_pipe-0.2.4/dpipe/prototypes/strategy/tests/optimization_fixtures.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/prototypes/strategy/tests/test_composition.py` & `deep_pipe-0.2.4/dpipe/prototypes/strategy/tests/test_composition.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/prototypes/strategy/tests/test_single_strategy.py` & `deep_pipe-0.2.4/dpipe/prototypes/strategy/tests/test_single_strategy.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/prototypes/strategy/train.py` & `deep_pipe-0.2.4/dpipe/prototypes/strategy/train.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/split/base.py` & `deep_pipe-0.2.4/dpipe/split/base.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/split/cv.py` & `deep_pipe-0.2.4/dpipe/split/cv.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/torch/functional.py` & `deep_pipe-0.2.4/dpipe/torch/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,16 @@
     """
     Calculates the ``criterion`` between the masked ``prediction`` and ``target``.
     ``args`` and ``kwargs`` are passed to ``criterion`` as additional arguments.
 
     If the ``mask`` is empty - returns 0 wrapped in a torch tensor.
     """
     if not mask.any():
-        return torch.tensor(0., requires_grad=True).to(prediction)
+        # https://github.com/neuro-ml/deep_pipe/issues/75
+        return 0 * prediction.flatten()[0]
 
     return criterion(prediction[mask], target[mask], **kwargs)
 
 
 # simply copied from np.moveaxis
 def moveaxis(x: torch.Tensor, source: AxesLike, destination: AxesLike):
     """
```

### Comparing `deep_pipe-0.2.3/dpipe/torch/model.py` & `deep_pipe-0.2.4/dpipe/torch/model.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/torch/utils.py` & `deep_pipe-0.2.4/dpipe/torch/utils.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/train/base.py` & `deep_pipe-0.2.4/dpipe/train/base.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/train/checkpoint.py` & `deep_pipe-0.2.4/dpipe/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/train/logging.py` & `deep_pipe-0.2.4/dpipe/train/logging.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/train/policy.py` & `deep_pipe-0.2.4/dpipe/train/policy.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/train/test_checkpoints.py` & `deep_pipe-0.2.4/dpipe/train/test_checkpoints.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/train/test_policy.py` & `deep_pipe-0.2.4/dpipe/train/test_policy.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/dpipe/train/validator.py` & `deep_pipe-0.2.4/dpipe/train/validator.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.3/setup.py` & `deep_pipe-0.2.4/setup.py`

 * *Files identical despite different names*

