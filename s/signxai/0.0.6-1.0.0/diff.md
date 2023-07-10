# Comparing `tmp/signxai-0.0.6.tar.gz` & `tmp/signxai-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nils/PycharmProjects/SIGN-XAI/dist/tmpm4zlf3wm/signxai-0.0.6.tar", last modified: Mon Jul 10 11:54:46 2023, max compression
+gzip compressed data, was "/home/nils/PycharmProjects/SIGN-XAI/dist/tmp9bsgagvd/signxai-1.0.0.tar", last modified: Mon Jul 10 12:00:46 2023, max compression
```

## Comparing `signxai-0.0.6.tar` & `signxai-1.0.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/
--rw-rw-r--   0 nils      (1000) nils      (1000)       38 2023-07-10 11:54:46.000000 signxai-0.0.6/setup.cfg
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/examples/
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 signxai-0.0.6/signxai/examples/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1046 2023-07-10 11:53:28.000000 signxai-0.0.6/signxai/examples/vgg16.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/
--rw-rw-r--   0 nils      (1000) nils      (1000)      253 2023-04-27 08:51:48.000000 signxai-0.0.6/signxai/methods/signed.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/tools/
--rw-rw-r--   0 nils      (1000) nils      (1000)      225 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tools/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    19540 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tools/pattern.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    18118 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tools/perturbate.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    19365 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/layers.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/applications/
--rw-rw-r--   0 nils      (1000) nils      (1000)    10473 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/applications/imagenet.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/applications/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4256 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/applications/mnist.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/tools/
--rw-rw-r--   0 nils      (1000) nils      (1000)     3969 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/tools/test_perturbate.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    12358 2022-05-24 09:53:27.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/tools/test_pattern.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/tools/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/
--rw-rw-r--   0 nils      (1000) nils      (1000)    10210 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3790 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1303 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_misc.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3948 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3025 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4878 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_base.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     7771 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1847 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1511 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_init.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/utils/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/utils/keras/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1759 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/utils/keras/test_graph.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/utils/keras/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)      967 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/utils/test_visualizations.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/utils/tests/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1189 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/utils/tests/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/tests/utils/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/
--rw-rw-r--   0 nils      (1000) nils      (1000)     8539 2023-07-10 11:08:26.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/pattern_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1948 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/misc.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    14700 2023-07-10 11:08:26.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/gradient_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     7094 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/deeptaylor.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    13638 2023-07-10 11:08:26.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/wrapper.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    26365 2022-05-11 10:33:05.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/reverse_map.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    20907 2022-04-06 15:20:24.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/base.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4395 2022-07-20 07:31:35.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/canonization/
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/canonization/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    15327 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/deeplift.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/relevance_based/
--rw-rw-r--   0 nils      (1000) nils      (1000)     3842 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/relevance_based/utils.py
--rw-rw-r--   0 nils      (1000) nils      (1000)       65 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/relevance_based/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    24163 2023-07-10 11:08:25.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    52929 2023-07-10 09:21:05.000000 signxai-0.0.6/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py
--rw-rw-r--   0 nils      (1000) nils      (1000)      216 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/backend/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1234 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/backend/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/backend/tensorflow.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/backend/torch.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/keras/
--rw-rw-r--   0 nils      (1000) nils      (1000)     5921 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/keras/backend.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    14517 2022-04-06 15:20:24.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/keras/checks.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2318 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/keras/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    43869 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/keras/graph.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4925 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/visualizations.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/tests/
--rw-rw-r--   0 nils      (1000) nils      (1000)     2818 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/tests/dryrun.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/tests/cases/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1313 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/tests/cases/mlp.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1634 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/tests/cases/special.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1383 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/tests/cases/helper.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3322 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/tests/cases/cnn.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2457 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/tests/cases/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1592 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/tests/cases/trivia.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/tests/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     5791 2022-02-16 10:22:41.000000 signxai-0.0.6/signxai/methods/innvestigate/utils/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 signxai-0.0.6/signxai/methods/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2603 2022-09-16 14:59:58.000000 signxai-0.0.6/signxai/methods/grad_cam.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    25764 2023-07-10 11:08:25.000000 signxai-0.0.6/signxai/methods/wrappers.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1499 2022-04-26 09:45:35.000000 signxai-0.0.6/signxai/methods/guided_backprop.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai/utils/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1898 2023-07-10 11:52:53.000000 signxai-0.0.6/signxai/utils/utils.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2023-07-10 10:28:07.000000 signxai-0.0.6/signxai/utils/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2322 2023-07-10 11:54:17.000000 signxai-0.0.6/README.md
--rw-rw-r--   0 nils      (1000) nils      (1000)       33 2023-07-10 11:40:05.000000 signxai-0.0.6/MANIFEST.in
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai.egg-info/
--rw-rw-r--   0 nils      (1000) nils      (1000)       53 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai.egg-info/requires.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)        1 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai.egg-info/dependency_links.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)     3706 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai.egg-info/SOURCES.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)        8 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai.egg-info/top_level.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)     3108 2023-07-10 11:54:46.000000 signxai-0.0.6/signxai.egg-info/PKG-INFO
--rw-rw-r--   0 nils      (1000) nils      (1000)     2054 2023-07-10 11:53:53.000000 signxai-0.0.6/setup.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3108 2023-07-10 11:54:46.000000 signxai-0.0.6/PKG-INFO
--rw-rw-r--   0 nils      (1000) nils      (1000)     2182 2023-07-10 08:27:19.000000 signxai-0.0.6/LICENSE
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/
+-rw-rw-r--   0 nils      (1000) nils      (1000)       38 2023-07-10 12:00:46.000000 signxai-1.0.0/setup.cfg
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/examples/
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 signxai-1.0.0/signxai/examples/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1046 2023-07-10 11:53:28.000000 signxai-1.0.0/signxai/examples/vgg16.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/
+-rw-rw-r--   0 nils      (1000) nils      (1000)      253 2023-04-27 08:51:48.000000 signxai-1.0.0/signxai/methods/signed.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/tools/
+-rw-rw-r--   0 nils      (1000) nils      (1000)      225 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tools/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    19540 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tools/pattern.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    18118 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tools/perturbate.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    19365 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/layers.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/applications/
+-rw-rw-r--   0 nils      (1000) nils      (1000)    10473 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/applications/imagenet.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/applications/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4256 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/applications/mnist.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/tools/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3969 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/tools/test_perturbate.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    12358 2022-05-24 09:53:27.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/tools/test_pattern.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/tools/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/
+-rw-rw-r--   0 nils      (1000) nils      (1000)    10210 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3790 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1303 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_misc.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3948 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3025 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4878 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_base.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     7771 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1847 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1511 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_init.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/utils/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/utils/keras/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1759 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/utils/keras/test_graph.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/utils/keras/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)      967 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/utils/test_visualizations.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/utils/tests/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1189 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/utils/tests/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/tests/utils/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     8539 2023-07-10 11:08:26.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/pattern_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1948 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/misc.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    14700 2023-07-10 11:08:26.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/gradient_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     7094 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/deeptaylor.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    13638 2023-07-10 11:08:26.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/wrapper.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    26365 2022-05-11 10:33:05.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/reverse_map.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    20907 2022-04-06 15:20:24.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/base.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4395 2022-07-20 07:31:35.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/canonization/
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/canonization/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    15327 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/deeplift.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/relevance_based/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3842 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/relevance_based/utils.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)       65 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/relevance_based/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    24163 2023-07-10 11:08:25.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    52929 2023-07-10 09:21:05.000000 signxai-1.0.0/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)      216 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/backend/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1234 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/backend/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/backend/tensorflow.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/backend/torch.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/keras/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     5921 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/keras/backend.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    14517 2022-04-06 15:20:24.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/keras/checks.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2318 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/keras/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    43869 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/keras/graph.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4925 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/visualizations.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/tests/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2818 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/tests/dryrun.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/tests/cases/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1313 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/tests/cases/mlp.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1634 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/tests/cases/special.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1383 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/tests/cases/helper.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3322 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/tests/cases/cnn.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2457 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/tests/cases/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1592 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/tests/cases/trivia.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/tests/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     5791 2022-02-16 10:22:41.000000 signxai-1.0.0/signxai/methods/innvestigate/utils/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 signxai-1.0.0/signxai/methods/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2603 2022-09-16 14:59:58.000000 signxai-1.0.0/signxai/methods/grad_cam.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    25764 2023-07-10 11:08:25.000000 signxai-1.0.0/signxai/methods/wrappers.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1499 2022-04-26 09:45:35.000000 signxai-1.0.0/signxai/methods/guided_backprop.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai/utils/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1898 2023-07-10 11:52:53.000000 signxai-1.0.0/signxai/utils/utils.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2023-07-10 10:28:07.000000 signxai-1.0.0/signxai/utils/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2403 2023-07-10 11:58:43.000000 signxai-1.0.0/README.md
+-rw-rw-r--   0 nils      (1000) nils      (1000)       33 2023-07-10 11:40:05.000000 signxai-1.0.0/MANIFEST.in
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai.egg-info/
+-rw-rw-r--   0 nils      (1000) nils      (1000)       53 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai.egg-info/requires.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)        1 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai.egg-info/dependency_links.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3706 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai.egg-info/SOURCES.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)        8 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai.egg-info/top_level.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3189 2023-07-10 12:00:46.000000 signxai-1.0.0/signxai.egg-info/PKG-INFO
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2054 2023-07-10 11:56:14.000000 signxai-1.0.0/setup.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3189 2023-07-10 12:00:46.000000 signxai-1.0.0/PKG-INFO
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2182 2023-07-10 08:27:19.000000 signxai-1.0.0/LICENSE
```

### Comparing `signxai-0.0.6/signxai/examples/vgg16.py` & `signxai-1.0.0/signxai/examples/vgg16.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tools/pattern.py` & `signxai-1.0.0/signxai/methods/innvestigate/tools/pattern.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tools/perturbate.py` & `signxai-1.0.0/signxai/methods/innvestigate/tools/perturbate.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/layers.py` & `signxai-1.0.0/signxai/methods/innvestigate/layers.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/applications/imagenet.py` & `signxai-1.0.0/signxai/methods/innvestigate/applications/imagenet.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/applications/mnist.py` & `signxai-1.0.0/signxai/methods/innvestigate/applications/mnist.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/tools/test_perturbate.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/tools/test_perturbate.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/tools/test_pattern.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/tools/test_pattern.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_misc.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_misc.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_base.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_base.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/analyzer/test_init.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/analyzer/test_init.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/utils/keras/test_graph.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/utils/keras/test_graph.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/utils/test_visualizations.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/utils/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py` & `signxai-1.0.0/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/analyzer/pattern_based.py` & `signxai-1.0.0/signxai/methods/innvestigate/analyzer/pattern_based.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/analyzer/misc.py` & `signxai-1.0.0/signxai/methods/innvestigate/analyzer/misc.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/analyzer/gradient_based.py` & `signxai-1.0.0/signxai/methods/innvestigate/analyzer/gradient_based.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/analyzer/deeptaylor.py` & `signxai-1.0.0/signxai/methods/innvestigate/analyzer/deeptaylor.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/analyzer/wrapper.py` & `signxai-1.0.0/signxai/methods/innvestigate/analyzer/wrapper.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/analyzer/reverse_map.py` & `signxai-1.0.0/signxai/methods/innvestigate/analyzer/reverse_map.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/analyzer/base.py` & `signxai-1.0.0/signxai/methods/innvestigate/analyzer/base.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/analyzer/__init__.py` & `signxai-1.0.0/signxai/methods/innvestigate/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/analyzer/deeplift.py` & `signxai-1.0.0/signxai/methods/innvestigate/analyzer/deeplift.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/analyzer/relevance_based/utils.py` & `signxai-1.0.0/signxai/methods/innvestigate/analyzer/relevance_based/utils.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py` & `signxai-1.0.0/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py` & `signxai-1.0.0/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/backend/__init__.py` & `signxai-1.0.0/signxai/methods/innvestigate/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/utils/keras/backend.py` & `signxai-1.0.0/signxai/methods/innvestigate/utils/keras/backend.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/utils/keras/checks.py` & `signxai-1.0.0/signxai/methods/innvestigate/utils/keras/checks.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/utils/keras/__init__.py` & `signxai-1.0.0/signxai/methods/innvestigate/utils/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/utils/keras/graph.py` & `signxai-1.0.0/signxai/methods/innvestigate/utils/keras/graph.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/utils/visualizations.py` & `signxai-1.0.0/signxai/methods/innvestigate/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/utils/tests/dryrun.py` & `signxai-1.0.0/signxai/methods/innvestigate/utils/tests/dryrun.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/utils/tests/cases/mlp.py` & `signxai-1.0.0/signxai/methods/innvestigate/utils/tests/cases/mlp.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/utils/tests/cases/special.py` & `signxai-1.0.0/signxai/methods/innvestigate/utils/tests/cases/special.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/utils/tests/cases/helper.py` & `signxai-1.0.0/signxai/methods/innvestigate/utils/tests/cases/helper.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/utils/tests/cases/cnn.py` & `signxai-1.0.0/signxai/methods/innvestigate/utils/tests/cases/cnn.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/utils/tests/cases/__init__.py` & `signxai-1.0.0/signxai/methods/innvestigate/utils/tests/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/utils/tests/cases/trivia.py` & `signxai-1.0.0/signxai/methods/innvestigate/utils/tests/cases/trivia.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/innvestigate/utils/__init__.py` & `signxai-1.0.0/signxai/methods/innvestigate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/grad_cam.py` & `signxai-1.0.0/signxai/methods/grad_cam.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/wrappers.py` & `signxai-1.0.0/signxai/methods/wrappers.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/methods/guided_backprop.py` & `signxai-1.0.0/signxai/methods/guided_backprop.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai/utils/utils.py` & `signxai-1.0.0/signxai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/README.md` & `signxai-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -63,10 +63,12 @@
 axs[0].imshow(img)
 axs[1].matshow(H1, cmap='seismic', clim=(-1, 1))
 axs[2].matshow(H2, cmap='seismic', clim=(-1, 1))
 
 plt.show()
 ```
 
+(Image credit for example used in this code: Greg Gjerdingen from Willmar, USA)
+
 ## Experiments
 
 To reproduce the experiments from our paper, please find a detailed description on https://github.com/nilsgumpfer/SIGN.
```

### Comparing `signxai-0.0.6/signxai.egg-info/SOURCES.txt` & `signxai-1.0.0/signxai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `signxai-0.0.6/signxai.egg-info/PKG-INFO` & `signxai-1.0.0/signxai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signxai
-Version: 0.0.6
+Version: 1.0.0
 Summary: SIGNed explanations: Unveiling relevant features by reducing bias
 Home-page: https://github.com/nilsgumpfer/SIGN-XAI
 Author: Nils Gumpfer
 Author-email: nils.gumpfer@kite.thm.de
 Maintainer: Nils Gumpfer
 Maintainer-email: nils.gumpfer@kite.thm.de
 License: BSD 2-Clause License
@@ -85,12 +85,14 @@
 axs[0].imshow(img)
 axs[1].matshow(H1, cmap='seismic', clim=(-1, 1))
 axs[2].matshow(H2, cmap='seismic', clim=(-1, 1))
 
 plt.show()
 ```
 
+(Image credit for example used in this code: Greg Gjerdingen from Willmar, USA)
+
 ## Experiments
 
 To reproduce the experiments from our paper, please find a detailed description on https://github.com/nilsgumpfer/SIGN.
```

### Comparing `signxai-0.0.6/setup.py` & `signxai-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='signxai',
-    version='0.0.6',
+    version='1.0.0',
     packages=['signxai.methods', 'signxai.methods.innvestigate', 'signxai.methods.innvestigate.tests', 'signxai.methods.innvestigate.tests.tools',
               'signxai.methods.innvestigate.tests.utils', 'signxai.methods.innvestigate.tests.utils.keras',
               'signxai.methods.innvestigate.tests.utils.tests', 'signxai.methods.innvestigate.tests.analyzer',
               'signxai.methods.innvestigate.tools', 'signxai.methods.innvestigate.utils', 'signxai.methods.innvestigate.utils.keras',
               'signxai.methods.innvestigate.utils.tests', 'signxai.methods.innvestigate.utils.tests.cases',
               'signxai.methods.innvestigate.backend', 'signxai.methods.innvestigate.analyzer',
               'signxai.methods.innvestigate.analyzer.canonization', 'signxai.methods.innvestigate.analyzer.relevance_based',
```

### Comparing `signxai-0.0.6/PKG-INFO` & `signxai-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signxai
-Version: 0.0.6
+Version: 1.0.0
 Summary: SIGNed explanations: Unveiling relevant features by reducing bias
 Home-page: https://github.com/nilsgumpfer/SIGN-XAI
 Author: Nils Gumpfer
 Author-email: nils.gumpfer@kite.thm.de
 Maintainer: Nils Gumpfer
 Maintainer-email: nils.gumpfer@kite.thm.de
 License: BSD 2-Clause License
@@ -85,12 +85,14 @@
 axs[0].imshow(img)
 axs[1].matshow(H1, cmap='seismic', clim=(-1, 1))
 axs[2].matshow(H2, cmap='seismic', clim=(-1, 1))
 
 plt.show()
 ```
 
+(Image credit for example used in this code: Greg Gjerdingen from Willmar, USA)
+
 ## Experiments
 
 To reproduce the experiments from our paper, please find a detailed description on https://github.com/nilsgumpfer/SIGN.
```

### Comparing `signxai-0.0.6/LICENSE` & `signxai-1.0.0/LICENSE`

 * *Files identical despite different names*

