# Comparing `tmp/signxai-0.0.3.tar.gz` & `tmp/signxai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nils/PycharmProjects/SIGN-XAI/dist/tmpo4uxjohw/signxai-0.0.3.tar", last modified: Mon Jul 10 11:29:36 2023, max compression
+gzip compressed data, was "/home/nils/PycharmProjects/SIGN-XAI/dist/tmpgvouzfpy/signxai-0.0.4.tar", last modified: Mon Jul 10 11:40:11 2023, max compression
```

## Comparing `signxai-0.0.3.tar` & `signxai-0.0.4.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/
--rw-rw-r--   0 nils      (1000) nils      (1000)       38 2023-07-10 11:29:36.000000 signxai-0.0.3/setup.cfg
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/examples/
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 signxai-0.0.3/signxai/examples/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1001 2023-07-10 11:24:24.000000 signxai-0.0.3/signxai/examples/vgg16.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/data/
--rw-rw-r--   0 nils      (1000) nils      (1000)  4924665 2022-07-11 11:25:40.000000 signxai-0.0.3/signxai/data/7867854122_b26957e9e3_o.jpg
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/
--rw-rw-r--   0 nils      (1000) nils      (1000)      253 2023-04-27 08:51:48.000000 signxai-0.0.3/signxai/methods/signed.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/tools/
--rw-rw-r--   0 nils      (1000) nils      (1000)      225 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tools/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    19540 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tools/pattern.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    18118 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tools/perturbate.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    19365 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/layers.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/applications/
--rw-rw-r--   0 nils      (1000) nils      (1000)    10473 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/applications/imagenet.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/applications/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4256 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/applications/mnist.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/tools/
--rw-rw-r--   0 nils      (1000) nils      (1000)     3969 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/tools/test_perturbate.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    12358 2022-05-24 09:53:27.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/tools/test_pattern.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/tools/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/
--rw-rw-r--   0 nils      (1000) nils      (1000)    10210 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3790 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1303 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_misc.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3948 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3025 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4878 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_base.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     7771 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1847 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1511 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_init.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/utils/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/utils/keras/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1759 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/utils/keras/test_graph.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/utils/keras/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)      967 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/utils/test_visualizations.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/utils/tests/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1189 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/utils/tests/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/tests/utils/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/
--rw-rw-r--   0 nils      (1000) nils      (1000)     8539 2023-07-10 11:08:26.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/pattern_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1948 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/misc.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    14700 2023-07-10 11:08:26.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/gradient_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     7094 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/deeptaylor.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    13638 2023-07-10 11:08:26.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/wrapper.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    26365 2022-05-11 10:33:05.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/reverse_map.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    20907 2022-04-06 15:20:24.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/base.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4395 2022-07-20 07:31:35.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/canonization/
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/canonization/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    15327 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/deeplift.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/relevance_based/
--rw-rw-r--   0 nils      (1000) nils      (1000)     3842 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/relevance_based/utils.py
--rw-rw-r--   0 nils      (1000) nils      (1000)       65 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/relevance_based/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    24163 2023-07-10 11:08:25.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    52929 2023-07-10 09:21:05.000000 signxai-0.0.3/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py
--rw-rw-r--   0 nils      (1000) nils      (1000)      216 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/backend/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1234 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/backend/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/backend/tensorflow.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/backend/torch.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/keras/
--rw-rw-r--   0 nils      (1000) nils      (1000)     5921 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/keras/backend.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    14517 2022-04-06 15:20:24.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/keras/checks.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2318 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/keras/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    43869 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/keras/graph.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4925 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/visualizations.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/tests/
--rw-rw-r--   0 nils      (1000) nils      (1000)     2818 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/tests/dryrun.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/tests/cases/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1313 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/tests/cases/mlp.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1634 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/tests/cases/special.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1383 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/tests/cases/helper.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3322 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/tests/cases/cnn.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2457 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/tests/cases/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1592 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/tests/cases/trivia.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/tests/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     5791 2022-02-16 10:22:41.000000 signxai-0.0.3/signxai/methods/innvestigate/utils/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 signxai-0.0.3/signxai/methods/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2603 2022-09-16 14:59:58.000000 signxai-0.0.3/signxai/methods/grad_cam.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    25764 2023-07-10 11:08:25.000000 signxai-0.0.3/signxai/methods/wrappers.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1499 2022-04-26 09:45:35.000000 signxai-0.0.3/signxai/methods/guided_backprop.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai/utils/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1754 2023-07-10 11:16:58.000000 signxai-0.0.3/signxai/utils/utils.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2023-07-10 10:28:07.000000 signxai-0.0.3/signxai/utils/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2279 2023-07-10 11:26:40.000000 signxai-0.0.3/README.md
--rw-rw-r--   0 nils      (1000) nils      (1000)       82 2023-07-10 11:08:26.000000 signxai-0.0.3/MANIFEST.in
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai.egg-info/
--rw-rw-r--   0 nils      (1000) nils      (1000)       36 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai.egg-info/requires.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)        1 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai.egg-info/dependency_links.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)     3747 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai.egg-info/SOURCES.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)        8 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai.egg-info/top_level.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)     3065 2023-07-10 11:29:36.000000 signxai-0.0.3/signxai.egg-info/PKG-INFO
--rw-rw-r--   0 nils      (1000) nils      (1000)     2034 2023-07-10 11:29:14.000000 signxai-0.0.3/setup.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3065 2023-07-10 11:29:36.000000 signxai-0.0.3/PKG-INFO
--rw-rw-r--   0 nils      (1000) nils      (1000)     2182 2023-07-10 08:27:19.000000 signxai-0.0.3/LICENSE
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/
+-rw-rw-r--   0 nils      (1000) nils      (1000)       38 2023-07-10 11:40:11.000000 signxai-0.0.4/setup.cfg
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/examples/
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 signxai-0.0.4/signxai/examples/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1001 2023-07-10 11:24:24.000000 signxai-0.0.4/signxai/examples/vgg16.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/data/
+-rw-rw-r--   0 nils      (1000) nils      (1000)  4924665 2022-07-11 11:25:40.000000 signxai-0.0.4/signxai/data/7867854122_b26957e9e3_o.jpg
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/
+-rw-rw-r--   0 nils      (1000) nils      (1000)      253 2023-04-27 08:51:48.000000 signxai-0.0.4/signxai/methods/signed.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/tools/
+-rw-rw-r--   0 nils      (1000) nils      (1000)      225 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tools/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    19540 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tools/pattern.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    18118 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tools/perturbate.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    19365 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/layers.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/applications/
+-rw-rw-r--   0 nils      (1000) nils      (1000)    10473 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/applications/imagenet.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/applications/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4256 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/applications/mnist.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/tools/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3969 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/tools/test_perturbate.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    12358 2022-05-24 09:53:27.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/tools/test_pattern.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/tools/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/
+-rw-rw-r--   0 nils      (1000) nils      (1000)    10210 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3790 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1303 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_misc.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3948 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3025 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4878 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_base.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     7771 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1847 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1511 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_init.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/utils/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/utils/keras/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1759 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/utils/keras/test_graph.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/utils/keras/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)      967 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/utils/test_visualizations.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/utils/tests/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1189 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/utils/tests/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/tests/utils/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     8539 2023-07-10 11:08:26.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/pattern_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1948 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/misc.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    14700 2023-07-10 11:08:26.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/gradient_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     7094 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/deeptaylor.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    13638 2023-07-10 11:08:26.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/wrapper.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    26365 2022-05-11 10:33:05.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/reverse_map.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    20907 2022-04-06 15:20:24.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/base.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4395 2022-07-20 07:31:35.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/canonization/
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/canonization/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    15327 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/deeplift.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/relevance_based/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3842 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/relevance_based/utils.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)       65 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/relevance_based/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    24163 2023-07-10 11:08:25.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    52929 2023-07-10 09:21:05.000000 signxai-0.0.4/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)      216 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/backend/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1234 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/backend/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/backend/tensorflow.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/backend/torch.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/keras/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     5921 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/keras/backend.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    14517 2022-04-06 15:20:24.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/keras/checks.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2318 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/keras/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    43869 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/keras/graph.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4925 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/visualizations.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/tests/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2818 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/tests/dryrun.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/tests/cases/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1313 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/tests/cases/mlp.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1634 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/tests/cases/special.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1383 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/tests/cases/helper.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3322 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/tests/cases/cnn.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2457 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/tests/cases/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1592 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/tests/cases/trivia.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/tests/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     5791 2022-02-16 10:22:41.000000 signxai-0.0.4/signxai/methods/innvestigate/utils/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 signxai-0.0.4/signxai/methods/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2603 2022-09-16 14:59:58.000000 signxai-0.0.4/signxai/methods/grad_cam.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    25764 2023-07-10 11:08:25.000000 signxai-0.0.4/signxai/methods/wrappers.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1499 2022-04-26 09:45:35.000000 signxai-0.0.4/signxai/methods/guided_backprop.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai/utils/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1754 2023-07-10 11:16:58.000000 signxai-0.0.4/signxai/utils/utils.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2023-07-10 10:28:07.000000 signxai-0.0.4/signxai/utils/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2278 2023-07-10 11:30:55.000000 signxai-0.0.4/README.md
+-rw-rw-r--   0 nils      (1000) nils      (1000)       33 2023-07-10 11:40:05.000000 signxai-0.0.4/MANIFEST.in
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai.egg-info/
+-rw-rw-r--   0 nils      (1000) nils      (1000)       36 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai.egg-info/requires.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)        1 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai.egg-info/dependency_links.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3747 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai.egg-info/SOURCES.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)        8 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai.egg-info/top_level.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3064 2023-07-10 11:40:11.000000 signxai-0.0.4/signxai.egg-info/PKG-INFO
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2107 2023-07-10 11:40:05.000000 signxai-0.0.4/setup.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3064 2023-07-10 11:40:11.000000 signxai-0.0.4/PKG-INFO
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2182 2023-07-10 08:27:19.000000 signxai-0.0.4/LICENSE
```

### Comparing `signxai-0.0.3/signxai/examples/vgg16.py` & `signxai-0.0.4/signxai/examples/vgg16.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/data/7867854122_b26957e9e3_o.jpg` & `signxai-0.0.4/signxai/data/7867854122_b26957e9e3_o.jpg`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tools/pattern.py` & `signxai-0.0.4/signxai/methods/innvestigate/tools/pattern.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tools/perturbate.py` & `signxai-0.0.4/signxai/methods/innvestigate/tools/perturbate.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/layers.py` & `signxai-0.0.4/signxai/methods/innvestigate/layers.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/applications/imagenet.py` & `signxai-0.0.4/signxai/methods/innvestigate/applications/imagenet.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/applications/mnist.py` & `signxai-0.0.4/signxai/methods/innvestigate/applications/mnist.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/tools/test_perturbate.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/tools/test_perturbate.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/tools/test_pattern.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/tools/test_pattern.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_misc.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_misc.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_base.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_base.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/analyzer/test_init.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/analyzer/test_init.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/utils/keras/test_graph.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/utils/keras/test_graph.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/utils/test_visualizations.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/utils/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py` & `signxai-0.0.4/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/analyzer/pattern_based.py` & `signxai-0.0.4/signxai/methods/innvestigate/analyzer/pattern_based.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/analyzer/misc.py` & `signxai-0.0.4/signxai/methods/innvestigate/analyzer/misc.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/analyzer/gradient_based.py` & `signxai-0.0.4/signxai/methods/innvestigate/analyzer/gradient_based.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/analyzer/deeptaylor.py` & `signxai-0.0.4/signxai/methods/innvestigate/analyzer/deeptaylor.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/analyzer/wrapper.py` & `signxai-0.0.4/signxai/methods/innvestigate/analyzer/wrapper.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/analyzer/reverse_map.py` & `signxai-0.0.4/signxai/methods/innvestigate/analyzer/reverse_map.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/analyzer/base.py` & `signxai-0.0.4/signxai/methods/innvestigate/analyzer/base.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/analyzer/__init__.py` & `signxai-0.0.4/signxai/methods/innvestigate/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/analyzer/deeplift.py` & `signxai-0.0.4/signxai/methods/innvestigate/analyzer/deeplift.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/analyzer/relevance_based/utils.py` & `signxai-0.0.4/signxai/methods/innvestigate/analyzer/relevance_based/utils.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py` & `signxai-0.0.4/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py` & `signxai-0.0.4/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/backend/__init__.py` & `signxai-0.0.4/signxai/methods/innvestigate/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/utils/keras/backend.py` & `signxai-0.0.4/signxai/methods/innvestigate/utils/keras/backend.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/utils/keras/checks.py` & `signxai-0.0.4/signxai/methods/innvestigate/utils/keras/checks.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/utils/keras/__init__.py` & `signxai-0.0.4/signxai/methods/innvestigate/utils/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/utils/keras/graph.py` & `signxai-0.0.4/signxai/methods/innvestigate/utils/keras/graph.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/utils/visualizations.py` & `signxai-0.0.4/signxai/methods/innvestigate/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/utils/tests/dryrun.py` & `signxai-0.0.4/signxai/methods/innvestigate/utils/tests/dryrun.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/utils/tests/cases/mlp.py` & `signxai-0.0.4/signxai/methods/innvestigate/utils/tests/cases/mlp.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/utils/tests/cases/special.py` & `signxai-0.0.4/signxai/methods/innvestigate/utils/tests/cases/special.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/utils/tests/cases/helper.py` & `signxai-0.0.4/signxai/methods/innvestigate/utils/tests/cases/helper.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/utils/tests/cases/cnn.py` & `signxai-0.0.4/signxai/methods/innvestigate/utils/tests/cases/cnn.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/utils/tests/cases/__init__.py` & `signxai-0.0.4/signxai/methods/innvestigate/utils/tests/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/utils/tests/cases/trivia.py` & `signxai-0.0.4/signxai/methods/innvestigate/utils/tests/cases/trivia.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/innvestigate/utils/__init__.py` & `signxai-0.0.4/signxai/methods/innvestigate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/grad_cam.py` & `signxai-0.0.4/signxai/methods/grad_cam.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/wrappers.py` & `signxai-0.0.4/signxai/methods/wrappers.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/methods/guided_backprop.py` & `signxai-0.0.4/signxai/methods/guided_backprop.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai/utils/utils.py` & `signxai-0.0.4/signxai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/README.md` & `signxai-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 <img src="https://ars.els-cdn.com/content/image/1-s2.0-S1566253523001999-ga1_lrg.jpg" title="Graphical Abstract" width="900px"/>
 
 ## Setup
 
 To install the package in your environment, run:
 
 ```shell
- pip3 install SIGN-XAI
+ pip3 install signxai
 ```
 
 
 ## Usage
 
 The below example illustrates the usage of the ```signxai``` package in combination with a VGG16 model trained on imagenet:
```

### Comparing `signxai-0.0.3/signxai.egg-info/SOURCES.txt` & `signxai-0.0.4/signxai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `signxai-0.0.3/signxai.egg-info/PKG-INFO` & `signxai-0.0.4/signxai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signxai
-Version: 0.0.3
+Version: 0.0.4
 Summary: SIGNed explanations: Unveiling relevant features by reducing bias
 Home-page: https://github.com/nilsgumpfer/SIGN-XAI
 Author: Nils Gumpfer
 Author-email: nils.gumpfer@kite.thm.de
 Maintainer: Nils Gumpfer
 Maintainer-email: nils.gumpfer@kite.thm.de
 License: BSD 2-Clause License
@@ -42,15 +42,15 @@
 <img src="https://ars.els-cdn.com/content/image/1-s2.0-S1566253523001999-ga1_lrg.jpg" title="Graphical Abstract" width="900px"/>
 
 ## Setup
 
 To install the package in your environment, run:
 
 ```shell
- pip3 install SIGN-XAI
+ pip3 install signxai
 ```
 
 
 ## Usage
 
 The below example illustrates the usage of the ```signxai``` package in combination with a VGG16 model trained on imagenet:
```

### Comparing `signxai-0.0.3/setup.py` & `signxai-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='signxai',
-    version='0.0.3',
+    version='0.0.4',
     packages=['signxai.methods', 'signxai.methods.innvestigate', 'signxai.methods.innvestigate.tests', 'signxai.methods.innvestigate.tests.tools',
               'signxai.methods.innvestigate.tests.utils', 'signxai.methods.innvestigate.tests.utils.keras',
               'signxai.methods.innvestigate.tests.utils.tests', 'signxai.methods.innvestigate.tests.analyzer',
               'signxai.methods.innvestigate.tools', 'signxai.methods.innvestigate.utils', 'signxai.methods.innvestigate.utils.keras',
               'signxai.methods.innvestigate.utils.tests', 'signxai.methods.innvestigate.utils.tests.cases',
               'signxai.methods.innvestigate.backend', 'signxai.methods.innvestigate.analyzer',
               'signxai.methods.innvestigate.analyzer.canonization', 'signxai.methods.innvestigate.analyzer.relevance_based',
               'signxai.methods.innvestigate.applications', 'signxai.examples', 'signxai.utils'],
+    data_files=[('data', ['signxai/data/7867854122_b26957e9e3_o.jpg'])],
     url='https://github.com/nilsgumpfer/SIGN-XAI',
     license='BSD 2-Clause License',
     author='Nils Gumpfer',
     author_email='nils.gumpfer@kite.thm.de',
     maintainer='Nils Gumpfer',
     maintainer_email='nils.gumpfer@kite.thm.de',
     description='SIGNed explanations: Unveiling relevant features by reducing bias',
```

### Comparing `signxai-0.0.3/PKG-INFO` & `signxai-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signxai
-Version: 0.0.3
+Version: 0.0.4
 Summary: SIGNed explanations: Unveiling relevant features by reducing bias
 Home-page: https://github.com/nilsgumpfer/SIGN-XAI
 Author: Nils Gumpfer
 Author-email: nils.gumpfer@kite.thm.de
 Maintainer: Nils Gumpfer
 Maintainer-email: nils.gumpfer@kite.thm.de
 License: BSD 2-Clause License
@@ -42,15 +42,15 @@
 <img src="https://ars.els-cdn.com/content/image/1-s2.0-S1566253523001999-ga1_lrg.jpg" title="Graphical Abstract" width="900px"/>
 
 ## Setup
 
 To install the package in your environment, run:
 
 ```shell
- pip3 install SIGN-XAI
+ pip3 install signxai
 ```
 
 
 ## Usage
 
 The below example illustrates the usage of the ```signxai``` package in combination with a VGG16 model trained on imagenet:
```

### Comparing `signxai-0.0.3/LICENSE` & `signxai-0.0.4/LICENSE`

 * *Files identical despite different names*

