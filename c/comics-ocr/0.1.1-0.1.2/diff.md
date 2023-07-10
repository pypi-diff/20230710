# Comparing `tmp/comics_ocr-0.1.1.tar.gz` & `tmp/comics_ocr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comics_ocr-0.1.1.tar", last modified: Mon Jul 10 18:18:48 2023, max compression
+gzip compressed data, was "comics_ocr-0.1.2.tar", last modified: Mon Jul 10 18:21:56 2023, max compression
```

## Comparing `comics_ocr-0.1.1.tar` & `comics_ocr-0.1.2.tar`

### file list

```diff
@@ -1,282 +1,282 @@
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.922486 comics_ocr-0.1.1/
--rw-r--r--   0 gsoykan20  (1001) gsoykan20  (1002)     1064 2023-07-10 18:02:00.000000 comics_ocr-0.1.1/LICENSE
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1381 2023-07-10 18:18:48.922486 comics_ocr-0.1.1/PKG-INFO
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      926 2023-07-10 18:16:39.000000 comics_ocr-0.1.1/README.md
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.902486 comics_ocr-0.1.1/comics_ocr/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2089 2023-07-10 18:18:46.000000 comics_ocr-0.1.1/comics_ocr/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3563 2023-07-10 17:14:47.000000 comics_ocr-0.1.1/comics_ocr/comics_ocr.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2841 2023-07-10 16:45:54.000000 comics_ocr-0.1.1/comics_ocr/text_extractor.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.906486 comics_ocr-0.1.1/comics_ocr.egg-info/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1381 2023-07-10 18:18:48.000000 comics_ocr-0.1.1/comics_ocr.egg-info/PKG-INFO
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     9292 2023-07-10 18:18:48.000000 comics_ocr-0.1.1/comics_ocr.egg-info/SOURCES.txt
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)        1 2023-07-10 18:18:48.000000 comics_ocr-0.1.1/comics_ocr.egg-info/dependency_links.txt
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      488 2023-07-10 18:18:48.000000 comics_ocr-0.1.1/comics_ocr.egg-info/requires.txt
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)       17 2023-07-10 18:18:48.000000 comics_ocr-0.1.1/comics_ocr.egg-info/top_level.txt
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.906486 comics_ocr-0.1.1/mmocr/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2431 2023-07-10 16:42:17.000000 comics_ocr-0.1.1/mmocr/__init__.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.906486 comics_ocr-0.1.1/mmocr/apis/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      495 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/apis/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     8081 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/apis/inference.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6152 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/apis/test.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6499 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/apis/train.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4324 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/apis/utils.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.906486 comics_ocr-0.1.1/mmocr/core/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      768 2022-02-14 08:40:49.000000 comics_ocr-0.1.1/mmocr/core/__init__.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.906486 comics_ocr-0.1.1/mmocr/core/deployment/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      296 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/core/deployment/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    12040 2022-02-14 08:40:49.000000 comics_ocr-0.1.1/mmocr/core/deployment/deploy_utils.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.906486 comics_ocr-0.1.1/mmocr/core/evaluation/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      400 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/core/evaluation/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6114 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/core/evaluation/hmean.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     8070 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/core/evaluation/hmean_ic13.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3955 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/core/evaluation/hmean_iou.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1033 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/core/evaluation/kie_metric.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3786 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/core/evaluation/ner_metric.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6237 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/core/evaluation/ocr_metric.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    18689 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/core/evaluation/utils.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3223 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/core/mask.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    30432 2022-02-14 08:40:49.000000 comics_ocr-0.1.1/mmocr/core/visualize.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.906486 comics_ocr-0.1.1/mmocr/datasets/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      941 2022-02-14 08:40:49.000000 comics_ocr-0.1.1/mmocr/datasets/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5380 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/base_dataset.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      353 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/builder.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6923 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/icdar_dataset.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     8705 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/kie_dataset.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1665 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/ner_dataset.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1309 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/ocr_dataset.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3455 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/ocr_seg_dataset.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    12082 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/openset_kie_dataset.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.906486 comics_ocr-0.1.1/mmocr/datasets/pipelines/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2006 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1732 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/box_utils.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4281 2022-07-21 09:24:24.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/crop.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2210 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/custom_format_bundle.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    11744 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/dbnet_transforms.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3368 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/kie_transforms.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6458 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/loading.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2051 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/ner_transforms.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     7760 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/ocr_seg_targets.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    15708 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/ocr_transforms.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3683 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/test_time_aug.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      496 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6004 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/base_textdet_targets.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     9113 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/dbnet_targets.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    24031 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/drrg_targets.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    14660 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/fcenet_targets.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2321 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/panet_targets.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      781 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/psenet_targets.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    20827 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/textsnake_targets.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4022 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/transform_wrappers.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    37543 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/datasets/pipelines/transforms.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4665 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/text_det_dataset.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6404 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/uniform_concat_dataset.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/datasets/utils/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      266 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/utils/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6891 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/utils/backend.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3659 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/utils/loader.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2691 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/datasets/utils/parser.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      872 2022-02-14 08:40:49.000000 comics_ocr-0.1.1/mmocr/models/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4452 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/builder.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/common/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      302 2022-02-14 08:40:49.000000 comics_ocr-0.1.1/mmocr/models/common/__init__.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/common/backbones/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)       91 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/common/backbones/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    21543 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/common/backbones/unet.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/common/detectors/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      129 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/common/detectors/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1380 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/common/detectors/single_stage.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/common/layers/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      159 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/common/layers/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6590 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/common/layers/transformer_layers.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/common/losses/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      151 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/common/losses/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      791 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/common/losses/dice_loss.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      992 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/common/losses/focal_loss.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/common/modules/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      361 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/common/modules/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5365 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/common/modules/transformer_module.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/kie/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      244 2022-02-14 08:40:49.000000 comics_ocr-0.1.1/mmocr/models/kie/__init__.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/kie/extractors/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)       94 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/kie/extractors/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5963 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/kie/extractors/sdmgr.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/kie/heads/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      107 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/kie/heads/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     7265 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/kie/heads/sdmgr_head.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/kie/losses/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      107 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/kie/losses/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1584 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/kie/losses/sdmgr_loss.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/ner/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      403 2023-07-10 16:45:23.000000 comics_ocr-0.1.1/mmocr/models/ner/__init__.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/ner/classifiers/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      119 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/classifiers/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1899 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/classifiers/ner_classifier.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/ner/convertors/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      116 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/convertors/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6706 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/convertors/ner_convertor.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/ner/decoders/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      107 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/decoders/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1374 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/decoders/fc_decoder.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/ner/encoders/
--rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)      113 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/encoders/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3143 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/encoders/bert_encoder.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.910487 comics_ocr-0.1.1/mmocr/models/ner/losses/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      214 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/losses/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2281 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/losses/masked_cross_entropy_loss.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2272 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/losses/masked_focal_loss.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.914487 comics_ocr-0.1.1/mmocr/models/ner/utils/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      145 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/utils/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      943 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/utils/activations.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    19532 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/ner/utils/bert.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.914487 comics_ocr-0.1.1/mmocr/models/textdet/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      392 2022-02-14 08:40:49.000000 comics_ocr-0.1.1/mmocr/models/textdet/__init__.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.914487 comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      381 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3549 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/db_head.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    10664 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/drrg_head.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5269 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/fce_head.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2948 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/head_mixin.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3087 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/pan_head.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1435 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/pse_head.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2898 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/textsnake_head.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.914487 comics_ocr-0.1.1/mmocr/models/textdet/detectors/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      506 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textdet/detectors/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      988 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/detectors/dbnet.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2118 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/detectors/drrg.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1242 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textdet/detectors/fcenet.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2238 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/detectors/ocr_mask_rcnn.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1009 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/detectors/panet.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      995 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/detectors/psenet.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2159 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/detectors/single_stage_text_detector.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2731 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/detectors/text_detector_mixin.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1007 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/detectors/textsnake.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.914487 comics_ocr-0.1.1/mmocr/models/textdet/losses/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      330 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textdet/losses/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6082 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/losses/db_loss.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    10071 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/losses/drrg_loss.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     7914 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/losses/fce_loss.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    12782 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/losses/pan_loss.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4184 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/losses/pse_loss.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     7876 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/losses/textsnake_loss.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.914487 comics_ocr-0.1.1/mmocr/models/textdet/modules/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      217 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textdet/modules/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2432 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textdet/modules/gcn.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    13094 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textdet/modules/local_graph.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    18637 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/modules/proposal_local_graph.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3716 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textdet/modules/utils.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.914487 comics_ocr-0.1.1/mmocr/models/textdet/necks/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      211 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textdet/necks/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5999 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textdet/necks/fpem_ffm.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     9362 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textdet/necks/fpn_cat.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3629 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/necks/fpn_unet.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4264 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textdet/necks/fpnf.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.914487 comics_ocr-0.1.1/mmocr/models/textdet/postprocess/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      571 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/postprocess/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      485 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/postprocess/base_postprocessor.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3467 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textdet/postprocess/db_postprocessor.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1565 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textdet/postprocess/drrg_postprocessor.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4087 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/postprocess/fce_postprocessor.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3375 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/postprocess/pan_postprocessor.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3190 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/postprocess/pse_postprocessor.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4812 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/postprocess/textsnake_postprocessor.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    16977 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textdet/postprocess/utils.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.914487 comics_ocr-0.1.1/mmocr/models/textrecog/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      771 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/__init__.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.918486 comics_ocr-0.1.1/mmocr/models/textrecog/backbones/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      397 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/backbones/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1418 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/backbones/nrtr_modality_transformer.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     8849 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/backbones/resnet.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5649 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/backbones/resnet31_ocr.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4405 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/backbones/resnet_abi.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2000 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/backbones/shallow_cnn.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2587 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/backbones/very_deep_vgg.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.918486 comics_ocr-0.1.1/mmocr/models/textrecog/convertors/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      306 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/convertors/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2718 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/convertors/abi.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5206 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/convertors/attn.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4746 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/convertors/base.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5414 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/convertors/ctc.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4455 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/convertors/seg.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.918486 comics_ocr-0.1.1/mmocr/models/textrecog/decoders/
--rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)      915 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/decoders/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6765 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/decoders/abinet_language_decoder.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6223 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/decoders/abinet_vision_decoder.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      894 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/decoders/base_decoder.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2360 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/decoders/crnn_decoder.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     7670 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/decoders/master_decoder.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6451 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/decoders/nrtr_decoder.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     7394 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/decoders/position_attention_decoder.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6412 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/decoders/robust_scanner_decoder.py
--rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)    18713 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/decoders/sar_decoder.py
--rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)     5469 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/decoders/sar_decoder_with_bs.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     8603 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/decoders/sequence_attention_decoder.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.918486 comics_ocr-0.1.1/mmocr/models/textrecog/encoders/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      504 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/encoders/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1706 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/encoders/abinet_vision_model.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      298 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/encoders/base_encoder.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1140 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/encoders/channel_reduction_encoder.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2887 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/encoders/nrtr_encoder.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3789 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/encoders/sar_encoder.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3034 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/encoders/satrn_encoder.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2662 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/encoders/transformer.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.918486 comics_ocr-0.1.1/mmocr/models/textrecog/fusers/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      104 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/fusers/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1705 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/fusers/abi_fuser.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.918486 comics_ocr-0.1.1/mmocr/models/textrecog/heads/
--rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)      101 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/heads/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2022 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/heads/seg_head.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.918486 comics_ocr-0.1.1/mmocr/models/textrecog/layers/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      602 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/layers/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5745 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/layers/conv_layer.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      782 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/layers/dot_product_attention_layer.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      561 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/layers/lstm_layer.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1052 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/layers/position_aware_layer.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      671 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/layers/robust_scanner_fusion_layer.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5409 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/layers/satrn_layers.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.918486 comics_ocr-0.1.1/mmocr/models/textrecog/losses/
--rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)      259 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/losses/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4660 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/losses/ce_loss.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3867 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/losses/ctc_loss.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4376 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/models/textrecog/losses/mix_loss.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2507 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/losses/seg_loss.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.922486 comics_ocr-0.1.1/mmocr/models/textrecog/necks/
--rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)       98 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/necks/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3173 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/necks/fpn_ocr.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.922486 comics_ocr-0.1.1/mmocr/models/textrecog/plugins/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      127 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/plugins/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6302 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/plugins/common.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.922486 comics_ocr-0.1.1/mmocr/models/textrecog/preprocessor/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      193 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/preprocessor/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      310 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/preprocessor/base_preprocessor.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    11877 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/models/textrecog/preprocessor/tps_preprocessor.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.922486 comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      536 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6505 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/abinet.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     8426 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/base.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      263 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/crnn.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6121 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/encode_decode_recognizer.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      294 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/master.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      298 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/nrtr.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      325 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/robust_scanner.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      295 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/sar.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      296 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/satrn.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4790 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/seg_recognizer.py
-drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:18:48.922486 comics_ocr-0.1.1/mmocr/utils/
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1204 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/utils/__init__.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6979 2023-07-10 16:39:44.000000 comics_ocr-0.1.1/mmocr/utils/box_util.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1609 2022-01-04 14:20:45.000000 comics_ocr-0.1.1/mmocr/utils/check_argument.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      465 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/utils/collect_env.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1200 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/utils/data_convert_util.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1075 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/utils/fileio.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1498 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/utils/img_util.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4192 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/utils/lmdb_util.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      952 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/utils/logger.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1976 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/utils/model.py
--rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)    33567 2022-07-25 09:27:50.000000 comics_ocr-0.1.1/mmocr/utils/ocr.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2219 2022-02-14 08:40:49.000000 comics_ocr-0.1.1/mmocr/utils/setup_env.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1331 2021-11-21 13:34:43.000000 comics_ocr-0.1.1/mmocr/utils/string_util.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      100 2022-06-08 12:55:11.000000 comics_ocr-0.1.1/mmocr/version.py
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      976 2023-07-10 18:18:48.926487 comics_ocr-0.1.1/setup.cfg
--rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      246 2023-07-10 18:12:52.000000 comics_ocr-0.1.1/setup.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.034659 comics_ocr-0.1.2/
+-rw-r--r--   0 gsoykan20  (1001) gsoykan20  (1002)     1064 2023-07-10 18:02:00.000000 comics_ocr-0.1.2/LICENSE
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1379 2023-07-10 18:21:56.034659 comics_ocr-0.1.2/PKG-INFO
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      924 2023-07-10 18:21:42.000000 comics_ocr-0.1.2/README.md
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.014659 comics_ocr-0.1.2/comics_ocr/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2089 2023-07-10 18:21:42.000000 comics_ocr-0.1.2/comics_ocr/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3563 2023-07-10 17:14:47.000000 comics_ocr-0.1.2/comics_ocr/comics_ocr.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2841 2023-07-10 16:45:54.000000 comics_ocr-0.1.2/comics_ocr/text_extractor.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.014659 comics_ocr-0.1.2/comics_ocr.egg-info/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1379 2023-07-10 18:21:55.000000 comics_ocr-0.1.2/comics_ocr.egg-info/PKG-INFO
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     9292 2023-07-10 18:21:55.000000 comics_ocr-0.1.2/comics_ocr.egg-info/SOURCES.txt
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)        1 2023-07-10 18:21:55.000000 comics_ocr-0.1.2/comics_ocr.egg-info/dependency_links.txt
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      488 2023-07-10 18:21:55.000000 comics_ocr-0.1.2/comics_ocr.egg-info/requires.txt
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)       17 2023-07-10 18:21:55.000000 comics_ocr-0.1.2/comics_ocr.egg-info/top_level.txt
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.014659 comics_ocr-0.1.2/mmocr/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2431 2023-07-10 16:42:17.000000 comics_ocr-0.1.2/mmocr/__init__.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.018659 comics_ocr-0.1.2/mmocr/apis/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      495 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/apis/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     8081 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/apis/inference.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6152 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/apis/test.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6499 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/apis/train.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4324 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/apis/utils.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.018659 comics_ocr-0.1.2/mmocr/core/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      768 2022-02-14 08:40:49.000000 comics_ocr-0.1.2/mmocr/core/__init__.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.018659 comics_ocr-0.1.2/mmocr/core/deployment/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      296 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/core/deployment/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    12040 2022-02-14 08:40:49.000000 comics_ocr-0.1.2/mmocr/core/deployment/deploy_utils.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.018659 comics_ocr-0.1.2/mmocr/core/evaluation/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      400 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/core/evaluation/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6114 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/core/evaluation/hmean.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     8070 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/core/evaluation/hmean_ic13.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3955 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/core/evaluation/hmean_iou.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1033 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/core/evaluation/kie_metric.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3786 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/core/evaluation/ner_metric.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6237 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/core/evaluation/ocr_metric.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    18689 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/core/evaluation/utils.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3223 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/core/mask.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    30432 2022-02-14 08:40:49.000000 comics_ocr-0.1.2/mmocr/core/visualize.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.018659 comics_ocr-0.1.2/mmocr/datasets/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      941 2022-02-14 08:40:49.000000 comics_ocr-0.1.2/mmocr/datasets/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5380 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/base_dataset.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      353 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/builder.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6923 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/icdar_dataset.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     8705 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/kie_dataset.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1665 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/ner_dataset.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1309 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/ocr_dataset.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3455 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/ocr_seg_dataset.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    12082 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/openset_kie_dataset.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.018659 comics_ocr-0.1.2/mmocr/datasets/pipelines/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2006 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1732 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/box_utils.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4281 2022-07-21 09:24:24.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/crop.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2210 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/custom_format_bundle.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    11744 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/dbnet_transforms.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3368 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/kie_transforms.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6458 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/loading.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2051 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/ner_transforms.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     7760 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/ocr_seg_targets.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    15708 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/ocr_transforms.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3683 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/test_time_aug.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      496 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6004 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/base_textdet_targets.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     9113 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/dbnet_targets.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    24031 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/drrg_targets.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    14660 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/fcenet_targets.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2321 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/panet_targets.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      781 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/psenet_targets.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    20827 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/textsnake_targets.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4022 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/transform_wrappers.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    37543 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/datasets/pipelines/transforms.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4665 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/text_det_dataset.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6404 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/uniform_concat_dataset.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/datasets/utils/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      266 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/utils/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6891 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/utils/backend.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3659 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/utils/loader.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2691 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/datasets/utils/parser.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      872 2022-02-14 08:40:49.000000 comics_ocr-0.1.2/mmocr/models/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4452 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/builder.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/common/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      302 2022-02-14 08:40:49.000000 comics_ocr-0.1.2/mmocr/models/common/__init__.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/common/backbones/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)       91 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/common/backbones/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    21543 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/common/backbones/unet.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/common/detectors/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      129 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/common/detectors/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1380 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/common/detectors/single_stage.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/common/layers/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      159 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/common/layers/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6590 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/common/layers/transformer_layers.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/common/losses/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      151 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/common/losses/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      791 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/common/losses/dice_loss.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      992 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/common/losses/focal_loss.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/common/modules/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      361 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/common/modules/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5365 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/common/modules/transformer_module.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/kie/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      244 2022-02-14 08:40:49.000000 comics_ocr-0.1.2/mmocr/models/kie/__init__.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/kie/extractors/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)       94 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/kie/extractors/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5963 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/kie/extractors/sdmgr.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/kie/heads/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      107 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/kie/heads/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     7265 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/kie/heads/sdmgr_head.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/kie/losses/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      107 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/kie/losses/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1584 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/kie/losses/sdmgr_loss.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/ner/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      403 2023-07-10 16:45:23.000000 comics_ocr-0.1.2/mmocr/models/ner/__init__.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/ner/classifiers/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      119 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/classifiers/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1899 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/classifiers/ner_classifier.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/ner/convertors/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      116 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/convertors/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6706 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/convertors/ner_convertor.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/ner/decoders/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      107 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/decoders/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1374 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/decoders/fc_decoder.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/ner/encoders/
+-rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)      113 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/encoders/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3143 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/encoders/bert_encoder.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.022659 comics_ocr-0.1.2/mmocr/models/ner/losses/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      214 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/losses/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2281 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/losses/masked_cross_entropy_loss.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2272 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/losses/masked_focal_loss.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.026659 comics_ocr-0.1.2/mmocr/models/ner/utils/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      145 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/utils/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      943 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/utils/activations.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    19532 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/ner/utils/bert.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.026659 comics_ocr-0.1.2/mmocr/models/textdet/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      392 2022-02-14 08:40:49.000000 comics_ocr-0.1.2/mmocr/models/textdet/__init__.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.026659 comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      381 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3549 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/db_head.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    10664 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/drrg_head.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5269 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/fce_head.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2948 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/head_mixin.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3087 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/pan_head.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1435 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/pse_head.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2898 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/textsnake_head.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.026659 comics_ocr-0.1.2/mmocr/models/textdet/detectors/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      506 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textdet/detectors/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      988 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/detectors/dbnet.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2118 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/detectors/drrg.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1242 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textdet/detectors/fcenet.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2238 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/detectors/ocr_mask_rcnn.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1009 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/detectors/panet.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      995 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/detectors/psenet.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2159 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/detectors/single_stage_text_detector.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2731 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/detectors/text_detector_mixin.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1007 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/detectors/textsnake.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.026659 comics_ocr-0.1.2/mmocr/models/textdet/losses/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      330 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textdet/losses/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6082 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/losses/db_loss.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    10071 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/losses/drrg_loss.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     7914 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/losses/fce_loss.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    12782 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/losses/pan_loss.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4184 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/losses/pse_loss.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     7876 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/losses/textsnake_loss.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.026659 comics_ocr-0.1.2/mmocr/models/textdet/modules/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      217 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textdet/modules/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2432 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textdet/modules/gcn.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    13094 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textdet/modules/local_graph.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    18637 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/modules/proposal_local_graph.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3716 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textdet/modules/utils.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.026659 comics_ocr-0.1.2/mmocr/models/textdet/necks/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      211 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textdet/necks/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5999 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textdet/necks/fpem_ffm.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     9362 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textdet/necks/fpn_cat.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3629 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/necks/fpn_unet.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4264 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textdet/necks/fpnf.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.026659 comics_ocr-0.1.2/mmocr/models/textdet/postprocess/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      571 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/postprocess/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      485 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/postprocess/base_postprocessor.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3467 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textdet/postprocess/db_postprocessor.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1565 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textdet/postprocess/drrg_postprocessor.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4087 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/postprocess/fce_postprocessor.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3375 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/postprocess/pan_postprocessor.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3190 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/postprocess/pse_postprocessor.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4812 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/postprocess/textsnake_postprocessor.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    16977 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textdet/postprocess/utils.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.030659 comics_ocr-0.1.2/mmocr/models/textrecog/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      771 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/__init__.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.030659 comics_ocr-0.1.2/mmocr/models/textrecog/backbones/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      397 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/backbones/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1418 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/backbones/nrtr_modality_transformer.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     8849 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/backbones/resnet.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5649 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/backbones/resnet31_ocr.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4405 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/backbones/resnet_abi.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2000 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/backbones/shallow_cnn.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2587 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/backbones/very_deep_vgg.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.030659 comics_ocr-0.1.2/mmocr/models/textrecog/convertors/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      306 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/convertors/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2718 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/convertors/abi.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5206 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/convertors/attn.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4746 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/convertors/base.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5414 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/convertors/ctc.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4455 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/convertors/seg.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.030659 comics_ocr-0.1.2/mmocr/models/textrecog/decoders/
+-rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)      915 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/decoders/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6765 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/decoders/abinet_language_decoder.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6223 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/decoders/abinet_vision_decoder.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      894 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/decoders/base_decoder.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2360 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/decoders/crnn_decoder.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     7670 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/decoders/master_decoder.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6451 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/decoders/nrtr_decoder.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     7394 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/decoders/position_attention_decoder.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6412 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/decoders/robust_scanner_decoder.py
+-rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)    18713 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/decoders/sar_decoder.py
+-rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)     5469 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/decoders/sar_decoder_with_bs.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     8603 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/decoders/sequence_attention_decoder.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.030659 comics_ocr-0.1.2/mmocr/models/textrecog/encoders/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      504 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/encoders/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1706 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/encoders/abinet_vision_model.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      298 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/encoders/base_encoder.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1140 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/encoders/channel_reduction_encoder.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2887 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/encoders/nrtr_encoder.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3789 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/encoders/sar_encoder.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3034 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/encoders/satrn_encoder.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2662 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/encoders/transformer.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.030659 comics_ocr-0.1.2/mmocr/models/textrecog/fusers/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      104 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/fusers/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1705 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/fusers/abi_fuser.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.030659 comics_ocr-0.1.2/mmocr/models/textrecog/heads/
+-rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)      101 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/heads/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2022 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/heads/seg_head.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.030659 comics_ocr-0.1.2/mmocr/models/textrecog/layers/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      602 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/layers/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5745 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/layers/conv_layer.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      782 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/layers/dot_product_attention_layer.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      561 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/layers/lstm_layer.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1052 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/layers/position_aware_layer.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      671 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/layers/robust_scanner_fusion_layer.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     5409 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/layers/satrn_layers.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.034659 comics_ocr-0.1.2/mmocr/models/textrecog/losses/
+-rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)      259 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/losses/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4660 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/losses/ce_loss.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3867 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/losses/ctc_loss.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4376 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/models/textrecog/losses/mix_loss.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2507 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/losses/seg_loss.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.034659 comics_ocr-0.1.2/mmocr/models/textrecog/necks/
+-rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)       98 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/necks/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     3173 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/necks/fpn_ocr.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.034659 comics_ocr-0.1.2/mmocr/models/textrecog/plugins/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      127 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/plugins/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6302 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/plugins/common.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.034659 comics_ocr-0.1.2/mmocr/models/textrecog/preprocessor/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      193 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/preprocessor/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      310 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/preprocessor/base_preprocessor.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)    11877 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/models/textrecog/preprocessor/tps_preprocessor.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.034659 comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      536 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6505 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/abinet.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     8426 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/base.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      263 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/crnn.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6121 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/encode_decode_recognizer.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      294 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/master.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      298 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/nrtr.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      325 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/robust_scanner.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      295 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/sar.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      296 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/satrn.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4790 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/seg_recognizer.py
+drwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)        0 2023-07-10 18:21:56.034659 comics_ocr-0.1.2/mmocr/utils/
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1204 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/utils/__init__.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     6979 2023-07-10 16:39:44.000000 comics_ocr-0.1.2/mmocr/utils/box_util.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1609 2022-01-04 14:20:45.000000 comics_ocr-0.1.2/mmocr/utils/check_argument.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      465 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/utils/collect_env.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1200 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/utils/data_convert_util.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1075 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/utils/fileio.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1498 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/utils/img_util.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     4192 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/utils/lmdb_util.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      952 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/utils/logger.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1976 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/utils/model.py
+-rwxrwxr-x   0 gsoykan20  (1001) gsoykan20  (1002)    33567 2022-07-25 09:27:50.000000 comics_ocr-0.1.2/mmocr/utils/ocr.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     2219 2022-02-14 08:40:49.000000 comics_ocr-0.1.2/mmocr/utils/setup_env.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)     1331 2021-11-21 13:34:43.000000 comics_ocr-0.1.2/mmocr/utils/string_util.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      100 2022-06-08 12:55:11.000000 comics_ocr-0.1.2/mmocr/version.py
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      976 2023-07-10 18:21:56.034659 comics_ocr-0.1.2/setup.cfg
+-rw-rw-r--   0 gsoykan20  (1001) gsoykan20  (1002)      246 2023-07-10 18:12:52.000000 comics_ocr-0.1.2/setup.py
```

### Comparing `comics_ocr-0.1.1/LICENSE` & `comics_ocr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/PKG-INFO` & `comics_ocr-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comics_ocr
-Version: 0.1.1
+Version: 0.1.2
 Summary: ComicsOCR is a Python package created for easily distributing OCR models trained for golden age of comics.
 Home-page: https://github.com/gsoykan/comics_ocr
 Author: Gürkan Soykan
 Author-email: grkansoykan@gmail.com
 License: MIT
 Keywords: comics_ocr,mmocr_comics
 Requires-Python: <4,>=3.8
@@ -12,19 +12,19 @@
 Provides-Extra: cuda
 Provides-Extra: cpu
 License-File: LICENSE
 
 to build locally after cloning
 
 ```shell
-pip install comics-ocr.[cuda] -f https://download.pytorch.org/whl/torch_stable.html
+pip install comics-ocr[cuda] -f https://download.pytorch.org/whl/torch_stable.html
 
 or 
 
-pip install comics-ocr.[cpu]
+pip install comics-ocr[cpu]
 ```
 
 You can get the necessary model checkpoints and configs from
 [COMICS TEXT+](https://github.com/gsoykan/comics_text_plus) repository.
 
 ## Usage
```

### Comparing `comics_ocr-0.1.1/README.md` & `comics_ocr-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 to build locally after cloning
 
 ```shell
-pip install comics-ocr.[cuda] -f https://download.pytorch.org/whl/torch_stable.html
+pip install comics-ocr[cuda] -f https://download.pytorch.org/whl/torch_stable.html
 
 or 
 
-pip install comics-ocr.[cpu]
+pip install comics-ocr[cpu]
 ```
 
 You can get the necessary model checkpoints and configs from
 [COMICS TEXT+](https://github.com/gsoykan/comics_text_plus) repository.
 
 ## Usage
```

### Comparing `comics_ocr-0.1.1/comics_ocr/__init__.py` & `comics_ocr-0.1.2/comics_ocr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from comics_ocr.comics_ocr import ComicsOCR
 
 __author__ = 'Gürkan Soykan'
 __email__ = 'grkansoykan@gmail.com'
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 # module level doc-string
 __doc__ = """
 COMICS OCR
 ================
 
 Description
```

### Comparing `comics_ocr-0.1.1/comics_ocr/comics_ocr.py` & `comics_ocr-0.1.2/comics_ocr/comics_ocr.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/comics_ocr/text_extractor.py` & `comics_ocr-0.1.2/comics_ocr/text_extractor.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/comics_ocr.egg-info/PKG-INFO` & `comics_ocr-0.1.2/comics_ocr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comics-ocr
-Version: 0.1.1
+Version: 0.1.2
 Summary: ComicsOCR is a Python package created for easily distributing OCR models trained for golden age of comics.
 Home-page: https://github.com/gsoykan/comics_ocr
 Author: Gürkan Soykan
 Author-email: grkansoykan@gmail.com
 License: MIT
 Keywords: comics_ocr,mmocr_comics
 Requires-Python: <4,>=3.8
@@ -12,19 +12,19 @@
 Provides-Extra: cuda
 Provides-Extra: cpu
 License-File: LICENSE
 
 to build locally after cloning
 
 ```shell
-pip install comics-ocr.[cuda] -f https://download.pytorch.org/whl/torch_stable.html
+pip install comics-ocr[cuda] -f https://download.pytorch.org/whl/torch_stable.html
 
 or 
 
-pip install comics-ocr.[cpu]
+pip install comics-ocr[cpu]
 ```
 
 You can get the necessary model checkpoints and configs from
 [COMICS TEXT+](https://github.com/gsoykan/comics_text_plus) repository.
 
 ## Usage
```

### Comparing `comics_ocr-0.1.1/comics_ocr.egg-info/SOURCES.txt` & `comics_ocr-0.1.2/comics_ocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/__init__.py` & `comics_ocr-0.1.2/mmocr/__init__.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/apis/inference.py` & `comics_ocr-0.1.2/mmocr/apis/inference.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/apis/test.py` & `comics_ocr-0.1.2/mmocr/apis/test.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/apis/train.py` & `comics_ocr-0.1.2/mmocr/apis/train.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/apis/utils.py` & `comics_ocr-0.1.2/mmocr/apis/utils.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/core/__init__.py` & `comics_ocr-0.1.2/mmocr/core/__init__.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/core/deployment/deploy_utils.py` & `comics_ocr-0.1.2/mmocr/core/deployment/deploy_utils.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/core/evaluation/hmean.py` & `comics_ocr-0.1.2/mmocr/core/evaluation/hmean.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/core/evaluation/hmean_ic13.py` & `comics_ocr-0.1.2/mmocr/core/evaluation/hmean_ic13.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/core/evaluation/hmean_iou.py` & `comics_ocr-0.1.2/mmocr/core/evaluation/hmean_iou.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/core/evaluation/kie_metric.py` & `comics_ocr-0.1.2/mmocr/core/evaluation/kie_metric.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/core/evaluation/ner_metric.py` & `comics_ocr-0.1.2/mmocr/core/evaluation/ner_metric.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/core/evaluation/ocr_metric.py` & `comics_ocr-0.1.2/mmocr/core/evaluation/ocr_metric.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/core/evaluation/utils.py` & `comics_ocr-0.1.2/mmocr/core/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/core/mask.py` & `comics_ocr-0.1.2/mmocr/core/mask.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/core/visualize.py` & `comics_ocr-0.1.2/mmocr/core/visualize.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/__init__.py` & `comics_ocr-0.1.2/mmocr/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/base_dataset.py` & `comics_ocr-0.1.2/mmocr/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/icdar_dataset.py` & `comics_ocr-0.1.2/mmocr/datasets/icdar_dataset.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/kie_dataset.py` & `comics_ocr-0.1.2/mmocr/datasets/kie_dataset.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/ner_dataset.py` & `comics_ocr-0.1.2/mmocr/datasets/ner_dataset.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/ocr_dataset.py` & `comics_ocr-0.1.2/mmocr/datasets/ocr_dataset.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/ocr_seg_dataset.py` & `comics_ocr-0.1.2/mmocr/datasets/ocr_seg_dataset.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/openset_kie_dataset.py` & `comics_ocr-0.1.2/mmocr/datasets/openset_kie_dataset.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/__init__.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/box_utils.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/box_utils.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/crop.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/crop.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/custom_format_bundle.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/custom_format_bundle.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/dbnet_transforms.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/dbnet_transforms.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/kie_transforms.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/kie_transforms.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/loading.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/ner_transforms.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/ner_transforms.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/ocr_seg_targets.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/ocr_seg_targets.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/ocr_transforms.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/ocr_transforms.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/test_time_aug.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/base_textdet_targets.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/base_textdet_targets.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/dbnet_targets.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/dbnet_targets.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/drrg_targets.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/drrg_targets.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/fcenet_targets.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/fcenet_targets.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/panet_targets.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/panet_targets.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/psenet_targets.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/psenet_targets.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/textdet_targets/textsnake_targets.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/textdet_targets/textsnake_targets.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/transform_wrappers.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/transform_wrappers.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/pipelines/transforms.py` & `comics_ocr-0.1.2/mmocr/datasets/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/text_det_dataset.py` & `comics_ocr-0.1.2/mmocr/datasets/text_det_dataset.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/uniform_concat_dataset.py` & `comics_ocr-0.1.2/mmocr/datasets/uniform_concat_dataset.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/utils/backend.py` & `comics_ocr-0.1.2/mmocr/datasets/utils/backend.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/utils/loader.py` & `comics_ocr-0.1.2/mmocr/datasets/utils/loader.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/datasets/utils/parser.py` & `comics_ocr-0.1.2/mmocr/datasets/utils/parser.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/__init__.py` & `comics_ocr-0.1.2/mmocr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/builder.py` & `comics_ocr-0.1.2/mmocr/models/builder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/common/backbones/unet.py` & `comics_ocr-0.1.2/mmocr/models/common/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/common/detectors/single_stage.py` & `comics_ocr-0.1.2/mmocr/models/common/detectors/single_stage.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/common/layers/transformer_layers.py` & `comics_ocr-0.1.2/mmocr/models/common/layers/transformer_layers.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/common/losses/dice_loss.py` & `comics_ocr-0.1.2/mmocr/models/common/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/common/losses/focal_loss.py` & `comics_ocr-0.1.2/mmocr/models/common/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/common/modules/transformer_module.py` & `comics_ocr-0.1.2/mmocr/models/common/modules/transformer_module.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/kie/extractors/sdmgr.py` & `comics_ocr-0.1.2/mmocr/models/kie/extractors/sdmgr.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/kie/heads/sdmgr_head.py` & `comics_ocr-0.1.2/mmocr/models/kie/heads/sdmgr_head.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/kie/losses/sdmgr_loss.py` & `comics_ocr-0.1.2/mmocr/models/kie/losses/sdmgr_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/ner/classifiers/ner_classifier.py` & `comics_ocr-0.1.2/mmocr/models/ner/classifiers/ner_classifier.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/ner/convertors/ner_convertor.py` & `comics_ocr-0.1.2/mmocr/models/ner/convertors/ner_convertor.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/ner/decoders/fc_decoder.py` & `comics_ocr-0.1.2/mmocr/models/ner/decoders/fc_decoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/ner/encoders/bert_encoder.py` & `comics_ocr-0.1.2/mmocr/models/ner/encoders/bert_encoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/ner/losses/masked_cross_entropy_loss.py` & `comics_ocr-0.1.2/mmocr/models/ner/losses/masked_cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/ner/losses/masked_focal_loss.py` & `comics_ocr-0.1.2/mmocr/models/ner/losses/masked_focal_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/ner/utils/activations.py` & `comics_ocr-0.1.2/mmocr/models/ner/utils/activations.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/ner/utils/bert.py` & `comics_ocr-0.1.2/mmocr/models/ner/utils/bert.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/db_head.py` & `comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/db_head.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/drrg_head.py` & `comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/drrg_head.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/fce_head.py` & `comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/fce_head.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/head_mixin.py` & `comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/head_mixin.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/pan_head.py` & `comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/pan_head.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/pse_head.py` & `comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/pse_head.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/dense_heads/textsnake_head.py` & `comics_ocr-0.1.2/mmocr/models/textdet/dense_heads/textsnake_head.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/detectors/dbnet.py` & `comics_ocr-0.1.2/mmocr/models/textdet/detectors/dbnet.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/detectors/drrg.py` & `comics_ocr-0.1.2/mmocr/models/textdet/detectors/drrg.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/detectors/fcenet.py` & `comics_ocr-0.1.2/mmocr/models/textdet/detectors/fcenet.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/detectors/ocr_mask_rcnn.py` & `comics_ocr-0.1.2/mmocr/models/textdet/detectors/ocr_mask_rcnn.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/detectors/panet.py` & `comics_ocr-0.1.2/mmocr/models/textdet/detectors/panet.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/detectors/psenet.py` & `comics_ocr-0.1.2/mmocr/models/textdet/detectors/psenet.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/detectors/single_stage_text_detector.py` & `comics_ocr-0.1.2/mmocr/models/textdet/detectors/single_stage_text_detector.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/detectors/text_detector_mixin.py` & `comics_ocr-0.1.2/mmocr/models/textdet/detectors/text_detector_mixin.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/detectors/textsnake.py` & `comics_ocr-0.1.2/mmocr/models/textdet/detectors/textsnake.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/losses/db_loss.py` & `comics_ocr-0.1.2/mmocr/models/textdet/losses/db_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/losses/drrg_loss.py` & `comics_ocr-0.1.2/mmocr/models/textdet/losses/drrg_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/losses/fce_loss.py` & `comics_ocr-0.1.2/mmocr/models/textdet/losses/fce_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/losses/pan_loss.py` & `comics_ocr-0.1.2/mmocr/models/textdet/losses/pan_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/losses/pse_loss.py` & `comics_ocr-0.1.2/mmocr/models/textdet/losses/pse_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/losses/textsnake_loss.py` & `comics_ocr-0.1.2/mmocr/models/textdet/losses/textsnake_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/modules/gcn.py` & `comics_ocr-0.1.2/mmocr/models/textdet/modules/gcn.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/modules/local_graph.py` & `comics_ocr-0.1.2/mmocr/models/textdet/modules/local_graph.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/modules/proposal_local_graph.py` & `comics_ocr-0.1.2/mmocr/models/textdet/modules/proposal_local_graph.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/modules/utils.py` & `comics_ocr-0.1.2/mmocr/models/textdet/modules/utils.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/necks/fpem_ffm.py` & `comics_ocr-0.1.2/mmocr/models/textdet/necks/fpem_ffm.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/necks/fpn_cat.py` & `comics_ocr-0.1.2/mmocr/models/textdet/necks/fpn_cat.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/necks/fpn_unet.py` & `comics_ocr-0.1.2/mmocr/models/textdet/necks/fpn_unet.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/necks/fpnf.py` & `comics_ocr-0.1.2/mmocr/models/textdet/necks/fpnf.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/postprocess/__init__.py` & `comics_ocr-0.1.2/mmocr/models/textdet/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/postprocess/db_postprocessor.py` & `comics_ocr-0.1.2/mmocr/models/textdet/postprocess/db_postprocessor.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/postprocess/drrg_postprocessor.py` & `comics_ocr-0.1.2/mmocr/models/textdet/postprocess/drrg_postprocessor.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/postprocess/fce_postprocessor.py` & `comics_ocr-0.1.2/mmocr/models/textdet/postprocess/fce_postprocessor.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/postprocess/pan_postprocessor.py` & `comics_ocr-0.1.2/mmocr/models/textdet/postprocess/pan_postprocessor.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/postprocess/pse_postprocessor.py` & `comics_ocr-0.1.2/mmocr/models/textdet/postprocess/pse_postprocessor.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/postprocess/textsnake_postprocessor.py` & `comics_ocr-0.1.2/mmocr/models/textdet/postprocess/textsnake_postprocessor.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textdet/postprocess/utils.py` & `comics_ocr-0.1.2/mmocr/models/textdet/postprocess/utils.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/__init__.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/__init__.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/backbones/nrtr_modality_transformer.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/backbones/nrtr_modality_transformer.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/backbones/resnet.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/backbones/resnet31_ocr.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/backbones/resnet31_ocr.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/backbones/resnet_abi.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/backbones/resnet_abi.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/backbones/shallow_cnn.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/backbones/shallow_cnn.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/backbones/very_deep_vgg.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/backbones/very_deep_vgg.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/convertors/abi.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/convertors/abi.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/convertors/attn.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/convertors/attn.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/convertors/base.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/convertors/base.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/convertors/ctc.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/convertors/ctc.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/convertors/seg.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/convertors/seg.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/decoders/__init__.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/decoders/abinet_language_decoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/decoders/abinet_language_decoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/decoders/abinet_vision_decoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/decoders/abinet_vision_decoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/decoders/base_decoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/decoders/base_decoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/decoders/crnn_decoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/decoders/crnn_decoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/decoders/master_decoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/decoders/master_decoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/decoders/nrtr_decoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/decoders/nrtr_decoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/decoders/position_attention_decoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/decoders/position_attention_decoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/decoders/robust_scanner_decoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/decoders/robust_scanner_decoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/decoders/sar_decoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/decoders/sar_decoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/decoders/sar_decoder_with_bs.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/decoders/sar_decoder_with_bs.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/decoders/sequence_attention_decoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/decoders/sequence_attention_decoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/encoders/abinet_vision_model.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/encoders/abinet_vision_model.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/encoders/channel_reduction_encoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/encoders/channel_reduction_encoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/encoders/nrtr_encoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/encoders/nrtr_encoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/encoders/sar_encoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/encoders/sar_encoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/encoders/satrn_encoder.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/encoders/satrn_encoder.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/encoders/transformer.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/encoders/transformer.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/fusers/abi_fuser.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/fusers/abi_fuser.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/heads/seg_head.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/heads/seg_head.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/layers/__init__.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/layers/conv_layer.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/layers/conv_layer.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/layers/dot_product_attention_layer.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/layers/dot_product_attention_layer.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/layers/lstm_layer.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/layers/lstm_layer.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/layers/position_aware_layer.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/layers/position_aware_layer.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/layers/robust_scanner_fusion_layer.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/layers/robust_scanner_fusion_layer.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/layers/satrn_layers.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/layers/satrn_layers.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/losses/ce_loss.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/losses/ce_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/losses/ctc_loss.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/losses/ctc_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/losses/mix_loss.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/losses/mix_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/losses/seg_loss.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/losses/seg_loss.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/necks/fpn_ocr.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/necks/fpn_ocr.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/plugins/common.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/plugins/common.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/preprocessor/tps_preprocessor.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/preprocessor/tps_preprocessor.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/__init__.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/__init__.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/abinet.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/abinet.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/base.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/base.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/encode_decode_recognizer.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/encode_decode_recognizer.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/models/textrecog/recognizer/seg_recognizer.py` & `comics_ocr-0.1.2/mmocr/models/textrecog/recognizer/seg_recognizer.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/utils/__init__.py` & `comics_ocr-0.1.2/mmocr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/utils/box_util.py` & `comics_ocr-0.1.2/mmocr/utils/box_util.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/utils/check_argument.py` & `comics_ocr-0.1.2/mmocr/utils/check_argument.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/utils/data_convert_util.py` & `comics_ocr-0.1.2/mmocr/utils/data_convert_util.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/utils/fileio.py` & `comics_ocr-0.1.2/mmocr/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/utils/img_util.py` & `comics_ocr-0.1.2/mmocr/utils/img_util.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/utils/lmdb_util.py` & `comics_ocr-0.1.2/mmocr/utils/lmdb_util.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/utils/logger.py` & `comics_ocr-0.1.2/mmocr/utils/logger.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/utils/model.py` & `comics_ocr-0.1.2/mmocr/utils/model.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/utils/ocr.py` & `comics_ocr-0.1.2/mmocr/utils/ocr.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/utils/setup_env.py` & `comics_ocr-0.1.2/mmocr/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/mmocr/utils/string_util.py` & `comics_ocr-0.1.2/mmocr/utils/string_util.py`

 * *Files identical despite different names*

### Comparing `comics_ocr-0.1.1/setup.cfg` & `comics_ocr-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = comics_ocr
-version = 0.1.1
+version = 0.1.2
 description = ComicsOCR is a Python package created for easily distributing OCR models trained for golden age of comics.
 author = Gürkan Soykan
 author_email = grkansoykan@gmail.com
 keywords = comics_ocr, mmocr_comics
 license = MIT
 url = https://github.com/gsoykan/comics_ocr
```

