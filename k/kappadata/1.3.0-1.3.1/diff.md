# Comparing `tmp/kappadata-1.3.0.tar.gz` & `tmp/kappadata-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappadata-1.3.0.tar", last modified: Mon Jul  3 08:01:28 2023, max compression
+gzip compressed data, was "kappadata-1.3.1.tar", last modified: Mon Jul 10 14:45:50 2023, max compression
```

## Comparing `kappadata-1.3.0.tar` & `kappadata-1.3.1.tar`

### file list

```diff
@@ -1,195 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.146218 kappadata-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-03 07:59:05.000000 kappadata-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-03 08:01:28.146218 kappadata-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-03 07:59:05.000000 kappadata-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.110219 kappadata-1.3.0/kappadata/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-03 08:01:10.000000 kappadata-1.3.0/kappadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.110219 kappadata-1.3.0/kappadata/caching/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/caching/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/caching/shared_dict_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.114219 kappadata-1.3.0/kappadata/collators/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.114219 kappadata-1.3.0/kappadata/collators/base/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/base/kd_collator_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/base/kd_compose_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/base/kd_single_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/kd_mix_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/pad_sequences_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.114219 kappadata-1.3.0/kappadata/common/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.114219 kappadata-1.3.0/kappadata/common/collators/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/collators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/collators/mae_finetune_mix_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.114219 kappadata-1.3.0/kappadata/common/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/datasets/kd_image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.114219 kappadata-1.3.0/kappadata/common/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/byol_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/imagenet_minaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/imagenet_noaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/mae_finetune_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.118219 kappadata-1.3.0/kappadata/common/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/norm/kd_ade20k_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/norm/kd_cifar100_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/norm/kd_cifar10_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/norm/kd_image_net_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.118219 kappadata-1.3.0/kappadata/common/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.118219 kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.118219 kappadata-1.3.0/kappadata/copying/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/copying/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/copying/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/copying/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.118219 kappadata-1.3.0/kappadata/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/datasets/kd_concat_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/datasets/kd_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/datasets/kd_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/datasets/kd_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/error_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.118219 kappadata-1.3.0/kappadata/loading/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/loading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/loading/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.122218 kappadata-1.3.0/kappadata/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/distributed_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/infinite_batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/interleaved_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/semi_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/sequential_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.130219 kappadata-1.3.0/kappadata/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.130219 kappadata-1.3.0/kappadata/transforms/base/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/kd_compose_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/kd_identity_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/kd_random_apply_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/kd_scheduled_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/kd_stochastic_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/kd_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/image_pos_embed_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/image_pos_embed_sincos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_additive_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_bucketize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_columnwise_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_grayscale.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_minsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_rand_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_rand_augment_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_additive_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_erasing.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_grayscale.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_resized_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_rearrange.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_simple_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_three_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_two_random_crop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.134219 kappadata-1.3.0/kappadata/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/norm/kd_image_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/norm/kd_image_range_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/norm/kd_norm_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/patchify_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/patchwise_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/patchwise_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/patchwise_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/save_state_to_context_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.134219 kappadata-1.3.0/kappadata/transforms/semseg/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/semseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_random_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_random_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/unpatchify_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.138218 kappadata-1.3.0/kappadata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/bounding_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/class_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/color_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/getall_class_as_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/magnitude_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/multi_crop_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/one_hot.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/param_checking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/pos_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/transform_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.138218 kappadata-1.3.0/kappadata/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_dataset_imgsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_jigsaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_mae_schematic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_masked_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_two_random_crop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.142218 kappadata-1.3.0/kappadata/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.142218 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/mode_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.146218 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.146218 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/x_repeat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/torch_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.110219 kappadata-1.3.0/kappadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-03 08:01:28.000000 kappadata-1.3.0/kappadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-07-03 08:01:28.000000 kappadata-1.3.0/kappadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:01:28.000000 kappadata-1.3.0/kappadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-03 08:01:28.000000 kappadata-1.3.0/kappadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 08:01:28.000000 kappadata-1.3.0/kappadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-03 07:59:05.000000 kappadata-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-03 08:01:28.146218 kappadata-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:50.023173 kappadata-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-10 14:43:25.000000 kappadata-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-10 14:45:50.023173 kappadata-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-10 14:43:25.000000 kappadata-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.979172 kappadata-1.3.1/kappadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 14:45:33.000000 kappadata-1.3.1/kappadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.979172 kappadata-1.3.1/kappadata/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/caching/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/caching/shared_dict_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.979172 kappadata-1.3.1/kappadata/collators/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/collators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.979172 kappadata-1.3.1/kappadata/collators/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/collators/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/collators/base/kd_collator_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/collators/base/kd_compose_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/collators/base/kd_single_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/collators/kd_mix_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/collators/pad_sequences_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.979172 kappadata-1.3.1/kappadata/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.979172 kappadata-1.3.1/kappadata/common/collators/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/collators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/collators/mae_finetune_mix_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.979172 kappadata-1.3.1/kappadata/common/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/datasets/kd_image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.979172 kappadata-1.3.1/kappadata/common/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/transforms/byol_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/transforms/imagenet_minaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/transforms/imagenet_noaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/transforms/mae_finetune_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.983172 kappadata-1.3.1/kappadata/common/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/transforms/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/transforms/norm/kd_ade20k_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/transforms/norm/kd_cifar100_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/transforms/norm/kd_cifar10_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/transforms/norm/kd_image_net_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.983172 kappadata-1.3.1/kappadata/common/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.983172 kappadata-1.3.1/kappadata/common/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/wrappers/sample_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.987172 kappadata-1.3.1/kappadata/copying/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/copying/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/copying/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/copying/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.987172 kappadata-1.3.1/kappadata/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/datasets/kd_concat_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/datasets/kd_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/datasets/kd_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/datasets/kd_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/error_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.987172 kappadata-1.3.1/kappadata/loading/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/loading/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.991172 kappadata-1.3.1/kappadata/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/samplers/distributed_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/samplers/infinite_batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/samplers/interleaved_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/samplers/semi_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/samplers/sequential_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:50.003172 kappadata-1.3.1/kappadata/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:50.003172 kappadata-1.3.1/kappadata/transforms/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/base/kd_compose_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/base/kd_identity_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/base/kd_random_apply_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/base/kd_scheduled_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/base/kd_stochastic_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/base/kd_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/image_pos_embed_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/image_pos_embed_sincos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_additive_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_bucketize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_columnwise_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_minsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_rand_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_rand_augment_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_random_additive_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_random_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_random_erasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_random_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_random_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_random_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_random_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_random_resized_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_random_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_random_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_rearrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_simple_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_three_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/kd_two_random_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:50.003172 kappadata-1.3.1/kappadata/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/norm/kd_image_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/norm/kd_image_range_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/norm/kd_norm_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/patchify_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/patchwise_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/patchwise_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/patchwise_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/save_state_to_context_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:50.007172 kappadata-1.3.1/kappadata/transforms/semseg/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/semseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/semseg/kd_semseg_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/semseg/kd_semseg_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/semseg/kd_semseg_random_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/semseg/kd_semseg_random_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/semseg/kd_semseg_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/transforms/unpatchify_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:50.011173 kappadata-1.3.1/kappadata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/bounding_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/class_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/color_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/getall_class_as_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/magnitude_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/multi_crop_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/param_checking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/pos_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/utils/transform_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:50.015173 kappadata-1.3.1/kappadata/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/visualization/visualize_dataset_imgsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/visualization/visualize_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/visualization/visualize_jigsaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/visualization/visualize_mae_schematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/visualization/visualize_masked_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/visualization/visualize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/visualization/visualize_two_random_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:50.015173 kappadata-1.3.1/kappadata/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:50.019173 kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/mode_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:50.023173 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:50.023173 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/x_repeat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-10 14:43:25.000000 kappadata-1.3.1/kappadata/wrappers/torch_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:49.979172 kappadata-1.3.1/kappadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-10 14:45:49.000000 kappadata-1.3.1/kappadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-10 14:45:49.000000 kappadata-1.3.1/kappadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:45:49.000000 kappadata-1.3.1/kappadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 14:45:49.000000 kappadata-1.3.1/kappadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 14:45:49.000000 kappadata-1.3.1/kappadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 14:43:25.000000 kappadata-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-10 14:45:50.027173 kappadata-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:45:50.023173 kappadata-1.3.1/test_unit_long/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:43:25.000000 kappadata-1.3.1/test_unit_long/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-10 14:43:25.000000 kappadata-1.3.1/test_unit_long/test_stochastic_transform_seed.py
```

### Comparing `kappadata-1.3.0/LICENSE` & `kappadata-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/PKG-INFO` & `kappadata-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappadata-1.3.0/README.md` & `kappadata-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/__init__.py` & `kappadata-1.3.1/kappadata/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 import kappadata.caching
 import kappadata.collators
 import kappadata.common
 import kappadata.copying
 import kappadata.datasets
 import kappadata.loading
```

### Comparing `kappadata-1.3.0/kappadata/caching/cached_dataset.py` & `kappadata-1.3.1/kappadata/caching/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/caching/shared_dict_dataset.py` & `kappadata-1.3.1/kappadata/caching/shared_dict_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/collators/base/kd_collator_base.py` & `kappadata-1.3.1/kappadata/collators/base/kd_collator_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/collators/base/kd_compose_collator.py` & `kappadata-1.3.1/kappadata/collators/base/kd_compose_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/collators/base/kd_single_collator.py` & `kappadata-1.3.1/kappadata/collators/base/kd_single_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/collators/kd_mix_collator.py` & `kappadata-1.3.1/kappadata/collators/kd_mix_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/collators/pad_sequences_collator.py` & `kappadata-1.3.1/kappadata/collators/pad_sequences_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/common/datasets/kd_image_folder.py` & `kappadata-1.3.1/kappadata/common/datasets/kd_image_folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/common/transforms/byol_transforms.py` & `kappadata-1.3.1/kappadata/common/transforms/byol_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/common/transforms/imagenet_minaug_transforms.py` & `kappadata-1.3.1/kappadata/common/transforms/imagenet_minaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/common/transforms/imagenet_noaug_transforms.py` & `kappadata-1.3.1/kappadata/common/transforms/imagenet_noaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/common/transforms/mae_finetune_transform.py` & `kappadata-1.3.1/kappadata/common/transforms/mae_finetune_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py` & `kappadata-1.3.1/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py` & `kappadata-1.3.1/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py` & `kappadata-1.3.1/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/copying/folder.py` & `kappadata-1.3.1/kappadata/copying/folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/copying/image_folder.py` & `kappadata-1.3.1/kappadata/copying/image_folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/datasets/kd_concat_dataset.py` & `kappadata-1.3.1/kappadata/datasets/kd_concat_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/datasets/kd_dataset.py` & `kappadata-1.3.1/kappadata/datasets/kd_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/datasets/kd_subset.py` & `kappadata-1.3.1/kappadata/datasets/kd_subset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/datasets/kd_wrapper.py` & `kappadata-1.3.1/kappadata/datasets/kd_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/factory.py` & `kappadata-1.3.1/kappadata/factory.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/samplers/distributed_sampler.py` & `kappadata-1.3.1/kappadata/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/samplers/infinite_batch_sampler.py` & `kappadata-1.3.1/kappadata/samplers/infinite_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/samplers/interleaved_sampler.py` & `kappadata-1.3.1/kappadata/samplers/interleaved_sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,27 +176,26 @@
         self.batch_sampler = _InterleavedBatchSampler(self)
 
     def get_data_loader(
             self,
             num_workers: int = 0,
             pin_memory: bool = False,
             prefetch_factor: int = None,
-            worker_init_fn = None,
     ) -> DataLoader:
         # the default value of prefetch_factor changed from 2 to None in pytorch 2.0 -> pass via optional kwarg
         kwargs = {}
         if num_workers > 0 and prefetch_factor is not None:
             kwargs["prefetch_factor"] = prefetch_factor
         return DataLoader(
             dataset=self.dataset,
             batch_sampler=self.batch_sampler,
             collate_fn=self.collator,
             num_workers=num_workers,
             pin_memory=pin_memory,
-            worker_init_fn=worker_init_fn,
+            worker_init_fn=self.dataset.worker_init_fn,
             **kwargs,
         )
 
     def __iter__(self):
         if self.epochs == 0 or self.updates == 0 or self.samples == 0:
             assert self.start_epoch == 0 and self.start_update == 0 and self.start_sample == 0
             yield from self._eval_loop()
```

### Comparing `kappadata-1.3.0/kappadata/samplers/random_sampler.py` & `kappadata-1.3.1/kappadata/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/samplers/semi_sampler.py` & `kappadata-1.3.1/kappadata/samplers/semi_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/__init__.py` & `kappadata-1.3.1/kappadata/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/base/kd_compose_transform.py` & `kappadata-1.3.1/kappadata/transforms/base/kd_compose_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/base/kd_random_apply_base.py` & `kappadata-1.3.1/kappadata/transforms/base/kd_random_apply_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/base/kd_scheduled_transform.py` & `kappadata-1.3.1/kappadata/transforms/base/kd_scheduled_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/base/kd_stochastic_transform.py` & `kappadata-1.3.1/kappadata/transforms/base/kd_stochastic_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/base/kd_transform.py` & `kappadata-1.3.1/kappadata/transforms/base/kd_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from torch.utils.data import get_worker_info
-
+import numpy as np
 
 class KDTransform:
     def __init__(self, ctx_prefix: str = None):
         self.ctx_prefix = ctx_prefix or type(self).__name__
         # sanity check to avoid accidentally overwriting base method
         assert type(self).scale_strength == KDTransform.scale_strength
         assert type(self).worker_init_fn == KDTransform.worker_init_fn
@@ -27,14 +27,15 @@
         # if num_workers the worker_init_fn can be called manually although this is not recommended
         # e.g. the counter of a scheduled transform will be a global object and therefore no longer be correct
         info = get_worker_info()
         if info is None:
             num_workers = 1
         else:
             num_workers = info.num_workers
+        self.set_rng(np.random.default_rng(seed=info.seed))
         self._worker_init_fn(rank, num_workers, **kwargs)
 
     def _worker_init_fn(self, rank, num_workers, **kwargs):
         pass
 
     def scale_strength(self, factor):
         assert 0. <= factor <= 1.
```

### Comparing `kappadata-1.3.0/kappadata/transforms/image_pos_embed_grid.py` & `kappadata-1.3.1/kappadata/transforms/image_pos_embed_grid.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/image_pos_embed_sincos.py` & `kappadata-1.3.1/kappadata/transforms/image_pos_embed_sincos.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_additive_gaussian_noise.py` & `kappadata-1.3.1/kappadata/transforms/kd_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_bucketize.py` & `kappadata-1.3.1/kappadata/transforms/kd_bucketize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_color_jitter.py` & `kappadata-1.3.1/kappadata/transforms/kd_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_columnwise_norm.py` & `kappadata-1.3.1/kappadata/transforms/kd_columnwise_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_gaussian_blur_pil.py` & `kappadata-1.3.1/kappadata/transforms/kd_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_gaussian_blur_tv.py` & `kappadata-1.3.1/kappadata/transforms/kd_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_minsize.py` & `kappadata-1.3.1/kappadata/transforms/kd_minsize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_rand_augment.py` & `kappadata-1.3.1/kappadata/transforms/kd_rand_augment.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_random_additive_gaussian_noise.py` & `kappadata-1.3.1/kappadata/transforms/kd_random_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_random_apply.py` & `kappadata-1.3.1/kappadata/transforms/kd_random_apply.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_random_color_jitter.py` & `kappadata-1.3.1/kappadata/transforms/kd_random_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_random_crop.py` & `kappadata-1.3.1/kappadata/transforms/kd_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_random_erasing.py` & `kappadata-1.3.1/kappadata/transforms/kd_random_erasing.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_random_gaussian_blur_pil.py` & `kappadata-1.3.1/kappadata/transforms/kd_random_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_random_gaussian_blur_tv.py` & `kappadata-1.3.1/kappadata/transforms/kd_random_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_random_grayscale.py` & `kappadata-1.3.1/kappadata/transforms/kd_random_grayscale.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_random_resized_crop.py` & `kappadata-1.3.1/kappadata/transforms/kd_random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_random_rotation.py` & `kappadata-1.3.1/kappadata/transforms/kd_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_random_solarize.py` & `kappadata-1.3.1/kappadata/transforms/kd_random_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_random_threshold.py` & `kappadata-1.3.1/kappadata/transforms/kd_random_threshold.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_resize.py` & `kappadata-1.3.1/kappadata/transforms/kd_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_simple_random_crop.py` & `kappadata-1.3.1/kappadata/transforms/kd_simple_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_solarize.py` & `kappadata-1.3.1/kappadata/transforms/kd_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_three_augment.py` & `kappadata-1.3.1/kappadata/transforms/kd_three_augment.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_threshold.py` & `kappadata-1.3.1/kappadata/transforms/kd_threshold.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/kd_two_random_crop.py` & `kappadata-1.3.1/kappadata/transforms/kd_two_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/norm/kd_image_norm.py` & `kappadata-1.3.1/kappadata/transforms/norm/kd_image_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/norm/kd_image_range_norm.py` & `kappadata-1.3.1/kappadata/transforms/norm/kd_image_range_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/norm/kd_norm_base.py` & `kappadata-1.3.1/kappadata/transforms/norm/kd_norm_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/patchify_image.py` & `kappadata-1.3.1/kappadata/transforms/patchify_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/patchwise_norm.py` & `kappadata-1.3.1/kappadata/transforms/patchwise_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/patchwise_random_rotation.py` & `kappadata-1.3.1/kappadata/transforms/patchwise_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_pad.py` & `kappadata-1.3.1/kappadata/transforms/semseg/kd_semseg_pad.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_random_crop.py` & `kappadata-1.3.1/kappadata/transforms/semseg/kd_semseg_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_random_resize.py` & `kappadata-1.3.1/kappadata/transforms/semseg/kd_semseg_random_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_resize.py` & `kappadata-1.3.1/kappadata/transforms/semseg/kd_semseg_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/utils/bounding_box_utils.py` & `kappadata-1.3.1/kappadata/utils/bounding_box_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/utils/class_counts.py` & `kappadata-1.3.1/kappadata/utils/class_counts.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/utils/color_histogram.py` & `kappadata-1.3.1/kappadata/utils/color_histogram.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/utils/hash_utils.py` & `kappadata-1.3.1/kappadata/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/utils/magnitude_sampler.py` & `kappadata-1.3.1/kappadata/utils/magnitude_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/utils/multi_crop_utils.py` & `kappadata-1.3.1/kappadata/utils/multi_crop_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/utils/pos_embed.py` & `kappadata-1.3.1/kappadata/utils/pos_embed.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/utils/save_image.py` & `kappadata-1.3.1/kappadata/utils/save_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/utils/transform_utils.py` & `kappadata-1.3.1/kappadata/utils/transform_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/visualization/visualize_dataset_imgsize.py` & `kappadata-1.3.1/kappadata/visualization/visualize_dataset_imgsize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/visualization/visualize_interpolation.py` & `kappadata-1.3.1/kappadata/visualization/visualize_interpolation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/visualization/visualize_jigsaw.py` & `kappadata-1.3.1/kappadata/visualization/visualize_jigsaw.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/visualization/visualize_mae_schematic.py` & `kappadata-1.3.1/kappadata/visualization/visualize_mae_schematic.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/visualization/visualize_masked_image.py` & `kappadata-1.3.1/kappadata/visualization/visualize_masked_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/visualization/visualize_transform.py` & `kappadata-1.3.1/kappadata/visualization/visualize_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/visualization/visualize_two_random_crop.py` & `kappadata-1.3.1/kappadata/visualization/visualize_two_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py` & `kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py` & `kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py` & `kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py` & `kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py` & `kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py` & `kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/subset_wrapper.py` & `kappadata-1.3.1/kappadata/wrappers/dataset_wrappers/subset_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/wrappers/mode_wrapper.py` & `kappadata-1.3.1/kappadata/wrappers/mode_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py` & `kappadata-1.3.1/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py` & `kappadata-1.3.1/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py` & `kappadata-1.3.1/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py` & `kappadata-1.3.1/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata/wrappers/torch_wrapper.py` & `kappadata-1.3.1/kappadata/wrappers/torch_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.0/kappadata.egg-info/PKG-INFO` & `kappadata-1.3.1/kappadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappadata-1.3.0/kappadata.egg-info/SOURCES.txt` & `kappadata-1.3.1/kappadata.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -149,19 +149,20 @@
 kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
 kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py
 kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
 kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
 kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
 kappadata/wrappers/dataset_wrappers/subset_wrapper.py
 kappadata/wrappers/sample_wrappers/__init__.py
-kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py
 kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
 kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
 kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
 kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py
 kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
 kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
 kappadata/wrappers/sample_wrappers/x_repeat_wrapper.py
 kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
 kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
 kappadata/wrappers/sample_wrappers/base/__init__.py
-kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
+kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
+test_unit_long/__init__.py
+test_unit_long/test_stochastic_transform_seed.py
```

### Comparing `kappadata-1.3.0/setup.cfg` & `kappadata-1.3.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.3.0
+version = 1.3.1
 name = kappadata
 description = pytorch dataset wrappers for in-memory caching
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BenediktAlkin/KappaData
 project_urls = 
 	Source Code = https://github.com/BenediktAlkin/KappaData
```

