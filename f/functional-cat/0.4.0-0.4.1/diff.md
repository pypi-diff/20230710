# Comparing `tmp/functional-cat-0.4.0.tar.gz` & `tmp/functional-cat-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functional-cat-0.4.0.tar", last modified: Thu Apr  6 18:52:35 2023, max compression
+gzip compressed data, was "functional-cat-0.4.1.tar", last modified: Mon Jul 10 17:57:19 2023, max compression
```

## Comparing `functional-cat-0.4.0.tar` & `functional-cat-0.4.1.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.996507 functional-cat-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-06 18:52:23.000000 functional-cat-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-06 18:52:34.996507 functional-cat-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-06 18:52:23.000000 functional-cat-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.984506 functional-cat-0.4.0/functional_cat/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.984506 functional-cat-0.4.0/functional_cat/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.988506 functional-cat-0.4.0/functional_cat/funcs/dlib/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/dlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/dlib/detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.988506 functional-cat-0.4.0/functional_cat/funcs/glip/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/glip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/glip/glip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.988506 functional-cat-0.4.0/functional_cat/funcs/mmcv/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.988506 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.988506 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.988506 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_datasets/ctw1500.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_datasets/icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_datasets/icdar2017.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_datasets/synthtext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.988506 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/dbnet_r18_fpnc.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/dbnet_r50dcnv2_fpnc.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/dbnetpp_r50dcnv2_fpnc.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/drrg_r50_fpn_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/fcenet_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/fcenet_r50dcnv2_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/ocr_mask_rcnn_r50_fpn_ohem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/ocr_mask_rcnn_r50_fpn_ohem_poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/panet_r18_fpem_ffm.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/panet_r50_fpem_ffm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/psenet_r50_fpnf.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_models/textsnake_r50_fpn_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.992506 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_pipelines/dbnet_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_pipelines/drrg_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_pipelines/fcenet_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_pipelines/maskrcnn_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_pipelines/panet_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_pipelines/psenet_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/det_pipelines/textsnake_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.992506 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/schedule_adadelta_18e.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/schedule_adadelta_5e.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/schedule_adam_600e.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/schedule_adam_step_12e.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/schedule_adam_step_20e.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/schedule_adam_step_5e.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/schedule_adam_step_600e.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/schedule_adam_step_6e.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/schedule_sgd_100k_iters.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/schedule_sgd_1200e.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/schedule_sgd_1500e.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/schedule_sgd_160e.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/_base_/schedules/schedule_sgd_600e.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.992506 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/textdet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/textdet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.992506 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/textdet/psenet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/textdet/psenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/configs/textdet/psenet/psenet_r50_fpnf_600e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/mmcv/mmocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.996507 functional-cat-0.4.0/functional_cat/funcs/onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/onnx/tiny_yolov3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/onnx/yolov4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.996507 functional-cat-0.4.0/functional_cat/funcs/torchvision/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/funcs/torchvision/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-06 18:52:23.000000 functional-cat-0.4.0/functional_cat/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.984506 functional-cat-0.4.0/functional_cat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-06 18:52:34.000000 functional-cat-0.4.0/functional_cat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-06 18:52:34.000000 functional-cat-0.4.0/functional_cat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 18:52:34.000000 functional-cat-0.4.0/functional_cat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-06 18:52:34.000000 functional-cat-0.4.0/functional_cat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-06 18:52:34.000000 functional-cat-0.4.0/functional_cat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-06 18:52:23.000000 functional-cat-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 18:52:34.996507 functional-cat-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-06 18:52:23.000000 functional-cat-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:52:34.996507 functional-cat-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-06 18:52:23.000000 functional-cat-0.4.0/tests/test_dlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-06 18:52:23.000000 functional-cat-0.4.0/tests/test_mmcv.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-06 18:52:23.000000 functional-cat-0.4.0/tests/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-06 18:52:23.000000 functional-cat-0.4.0/tests/test_torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.406034 functional-cat-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.394034 functional-cat-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.394034 functional-cat-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.github/workflows/build-and-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.github/workflows/docker-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.github/workflows/test-catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.github/workflows/unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-10 17:57:08.000000 functional-cat-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-10 17:57:08.000000 functional-cat-0.4.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 17:57:08.000000 functional-cat-0.4.1/Dockerfile.glip
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-10 17:57:08.000000 functional-cat-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 17:57:08.000000 functional-cat-0.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-10 17:57:19.406034 functional-cat-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-10 17:57:08.000000 functional-cat-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-10 17:57:08.000000 functional-cat-0.4.1/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat/funcs/dlib/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/dlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/dlib/detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat/funcs/glip/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/glip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/glip/glip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat/funcs/onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/onnx/tiny_yolov3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/onnx/yolov4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat/funcs/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/funcs/torchvision/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-07-10 17:57:08.000000 functional-cat-0.4.1/functional_cat/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/functional_cat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-10 17:57:19.000000 functional-cat-0.4.1/functional_cat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-10 17:57:19.000000 functional-cat-0.4.1/functional_cat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:57:19.000000 functional-cat-0.4.1/functional_cat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-10 17:57:19.000000 functional-cat-0.4.1/functional_cat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 17:57:19.000000 functional-cat-0.4.1/functional_cat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-10 17:57:08.000000 functional-cat-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/sample_imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)    60686 2023-07-10 17:57:08.000000 functional-cat-0.4.1/sample_imgs/cat.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   123080 2023-07-10 17:57:08.000000 functional-cat-0.4.1/sample_imgs/gang.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    67910 2023-07-10 17:57:08.000000 functional-cat-0.4.1/sample_imgs/letter_box.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    33591 2023-07-10 17:57:08.000000 functional-cat-0.4.1/sample_imgs/mona_lisa.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    23918 2023-07-10 17:57:08.000000 functional-cat-0.4.1/sample_imgs/street_sign.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 17:57:19.406034 functional-cat-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 17:57:08.000000 functional-cat-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.398034 functional-cat-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-10 17:57:08.000000 functional-cat-0.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 17:57:08.000000 functional-cat-0.4.1/tests/test_dlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-10 17:57:08.000000 functional-cat-0.4.1/tests/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-10 17:57:08.000000 functional-cat-0.4.1/tests/test_torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.402034 functional-cat-0.4.1/web/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/.env
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/create_tasks_and_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/netlify.toml
+-rw-r--r--   0 runner    (1001) docker     (123)  1237799 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.402034 functional-cat-0.4.1/web/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/_redirects
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34494 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79636 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:57:19.406034 functional-cat-0.4.1/web/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/AboutPage.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/App.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/App.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/FuncGrid.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/Header.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/HomePage.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/TasksPage.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/TypesPage.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/Wrapper.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/func.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)    34380 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/funcs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/pythonClassMeta.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/react-app-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/reportWebVitals.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/src/setupTests.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-10 17:57:08.000000 functional-cat-0.4.1/web/tsconfig.json
```

### Comparing `functional-cat-0.4.0/LICENSE` & `functional-cat-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.0/PKG-INFO` & `functional-cat-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functional-cat
-Version: 0.4.0
+Version: 0.4.1
 Summary: Catalog of functions
 License: Copyright 2022 Eric O. Korman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
@@ -25,15 +25,14 @@
         
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: torch
 Provides-Extra: onnx
 Provides-Extra: onnx-cpu
 Provides-Extra: onnx-gpu
-Provides-Extra: mmcv
 Provides-Extra: catalog
 Provides-Extra: glip
 Provides-Extra: dlib
 Provides-Extra: test
 License-File: LICENSE
 
 # functional cat
```

### Comparing `functional-cat-0.4.0/functional_cat/data_types.py` & `functional-cat-0.4.1/functional_cat/data_types.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.0/functional_cat/funcs/dlib/detection.py` & `functional-cat-0.4.1/functional_cat/funcs/dlib/detection.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.0/functional_cat/funcs/glip/glip.py` & `functional-cat-0.4.1/functional_cat/funcs/glip/glip.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.0/functional_cat/funcs/onnx/tiny_yolov3.py` & `functional-cat-0.4.1/functional_cat/funcs/onnx/tiny_yolov3.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.0/functional_cat/funcs/onnx/yolov4.py` & `functional-cat-0.4.1/functional_cat/funcs/onnx/yolov4.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,9 +319,9 @@
             Detection(
                 boundary=BoundingPolygon.from_bbox(
                     xmin=pred[0], ymin=pred[1], xmax=pred[2], ymax=pred[3]
                 ),
                 class_label=self.class_labels[int(pred[5])],
                 score=pred[4],
             )
-            for pred in preds
+            for pred in preds if pred[4] >= score_thres
         ]
```

### Comparing `functional-cat-0.4.0/functional_cat/funcs/torchvision/__init__.py` & `functional-cat-0.4.1/functional_cat/funcs/torchvision/__init__.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.0/functional_cat/funcs/torchvision/detection.py` & `functional-cat-0.4.1/functional_cat/funcs/torchvision/detection.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.0/functional_cat/io.py` & `functional-cat-0.4.1/functional_cat/io.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.0/functional_cat/registry.py` & `functional-cat-0.4.1/functional_cat/registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -112,40 +112,14 @@
             gpu_support=True,
             example_img=example_img,
             colab_link="https://colab.research.google.com/drive/1zolH3JooXbAKVPXLGJ6LcDLOFjf-MYYH",
         ),
     ]
 
 
-def create_mmcv_model_metas(
-    example_img: Image.Image = None,
-) -> List[ModelMeta]:
-    mmocr_install_snippet = (
-        "# Please see https://mmocr.readthedocs.io/en/latest/install.html for installing MMOCR.\n"
-        "# Then run:\n"
-        "pip install functional-cat"
-    )
-    from functional_cat.funcs.mmcv import MMOCRTextDetector
-
-    return [
-        ModelMeta(
-            name="ps_ic15",
-            class_=MMOCRTextDetector,
-            constructor_args={"model_name": "PS_IC15"},
-            description="PS_IC15 text detector from MMOCR. See https://mmocr.readthedocs.io/en/stable/textdet_models.html",
-            framework=Framework.MMCV,
-            install_snippet=mmocr_install_snippet,
-            cpu_support=True,
-            gpu_support=True,
-            example_img=example_img,
-            colab_link="https://colab.research.google.com/drive/1k7L7pJCPgltSwLf6N-cW2KvCF5pprU3W",
-        )
-    ]
-
-
 def create_glip_model_metas(
     example_img: Image.Image = None,
 ) -> List[ModelMeta]:
     description = (
         "GLIP is a zero-shot object detector: it can run object detection on arbitrary"
         ' class labels, which here get passed in model instantiation. GLIP-T is the "tiny" version'
         " and GLIP-L is the larger version."
```

### Comparing `functional-cat-0.4.0/functional_cat.egg-info/PKG-INFO` & `functional-cat-0.4.1/functional_cat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functional-cat
-Version: 0.4.0
+Version: 0.4.1
 Summary: Catalog of functions
 License: Copyright 2022 Eric O. Korman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
@@ -25,15 +25,14 @@
         
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: torch
 Provides-Extra: onnx
 Provides-Extra: onnx-cpu
 Provides-Extra: onnx-gpu
-Provides-Extra: mmcv
 Provides-Extra: catalog
 Provides-Extra: glip
 Provides-Extra: dlib
 Provides-Extra: test
 License-File: LICENSE
 
 # functional cat
```

### Comparing `functional-cat-0.4.0/pyproject.toml` & `functional-cat-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [project]
 name = "functional-cat"
-version = "0.4.0"
+dynamic = ["version"]
 description = "Catalog of functions"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 dependencies = ["requests", "Pillow >= 9.1.0", "tqdm", "numpy >= 1.23"]
 
 [build-system]
-requires =  ["setuptools>=61.0"]
+requires =  ["setuptools>=61.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project.optional-dependencies]
 torch = [
   "torch >= 1.12.0",
   "torchvision >= 0.13.0"
 ]
 onnx = ["onnxruntime >= 1.11", "scipy"]
 onnx-cpu = ["onnxruntime >= 1.11"]
 onnx-gpu = ["onnxruntime-gpu >= 1.11"]
-mmcv = [] # this is installed separately
 catalog = ["boto3", "python-dotenv"]
 glip = ["glip-object-detection"]
 dlib = ["dlib"]
 test = ["pytest"]
 
 [tool.black]
 line-length = 79
@@ -31,7 +30,9 @@
 [tool.isort]
 line_length = 79
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
+
+[tool.setuptools_scm]
```

### Comparing `functional-cat-0.4.0/tests/test_dlib.py` & `functional-cat-0.4.1/tests/test_dlib.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.0/tests/test_onnx.py` & `functional-cat-0.4.1/tests/test_onnx.py`

 * *Files identical despite different names*

### Comparing `functional-cat-0.4.0/tests/test_torchvision.py` & `functional-cat-0.4.1/tests/test_torchvision.py`

 * *Files identical despite different names*

