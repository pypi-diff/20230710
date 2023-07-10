# Comparing `tmp/SIGN-XAI-1.0.0.tar.gz` & `tmp/SIGN-XAI-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nils/PycharmProjects/SIGN-XAI/dist/tmpdtj8yifa/SIGN-XAI-1.0.0.tar", last modified: Mon Jul 10 10:32:06 2023, max compression
+gzip compressed data, was "/home/nils/PycharmProjects/SIGN-XAI/dist/tmperv66kuu/SIGN-XAI-1.0.1.tar", last modified: Mon Jul 10 10:45:02 2023, max compression
```

## Comparing `SIGN-XAI-1.0.0.tar` & `SIGN-XAI-1.0.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/
--rw-rw-r--   0 nils      (1000) nils      (1000)       38 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/setup.cfg
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/examples/
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 SIGN-XAI-1.0.0/examples/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)      824 2023-07-10 10:29:14.000000 SIGN-XAI-1.0.0/examples/vgg16.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1120 2023-07-10 09:52:50.000000 SIGN-XAI-1.0.0/README.md
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/SIGN_XAI.egg-info/
--rw-rw-r--   0 nils      (1000) nils      (1000)       36 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/SIGN_XAI.egg-info/requires.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)        1 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/SIGN_XAI.egg-info/dependency_links.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)     3200 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/SIGN_XAI.egg-info/SOURCES.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)       23 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/SIGN_XAI.egg-info/top_level.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)      767 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/SIGN_XAI.egg-info/PKG-INFO
--rw-rw-r--   0 nils      (1000) nils      (1000)       74 2023-07-10 10:29:14.000000 SIGN-XAI-1.0.0/MANIFEST.in
--rw-rw-r--   0 nils      (1000) nils      (1000)     1679 2023-07-10 10:30:15.000000 SIGN-XAI-1.0.0/setup.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/data/
--rw-rw-r--   0 nils      (1000) nils      (1000)  4924665 2022-07-11 11:25:40.000000 SIGN-XAI-1.0.0/data/7867854122_b26957e9e3_o.jpg
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/
--rw-rw-r--   0 nils      (1000) nils      (1000)      253 2023-04-27 08:51:48.000000 SIGN-XAI-1.0.0/methods/signed.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/tools/
--rw-rw-r--   0 nils      (1000) nils      (1000)      225 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tools/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    19540 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tools/pattern.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    18118 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tools/perturbate.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    19365 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/layers.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/applications/
--rw-rw-r--   0 nils      (1000) nils      (1000)    10473 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/applications/imagenet.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/applications/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4256 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/applications/mnist.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/tools/
--rw-rw-r--   0 nils      (1000) nils      (1000)     3969 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/tools/test_perturbate.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    12358 2022-05-24 09:53:27.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/tools/test_pattern.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/tools/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/
--rw-rw-r--   0 nils      (1000) nils      (1000)    10210 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_relevance_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3790 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_wrapper.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1303 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_misc.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3948 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_deeplift.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3025 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_pattern_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4878 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_base.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     7771 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_gradient_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1847 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_deeptaylor.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1511 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_init.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/utils/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/utils/keras/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1759 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/utils/keras/test_graph.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/utils/keras/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)      967 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/utils/test_visualizations.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/utils/tests/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1189 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/utils/tests/test_dryrun.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/utils/tests/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/tests/utils/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/
--rw-rw-r--   0 nils      (1000) nils      (1000)     8632 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/pattern_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1948 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/misc.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    14767 2022-04-19 15:27:53.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/gradient_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     7094 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/deeptaylor.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    14225 2023-04-14 13:23:46.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/wrapper.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    26365 2022-05-11 10:33:05.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/reverse_map.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    20907 2022-04-06 15:20:24.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/base.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4395 2022-07-20 07:31:35.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/canonization/
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/canonization/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    15327 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/deeplift.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/relevance_based/
--rw-rw-r--   0 nils      (1000) nils      (1000)     3842 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/relevance_based/utils.py
--rw-rw-r--   0 nils      (1000) nils      (1000)       65 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/relevance_based/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    24188 2022-07-20 07:29:13.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    52929 2023-07-10 09:21:05.000000 SIGN-XAI-1.0.0/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py
--rw-rw-r--   0 nils      (1000) nils      (1000)      216 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/backend/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1234 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/backend/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/backend/tensorflow.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/backend/torch.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/keras/
--rw-rw-r--   0 nils      (1000) nils      (1000)     5921 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/keras/backend.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    14517 2022-04-06 15:20:24.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/keras/checks.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2318 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/keras/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    43869 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/keras/graph.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4925 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/visualizations.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/
--rw-rw-r--   0 nils      (1000) nils      (1000)     2818 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/dryrun.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/cases/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1313 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/cases/mlp.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1634 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/cases/special.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1383 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/cases/helper.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3322 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/cases/cnn.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2457 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/cases/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1592 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/cases/trivia.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     5791 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.0/methods/innvestigate/utils/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 SIGN-XAI-1.0.0/methods/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2603 2022-09-16 14:59:58.000000 SIGN-XAI-1.0.0/methods/grad_cam.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    25732 2023-07-10 10:29:31.000000 SIGN-XAI-1.0.0/methods/wrappers.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1499 2022-04-26 09:45:35.000000 SIGN-XAI-1.0.0/methods/guided_backprop.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/utils/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1654 2023-07-10 10:29:50.000000 SIGN-XAI-1.0.0/utils/utils.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2023-07-10 10:28:07.000000 SIGN-XAI-1.0.0/utils/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)      767 2023-07-10 10:32:06.000000 SIGN-XAI-1.0.0/PKG-INFO
--rw-rw-r--   0 nils      (1000) nils      (1000)     2182 2023-07-10 08:27:19.000000 SIGN-XAI-1.0.0/LICENSE
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/
+-rw-rw-r--   0 nils      (1000) nils      (1000)       38 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/setup.cfg
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/examples/
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 SIGN-XAI-1.0.1/examples/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)      824 2023-07-10 10:29:14.000000 SIGN-XAI-1.0.1/examples/vgg16.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1120 2023-07-10 09:52:50.000000 SIGN-XAI-1.0.1/README.md
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/SIGN_XAI.egg-info/
+-rw-rw-r--   0 nils      (1000) nils      (1000)       36 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/SIGN_XAI.egg-info/requires.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)        1 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/SIGN_XAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3200 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/SIGN_XAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)       23 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/SIGN_XAI.egg-info/top_level.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1920 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/SIGN_XAI.egg-info/PKG-INFO
+-rw-rw-r--   0 nils      (1000) nils      (1000)       74 2023-07-10 10:29:14.000000 SIGN-XAI-1.0.1/MANIFEST.in
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1831 2023-07-10 10:44:35.000000 SIGN-XAI-1.0.1/setup.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/data/
+-rw-rw-r--   0 nils      (1000) nils      (1000)  4924665 2022-07-11 11:25:40.000000 SIGN-XAI-1.0.1/data/7867854122_b26957e9e3_o.jpg
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/
+-rw-rw-r--   0 nils      (1000) nils      (1000)      253 2023-04-27 08:51:48.000000 SIGN-XAI-1.0.1/methods/signed.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/tools/
+-rw-rw-r--   0 nils      (1000) nils      (1000)      225 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tools/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    19540 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tools/pattern.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    18118 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tools/perturbate.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    19365 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/layers.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/applications/
+-rw-rw-r--   0 nils      (1000) nils      (1000)    10473 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/applications/imagenet.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/applications/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4256 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/applications/mnist.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/tools/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3969 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/tools/test_perturbate.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    12358 2022-05-24 09:53:27.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/tools/test_pattern.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/tools/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/
+-rw-rw-r--   0 nils      (1000) nils      (1000)    10210 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_relevance_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3790 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_wrapper.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1303 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_misc.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3948 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_deeplift.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3025 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_pattern_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4878 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_base.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     7771 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_gradient_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1847 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_deeptaylor.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1511 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_init.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/utils/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/utils/keras/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1759 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/utils/keras/test_graph.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/utils/keras/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)      967 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/utils/test_visualizations.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/utils/tests/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1189 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/utils/tests/test_dryrun.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/utils/tests/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/tests/utils/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     8632 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/pattern_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1948 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/misc.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    14767 2022-04-19 15:27:53.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/gradient_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     7094 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/deeptaylor.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    14225 2023-04-14 13:23:46.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/wrapper.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    26365 2022-05-11 10:33:05.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/reverse_map.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    20907 2022-04-06 15:20:24.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/base.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4395 2022-07-20 07:31:35.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/canonization/
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/canonization/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    15327 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/deeplift.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/relevance_based/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3842 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/relevance_based/utils.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)       65 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/relevance_based/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    24188 2022-07-20 07:29:13.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    52929 2023-07-10 09:21:05.000000 SIGN-XAI-1.0.1/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)      216 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/backend/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1234 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/backend/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/backend/tensorflow.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/backend/torch.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/keras/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     5921 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/keras/backend.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    14517 2022-04-06 15:20:24.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/keras/checks.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2318 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/keras/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    43869 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/keras/graph.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4925 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/visualizations.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2818 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/dryrun.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/cases/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1313 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/cases/mlp.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1634 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/cases/special.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1383 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/cases/helper.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3322 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/cases/cnn.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2457 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/cases/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1592 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/cases/trivia.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     5791 2022-02-16 10:22:41.000000 SIGN-XAI-1.0.1/methods/innvestigate/utils/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 SIGN-XAI-1.0.1/methods/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2603 2022-09-16 14:59:58.000000 SIGN-XAI-1.0.1/methods/grad_cam.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    25732 2023-07-10 10:29:31.000000 SIGN-XAI-1.0.1/methods/wrappers.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1499 2022-04-26 09:45:35.000000 SIGN-XAI-1.0.1/methods/guided_backprop.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/utils/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1654 2023-07-10 10:29:50.000000 SIGN-XAI-1.0.1/utils/utils.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2023-07-10 10:28:07.000000 SIGN-XAI-1.0.1/utils/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1920 2023-07-10 10:45:02.000000 SIGN-XAI-1.0.1/PKG-INFO
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2182 2023-07-10 08:27:19.000000 SIGN-XAI-1.0.1/LICENSE
```

### Comparing `SIGN-XAI-1.0.0/examples/vgg16.py` & `SIGN-XAI-1.0.1/examples/vgg16.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/README.md` & `SIGN-XAI-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/SIGN_XAI.egg-info/SOURCES.txt` & `SIGN-XAI-1.0.1/SIGN_XAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/setup.py` & `SIGN-XAI-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from setuptools import setup
 
+with open('README.md') as f:
+    long_description = f.read()
+
 setup(
     name='SIGN-XAI',
-    version='1.0.0',
+    version='1.0.1',
     packages=['methods', 'methods.innvestigate', 'methods.innvestigate.tests', 'methods.innvestigate.tests.tools',
               'methods.innvestigate.tests.utils', 'methods.innvestigate.tests.utils.keras',
               'methods.innvestigate.tests.utils.tests', 'methods.innvestigate.tests.analyzer',
               'methods.innvestigate.tools', 'methods.innvestigate.utils', 'methods.innvestigate.utils.keras',
               'methods.innvestigate.utils.tests', 'methods.innvestigate.utils.tests.cases',
               'methods.innvestigate.backend', 'methods.innvestigate.analyzer',
               'methods.innvestigate.analyzer.canonization', 'methods.innvestigate.analyzer.relevance_based',
@@ -14,14 +17,16 @@
     url='https://github.com/nilsgumpfer/SIGN-XAI',
     license='BSD 2-Clause License',
     author='Nils Gumpfer',
     author_email='nils.gumpfer@kite.thm.de',
     maintainer='Nils Gumpfer',
     maintainer_email='nils.gumpfer@kite.thm.de',
     description='SIGNed explanations: Unveiling relevant features by reducing bias',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     keywords=['XAI', 'SIGN', 'LRP'],
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: BSD License',
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
```

### Comparing `SIGN-XAI-1.0.0/data/7867854122_b26957e9e3_o.jpg` & `SIGN-XAI-1.0.1/data/7867854122_b26957e9e3_o.jpg`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tools/pattern.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tools/pattern.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tools/perturbate.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tools/perturbate.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/layers.py` & `SIGN-XAI-1.0.1/methods/innvestigate/layers.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/applications/imagenet.py` & `SIGN-XAI-1.0.1/methods/innvestigate/applications/imagenet.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/applications/mnist.py` & `SIGN-XAI-1.0.1/methods/innvestigate/applications/mnist.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/tools/test_perturbate.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/tools/test_perturbate.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/tools/test_pattern.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/tools/test_pattern.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_relevance_based.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_relevance_based.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_wrapper.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_misc.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_misc.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_deeplift.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_deeplift.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_pattern_based.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_pattern_based.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_base.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_base.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_gradient_based.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_gradient_based.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_deeptaylor.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_deeptaylor.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/analyzer/test_init.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/analyzer/test_init.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/utils/keras/test_graph.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/utils/keras/test_graph.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/utils/test_visualizations.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/utils/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/tests/utils/tests/test_dryrun.py` & `SIGN-XAI-1.0.1/methods/innvestigate/tests/utils/tests/test_dryrun.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/analyzer/pattern_based.py` & `SIGN-XAI-1.0.1/methods/innvestigate/analyzer/pattern_based.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/analyzer/misc.py` & `SIGN-XAI-1.0.1/methods/innvestigate/analyzer/misc.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/analyzer/gradient_based.py` & `SIGN-XAI-1.0.1/methods/innvestigate/analyzer/gradient_based.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/analyzer/deeptaylor.py` & `SIGN-XAI-1.0.1/methods/innvestigate/analyzer/deeptaylor.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/analyzer/wrapper.py` & `SIGN-XAI-1.0.1/methods/innvestigate/analyzer/wrapper.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/analyzer/reverse_map.py` & `SIGN-XAI-1.0.1/methods/innvestigate/analyzer/reverse_map.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/analyzer/base.py` & `SIGN-XAI-1.0.1/methods/innvestigate/analyzer/base.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/analyzer/__init__.py` & `SIGN-XAI-1.0.1/methods/innvestigate/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/analyzer/deeplift.py` & `SIGN-XAI-1.0.1/methods/innvestigate/analyzer/deeplift.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/analyzer/relevance_based/utils.py` & `SIGN-XAI-1.0.1/methods/innvestigate/analyzer/relevance_based/utils.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py` & `SIGN-XAI-1.0.1/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py` & `SIGN-XAI-1.0.1/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/backend/__init__.py` & `SIGN-XAI-1.0.1/methods/innvestigate/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/utils/keras/backend.py` & `SIGN-XAI-1.0.1/methods/innvestigate/utils/keras/backend.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/utils/keras/checks.py` & `SIGN-XAI-1.0.1/methods/innvestigate/utils/keras/checks.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/utils/keras/__init__.py` & `SIGN-XAI-1.0.1/methods/innvestigate/utils/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/utils/keras/graph.py` & `SIGN-XAI-1.0.1/methods/innvestigate/utils/keras/graph.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/utils/visualizations.py` & `SIGN-XAI-1.0.1/methods/innvestigate/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/dryrun.py` & `SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/dryrun.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/cases/mlp.py` & `SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/cases/mlp.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/cases/special.py` & `SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/cases/special.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/cases/helper.py` & `SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/cases/helper.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/cases/cnn.py` & `SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/cases/cnn.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/cases/__init__.py` & `SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/utils/tests/cases/trivia.py` & `SIGN-XAI-1.0.1/methods/innvestigate/utils/tests/cases/trivia.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/innvestigate/utils/__init__.py` & `SIGN-XAI-1.0.1/methods/innvestigate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/grad_cam.py` & `SIGN-XAI-1.0.1/methods/grad_cam.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/wrappers.py` & `SIGN-XAI-1.0.1/methods/wrappers.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/methods/guided_backprop.py` & `SIGN-XAI-1.0.1/methods/guided_backprop.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/utils/utils.py` & `SIGN-XAI-1.0.1/utils/utils.py`

 * *Files identical despite different names*

### Comparing `SIGN-XAI-1.0.0/LICENSE` & `SIGN-XAI-1.0.1/LICENSE`

 * *Files identical despite different names*

