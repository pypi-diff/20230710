# Comparing `tmp/vision_datasets-1.0.0.tar.gz` & `tmp/vision_datasets-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_datasets-1.0.0.tar", last modified: Wed Jun 28 07:31:59 2023, max compression
+gzip compressed data, was "vision_datasets-1.0.1.tar", last modified: Mon Jul 10 20:31:16 2023, max compression
```

## Comparing `vision_datasets-1.0.0.tar` & `vision_datasets-1.0.1.tar`

### file list

```diff
@@ -1,161 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.336434 vision_datasets-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-06-28 07:31:59.336434 vision_datasets-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 07:31:59.340435 vision_datasets-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.304434 vision_datasets-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.304434 vision_datasets-1.0.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/resources/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_box_alteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.308434 vision_datasets-1.0.0/tests/test_coco_adaptor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_coco_adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_coco_adaptor/coco_adaptor_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_coco_adaptor/test_image_caption_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_coco_adaptor/test_image_matting_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_coco_adaptor/test_image_regression_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_coco_adaptor/test_image_text_matching_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_coco_adaptor/test_multiclass_classification_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_coco_adaptor/test_multilabel_classification_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_coco_adaptor/test_multitask_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_coco_adaptor/test_object_detection_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_coco_adaptor/test_text_2_image_retrieval_coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_coco_format_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_dataset_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    45616 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_dataset_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_dataset_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_detection_as_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_ic_od_as_image_text_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_iris_format_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.308434 vision_datasets-1.0.0/tests/test_manifest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_manifest/test_pickleable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_manifest_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.308434 vision_datasets-1.0.0/tests/test_manifest_to_coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_manifest_to_coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_manifest_to_coco/test_manifest_to_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.308434 vision_datasets-1.0.0/tests/test_merge_manifest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_merge_manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_merge_manifest/test_manifest_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_pytorch_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.312434 vision_datasets-1.0.0/tests/test_sample/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_sample/test_sample_manfiest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.312434 vision_datasets-1.0.0/tests/test_spawn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_spawn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_spawn/test_spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.312434 vision_datasets-1.0.0/vision_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.316434 vision_datasets-1.0.0/vision_datasets/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/commands/check_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/commands/converter_od_to_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/commands/converter_to_aml_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/commands/converter_to_tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/commands/converter_tsv_to_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/commands/download_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/commands/list_operations_by_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/commands/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.320434 vision_datasets-1.0.0/vision_datasets/common/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.320434 vision_datasets-1.0.0/vision_datasets/common/data_manifest/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/data_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/iris_data_manifest_adaptor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.324434 vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/balanced_instance_weights_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/generate_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/remove_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_manifest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.324434 vision_datasets-1.0.0/vision_datasets/common/data_reader/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_reader/dataset_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_reader/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/data_reader/image_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.328434 vision_datasets-1.0.0/vision_datasets/common/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/dataset/torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/dataset/vision_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/dataset_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.328434 vision_datasets-1.0.0/vision_datasets/common/dataset_management/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/dataset_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/dataset_management/dataset_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/dataset_management/dataset_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.328434 vision_datasets-1.0.0/vision_datasets/common/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/factory/coco_manifest_adaptor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/factory/data_manifest_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.332435 vision_datasets-1.0.0/vision_datasets/common/factory/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/factory/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/factory/operations/balanced_instance_weights_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/factory/operations/coco_generator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/factory/operations/manifest_merger_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/factory/operations/sampler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/factory/operations/spawn_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/factory/operations/split_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/factory/operations/supported_operations_by_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.332435 vision_datasets-1.0.0/vision_datasets/image_caption/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_caption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_caption/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_caption/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_caption/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.332435 vision_datasets-1.0.0/vision_datasets/image_classification/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_classification/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_classification/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_classification/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.332435 vision_datasets-1.0.0/vision_datasets/image_matting/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_matting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_matting/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_matting/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_matting/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.336434 vision_datasets-1.0.0/vision_datasets/image_object_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_object_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_object_detection/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_object_detection/detection_as_classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_object_detection/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_object_detection/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.336434 vision_datasets-1.0.0/vision_datasets/image_regression/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_regression/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_regression/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_regression/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.336434 vision_datasets-1.0.0/vision_datasets/image_text_matching/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_text_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_text_matching/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_text_matching/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_text_matching/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/image_text_matching/vision_as_image_text_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.336434 vision_datasets-1.0.0/vision_datasets/multi_task/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/multi_task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/multi_task/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/multi_task/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.336434 vision_datasets-1.0.0/vision_datasets/text_2_image_retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/text_2_image_retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/text_2_image_retrieval/coco_manifest_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/text_2_image_retrieval/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-28 07:31:45.000000 vision_datasets-1.0.0/vision_datasets/text_2_image_retrieval/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:31:59.312434 vision_datasets-1.0.0/vision_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-06-28 07:31:59.000000 vision_datasets-1.0.0/vision_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-06-28 07:31:59.000000 vision_datasets-1.0.0/vision_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 07:31:59.000000 vision_datasets-1.0.0/vision_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-28 07:31:59.000000 vision_datasets-1.0.0/vision_datasets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-28 07:31:59.000000 vision_datasets-1.0.0/vision_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 07:31:59.000000 vision_datasets-1.0.0/vision_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.921956 vision_datasets-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.921956 vision_datasets-1.0.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/resources/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_box_alteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_coco_adaptor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/coco_adaptor_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_caption_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_matting_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_regression_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_text_matching_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_multiclass_classification_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_multilabel_classification_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_multitask_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_object_detection_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_adaptor/test_text_2_image_retrieval_coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_coco_format_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_dataset_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45616 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_dataset_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_dataset_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_detection_as_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_ic_od_as_image_text_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_iris_format_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_manifest/test_pickleable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_manifest_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_manifest_to_coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_manifest_to_coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_manifest_to_coco/test_manifest_to_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_merge_manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_merge_manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_merge_manifest/test_manifest_merge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_sample/test_sample_manfiest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_spawn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_spawn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_spawn/test_spawn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/tests/test_torch_dataest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_torch_dataest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_torch_dataest/test_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/vision_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.929956 vision_datasets-1.0.1/vision_datasets/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/check_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/converter_od_to_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/converter_to_aml_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/converter_to_tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/converter_tsv_to_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/download_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/list_operations_by_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/commands/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.929956 vision_datasets-1.0.1/vision_datasets/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.929956 vision_datasets-1.0.1/vision_datasets/common/data_manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/data_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/iris_data_manifest_adaptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.929956 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/balanced_instance_weights_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/generate_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/remove_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_manifest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.929956 vision_datasets-1.0.1/vision_datasets/common/data_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_reader/dataset_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_reader/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/data_reader/image_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/common/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset/torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset/vision_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/common/dataset_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset_management/dataset_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/dataset_management/dataset_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/common/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/coco_manifest_adaptor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/data_manifest_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/common/factory/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/balanced_instance_weights_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/coco_generator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/manifest_merger_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/sampler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/spawn_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/split_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/factory/operations/supported_operations_by_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/image_caption/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_caption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_caption/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_caption/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_caption/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/image_classification/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_classification/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_classification/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_classification/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.933956 vision_datasets-1.0.1/vision_datasets/image_matting/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_matting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_matting/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_matting/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_matting/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/vision_datasets/image_object_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_object_detection/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_object_detection/detection_as_classification_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_object_detection/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_object_detection/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/vision_datasets/image_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_regression/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_regression/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_regression/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/vision_datasets/image_text_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_text_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_text_matching/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_text_matching/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_text_matching/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/image_text_matching/vision_as_image_text_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/vision_datasets/multi_task/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/multi_task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/multi_task/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/multi_task/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.937956 vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/coco_manifest_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-10 20:31:05.000000 vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:31:16.925956 vision_datasets-1.0.1/vision_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-07-10 20:31:16.000000 vision_datasets-1.0.1/vision_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-10 20:31:16.000000 vision_datasets-1.0.1/vision_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:31:16.000000 vision_datasets-1.0.1/vision_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-10 20:31:16.000000 vision_datasets-1.0.1/vision_datasets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-10 20:31:16.000000 vision_datasets-1.0.1/vision_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 20:31:16.000000 vision_datasets-1.0.1/vision_datasets.egg-info/top_level.txt
```

### Comparing `vision_datasets-1.0.0/LICENSE` & `vision_datasets-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/PKG-INFO` & `vision_datasets-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision_datasets
-Version: 1.0.0
+Version: 1.0.1
 Summary: A utility repo for vision dataset access and management.
 Home-page: https://github.com/microsoft/vision-datasets
 Author: Ping Jin, Shohei Ono
 License: MIT
 Keywords: vision datasets classification detection
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -122,21 +122,21 @@
 This repo offers the class `DatasetHub` for this purpose. Once instantiated with a json including the `DatasetInfo` for all datasets, you can retrieve a `VisionDataset` by
 
 ```python
 import pathlib
 from vision_datasets.common import Usages, DatasetHub
 
 dataset_infos_json_path = 'datasets.json'
-dataset_hub = DatasetHub(pathlib.Path(dataset_infos_json_path).read_text())
-stanford_cars = dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage=Usages.TRAIN)
+dataset_hub = DatasetHub(pathlib.Path(dataset_infos_json_path).read_text(), blob_container_sas, local_dir)
+stanford_cars = dataset_hub.create_manifest_dataset('stanford-cars', version=1, usage=Usages.TRAIN)
 
 # note that you can pass multiple datasets.json to DatasetHub, it can combine them all
 # example: DatasetHub([ds_json1, ds_json2, ...])
 # note that you can specify multiple usages in create_manifest_dataset call
-# example dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage=[Usages.TRAIN, Usages.VAL])
+# example dataset_hub.create_manifest_dataset('stanford-cars', version=1, usage=[Usages.TRAIN, Usages.VAL])
 
 for img, targets, sample_idx_str in stanford_cars:
     img.show()
     img.close()
     print(targets)
 ```
```

### Comparing `vision_datasets-1.0.0/README.md` & `vision_datasets-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -103,21 +103,21 @@
 This repo offers the class `DatasetHub` for this purpose. Once instantiated with a json including the `DatasetInfo` for all datasets, you can retrieve a `VisionDataset` by
 
 ```python
 import pathlib
 from vision_datasets.common import Usages, DatasetHub
 
 dataset_infos_json_path = 'datasets.json'
-dataset_hub = DatasetHub(pathlib.Path(dataset_infos_json_path).read_text())
-stanford_cars = dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage=Usages.TRAIN)
+dataset_hub = DatasetHub(pathlib.Path(dataset_infos_json_path).read_text(), blob_container_sas, local_dir)
+stanford_cars = dataset_hub.create_manifest_dataset('stanford-cars', version=1, usage=Usages.TRAIN)
 
 # note that you can pass multiple datasets.json to DatasetHub, it can combine them all
 # example: DatasetHub([ds_json1, ds_json2, ...])
 # note that you can specify multiple usages in create_manifest_dataset call
-# example dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage=[Usages.TRAIN, Usages.VAL])
+# example dataset_hub.create_manifest_dataset('stanford-cars', version=1, usage=[Usages.TRAIN, Usages.VAL])
 
 for img, targets, sample_idx_str in stanford_cars:
     img.show()
     img.close()
     print(targets)
 ```
```

### Comparing `vision_datasets-1.0.0/setup.py` & `vision_datasets-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 from os import path
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 
 # Get the long description from the README file
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(name='vision_datasets',
@@ -17,19 +17,22 @@
                  version=VERSION,
                  python_requires='>=3.8',
                  license='MIT',
                  keywords='vision datasets classification detection',
                  packages=setuptools.find_packages(),
                  package_data={'': ['resources/*']},
                  install_requires=[
+                     'azure-identity',
+                     'azure-storage-blob',
                      'numpy>=1.18.3',
                      'Pillow>=6.2.2',
                      'requests>=2.23.0',
                      'tenacity>=6.2.0',
                      'tqdm',
+                     'torch',
                      'matplotlib'
                  ],
                  classifiers=[
                      'Development Status :: 4 - Beta',
                      'Intended Audience :: Developers',
                      'License :: OSI Approved :: MIT License',
                      'Programming Language :: Python :: 3.8',
```

### Comparing `vision_datasets-1.0.0/tests/resources/util.py` & `vision_datasets-1.0.1/tests/resources/util.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_box_alteration.py` & `vision_datasets-1.0.1/tests/test_box_alteration.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_coco_adaptor/coco_adaptor_base.py` & `vision_datasets-1.0.1/tests/test_coco_adaptor/coco_adaptor_base.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_coco_adaptor/test_image_caption_coco_manifest_adaptor.py` & `vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_caption_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_coco_adaptor/test_image_matting_coco_manifest_adaptor.py` & `vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_matting_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_coco_adaptor/test_image_regression_coco_manifest_adaptor.py` & `vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_regression_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_coco_adaptor/test_image_text_matching_coco_manifest_adaptor.py` & `vision_datasets-1.0.1/tests/test_coco_adaptor/test_image_text_matching_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_coco_adaptor/test_multiclass_classification_coco_manifest_adaptor.py` & `vision_datasets-1.0.1/tests/test_coco_adaptor/test_multiclass_classification_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_coco_adaptor/test_multilabel_classification_coco_manifest_adaptor.py` & `vision_datasets-1.0.1/tests/test_coco_adaptor/test_multilabel_classification_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_coco_adaptor/test_object_detection_coco_manifest_adaptor.py` & `vision_datasets-1.0.1/tests/test_coco_adaptor/test_object_detection_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_coco_adaptor/test_text_2_image_retrieval_coco_manifest_adaptor.py` & `vision_datasets-1.0.1/tests/test_coco_adaptor/test_text_2_image_retrieval_coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_coco_format_manifest.py` & `vision_datasets-1.0.1/tests/test_coco_format_manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_dataset_downloader.py` & `vision_datasets-1.0.1/tests/test_dataset_downloader.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_dataset_manifest.py` & `vision_datasets-1.0.1/tests/test_dataset_manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_dataset_registry.py` & `vision_datasets-1.0.1/tests/test_dataset_registry.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_detection_as_classification.py` & `vision_datasets-1.0.1/tests/test_detection_as_classification.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_file_reader.py` & `vision_datasets-1.0.1/tests/test_file_reader.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_fixtures.py` & `vision_datasets-1.0.1/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_ic_od_as_image_text_dataset.py` & `vision_datasets-1.0.1/tests/test_ic_od_as_image_text_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_iris_format_manifest.py` & `vision_datasets-1.0.1/tests/test_iris_format_manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_manifest/test_pickleable.py` & `vision_datasets-1.0.1/tests/test_manifest/test_pickleable.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_manifest_dataset.py` & `vision_datasets-1.0.1/tests/test_manifest_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_manifest_to_coco/test_manifest_to_coco.py` & `vision_datasets-1.0.1/tests/test_manifest_to_coco/test_manifest_to_coco.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_merge_manifest/test_manifest_merge.py` & `vision_datasets-1.0.1/tests/test_merge_manifest/test_manifest_merge.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_sample/test_sample_manfiest.py` & `vision_datasets-1.0.1/tests/test_sample/test_sample_manfiest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_spawn/test_spawn.py` & `vision_datasets-1.0.1/tests/test_spawn/test_spawn.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/tests/test_utils.py` & `vision_datasets-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/__init__.py` & `vision_datasets-1.0.1/vision_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/commands/check_dataset.py` & `vision_datasets-1.0.1/vision_datasets/commands/check_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,29 +114,29 @@
     add_args_to_locate_dataset(parser)
     parser.add_argument('--quick_check', '-q', action='store_true', default=False, help='Randomly check a few data samples from the dataset.')
 
     args = parser.parse_args()
     prefix = logging_prefix(args.name, args.version)
 
     data_reg_json, usages = get_or_generate_data_reg_json_and_usages(args)
-    dataset_hub = DatasetHub(data_reg_json)
+    dataset_hub = DatasetHub(data_reg_json, args.blob_container, args.local_dir.as_posix())
     dataset_info = dataset_hub.dataset_registry.get_dataset_info(args.name, args.version)
 
     if not dataset_info:
         logger.error(f'{prefix} dataset does not exist.')
         return
 
     if args.blob_container and args.local_dir:
         args.local_dir.mkdir(parents=True, exist_ok=True)
 
     for usage in usages:
         logger.info(f'{prefix} Check dataset with usage: {usage}.')
 
         # if args.local_dir is none, then this check will directly try to access data from azure blob. Images must be present in uncompressed folder on azure blob.
-        dataset = dataset_hub.create_manifest_dataset(container_sas=args.blob_container, local_dir=args.local_dir, name=dataset_info.name, version=args.version, usage=usage, coordinates='absolute')
+        dataset = dataset_hub.create_vision_dataset(name=dataset_info.name, version=args.version, usage=usage, coordinates='absolute')
         if dataset:
             err_msg_file = pathlib.Path(f'{args.name}_{usage}_errors.txt')
             errors = []
             if args.data_type in [DatasetTypes.IMAGE_CLASSIFICATION_MULTICLASS, DatasetTypes.IMAGE_CLASSIFICATION_MULTILABEL, DatasetTypes.IMAGE_OBJECT_DETECTION]:
                 errors.extend(classification_detection_check(dataset))
 
             if args.quick_check:
```

### Comparing `vision_datasets-1.0.0/vision_datasets/commands/converter_od_to_ic.py` & `vision_datasets-1.0.1/vision_datasets/commands/converter_od_to_ic.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     return parser
 
 
 def process_usage(params):
     args, data_reg_json, aug_params, usage = params
 
     logger.info(f'download dataset manifest for {args.name}...')
-    dataset_resources = DatasetHub(data_reg_json)
-    dataset = dataset_resources.create_manifest_dataset(args.blob_container, str(args.local_dir.as_posix()), args.name, usage=usage, coordinates='absolute')
+    dataset_resources = DatasetHub(data_reg_json, args.blob_container, args.local_dir.as_posix())
+    dataset = dataset_resources.create_vision_dataset(args.name, usage=usage, coordinates='absolute')
     if not dataset:
         logger.info(f'Skipping non-existent phase {usage}.')
         return
 
     if dataset.dataset_info.type != DatasetTypes.IMAGE_OBJECT_DETECTION:
         raise ValueError(f'Data type must be {DatasetTypes.IMAGE_OBJECT_DETECTION}')
     logger.info(f'start conversion for {args.name}...')
```

### Comparing `vision_datasets-1.0.0/vision_datasets/commands/converter_to_aml_coco.py` & `vision_datasets-1.0.1/vision_datasets/commands/converter_to_aml_coco.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,27 +29,27 @@
 
 def main():
     args = create_arg_parser().parse_args()
     assert args.blob_container, '"blob_container" is required for generating "coco_url"'
     assert args.local_dir is None, 'Accessing data from "local_dir" is not supported for now. Data must be present in blob_container.'
 
     data_reg_json, usages = get_or_generate_data_reg_json_and_usages(args)
-    dataset_hub = DatasetHub(data_reg_json)
+    dataset_hub = DatasetHub(data_reg_json, args.blob_container, args.local_dir)
     dataset_info = dataset_hub.dataset_registry.get_dataset_info(args.name, args.version)
 
     if not dataset_info:
         logger.error(f'dataset {args.name} does not exist.')
         return
 
     assert dataset_info.type in [DatasetTypes.IMAGE_CLASSIFICATION_MULTICLASS, DatasetTypes.IMAGE_CLASSIFICATION_MULTILABEL, DatasetTypes.IMAGE_OBJECT_DETECTION]
 
     coco_gen = CocoDictGeneratorFactory.create(dataset_info.type)
     file_reader = FileReader()
     for usage in usages:
-        manifest = dataset_hub.create_dataset_manifest(args.blob_container, None, args.name, version=1, usage=usage)
+        manifest = dataset_hub.create_dataset_manifest(args.name, version=1, usage=usage)
         if not manifest:
             logger.info(f'{usage} not exist. Skipping.')
             continue
 
         manifest = manifest[0]
         coco_dict = coco_gen.run(manifest)
         for image in tqdm(coco_dict['images'], f'{usage}: Processing images...'):
```

### Comparing `vision_datasets-1.0.0/vision_datasets/commands/converter_to_tsv.py` & `vision_datasets-1.0.1/vision_datasets/commands/converter_to_tsv.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,23 +28,23 @@
     dataset_info = DatasetRegistry(data_reg_json).get_dataset_info(args.name, args.version)
     if not dataset_info:
         logger.error(f'{prefix} dataset does not exist.')
         return
     else:
         logger.info(f'{prefix} dataset found in registration file.')
 
-    vision_datasets = DatasetHub(data_reg_json)
+    vision_datasets = DatasetHub(data_reg_json, args.blob_container, args.local_dir.as_posix())
     if args.blob_container and args.local_dir:
         args.local_dir.mkdir(parents=True, exist_ok=True)
 
     for usage in usages:
         logger.info(f'{prefix} Check dataset with usage: {usage}.')
 
         # if args.local_dir is none, then this check will directly try to access data from azure blob. Images must be present in uncompressed folder on azure blob.
-        dataset_manifest = vision_datasets.create_dataset_manifest(container_sas=args.blob_container, local_dir=args.local_dir, name=dataset_info.name, version=args.version, usage=usage)
+        dataset_manifest = vision_datasets.create_dataset_manifest(name=dataset_info.name, version=args.version, usage=usage)
         if dataset_manifest:
             dataset_manifest = dataset_manifest[0]
             convert_to_tsv(dataset_manifest, args.output_dir / f"{usage}.tsv")
         else:
             logger.info(f'{prefix} No split for {usage} available.')
```

### Comparing `vision_datasets-1.0.0/vision_datasets/commands/converter_tsv_to_coco.py` & `vision_datasets-1.0.1/vision_datasets/commands/converter_tsv_to_coco.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/commands/download_dataset.py` & `vision_datasets-1.0.1/vision_datasets/commands/download_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Download a dataset from shared storage either in original format or converted to TSV
 """
 
 import argparse
 import pathlib
-import tempfile
 
 from vision_datasets.common import DatasetHub, DatasetRegistry, DatasetTypes
 from vision_datasets.commands.utils import add_args_to_locate_dataset_from_name_and_reg_json, convert_to_tsv, get_or_generate_data_reg_json_and_usages, set_up_cmd_logger
 
 logger = set_up_cmd_logger(__name__)
 
 TSV_SUPPORTED_TYPES = [DatasetTypes.IMAGE_CAPTION, DatasetTypes.IMAGE_OBJECT_DETECTION, DatasetTypes.IMAGE_CLASSIFICATION_MULTICLASS, DatasetTypes.IMAGE_CLASSIFICATION_MULTILABEL]
@@ -23,36 +22,34 @@
     parser = argparse.ArgumentParser('Download dataset from the shared storage')
     add_args_to_locate_dataset_from_name_and_reg_json(parser)
 
     parser.add_argument('--to_tsv', '-t', help='to tsv format or not.', action='store_true')
 
     args = parser.parse_args()
     dataset_reg_json, usages = get_or_generate_data_reg_json_and_usages(args)
-    dataset_hub = DatasetHub(dataset_reg_json)
+    dataset_hub = DatasetHub(dataset_reg_json, args.blob_container, args.local_dir)
     name = args.name
     dataset_info = dataset_hub.dataset_registry.get_dataset_info(name)
     args.local_dir.mkdir(parents=True, exist_ok=True)
 
     if args.to_tsv:
         if dataset_info.type not in TSV_SUPPORTED_TYPES:
             logger.error(f'Unsupported data type for converting to TSV: {dataset_info.type}.')
             return
 
-        with tempfile.TemporaryDirectory() as temp_dir:
-            dataset_info.root_folder = temp_dir / pathlib.Path(dataset_info.root_folder)
-            logger.info(f'downloading {name}...')
-            for usage in usages:
-                dataset_manifest = dataset_hub.create_dataset_manifest(args.blob_container, temp_dir, name, usage=usage)
-                if not dataset_manifest:
-                    continue
+        logger.info(f'downloading {name}...')
+        for usage in usages:
+            dataset_manifest = dataset_hub.create_dataset_manifest(name, usage=usage)
+            if not dataset_manifest:
+                continue
 
-                dataset_manifest = dataset_manifest[0]
+            dataset_manifest = dataset_manifest[0]
 
-                logger.info(f'converting {name}, usage {usage} to TSV format...')
-                convert_to_tsv(dataset_manifest, pathlib.Path(args.local_dir) / f'{name}-{usage}.tsv')
+            logger.info(f'converting {name}, usage {usage} to TSV format...')
+            convert_to_tsv(dataset_manifest, pathlib.Path(args.local_dir) / f'{name}-{usage}.tsv')
     else:
         for usage in usages:
-            dataset_hub.create_manifest_dataset(args.blob_container, args.local_dir, name, usage=usage)
+            dataset_hub.create_vision_dataset(name, usage=usage)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `vision_datasets-1.0.0/vision_datasets/commands/list_operations_by_data_type.py` & `vision_datasets-1.0.1/vision_datasets/commands/list_operations_by_data_type.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/commands/utils.py` & `vision_datasets-1.0.1/vision_datasets/commands/utils.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/__init__.py` & `vision_datasets-1.0.1/vision_datasets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/constants.py` & `vision_datasets-1.0.1/vision_datasets/common/constants.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/__init__.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/coco_manifest_adaptor.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/data_manifest.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/data_manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/iris_data_manifest_adaptor.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/iris_data_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/__init__.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/balanced_instance_weights_generator.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/balanced_instance_weights_generator.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/filter.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/filter.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/generate_coco.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/generate_coco.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/merge.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/merge.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/remove_categories.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/remove_categories.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/sample.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/sample.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/spawn.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/spawn.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/operations/split.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/operations/split.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_manifest/utils.py` & `vision_datasets-1.0.1/vision_datasets/common/data_manifest/utils.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_reader/file_reader.py` & `vision_datasets-1.0.1/vision_datasets/common/data_reader/file_reader.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/data_reader/image_loader.py` & `vision_datasets-1.0.1/vision_datasets/common/data_reader/image_loader.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/dataset/base_dataset.py` & `vision_datasets-1.0.1/vision_datasets/common/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/dataset/dataset.py` & `vision_datasets-1.0.1/vision_datasets/common/dataset/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from abc import ABC
+from abc import ABC, abstractclassmethod
 from inspect import signature
 
 import torch
 from PIL import ImageFile
 
 
 def _identity(*args):
     return args
 
 
 class _ImageOnlyTransform:
     def __init__(self, transform):
         self._transform = transform
 
-    def __call__(self, image, boxes):
-        return self._transform(image), boxes
+    def __call__(self, image, targets):
+        return self._transform(image), targets
 
 
 class Dataset(torch.utils.data.Dataset, ABC):
     def __init__(self, transform=None):
         super().__init__()
         self.transform = transform
         # Work around for corrupted files in datasets
         ImageFile.LOAD_TRUNCATED_IMAGES = True
 
     @property
-    def labels(self):
-        """Returns a list of labels."""
+    @abstractclassmethod
+    def categories(self):
+        """Returns a list of categories."""
         raise NotImplementedError
 
     @property
     def transform(self):
         return self._transform
 
     @transform.setter
```

### Comparing `vision_datasets-1.0.0/vision_datasets/common/dataset/torch_dataset.py` & `vision_datasets-1.0.1/vision_datasets/common/dataset/torch_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import logging
 
-from .vision_dataset import VisionDataset
 from .dataset import Dataset
+from .vision_dataset import VisionDataset
 
 logger = logging.getLogger(__name__)
 
 
 class TorchDataset(Dataset):
     """
     Dataset class used for pytorch training
     """
 
     def __init__(self, manifest_dataset: VisionDataset, transform=None):
         Dataset.__init__(self, transform)
         self.dataset = manifest_dataset
 
     @property
-    def labels(self):
+    def categories(self):
         return self.dataset.categories
 
     @property
     def dataset_resources(self):
         return self.dataset.dataset_resources
 
     @property
     def dataset_info(self):
         return self.dataset.dataset_info
 
     def __getitem__(self, index):
         if isinstance(index, int):
             image, target, idx_str = self.dataset[index]
-            image, target = self.transform(image, target.label_data)
+            image, target = self.transform(image, target)
             return image, target, idx_str
         else:
             return [self.transform(img, target) + (idx,) for img, target, idx in self.dataset[index]]
 
     def __len__(self):
         return len(self.dataset)
```

### Comparing `vision_datasets-1.0.0/vision_datasets/common/dataset/vision_dataset.py` & `vision_datasets-1.0.1/vision_datasets/common/dataset/vision_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/dataset_info.py` & `vision_datasets-1.0.1/vision_datasets/common/dataset_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,17 @@
             if usage_str in dataset_info_dict:
                 self.index_files[usage] = dataset_info_dict[usage_str]['index_path']
                 self.files_for_local_usage[usage] = dataset_info_dict[usage_str].get('files_for_local_usage', [])
 
         if self.data_format == AnnotationFormats.IRIS:
             self.labelmap = dataset_info_dict.get('labelmap')
             self.image_metadata_path = dataset_info_dict.get('image_metadata_path')
+        else:
+            self.labelmap = None
+            self.image_metadata_path = None
 
 
 class MultiTaskDatasetInfo(BaseDatasetInfo):
     def __init__(self, dataset_info_dict):
         if 'tasks' not in dataset_info_dict:
             raise ValueError
         data_type = _data_type_to_enum(dataset_info_dict.get('type'))
```

### Comparing `vision_datasets-1.0.0/vision_datasets/common/dataset_management/dataset_hub.py` & `vision_datasets-1.0.1/vision_datasets/common/dataset_management/dataset_hub.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,78 +14,73 @@
 
 class DatasetHub(object):
     """
     Hub class for managing vision dataset resources, with a few common utilities for creating a dataset.
     This hub class works with both resources on local disk or on azure blob.
     """
 
-    def __init__(self, dataset_json_str: Union[str, list]):
+    def __init__(self, dataset_json_str: Union[str, list], container_url: str, local_dir: str):
         """
-
+            If local_dir is provided, manifest_dataset consumes data from local disk. If data not present on local disk, it will be automatically downloaded.
+            if container_url is provided but local_dir not provided, manifest_dataset consumes data directly from container_url.
+            Note that for data stored in zipped files, they can be consumed locally without unzip. However, in blob they must be stored in unzipped folders. In this case image/label file paths can
+            stay with paths to data in zipped files, as dataset class will automatically look in the folder names same with the zip file names.
         Args:
             dataset_json_str (str, list): dataset registry json, containing multiple dataset_info for different datasets, or a list of dataset reg json
             retrievable by their names, versions and usages.
+            container_url (str): sas url to the container where datasets can be found/downloaded from
+            local_dir (str): local directory where datasets can be found/downloaded to
         """
         if not dataset_json_str:
             raise ValueError
-
+        if not container_url and not local_dir:
+            raise ValueError('either container_url or local_dir should be provided.')
         self.dataset_registry = DatasetRegistry(dataset_json_str)
+        self.container_url = container_url
+        self.local_dir = local_dir
 
-    def create_manifest_dataset(self, container_sas: str, local_dir: str, name: str, version: int = None, usage: Union[str, List] = Usages.TRAIN, coordinates: str = 'relative',
-                                few_shot_samples_per_class=None, rnd_seed=0):
+    def create_vision_dataset(self, name: str, version: int = None, usage: Union[str, List] = Usages.TRAIN, coordinates: str = 'relative',
+                              few_shot_samples_per_class=None, rnd_seed=0):
         """Create manifest dataset.
-            If local_dir is provided, manifest_dataset consumes data from local disk. If data not present on local disk, it will be automatically downloaded.
-            if container_sas is provided but local_dir not provided, manifest_dataset consumes data directly from container_sas.
 
             Note that for data stored in zipped files, they can be consumed locally without unzip. However, in blob they must be stored in unzipped folders. In this case image/label file paths can
             stay with paths to data in zipped files, as dataset class will automatically look in the folder names same with the zip file names.
 
         Args:
-            container_sas: sas url to the container where datasets can be found/downloaded from
-            local_dir: local directory where datasets can be found/downloaded to
             name: dataset name
             version: dataset version, if not specified, latest version will be returned
             usage: usage(s) of the dataset, 'train', 'val' or 'test' or a list of usages
             coordinates: format of the bounding boxes, can be 'relative' or 'absolute'
             few_shot_samples_per_class (int): get a sampled dataset with N images at most for each class (for detection and multilabel case, not guaranteed.)
             rnd_seed (int): random seed for few shot sampling
 
         Returns:
             an instance of dataset for local usage
         """
-        result = self.create_dataset_manifest(container_sas, local_dir, name, version, usage, few_shot_samples_per_class, rnd_seed)
+        result = self.create_dataset_manifest(name, version, usage, few_shot_samples_per_class, rnd_seed)
         if result:
             manifest, dataset_info, downloader_resources = result
         else:
             return None
 
         return VisionDataset(dataset_info, manifest, coordinates, downloader_resources)
 
-    def create_dataset_manifest(self, container_sas: str, local_dir: str, name: str, version: int = None, usage: Union[str, List] = Usages.TRAIN, few_shot_samples_per_class=None, rnd_seed=0):
+    def create_dataset_manifest(self, name: str, version: int = None, usage: Union[str, List] = Usages.TRAIN, few_shot_samples_per_class=None, rnd_seed=0):
         """Create dataset manifest.
-            If local_dir is provided, manifest_dataset consumes data from local disk. If data not present on local disk, it will be automatically downloaded.
-            if container_sas is provided but local_dir not provided, manifest_dataset consumes data directly from container_sas.
-
-            Note that for data stored in zipped files, they can be consumed locally without unzip. However, in blob they must be stored in unzipped folders. In this case image/label file paths can
-            stay with paths to data in zipped files, as dataset class will automatically look in the folder names same with the zip file names.
 
         Args:
-            container_sas: sas url to the container where datasets can be found/downloaded from
-            local_dir: local directory where datasets can be found/downloaded to
             name: dataset name
             version: dataset version, if not specified, latest version will be returned
             usage: usage(s) of the dataset, 'train', 'val' or 'test' or a list of usages
             few_shot_samples_per_class (int): get a sampled dataset with N images at most for each class (for detection and multilabel case, not guaranteed.)
             rnd_seed (int): random seed for few shot sampling
 
         Returns:
             dataset manifest, dataset_info, downloaded_resources, if dataset exists, else None
         """
-        if not container_sas and not local_dir:
-            raise ValueError('either container_sas or local_dir should be provided.')
         if not name:
             raise ValueError
         if not usage:
             raise ValueError
 
         usages = usage if isinstance(usage, list) else [usage]
 
@@ -98,29 +93,29 @@
 
         if isinstance(dataset_info, MultiTaskDatasetInfo):
             for task_info in dataset_info.sub_task_infos.values():
                 task_info.index_files = {usage: task_info.index_files[usage] for usage in usages if usage in task_info.index_files}
         else:
             dataset_info.index_files = {usage: dataset_info.index_files[usage] for usage in usages if usage in dataset_info.index_files}
 
-        if container_sas and local_dir:
-            downloader = DatasetDownloader(container_sas, self.dataset_registry.get_dataset_info(name, version))
-            downloader_resources_usage = downloader.download(local_dir, usages)
+        if self.container_url and self.local_dir:
+            downloader = DatasetDownloader(self.container_url, self.dataset_registry.get_dataset_info(name, version))
+            downloader_resources_usage = downloader.download(self.local_dir, usages)
         else:
             downloader_resources_usage = None
 
         for usage in usages:
-            manifest_usage = DataManifestFactory.create(dataset_info, usage, local_dir or container_sas)
+            manifest_usage = DataManifestFactory.create(dataset_info, usage, self.local_dir or self.container_url)
             if manifest_usage is not None:
+                print(f"!! {usage}")
                 merger = ManifestMerger(ManifestMergeStrategyFactory.create(dataset_info.type))
                 manifest = merger.run(manifest, manifest_usage) if manifest else manifest_usage
 
             if downloader_resources_usage:
                 downloader_resources = DownloadedDatasetsResources.merge(downloader_resources, downloader_resources_usage) if downloader_resources else downloader_resources_usage
-
         if manifest is None:
             return None
 
         if few_shot_samples_per_class:
             original_img_cnt = len(manifest.images)
             manifest = manifest.sample_few_shot_subset(few_shot_samples_per_class, rnd_seed)
             logger.info(f'Create a few-shot dataset with n samples per class = {few_shot_samples_per_class}. # images: {original_img_cnt} => {len(manifest.images)}')
```

### Comparing `vision_datasets-1.0.0/vision_datasets/common/dataset_management/dataset_registry.py` & `vision_datasets-1.0.1/vision_datasets/common/dataset_management/dataset_registry.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/factory/__init__.py` & `vision_datasets-1.0.1/vision_datasets/common/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/factory/data_manifest_factory.py` & `vision_datasets-1.0.1/vision_datasets/common/factory/data_manifest_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/factory/operations/__init__.py` & `vision_datasets-1.0.1/vision_datasets/common/factory/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/factory/operations/balanced_instance_weights_factory.py` & `vision_datasets-1.0.1/vision_datasets/common/factory/operations/balanced_instance_weights_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/factory/operations/coco_generator_factory.py` & `vision_datasets-1.0.1/vision_datasets/common/factory/operations/coco_generator_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/factory/operations/manifest_merger_factory.py` & `vision_datasets-1.0.1/vision_datasets/common/factory/operations/manifest_merger_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/factory/operations/sampler_factory.py` & `vision_datasets-1.0.1/vision_datasets/common/factory/operations/sampler_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/factory/operations/spawn_factory.py` & `vision_datasets-1.0.1/vision_datasets/common/factory/operations/spawn_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/factory/operations/split_factory.py` & `vision_datasets-1.0.1/vision_datasets/common/factory/operations/split_factory.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/common/utils.py` & `vision_datasets-1.0.1/vision_datasets/common/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,16 +55,16 @@
             return unix_path(os.path.join(*to_join))
     else:
         full_path_func = unix_path
 
     return full_path_func
 
 
-def _construct_full_url_generator(container_sas: str):
-    if not container_sas:
+def _construct_full_url_generator(container_url: str):
+    if not container_url:
         return unix_path
 
     def add_path_to_url(url, path_or_dir):
         if not url:
             raise ValueError
 
         if not path_or_dir:
@@ -74,15 +74,15 @@
         path = unix_path(os.path.join(parts[2], path_or_dir))
         url = urlparse.urlunparse((parts[0], parts[1], path, parts[3], parts[4], parts[5]))
 
         return url
 
     def func(file_path):
         file_path = file_path.replace('.zip@', '/')  # cannot read from zip file with path targeting a url
-        return add_path_to_url(container_sas, file_path)
+        return add_path_to_url(container_url, file_path)
 
     return func
 
 
 def construct_full_url_or_path_func(url_or_root_dir: Union[str, pathlib.Path], prefix_dir: Union[str, pathlib.Path] = None):
     if url_or_root_dir and can_be_url(url_or_root_dir):
         return lambda path: _construct_full_url_generator(url_or_root_dir)(_construct_full_path_generator([prefix_dir])(path))
```

### Comparing `vision_datasets-1.0.0/vision_datasets/image_caption/coco_manifest_adaptor.py` & `vision_datasets-1.0.1/vision_datasets/image_caption/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_caption/operations.py` & `vision_datasets-1.0.1/vision_datasets/image_caption/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_classification/coco_manifest_adaptor.py` & `vision_datasets-1.0.1/vision_datasets/image_classification/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_classification/manifest.py` & `vision_datasets-1.0.1/vision_datasets/image_classification/manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_classification/operations.py` & `vision_datasets-1.0.1/vision_datasets/image_classification/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_matting/coco_manifest_adaptor.py` & `vision_datasets-1.0.1/vision_datasets/image_matting/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_matting/manifest.py` & `vision_datasets-1.0.1/vision_datasets/image_matting/manifest.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_matting/operations.py` & `vision_datasets-1.0.1/vision_datasets/image_matting/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_object_detection/__init__.py` & `vision_datasets-1.0.1/vision_datasets/image_object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_object_detection/coco_manifest_adaptor.py` & `vision_datasets-1.0.1/vision_datasets/image_object_detection/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_object_detection/detection_as_classification_dataset.py` & `vision_datasets-1.0.1/vision_datasets/image_object_detection/detection_as_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_object_detection/operations.py` & `vision_datasets-1.0.1/vision_datasets/image_object_detection/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_regression/coco_manifest_adaptor.py` & `vision_datasets-1.0.1/vision_datasets/image_regression/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_regression/operations.py` & `vision_datasets-1.0.1/vision_datasets/image_regression/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_text_matching/coco_manifest_adaptor.py` & `vision_datasets-1.0.1/vision_datasets/image_text_matching/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_text_matching/operations.py` & `vision_datasets-1.0.1/vision_datasets/image_text_matching/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/image_text_matching/vision_as_image_text_dataset.py` & `vision_datasets-1.0.1/vision_datasets/image_text_matching/vision_as_image_text_dataset.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/multi_task/coco_manifest_adaptor.py` & `vision_datasets-1.0.1/vision_datasets/multi_task/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/multi_task/operations.py` & `vision_datasets-1.0.1/vision_datasets/multi_task/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/text_2_image_retrieval/coco_manifest_adaptor.py` & `vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/coco_manifest_adaptor.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets/text_2_image_retrieval/operations.py` & `vision_datasets-1.0.1/vision_datasets/text_2_image_retrieval/operations.py`

 * *Files identical despite different names*

### Comparing `vision_datasets-1.0.0/vision_datasets.egg-info/PKG-INFO` & `vision_datasets-1.0.1/vision_datasets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-datasets
-Version: 1.0.0
+Version: 1.0.1
 Summary: A utility repo for vision dataset access and management.
 Home-page: https://github.com/microsoft/vision-datasets
 Author: Ping Jin, Shohei Ono
 License: MIT
 Keywords: vision datasets classification detection
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -122,21 +122,21 @@
 This repo offers the class `DatasetHub` for this purpose. Once instantiated with a json including the `DatasetInfo` for all datasets, you can retrieve a `VisionDataset` by
 
 ```python
 import pathlib
 from vision_datasets.common import Usages, DatasetHub
 
 dataset_infos_json_path = 'datasets.json'
-dataset_hub = DatasetHub(pathlib.Path(dataset_infos_json_path).read_text())
-stanford_cars = dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage=Usages.TRAIN)
+dataset_hub = DatasetHub(pathlib.Path(dataset_infos_json_path).read_text(), blob_container_sas, local_dir)
+stanford_cars = dataset_hub.create_manifest_dataset('stanford-cars', version=1, usage=Usages.TRAIN)
 
 # note that you can pass multiple datasets.json to DatasetHub, it can combine them all
 # example: DatasetHub([ds_json1, ds_json2, ...])
 # note that you can specify multiple usages in create_manifest_dataset call
-# example dataset_hub.create_manifest_dataset(blob_container_sas, local_dir, 'stanford-cars', version=1, usage=[Usages.TRAIN, Usages.VAL])
+# example dataset_hub.create_manifest_dataset('stanford-cars', version=1, usage=[Usages.TRAIN, Usages.VAL])
 
 for img, targets, sample_idx_str in stanford_cars:
     img.show()
     img.close()
     print(targets)
 ```
```

### Comparing `vision_datasets-1.0.0/vision_datasets.egg-info/SOURCES.txt` & `vision_datasets-1.0.1/vision_datasets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 tests/test_dataset_registry.py
 tests/test_detection_as_classification.py
 tests/test_file_reader.py
 tests/test_fixtures.py
 tests/test_ic_od_as_image_text_dataset.py
 tests/test_iris_format_manifest.py
 tests/test_manifest_dataset.py
-tests/test_pytorch_dataset.py
 tests/test_utils.py
 tests/resources/__init__.py
 tests/resources/util.py
 tests/test_coco_adaptor/__init__.py
 tests/test_coco_adaptor/coco_adaptor_base.py
 tests/test_coco_adaptor/test_image_caption_coco_manifest_adaptor.py
 tests/test_coco_adaptor/test_image_matting_coco_manifest_adaptor.py
@@ -34,14 +33,16 @@
 tests/test_manifest_to_coco/test_manifest_to_coco.py
 tests/test_merge_manifest/__init__.py
 tests/test_merge_manifest/test_manifest_merge.py
 tests/test_sample/__init__.py
 tests/test_sample/test_sample_manfiest.py
 tests/test_spawn/__init__.py
 tests/test_spawn/test_spawn.py
+tests/test_torch_dataest/__init__.py
+tests/test_torch_dataest/test_torch_dataset.py
 vision_datasets/__init__.py
 vision_datasets.egg-info/PKG-INFO
 vision_datasets.egg-info/SOURCES.txt
 vision_datasets.egg-info/dependency_links.txt
 vision_datasets.egg-info/entry_points.txt
 vision_datasets.egg-info/requires.txt
 vision_datasets.egg-info/top_level.txt
```

