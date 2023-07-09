# Comparing `tmp/Kinho-1.0.1.tar.gz` & `tmp/Kinho-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kinho-1.0.1.tar", last modified: Sat Jun 24 10:36:35 2023, max compression
+gzip compressed data, was "Kinho-1.1.0.tar", last modified: Sun Jul  9 22:02:11 2023, max compression
```

## Comparing `Kinho-1.0.1.tar` & `Kinho-1.1.0.tar`

### file list

```diff
@@ -1,54 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.673499 Kinho-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.669499 Kinho-1.0.1/Kinho/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.669499 Kinho-1.0.1/Kinho/brain/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.669499 Kinho-1.0.1/Kinho/brain/decoder/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/decoder/d_float.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/decoder/d_int.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/decoder/d_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.669499 Kinho-1.0.1/Kinho/brain/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/encoder/e_float.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/encoder/e_int.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/encoder/e_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/encoder/e_xor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.673499 Kinho-1.0.1/Kinho/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/dactivation.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/dlayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/dloss.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/dselector.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/updateWeights.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.673499 Kinho-1.0.1/Kinho/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.673499 Kinho-1.0.1/Kinho/lib/GPU/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/lib/GPU/CPU_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/lib/GPU/Function.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/lib/GPU/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/lib/GPU/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/neural.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.673499 Kinho-1.0.1/Kinho/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/transfer/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.669499 Kinho-1.0.1/Kinho.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-24 10:36:35.000000 Kinho-1.0.1/Kinho.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-24 10:36:35.000000 Kinho-1.0.1/Kinho.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:36:35.000000 Kinho-1.0.1/Kinho.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-24 10:36:35.000000 Kinho-1.0.1/Kinho.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 10:36:18.000000 Kinho-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-24 10:36:35.673499 Kinho-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-24 10:36:18.000000 Kinho-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 10:36:35.673499 Kinho-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-24 10:36:19.000000 Kinho-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.673499 Kinho-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-24 10:36:19.000000 Kinho-1.0.1/tests/test_learn_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.730680 Kinho-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.714679 Kinho-1.1.0/Kinho/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.714679 Kinho-1.1.0/Kinho/brain/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/brain/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.714679 Kinho-1.1.0/Kinho/brain/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/brain/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/brain/decoder/d_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/brain/decoder/d_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/brain/decoder/d_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.718679 Kinho-1.1.0/Kinho/brain/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/brain/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/brain/encoder/e_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/brain/encoder/e_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/brain/encoder/e_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/brain/encoder/e_xor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/brain/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.718679 Kinho-1.1.0/Kinho/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.718679 Kinho-1.1.0/Kinho/lib/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/cpu/dot_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/cpu/dot_matrix_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/cpu/mse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/cpu/mse_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/cpu/partial_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/cpu/sigmoid2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/cpu/sigmoid2_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/cpu/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/cpu/softmax_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/cpu/stochastic_gradient_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/cpu/transpose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.722679 Kinho-1.1.0/Kinho/lib/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/dot_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/dot_matrix_derivate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.726679 Kinho-1.1.0/Kinho/lib/gpu/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/average_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/divide_by_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/inverse_matrix_multiplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/list_multiplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/matrix_multiplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/memset_arr_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/memset_arr_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/memset_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/memset_dim_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/mse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/mse_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/partial_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/sigmoid_0_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/sigmoid_0_1_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/softmax_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/sum_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/transpose_dot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.726679 Kinho-1.1.0/Kinho/lib/gpu/kernel/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/utils/ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/kernel/utils/grid_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/mse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/mse_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/partial_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/sigmoid2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/sigmoid2_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/softmax_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/stochastic_gradient_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/lib/gpu/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17543 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/neural.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.726679 Kinho-1.1.0/Kinho/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-09 22:01:51.000000 Kinho-1.1.0/Kinho/transfer/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.714679 Kinho-1.1.0/Kinho.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-09 22:02:11.000000 Kinho-1.1.0/Kinho.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-09 22:02:11.000000 Kinho-1.1.0/Kinho.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:02:11.000000 Kinho-1.1.0/Kinho.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 22:02:11.000000 Kinho-1.1.0/Kinho.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-09 22:01:51.000000 Kinho-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-09 22:02:11.730680 Kinho-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-09 22:01:51.000000 Kinho-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:02:11.730680 Kinho-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-09 22:01:51.000000 Kinho-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.730680 Kinho-1.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:02:11.730680 Kinho-1.1.0/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/lib/test_dot_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/lib/test_dot_matrix_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/lib/test_mse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/lib/test_mse_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/lib/test_partial_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/lib/test_sigmoid2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/lib/test_sigmoid2_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/lib/test_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/lib/test_softmax_derivate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/lib/test_stochastic_gradient_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/lib/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/test_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/test_learn_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/test_mirroring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-09 22:01:51.000000 Kinho-1.1.0/tests/test_send.py
```

### Comparing `Kinho-1.0.1/Kinho/brain/builder.py` & `Kinho-1.1.0/Kinho/brain/builder.py`

 * *Files identical despite different names*

### Comparing `Kinho-1.0.1/Kinho/brain/wrapper.py` & `Kinho-1.1.0/Kinho/brain/wrapper.py`

 * *Files identical despite different names*

### Comparing `Kinho-1.0.1/Kinho.egg-info/PKG-INFO` & `Kinho-1.1.0/Kinho.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kinho
-Version: 1.0.1
+Version: 1.1.0
 Summary: A library to classify images with deep learning.
 Home-page: https://github.com/kinhosz/Neural
 Author: Kinhosz
 Author-email: scruz.josecarlos@gmail.com
 License: MIT
 Keywords: dev,web
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Kinho-1.0.1/LICENSE` & `Kinho-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Kinho-1.0.1/PKG-INFO` & `Kinho-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kinho
-Version: 1.0.1
+Version: 1.1.0
 Summary: A library to classify images with deep learning.
 Home-page: https://github.com/kinhosz/Neural
 Author: Kinhosz
 Author-email: scruz.josecarlos@gmail.com
 License: MIT
 Keywords: dev,web
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Kinho-1.0.1/README.md` & `Kinho-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ## Como instalar
 ```
 pip install Kinho
 ```
 
 ## Métodos:
 ```py
-def __init__(sizes=None, brain_path=None, eta=0.01, gpu=False):
+def __init__(sizes=None, brain_path=None, eta=0.01, gpu=False, mini_batch_size=1):
     pass
 
 def send(input):
     pass
 
 def learn(input, output):
     pass
@@ -29,24 +29,25 @@
 ### Neural (constructor)
 
 #### Parâmetros:
 - `sizes (list of floats)`: lista com o número de neurônios em cada camada da rede, onde o primeiro elemento da lista é a quantidade de neurônios na camada de entrada, o último é a quantidade de neurônios na camada de saída e os elementos intermediários são as quantidades de neurônios nas camadas ocultas.
 - `brain_path(string)`: caminho de um arquivo `x.brain`, de um modelo pré-treinado que você já tenha salvo em seu diretório.
 - `eta (float)`: taxa de aprendizado. Caso não seja definida, assumimos uma taxa padrão de __0.01__.
 - `gpu (bool)`: se __True__, permite que a rede neural automaticamente mude o contexto para utilização da GPU para melhoria de performance.
+- `mini_batch_size(int)`: potência de 2. A rede processará o aprendizado em paralelo com o tamanho do mini-batch passado. Se a opção da gpu não for selecionada, a rede continuará tratando os dados com o mesmo tamanho do mini-batch, mas sem paralelização. O tamanho do mini-batch depende da memória disponível, um tamanho de 128 costuma ser melhor.
 
 Exemplo:
 ```py
 from Kinho import Neural
 
-net_without_imported_model = Neural(sizes=[10, 200, 300, 50, 5], eta=0.1, gpu=True)
+net_without_imported_model = Neural(sizes=[10, 200, 300, 50, 5], eta=0.1, gpu=True, mini_batch_size=16)
 '''
     Uma rede com 3 camadas ocultas (200, 300, 50). Uma camada de input com 10 entradas e,
     uma camada de output com 5 saídas. Taxa de aprendizado 0.1 e todos os pesos sinápticos
-    aleatórios.
+    aleatórios, com um mini-batch de tamanho 16. 
 '''
 
 net_with_imported_model = Neural(brain_path='./pre-trained/mnist_model.brain', eta=0.1, gpu=True)
 '''
     Uma rede com a arquitetura e todos os pesos e biases importados de um modelo previamente treinado dentro do caminho <brain_path>.
 '''
```

### Comparing `Kinho-1.0.1/setup.py` & `Kinho-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `Kinho-1.0.1/tests/test_learn_rate.py` & `Kinho-1.1.0/tests/test_learn_rate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from Kinho import Neural
 from .shared import Shared
 
 import random
 
 shared = Shared()
 
-LEARN_RATE = 0.6
+LEARN_RATE = 0.4
 
 def learn_rate(robot: Neural, epoch: int):
     images = shared.images()
     labels = shared.labels()
     
     zipped_data = [(img, lbl) for img, lbl in zip(images, labels)]
     random.shuffle(zipped_data)
@@ -18,27 +18,31 @@
     TEST_SIZE = int(len(zipped_data) * ALPHA)
     
     test = zipped_data[:TEST_SIZE]
     train = zipped_data[TEST_SIZE:]
     
     for i in range(epoch):
         for input in train:
-            robot.learn(x=input[0], y=shared.densityArr(input[1], 10))
+            robot.learn(input[0], shared.densityArr(input[1], 10))
     
     hits = 0
     for input in test:
-        out = robot.send(l=input[0])
+        out = robot.send(input[0])
         if shared.greaterIdx(out) == input[1]:
             hits += 1
     
     return hits/TEST_SIZE
 
 def test_learn_rate_cpu():
-    robot = Neural(sizes=[28*28, 15, 10], eta=0.1, gpu=False)
+    robot = Neural(sizes=[28*28, 15, 10], eta=1.0, gpu=False)
     
     assert learn_rate(robot=robot, epoch=1) >= LEARN_RATE
 
 def test_learn_rate_gpu():
-    robot = Neural(sizes=[28*28, 15, 10], eta=0.1, gpu=True)
+    robot = Neural(sizes=[28*28, 15, 10], eta=1.0, gpu=True)
     
     assert learn_rate(robot=robot, epoch=1) >= LEARN_RATE
 
+def test_learn_rate_batch16_gpu():
+    robot = Neural(sizes=[28*28, 15, 10], eta=1.0, gpu=True, mini_batch_size=16)
+    
+    assert learn_rate(robot=robot, epoch=10) >= 0.5
```

