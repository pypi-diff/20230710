# Comparing `tmp/model_constructor-0.3.2.tar.gz` & `tmp/model_constructor-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_constructor-0.3.2.tar", last modified: Thu Dec 22 08:12:57 2022, max compression
+gzip compressed data, was "model_constructor-0.4.tar", last modified: Mon Jul 10 13:23:02 2023, max compression
```

## Comparing `model_constructor-0.3.2.tar` & `model_constructor-0.4.tar`

### file list

```diff
@@ -1,29 +1,44 @@
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2022-12-22 08:12:57.258488 model_constructor-0.3.2/
--rw-rw-r--   0 aya       (1000) aya       (1000)     2348 2021-12-22 07:36:39.000000 model_constructor-0.3.2/CONTRIBUTING.md
--rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2021-12-22 07:36:39.000000 model_constructor-0.3.2/LICENSE
--rw-rw-r--   0 aya       (1000) aya       (1000)      111 2021-12-22 07:36:39.000000 model_constructor-0.3.2/MANIFEST.in
--rw-rw-r--   0 aya       (1000) aya       (1000)    43532 2022-12-22 08:12:57.258488 model_constructor-0.3.2/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)    43013 2022-12-22 06:26:10.000000 model_constructor-0.3.2/README.md
--rw-rw-r--   0 aya       (1000) aya       (1000)      752 2022-08-02 08:52:12.000000 model_constructor-0.3.2/settings.ini
--rw-rw-r--   0 aya       (1000) aya       (1000)      690 2022-12-22 08:12:57.258488 model_constructor-0.3.2/setup.cfg
--rw-rw-r--   0 aya       (1000) aya       (1000)      597 2022-11-16 08:37:06.000000 model_constructor-0.3.2/setup.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2022-12-22 08:12:57.230489 model_constructor-0.3.2/src/
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2022-12-22 08:12:57.250488 model_constructor-0.3.2/src/model_constructor/
--rw-rw-r--   0 aya       (1000) aya       (1000)      242 2022-12-21 15:06:47.000000 model_constructor-0.3.2/src/model_constructor/__init__.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     4846 2022-12-21 12:58:40.000000 model_constructor-0.3.2/src/model_constructor/activations.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     6555 2022-12-21 12:59:00.000000 model_constructor-0.3.2/src/model_constructor/base_constructor.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     4145 2022-12-21 12:59:12.000000 model_constructor-0.3.2/src/model_constructor/convmixer.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     9605 2022-12-21 15:06:47.000000 model_constructor-0.3.2/src/model_constructor/layers.py
--rw-rw-r--   0 aya       (1000) aya       (1000)    12892 2022-12-21 15:06:47.000000 model_constructor-0.3.2/src/model_constructor/model_constructor.py
--rw-rw-r--   0 aya       (1000) aya       (1000)      436 2022-12-21 15:06:47.000000 model_constructor-0.3.2/src/model_constructor/mxresnet.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     8963 2022-12-21 13:00:29.000000 model_constructor-0.3.2/src/model_constructor/net.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     7257 2022-12-21 15:06:47.000000 model_constructor-0.3.2/src/model_constructor/twist.py
--rw-rw-r--   0 aya       (1000) aya       (1000)       22 2022-12-21 18:45:15.000000 model_constructor-0.3.2/src/model_constructor/version.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2397 2022-12-21 15:06:47.000000 model_constructor-0.3.2/src/model_constructor/xresnet.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     4500 2022-12-22 06:21:58.000000 model_constructor-0.3.2/src/model_constructor/yaresnet.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2022-12-22 08:12:57.254488 model_constructor-0.3.2/src/model_constructor.egg-info/
--rw-rw-r--   0 aya       (1000) aya       (1000)    43532 2022-12-22 08:12:57.000000 model_constructor-0.3.2/src/model_constructor.egg-info/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)      718 2022-12-22 08:12:57.000000 model_constructor-0.3.2/src/model_constructor.egg-info/SOURCES.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)        1 2022-12-22 08:12:57.000000 model_constructor-0.3.2/src/model_constructor.egg-info/dependency_links.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       48 2022-12-22 08:12:57.000000 model_constructor-0.3.2/src/model_constructor.egg-info/requires.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       18 2022-12-22 08:12:57.000000 model_constructor-0.3.2/src/model_constructor.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-10 13:23:02.112471 model_constructor-0.4/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2348 2021-12-22 07:36:39.000000 model_constructor-0.4/CONTRIBUTING.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2021-12-22 07:36:39.000000 model_constructor-0.4/LICENSE
+-rw-rw-r--   0 aya       (1000) aya       (1000)      111 2021-12-22 07:36:39.000000 model_constructor-0.4/MANIFEST.in
+-rw-rw-r--   0 aya       (1000) aya       (1000)    38242 2023-07-10 13:23:02.112471 model_constructor-0.4/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)    37725 2023-07-07 16:51:56.000000 model_constructor-0.4/README.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)      752 2022-08-02 08:52:12.000000 model_constructor-0.4/settings.ini
+-rw-rw-r--   0 aya       (1000) aya       (1000)      690 2023-07-10 13:23:02.112471 model_constructor-0.4/setup.cfg
+-rw-rw-r--   0 aya       (1000) aya       (1000)      597 2022-11-16 08:37:06.000000 model_constructor-0.4/setup.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-10 13:23:02.104471 model_constructor-0.4/src/
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-10 13:23:02.108471 model_constructor-0.4/src/model_constructor/
+-rw-rw-r--   0 aya       (1000) aya       (1000)      124 2023-07-06 10:40:14.000000 model_constructor-0.4/src/model_constructor/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4903 2023-07-06 10:40:14.000000 model_constructor-0.4/src/model_constructor/activations.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     8963 2023-07-10 12:49:31.000000 model_constructor-0.4/src/model_constructor/base_constructor.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     6144 2023-07-10 12:11:14.000000 model_constructor-0.4/src/model_constructor/blocks.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     5461 2023-07-10 12:47:21.000000 model_constructor-0.4/src/model_constructor/convmixer.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4464 2023-07-10 13:06:56.000000 model_constructor-0.4/src/model_constructor/helpers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)    10091 2023-07-10 12:44:50.000000 model_constructor-0.4/src/model_constructor/layers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     7847 2023-07-10 12:49:20.000000 model_constructor-0.4/src/model_constructor/model_constructor.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      364 2023-07-10 12:31:14.000000 model_constructor-0.4/src/model_constructor/mxresnet.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     9349 2023-07-10 12:50:04.000000 model_constructor-0.4/src/model_constructor/net.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     7220 2023-07-10 12:50:10.000000 model_constructor-0.4/src/model_constructor/twist.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11851 2023-07-10 12:45:33.000000 model_constructor-0.4/src/model_constructor/universal_blocks.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       20 2023-07-10 13:11:31.000000 model_constructor-0.4/src/model_constructor/version.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1581 2023-07-10 12:35:45.000000 model_constructor-0.4/src/model_constructor/xresnet.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     6371 2023-07-10 12:35:59.000000 model_constructor-0.4/src/model_constructor/yaresnet.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-10 13:23:02.112471 model_constructor-0.4/src/model_constructor.egg-info/
+-rw-rw-r--   0 aya       (1000) aya       (1000)    38242 2023-07-10 13:23:02.000000 model_constructor-0.4/src/model_constructor.egg-info/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1089 2023-07-10 13:23:02.000000 model_constructor-0.4/src/model_constructor.egg-info/SOURCES.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-07-10 13:23:02.000000 model_constructor-0.4/src/model_constructor.egg-info/dependency_links.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       67 2023-07-10 13:23:02.000000 model_constructor-0.4/src/model_constructor.egg-info/requires.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       18 2023-07-10 13:23:02.000000 model_constructor-0.4/src/model_constructor.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-10 13:23:02.112471 model_constructor-0.4/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3889 2022-12-21 15:06:47.000000 model_constructor-0.4/tests/test_Net.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1791 2023-07-06 10:40:14.000000 model_constructor-0.4/tests/test_blocks.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1840 2023-05-24 06:20:35.000000 model_constructor-0.4/tests/test_blocks_universal.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      902 2022-12-21 15:06:47.000000 model_constructor-0.4/tests/test_convmixer.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2668 2023-07-07 10:14:14.000000 model_constructor-0.4/tests/test_helpers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2870 2023-05-24 06:20:35.000000 model_constructor-0.4/tests/test_layers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1669 2022-12-21 15:06:47.000000 model_constructor-0.4/tests/test_layers_depr.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     5040 2023-07-10 13:07:26.000000 model_constructor-0.4/tests/test_mc.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1325 2023-07-10 12:32:36.000000 model_constructor-0.4/tests/test_models.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      995 2023-05-24 06:20:35.000000 model_constructor-0.4/tests/test_models_old.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1070 2023-07-10 12:33:17.000000 model_constructor-0.4/tests/test_models_universal_blocks.py
```

### Comparing `model_constructor-0.3.2/CONTRIBUTING.md` & `model_constructor-0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `model_constructor-0.3.2/LICENSE` & `model_constructor-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `model_constructor-0.3.2/PKG-INFO` & `model_constructor-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model_constructor
-Version: 0.3.2
+Version: 0.4
 Summary: Pytorch models constructor.
 Home-page: https://github.com/ayasyrev/model_constructor
 Author: Yasyrev Andrei
 Author-email: a.yasyrev@gmail.com
 License: apache2
 Keywords: pytorch models
 Classifier: Programming Language :: Python :: 3
@@ -50,97 +50,73 @@
 mc
 ```
 <details open> <summary>output</summary>  
     <pre>ModelConstructor
       in_chans: 3, num_classes: 1000
       expansion: 1, groups: 1, dw: False, div_groups: None
       act_fn: ReLU, sa: False, se: False
-      stem sizes: [32, 32, 64], stride on 0
+      stem sizes: [64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]<pre>
+      layers: [2, 2, 2, 2]</pre>
 </details>
 
 
 
 Check all parameters with `print_cfg` method:
 
 
 ```python
 mc.print_cfg()
 ```
 <details open> <summary>output</summary>  
-    <pre>ModelConstructor(
-      in_chans=3
-      num_classes=1000
-      block='ResBlock'
-      conv_layer='ConvBnAct'
-      block_sizes=[64, 128, 256, 512]
-      layers=[2, 2, 2, 2]
-      norm='BatchNorm2d'
-      act_fn='ReLU'
-      pool="AvgPool2d {'kernel_size': 2, 'ceil_mode': True}"
-      expansion=1
-      groups=1
-      bn_1st=True
-      zero_bn=True
-      stem_sizes=[32, 32, 64]
-      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
-      init_cnn='init_cnn'
-      make_stem='make_stem'
-      make_layer='make_layer'
-      make_body='make_body'
-      make_head='make_head')
-    <pre>
+    <pre>ModelConstructor
+      in_chans: 3, num_classes: 1000
+      expansion: 1, groups: 1, dw: False, div_groups: None
+      act_fn: ReLU, sa: False, se: False
+      stem sizes: [64], stride on 0
+      body sizes [64, 128, 256, 512]
+      layers: [2, 2, 2, 2]
+    </pre>
 </details>
 
-Now we have model constructor, default setting as xresnet18. And we can get model after call it.
+Now we have model constructor, default setting as resnet18. And we can get model after call it.
 
 
 ```python
 
 model = mc()
 model
 ```
 <details> <summary>output</summary>  
-    <pre>ModelConstructor(
+    </pre>ModelConstructor(
       (stem): Sequential(
-        (conv_0): ConvBnAct(
-          (conv): Conv2d(3, 32, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
-          (bn): BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-          (act_fn): ReLU(inplace=True)
-        )
         (conv_1): ConvBnAct(
-          (conv): Conv2d(32, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
-          (bn): BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-          (act_fn): ReLU(inplace=True)
-        )
-        (conv_2): ConvBnAct(
-          (conv): Conv2d(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
+          (conv): Conv2d(3, 64, kernel_size=(7, 7), stride=(2, 2), padding=(3, 3), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): ReLU(inplace=True)
         )
         (stem_pool): MaxPool2d(kernel_size=3, stride=2, padding=1, dilation=1, ceil_mode=False)
       )
       (body): Sequential(
         (l_0): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -148,36 +124,35 @@
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
         )
         (l_1): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -185,36 +160,35 @@
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
         )
         (l_2): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -222,36 +196,35 @@
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
         )
         (l_3): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -264,377 +237,311 @@
         )
       )
       (head): Sequential(
         (pool): AdaptiveAvgPool2d(output_size=1)
         (flat): Flatten(start_dim=1, end_dim=-1)
         (fc): Linear(in_features=512, out_features=1000, bias=True)
       )
-    )<pre>
+    )</pre>
 </details>
 
 
 
 If you want to change model, just change constructor parameters.  
-Lets create xresnet50.
+Lets create resnet50.
 
 
 ```python
 mc.expansion = 4
 mc.layers = [3,4,6,3]
 ```
 
+We can check, what we changed (compare to default constructor).
+
+
+```python
+mc.changed_fields
+```
+<details open> <summary>output</summary>  
+    <pre>{'layers': [3, 4, 6, 3], 'expansion': 4}</pre>
+</details>
+
+
+
+
+```python
+mc.print_changed_fields()
+```
+<details open> <summary>output</summary>  
+    <pre>Changed fields:
+    layers: [3, 4, 6, 3]
+    expansion: 4
+    </pre>
+</details>
+
 Now we can look at model parts - stem, body, head.  
 
 
 ```python
 
 mc.body
 ```
 <details> <summary>output</summary>  
-    <pre>Sequential(
+    </pre>Sequential(
       (l_0): Sequential(
-        (bl_0): ResBlock(
+        (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(64, 64, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-            )
-          )
-          (id_conv): Sequential(
-            (id_conv): ConvBnAct(
-              (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_1): ResBlock(
+        (bl_1): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(256, 64, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_2): ResBlock(
+        (bl_2): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(256, 64, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
       )
       (l_1): Sequential(
-        (bl_0): ResBlock(
+        (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(256, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
-              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
+              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(128, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (id_conv): Sequential(
-            (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
             (id_conv): ConvBnAct(
-              (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
+              (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(2, 2), bias=False)
+              (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_1): ResBlock(
+        (bl_1): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(512, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(128, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_2): ResBlock(
+        (bl_2): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(512, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(128, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_3): ResBlock(
+        (bl_3): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(512, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(128, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
       )
       (l_2): Sequential(
-        (bl_0): ResBlock(
+        (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(512, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
-              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (id_conv): Sequential(
-            (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
             (id_conv): ConvBnAct(
-              (conv): Conv2d(512, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
+              (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(2, 2), bias=False)
+              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_1): ResBlock(
+        (bl_1): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_2): ResBlock(
+        (bl_2): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_3): ResBlock(
+        (bl_3): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_4): ResBlock(
+        (bl_4): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_5): ResBlock(
+        (bl_5): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
       )
       (l_3): Sequential(
-        (bl_0): ResBlock(
+        (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
-              (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
+              (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(512, 2048, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(2048, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (id_conv): Sequential(
-            (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
             (id_conv): ConvBnAct(
-              (conv): Conv2d(1024, 2048, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(2048, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
+              (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(2, 2), bias=False)
+              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_1): ResBlock(
+        (bl_1): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(2048, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(512, 2048, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(2048, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_2): ResBlock(
+        (bl_2): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(2048, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(512, 2048, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(2048, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
       )
-    )<pre>
+    )</pre>
 </details>
 
 
 
 ## Create constructor from config.
 
 Alternative we can create config first and than create constructor from it. 
@@ -642,37 +549,60 @@
 
 ```python
 from model_constructor import ModelCfg
 ```
 
 
 ```python
-cfg = ModelCfg()
+cfg = ModelCfg(
+    num_classes=10,
+    act_fn=nn.Mish,
+)
 print(cfg)
 ```
 <details open> <summary>output</summary>  
-    <pre>in_chans=3 num_classes=1000 block='ResBlock' conv_layer='ConvBnAct' block_sizes=[64, 128, 256, 512] layers=[2, 2, 2, 2] norm='BatchNorm2d' act_fn='ReLU' pool="AvgPool2d {'kernel_size': 2, 'ceil_mode': True}" expansion=1 groups=1 bn_1st=True zero_bn=True stem_sizes=[32, 32, 64] stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}" init_cnn='init_cnn' make_stem='make_stem' make_layer='make_layer' make_body='make_body' make_head='make_head'
-    <pre>
+    <pre>in_chans=3 num_classes=10 block='BasicBlock' conv_layer='ConvBnAct' block_sizes=[64, 128, 256, 512] layers=[2, 2, 2, 2] norm='BatchNorm2d' act_fn='Mish' expansion=1 groups=1 bn_1st=True zero_bn=True stem_sizes=[64] stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+    </pre>
+</details>
+
+When creating config or constructor we can use string annotation for nn.Modules - it useful when creating model from config files.
+
+
+```python
+cfg = ModelCfg(
+    num_classes=10,
+    act_fn="nn.SELU",
+)
+print(cfg.act_fn)
+```
+<details open> <summary>output</summary>  
+    <pre>class 'torch.nn.modules.activation.SELU'
+    </pre>
 </details>
 
 Now we can create constructor from config:
 
 
 ```python
 mc = ModelConstructor.from_cfg(cfg)
 mc
 ```
 <details open> <summary>output</summary>  
+    <pre>Deprecated. Pass se_module as se argument, se_reduction as arg to se.
+    Deprecated. Pass se_module as se argument, se_reduction as arg to se.
+    </pre>
+</details>
+<details open> <summary>output</summary>  
     <pre>ModelConstructor
-      in_chans: 3, num_classes: 1000
+      in_chans: 3, num_classes: 10
       expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: False, se: False
-      stem sizes: [32, 32, 64], stride on 0
+      act_fn: ReLU, sa: <class 'model_constructor.layers.SimpleSelfAttention'>, se: SEModule
+      stem sizes: [64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]<pre>
+      layers: [2, 2, 2, 2]</pre>
 </details>
 
 
 
 ## More modification.
 
 Main purpose of this module - fast and easy modify model.
@@ -688,24 +618,29 @@
 mc = ModelConstructor(name='MxResNet')
 ```
 
 Then lets modify stem.
 
 
 ```python
+from model_constructor.xresnet import xresnet_stem
+```
+
+
+```python
+mc.make_stem = xresnet_stem
 mc.stem_sizes = [3,32,64,64]
 ```
 
 Now lets change activation function to Mish.
 Here is link to [forum discussion](https://forums.fast.ai/t/meet-mish-new-activation-function-possible-successor-to-relu)    
 We'v got Mish is in model_constructor.activations, but from pytorch 1.9 take it from torch:
 
 
 ```python
-# from model_constructor.activations import Mish
 from torch.nn import Mish
 ```
 
 
 ```python
 mc.act_fn = Mish
 ```
@@ -717,29 +652,42 @@
 <details open> <summary>output</summary>  
     <pre>MxResNet
       in_chans: 3, num_classes: 1000
       expansion: 1, groups: 1, dw: False, div_groups: None
       act_fn: Mish, sa: False, se: False
       stem sizes: [3, 32, 64, 64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]<pre>
+      layers: [2, 2, 2, 2]</pre>
 </details>
 
 
 
+
+```python
+mc.print_changed_fields()
+```
+<details open> <summary>output</summary>  
+    <pre>Changed fields:
+    name: MxResNet
+    act_fn: Mish
+    stem_sizes: [3, 32, 64, 64]
+    make_stem: xresnet_stem
+    </pre>
+</details>
+
 Here is model:  
 
 
 ```python
 
 mc()
 ```
 <details> <summary>output</summary>  
-    <pre>MxResNet(
-      stem_sizes: [3, 32, 64, 64], act_fn: Mish
+    </pre>MxResNet(
+      act_fn: Mish, stem_sizes: [3, 32, 64, 64], make_stem: xresnet_stem
       (stem): Sequential(
         (conv_0): ConvBnAct(
           (conv): Conv2d(3, 3, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(3, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
         (conv_1): ConvBnAct(
@@ -757,29 +705,29 @@
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
         (stem_pool): MaxPool2d(kernel_size=3, stride=2, padding=1, dilation=1, ceil_mode=False)
       )
       (body): Sequential(
         (l_0): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -787,36 +735,35 @@
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
         )
         (l_1): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -824,36 +771,35 @@
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
         )
         (l_2): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -861,36 +807,35 @@
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
         )
         (l_3): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -903,30 +848,45 @@
         )
       )
       (head): Sequential(
         (pool): AdaptiveAvgPool2d(output_size=1)
         (flat): Flatten(start_dim=1, end_dim=-1)
         (fc): Linear(in_features=512, out_features=1000, bias=True)
       )
-    )<pre>
+    )</pre>
 </details>
 
 
 
 ## MXResNet50
 
 Now lets make MxResNet50
 
 
 ```python
 mc.expansion = 4
 mc.layers = [3,4,6,3]
-mc.name = 'mxresnet50'
+mc.name = "mxresnet50"
 ```
 
+
+```python
+mc.print_changed_fields()
+```
+<details open> <summary>output</summary>  
+    <pre>Changed fields:
+    name: mxresnet50
+    layers: [3, 4, 6, 3]
+    act_fn: Mish
+    expansion: 4
+    stem_sizes: [3, 32, 64, 64]
+    make_stem: xresnet_stem
+    </pre>
+</details>
+
 Now we have mxresnet50 constructor.  
 We can inspect every parts of it.  
 And after call it we got model.
 
 
 ```python
 mc
@@ -934,152 +894,141 @@
 <details open> <summary>output</summary>  
     <pre>mxresnet50
       in_chans: 3, num_classes: 1000
       expansion: 4, groups: 1, dw: False, div_groups: None
       act_fn: Mish, sa: False, se: False
       stem sizes: [3, 32, 64, 64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [3, 4, 6, 3]<pre>
+      layers: [3, 4, 6, 3]</pre>
 </details>
 
 
 
 
 ```python
 
 mc.stem.conv_1
 ```
 <details> <summary>output</summary>  
-    <pre>ConvBnAct(
+    </pre>ConvBnAct(
       (conv): Conv2d(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
       (bn): BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
       (act_fn): Mish(inplace=True)
-    )<pre>
+    )</pre>
 </details>
 
 
 
 
 ```python
 
 mc.body.l_0.bl_0
 ```
 <details> <summary>output</summary>  
-    <pre>ResBlock(
+    </pre>BasicBlock(
       (convs): Sequential(
         (conv_0): ConvBnAct(
-          (conv): Conv2d(64, 64, kernel_size=(1, 1), stride=(1, 1), bias=False)
+          (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
         (conv_1): ConvBnAct(
           (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-          (act_fn): Mish(inplace=True)
-        )
-        (conv_2): ConvBnAct(
-          (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-          (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-        )
-      )
-      (id_conv): Sequential(
-        (id_conv): ConvBnAct(
-          (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-          (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
         )
       )
       (act_fn): Mish(inplace=True)
-    )<pre>
+    )</pre>
 </details>
 
 
 
 We can get model direct way:
 
 
 ```python
-mc = ModelConstructor(name="MxResNet", act_fn=Mish, layers=[3,4,6,3], expansion=4, stem_sizes=[32,64,64])
+mc = ModelConstructor(
+    name="MxResNet",
+    act_fn=Mish,
+    layers=[3,4,6,3],
+    expansion=4,
+    make_stem=xresnet_stem,
+    stem_sizes=[32,64,64]
+)
 model = mc()
 ```
 
-Or create with config:
+Another way:
 
 
 ```python
-mc = ModelConstructor.from_cfg(
-    ModelCfg(name="MxResNet", act_fn=Mish, layers=[3,4,6,3], expansion=4, stem_sizes=[32,64,64])
+model = ModelConstructor.create_model(
+    name="MxResNet",
+    act_fn=Mish,
+    layers=[3,4,6,3],
+    expansion=4,
+    make_stem=xresnet_stem,
+    stem_sizes=[32,64,64]
 )
-model = mc()
 ```
 
 ## YaResNet
 
 Now lets change Resblock to YaResBlock (Yet another ResNet, former NewResBlock) is in lib from version 0.1.0
 
 
 ```python
-from model_constructor.yaresnet import YaResBlock
+from model_constructor.yaresnet import YaBasicBlock
 ```
 
 
 ```python
 mc = ModelConstructor(name="YaResNet")
-mc.block = YaResBlock
+mc.block = YaBasicBlock
 ```
 
 Or in one line:
 
 
 ```python
-mc = ModelConstructor(name="YaResNet", block=YaResBlock)
+mc = ModelConstructor(name="YaResNet", block=YaBasicBlock)
 ```
 
 That all. Now we have YaResNet constructor
 
 
 ```python
 
 mc.print_cfg()
 ```
 <details> <summary>output</summary>  
-    <pre>ModelConstructor(
-      name='YaResNet'
-      in_chans=3
-      num_classes=1000
-      block='YaResBlock'
-      conv_layer='ConvBnAct'
-      block_sizes=[64, 128, 256, 512]
-      layers=[2, 2, 2, 2]
-      norm='BatchNorm2d'
-      act_fn='ReLU'
-      pool="AvgPool2d {'kernel_size': 2, 'ceil_mode': True}"
-      expansion=1
-      groups=1
-      bn_1st=True
-      zero_bn=True
-      stem_sizes=[32, 32, 64]
-      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
-      init_cnn='init_cnn'
-      make_stem='make_stem'
-      make_layer='make_layer'
-      make_body='make_body'
-      make_head='make_head')
-    <pre>
+    </pre>YaResNet
+      in_chans: 3, num_classes: 1000
+      expansion: 1, groups: 1, dw: False, div_groups: None
+      act_fn: ReLU, sa: False, se: False
+      stem sizes: [64], stride on 0
+      body sizes [64, 128, 256, 512]
+      layers: [2, 2, 2, 2]
+    </pre>
 </details>
 
 Let see what we have.
 
 
 ```python
 
 mc.body.l_1.bl_0
 ```
 <details> <summary>output</summary>  
-    <pre>YaResBlock(
-      (reduce): AvgPool2d(kernel_size=2, stride=2, padding=0)
+    </pre>YaBasicBlock(
+      (reduce): ConvBnAct(
+        (conv): Conv2d(64, 64, kernel_size=(1, 1), stride=(2, 2), bias=False)
+        (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
+        (act_fn): ReLU(inplace=True)
+      )
       (convs): Sequential(
         (conv_0): ConvBnAct(
           (conv): Conv2d(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): ReLU(inplace=True)
         )
         (conv_1): ConvBnAct(
@@ -1088,75 +1037,67 @@
         )
       )
       (id_conv): ConvBnAct(
         (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
         (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
       )
       (merge): ReLU(inplace=True)
-    )<pre>
+    )</pre>
 </details>
 
 
 
-Lets create `Resnet34` like model constructor:
+Lets create `xResnet34` like model constructor:
 
 
 ```python
+from typing import Callable
+
+from model_constructor.helpers import ModSeq
+
+
 class YaResnet34(ModelConstructor):
-    block: type[nn.Module] = YaResBlock
+    block: type[nn.Module] = YaBasicBlock
     layers: list[int] = [3, 4, 6, 3]
+    make_stem: Callable[[ModelCfg], ModSeq] = xresnet_stem
 ```
 
 
 ```python
 mc = YaResnet34()
 mc.print_cfg()
 ```
 <details open> <summary>output</summary>  
-    <pre>YaResnet34(
-      in_chans=3
-      num_classes=1000
-      block='YaResBlock'
-      conv_layer='ConvBnAct'
-      block_sizes=[64, 128, 256, 512]
-      layers=[3, 4, 6, 3]
-      norm='BatchNorm2d'
-      act_fn='ReLU'
-      pool="AvgPool2d {'kernel_size': 2, 'ceil_mode': True}"
-      expansion=1
-      groups=1
-      bn_1st=True
-      zero_bn=True
-      stem_sizes=[32, 32, 64]
-      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
-      init_cnn='init_cnn'
-      make_stem='make_stem'
-      make_layer='make_layer'
-      make_body='make_body'
-      make_head='make_head')
-    <pre>
+    <pre>YaResnet34
+      in_chans: 3, num_classes: 1000
+      expansion: 1, groups: 1, dw: False, div_groups: None
+      act_fn: ReLU, sa: False, se: False
+      stem sizes: [64], stride on 0
+      body sizes [64, 128, 256, 512]
+      layers: [3, 4, 6, 3]
+    </pre>
 </details>
 
-And `Resnet50` like model can be inherited from `YaResnet34`:
+And `xResnet50` like model can be inherited from `YaResnet34`:
 
 
 ```python
 class YaResnet50(YaResnet34):
-    expansion = 4
+    expansion: int = 4
 ```
 
 
 ```python
 mc = YaResnet50()
 mc
 ```
 <details open> <summary>output</summary>  
     <pre>YaResnet50
       in_chans: 3, num_classes: 1000
       expansion: 4, groups: 1, dw: False, div_groups: None
       act_fn: ReLU, sa: False, se: False
-      stem sizes: [32, 32, 64], stride on 0
+      stem sizes: [64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [3, 4, 6, 3]<pre>
+      layers: [3, 4, 6, 3]</pre>
 </details>
```

### Comparing `model_constructor-0.3.2/README.md` & `model_constructor-0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -33,97 +33,73 @@
 mc
 ```
 <details open> <summary>output</summary>  
     <pre>ModelConstructor
       in_chans: 3, num_classes: 1000
       expansion: 1, groups: 1, dw: False, div_groups: None
       act_fn: ReLU, sa: False, se: False
-      stem sizes: [32, 32, 64], stride on 0
+      stem sizes: [64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]<pre>
+      layers: [2, 2, 2, 2]</pre>
 </details>
 
 
 
 Check all parameters with `print_cfg` method:
 
 
 ```python
 mc.print_cfg()
 ```
 <details open> <summary>output</summary>  
-    <pre>ModelConstructor(
-      in_chans=3
-      num_classes=1000
-      block='ResBlock'
-      conv_layer='ConvBnAct'
-      block_sizes=[64, 128, 256, 512]
-      layers=[2, 2, 2, 2]
-      norm='BatchNorm2d'
-      act_fn='ReLU'
-      pool="AvgPool2d {'kernel_size': 2, 'ceil_mode': True}"
-      expansion=1
-      groups=1
-      bn_1st=True
-      zero_bn=True
-      stem_sizes=[32, 32, 64]
-      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
-      init_cnn='init_cnn'
-      make_stem='make_stem'
-      make_layer='make_layer'
-      make_body='make_body'
-      make_head='make_head')
-    <pre>
+    <pre>ModelConstructor
+      in_chans: 3, num_classes: 1000
+      expansion: 1, groups: 1, dw: False, div_groups: None
+      act_fn: ReLU, sa: False, se: False
+      stem sizes: [64], stride on 0
+      body sizes [64, 128, 256, 512]
+      layers: [2, 2, 2, 2]
+    </pre>
 </details>
 
-Now we have model constructor, default setting as xresnet18. And we can get model after call it.
+Now we have model constructor, default setting as resnet18. And we can get model after call it.
 
 
 ```python
 
 model = mc()
 model
 ```
 <details> <summary>output</summary>  
-    <pre>ModelConstructor(
+    </pre>ModelConstructor(
       (stem): Sequential(
-        (conv_0): ConvBnAct(
-          (conv): Conv2d(3, 32, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
-          (bn): BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-          (act_fn): ReLU(inplace=True)
-        )
         (conv_1): ConvBnAct(
-          (conv): Conv2d(32, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
-          (bn): BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-          (act_fn): ReLU(inplace=True)
-        )
-        (conv_2): ConvBnAct(
-          (conv): Conv2d(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
+          (conv): Conv2d(3, 64, kernel_size=(7, 7), stride=(2, 2), padding=(3, 3), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): ReLU(inplace=True)
         )
         (stem_pool): MaxPool2d(kernel_size=3, stride=2, padding=1, dilation=1, ceil_mode=False)
       )
       (body): Sequential(
         (l_0): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -131,36 +107,35 @@
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
         )
         (l_1): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -168,36 +143,35 @@
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
         )
         (l_2): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -205,36 +179,35 @@
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
         )
         (l_3): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -247,377 +220,311 @@
         )
       )
       (head): Sequential(
         (pool): AdaptiveAvgPool2d(output_size=1)
         (flat): Flatten(start_dim=1, end_dim=-1)
         (fc): Linear(in_features=512, out_features=1000, bias=True)
       )
-    )<pre>
+    )</pre>
 </details>
 
 
 
 If you want to change model, just change constructor parameters.  
-Lets create xresnet50.
+Lets create resnet50.
 
 
 ```python
 mc.expansion = 4
 mc.layers = [3,4,6,3]
 ```
 
+We can check, what we changed (compare to default constructor).
+
+
+```python
+mc.changed_fields
+```
+<details open> <summary>output</summary>  
+    <pre>{'layers': [3, 4, 6, 3], 'expansion': 4}</pre>
+</details>
+
+
+
+
+```python
+mc.print_changed_fields()
+```
+<details open> <summary>output</summary>  
+    <pre>Changed fields:
+    layers: [3, 4, 6, 3]
+    expansion: 4
+    </pre>
+</details>
+
 Now we can look at model parts - stem, body, head.  
 
 
 ```python
 
 mc.body
 ```
 <details> <summary>output</summary>  
-    <pre>Sequential(
+    </pre>Sequential(
       (l_0): Sequential(
-        (bl_0): ResBlock(
+        (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(64, 64, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-            )
-          )
-          (id_conv): Sequential(
-            (id_conv): ConvBnAct(
-              (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_1): ResBlock(
+        (bl_1): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(256, 64, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_2): ResBlock(
+        (bl_2): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(256, 64, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
       )
       (l_1): Sequential(
-        (bl_0): ResBlock(
+        (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(256, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
-              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
+              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(128, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (id_conv): Sequential(
-            (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
             (id_conv): ConvBnAct(
-              (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
+              (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(2, 2), bias=False)
+              (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_1): ResBlock(
+        (bl_1): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(512, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(128, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_2): ResBlock(
+        (bl_2): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(512, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(128, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_3): ResBlock(
+        (bl_3): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(512, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(128, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
       )
       (l_2): Sequential(
-        (bl_0): ResBlock(
+        (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(512, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
-              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (id_conv): Sequential(
-            (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
             (id_conv): ConvBnAct(
-              (conv): Conv2d(512, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
+              (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(2, 2), bias=False)
+              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_1): ResBlock(
+        (bl_1): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_2): ResBlock(
+        (bl_2): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_3): ResBlock(
+        (bl_3): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_4): ResBlock(
+        (bl_4): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_5): ResBlock(
+        (bl_5): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
       )
       (l_3): Sequential(
-        (bl_0): ResBlock(
+        (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
-              (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
+              (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(512, 2048, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(2048, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (id_conv): Sequential(
-            (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
             (id_conv): ConvBnAct(
-              (conv): Conv2d(1024, 2048, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(2048, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
+              (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(2, 2), bias=False)
+              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_1): ResBlock(
+        (bl_1): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(2048, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(512, 2048, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(2048, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_2): ResBlock(
+        (bl_2): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(2048, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(512, 2048, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(2048, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
       )
-    )<pre>
+    )</pre>
 </details>
 
 
 
 ## Create constructor from config.
 
 Alternative we can create config first and than create constructor from it. 
@@ -625,37 +532,60 @@
 
 ```python
 from model_constructor import ModelCfg
 ```
 
 
 ```python
-cfg = ModelCfg()
+cfg = ModelCfg(
+    num_classes=10,
+    act_fn=nn.Mish,
+)
 print(cfg)
 ```
 <details open> <summary>output</summary>  
-    <pre>in_chans=3 num_classes=1000 block='ResBlock' conv_layer='ConvBnAct' block_sizes=[64, 128, 256, 512] layers=[2, 2, 2, 2] norm='BatchNorm2d' act_fn='ReLU' pool="AvgPool2d {'kernel_size': 2, 'ceil_mode': True}" expansion=1 groups=1 bn_1st=True zero_bn=True stem_sizes=[32, 32, 64] stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}" init_cnn='init_cnn' make_stem='make_stem' make_layer='make_layer' make_body='make_body' make_head='make_head'
-    <pre>
+    <pre>in_chans=3 num_classes=10 block='BasicBlock' conv_layer='ConvBnAct' block_sizes=[64, 128, 256, 512] layers=[2, 2, 2, 2] norm='BatchNorm2d' act_fn='Mish' expansion=1 groups=1 bn_1st=True zero_bn=True stem_sizes=[64] stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+    </pre>
+</details>
+
+When creating config or constructor we can use string annotation for nn.Modules - it useful when creating model from config files.
+
+
+```python
+cfg = ModelCfg(
+    num_classes=10,
+    act_fn="nn.SELU",
+)
+print(cfg.act_fn)
+```
+<details open> <summary>output</summary>  
+    <pre>class 'torch.nn.modules.activation.SELU'
+    </pre>
 </details>
 
 Now we can create constructor from config:
 
 
 ```python
 mc = ModelConstructor.from_cfg(cfg)
 mc
 ```
 <details open> <summary>output</summary>  
+    <pre>Deprecated. Pass se_module as se argument, se_reduction as arg to se.
+    Deprecated. Pass se_module as se argument, se_reduction as arg to se.
+    </pre>
+</details>
+<details open> <summary>output</summary>  
     <pre>ModelConstructor
-      in_chans: 3, num_classes: 1000
+      in_chans: 3, num_classes: 10
       expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: False, se: False
-      stem sizes: [32, 32, 64], stride on 0
+      act_fn: ReLU, sa: <class 'model_constructor.layers.SimpleSelfAttention'>, se: SEModule
+      stem sizes: [64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]<pre>
+      layers: [2, 2, 2, 2]</pre>
 </details>
 
 
 
 ## More modification.
 
 Main purpose of this module - fast and easy modify model.
@@ -671,24 +601,29 @@
 mc = ModelConstructor(name='MxResNet')
 ```
 
 Then lets modify stem.
 
 
 ```python
+from model_constructor.xresnet import xresnet_stem
+```
+
+
+```python
+mc.make_stem = xresnet_stem
 mc.stem_sizes = [3,32,64,64]
 ```
 
 Now lets change activation function to Mish.
 Here is link to [forum discussion](https://forums.fast.ai/t/meet-mish-new-activation-function-possible-successor-to-relu)    
 We'v got Mish is in model_constructor.activations, but from pytorch 1.9 take it from torch:
 
 
 ```python
-# from model_constructor.activations import Mish
 from torch.nn import Mish
 ```
 
 
 ```python
 mc.act_fn = Mish
 ```
@@ -700,29 +635,42 @@
 <details open> <summary>output</summary>  
     <pre>MxResNet
       in_chans: 3, num_classes: 1000
       expansion: 1, groups: 1, dw: False, div_groups: None
       act_fn: Mish, sa: False, se: False
       stem sizes: [3, 32, 64, 64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]<pre>
+      layers: [2, 2, 2, 2]</pre>
 </details>
 
 
 
+
+```python
+mc.print_changed_fields()
+```
+<details open> <summary>output</summary>  
+    <pre>Changed fields:
+    name: MxResNet
+    act_fn: Mish
+    stem_sizes: [3, 32, 64, 64]
+    make_stem: xresnet_stem
+    </pre>
+</details>
+
 Here is model:  
 
 
 ```python
 
 mc()
 ```
 <details> <summary>output</summary>  
-    <pre>MxResNet(
-      stem_sizes: [3, 32, 64, 64], act_fn: Mish
+    </pre>MxResNet(
+      act_fn: Mish, stem_sizes: [3, 32, 64, 64], make_stem: xresnet_stem
       (stem): Sequential(
         (conv_0): ConvBnAct(
           (conv): Conv2d(3, 3, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(3, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
         (conv_1): ConvBnAct(
@@ -740,29 +688,29 @@
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
         (stem_pool): MaxPool2d(kernel_size=3, stride=2, padding=1, dilation=1, ceil_mode=False)
       )
       (body): Sequential(
         (l_0): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -770,36 +718,35 @@
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
         )
         (l_1): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -807,36 +754,35 @@
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
         )
         (l_2): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -844,36 +790,35 @@
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
         )
         (l_3): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -886,30 +831,45 @@
         )
       )
       (head): Sequential(
         (pool): AdaptiveAvgPool2d(output_size=1)
         (flat): Flatten(start_dim=1, end_dim=-1)
         (fc): Linear(in_features=512, out_features=1000, bias=True)
       )
-    )<pre>
+    )</pre>
 </details>
 
 
 
 ## MXResNet50
 
 Now lets make MxResNet50
 
 
 ```python
 mc.expansion = 4
 mc.layers = [3,4,6,3]
-mc.name = 'mxresnet50'
+mc.name = "mxresnet50"
 ```
 
+
+```python
+mc.print_changed_fields()
+```
+<details open> <summary>output</summary>  
+    <pre>Changed fields:
+    name: mxresnet50
+    layers: [3, 4, 6, 3]
+    act_fn: Mish
+    expansion: 4
+    stem_sizes: [3, 32, 64, 64]
+    make_stem: xresnet_stem
+    </pre>
+</details>
+
 Now we have mxresnet50 constructor.  
 We can inspect every parts of it.  
 And after call it we got model.
 
 
 ```python
 mc
@@ -917,152 +877,141 @@
 <details open> <summary>output</summary>  
     <pre>mxresnet50
       in_chans: 3, num_classes: 1000
       expansion: 4, groups: 1, dw: False, div_groups: None
       act_fn: Mish, sa: False, se: False
       stem sizes: [3, 32, 64, 64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [3, 4, 6, 3]<pre>
+      layers: [3, 4, 6, 3]</pre>
 </details>
 
 
 
 
 ```python
 
 mc.stem.conv_1
 ```
 <details> <summary>output</summary>  
-    <pre>ConvBnAct(
+    </pre>ConvBnAct(
       (conv): Conv2d(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
       (bn): BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
       (act_fn): Mish(inplace=True)
-    )<pre>
+    )</pre>
 </details>
 
 
 
 
 ```python
 
 mc.body.l_0.bl_0
 ```
 <details> <summary>output</summary>  
-    <pre>ResBlock(
+    </pre>BasicBlock(
       (convs): Sequential(
         (conv_0): ConvBnAct(
-          (conv): Conv2d(64, 64, kernel_size=(1, 1), stride=(1, 1), bias=False)
+          (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
         (conv_1): ConvBnAct(
           (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-          (act_fn): Mish(inplace=True)
-        )
-        (conv_2): ConvBnAct(
-          (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-          (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-        )
-      )
-      (id_conv): Sequential(
-        (id_conv): ConvBnAct(
-          (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-          (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
         )
       )
       (act_fn): Mish(inplace=True)
-    )<pre>
+    )</pre>
 </details>
 
 
 
 We can get model direct way:
 
 
 ```python
-mc = ModelConstructor(name="MxResNet", act_fn=Mish, layers=[3,4,6,3], expansion=4, stem_sizes=[32,64,64])
+mc = ModelConstructor(
+    name="MxResNet",
+    act_fn=Mish,
+    layers=[3,4,6,3],
+    expansion=4,
+    make_stem=xresnet_stem,
+    stem_sizes=[32,64,64]
+)
 model = mc()
 ```
 
-Or create with config:
+Another way:
 
 
 ```python
-mc = ModelConstructor.from_cfg(
-    ModelCfg(name="MxResNet", act_fn=Mish, layers=[3,4,6,3], expansion=4, stem_sizes=[32,64,64])
+model = ModelConstructor.create_model(
+    name="MxResNet",
+    act_fn=Mish,
+    layers=[3,4,6,3],
+    expansion=4,
+    make_stem=xresnet_stem,
+    stem_sizes=[32,64,64]
 )
-model = mc()
 ```
 
 ## YaResNet
 
 Now lets change Resblock to YaResBlock (Yet another ResNet, former NewResBlock) is in lib from version 0.1.0
 
 
 ```python
-from model_constructor.yaresnet import YaResBlock
+from model_constructor.yaresnet import YaBasicBlock
 ```
 
 
 ```python
 mc = ModelConstructor(name="YaResNet")
-mc.block = YaResBlock
+mc.block = YaBasicBlock
 ```
 
 Or in one line:
 
 
 ```python
-mc = ModelConstructor(name="YaResNet", block=YaResBlock)
+mc = ModelConstructor(name="YaResNet", block=YaBasicBlock)
 ```
 
 That all. Now we have YaResNet constructor
 
 
 ```python
 
 mc.print_cfg()
 ```
 <details> <summary>output</summary>  
-    <pre>ModelConstructor(
-      name='YaResNet'
-      in_chans=3
-      num_classes=1000
-      block='YaResBlock'
-      conv_layer='ConvBnAct'
-      block_sizes=[64, 128, 256, 512]
-      layers=[2, 2, 2, 2]
-      norm='BatchNorm2d'
-      act_fn='ReLU'
-      pool="AvgPool2d {'kernel_size': 2, 'ceil_mode': True}"
-      expansion=1
-      groups=1
-      bn_1st=True
-      zero_bn=True
-      stem_sizes=[32, 32, 64]
-      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
-      init_cnn='init_cnn'
-      make_stem='make_stem'
-      make_layer='make_layer'
-      make_body='make_body'
-      make_head='make_head')
-    <pre>
+    </pre>YaResNet
+      in_chans: 3, num_classes: 1000
+      expansion: 1, groups: 1, dw: False, div_groups: None
+      act_fn: ReLU, sa: False, se: False
+      stem sizes: [64], stride on 0
+      body sizes [64, 128, 256, 512]
+      layers: [2, 2, 2, 2]
+    </pre>
 </details>
 
 Let see what we have.
 
 
 ```python
 
 mc.body.l_1.bl_0
 ```
 <details> <summary>output</summary>  
-    <pre>YaResBlock(
-      (reduce): AvgPool2d(kernel_size=2, stride=2, padding=0)
+    </pre>YaBasicBlock(
+      (reduce): ConvBnAct(
+        (conv): Conv2d(64, 64, kernel_size=(1, 1), stride=(2, 2), bias=False)
+        (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
+        (act_fn): ReLU(inplace=True)
+      )
       (convs): Sequential(
         (conv_0): ConvBnAct(
           (conv): Conv2d(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): ReLU(inplace=True)
         )
         (conv_1): ConvBnAct(
@@ -1071,75 +1020,67 @@
         )
       )
       (id_conv): ConvBnAct(
         (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
         (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
       )
       (merge): ReLU(inplace=True)
-    )<pre>
+    )</pre>
 </details>
 
 
 
-Lets create `Resnet34` like model constructor:
+Lets create `xResnet34` like model constructor:
 
 
 ```python
+from typing import Callable
+
+from model_constructor.helpers import ModSeq
+
+
 class YaResnet34(ModelConstructor):
-    block: type[nn.Module] = YaResBlock
+    block: type[nn.Module] = YaBasicBlock
     layers: list[int] = [3, 4, 6, 3]
+    make_stem: Callable[[ModelCfg], ModSeq] = xresnet_stem
 ```
 
 
 ```python
 mc = YaResnet34()
 mc.print_cfg()
 ```
 <details open> <summary>output</summary>  
-    <pre>YaResnet34(
-      in_chans=3
-      num_classes=1000
-      block='YaResBlock'
-      conv_layer='ConvBnAct'
-      block_sizes=[64, 128, 256, 512]
-      layers=[3, 4, 6, 3]
-      norm='BatchNorm2d'
-      act_fn='ReLU'
-      pool="AvgPool2d {'kernel_size': 2, 'ceil_mode': True}"
-      expansion=1
-      groups=1
-      bn_1st=True
-      zero_bn=True
-      stem_sizes=[32, 32, 64]
-      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
-      init_cnn='init_cnn'
-      make_stem='make_stem'
-      make_layer='make_layer'
-      make_body='make_body'
-      make_head='make_head')
-    <pre>
+    <pre>YaResnet34
+      in_chans: 3, num_classes: 1000
+      expansion: 1, groups: 1, dw: False, div_groups: None
+      act_fn: ReLU, sa: False, se: False
+      stem sizes: [64], stride on 0
+      body sizes [64, 128, 256, 512]
+      layers: [3, 4, 6, 3]
+    </pre>
 </details>
 
-And `Resnet50` like model can be inherited from `YaResnet34`:
+And `xResnet50` like model can be inherited from `YaResnet34`:
 
 
 ```python
 class YaResnet50(YaResnet34):
-    expansion = 4
+    expansion: int = 4
 ```
 
 
 ```python
 mc = YaResnet50()
 mc
 ```
 <details open> <summary>output</summary>  
     <pre>YaResnet50
       in_chans: 3, num_classes: 1000
       expansion: 4, groups: 1, dw: False, div_groups: None
       act_fn: ReLU, sa: False, se: False
-      stem sizes: [32, 32, 64], stride on 0
+      stem sizes: [64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [3, 4, 6, 3]<pre>
+      layers: [3, 4, 6, 3]</pre>
 </details>
```

### Comparing `model_constructor-0.3.2/settings.ini` & `model_constructor-0.4/settings.ini`

 * *Files identical despite different names*

### Comparing `model_constructor-0.3.2/setup.cfg` & `model_constructor-0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `model_constructor-0.3.2/setup.py` & `model_constructor-0.4/setup.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.3.2/src/model_constructor/activations.py` & `model_constructor-0.4/src/model_constructor/activations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 # forked from https://github.com/rwightman/pytorch-image-models/timm/models/layers/activations.py
 import torch
 from torch import nn as nn
 from torch.nn import functional as F
 from torch.nn import Mish
 
 
-__all__ = ['mish', 'Mish', 'mish_jit', 'MishJit', 'mish_jit_fwd', 'mish_jit_bwd', 'MishJitAutoFn', 'mish_me', 'MishMe',
-           'hard_mish_jit', 'HardMishJit', 'hard_mish_jit_fwd', 'hard_mish_jit_bwd', 'HardMishJitAutoFn',
-           'hard_mish_me', 'HardMishMe']
+__all__ = [
+    "mish",
+    "Mish",
+    "mish_jit",
+    "MishJit",
+    "mish_jit_fwd",
+    "mish_jit_bwd",
+    "MishJitAutoFn",
+    "mish_me",
+    "MishMe",
+    "hard_mish_jit",
+    "HardMishJit",
+    "hard_mish_jit_fwd",
+    "hard_mish_jit_bwd",
+    "HardMishJitAutoFn",
+    "hard_mish_me",
+    "HardMishMe",
+]
 
 
 def mish(x, inplace: bool = False):
     """Mish: A Self Regularized Non-Monotonic Neural Activation Function - https://arxiv.org/abs/1908.08681
     NOTE: I don't have a working inplace variant
     """
     return x.mul(F.softplus(x).tanh())
@@ -36,15 +51,16 @@
     """
     return x.mul(F.softplus(x).tanh())
 
 
 class MishJit(nn.Module):
     def __init__(self, inplace: bool = False):
         """Jit version of Mish.
-        Mish: A Self Regularized Non-Monotonic Neural Activation Function - https://arxiv.org/abs/1908.08681"""
+        Mish: A Self Regularized Non-Monotonic Neural Activation Function - https://arxiv.org/abs/1908.08681
+        """
         super(MishJit, self).__init__()
 
     def forward(self, x):
         return mish_jit(x)
 
 
 @torch.jit.script
@@ -57,16 +73,17 @@
 def mish_jit_bwd(x, grad_output):
     x_sigmoid = torch.sigmoid(x)
     x_tanh_sp = F.softplus(x).tanh()
     return grad_output.mul(x_tanh_sp + x * x_sigmoid * (1 - x_tanh_sp * x_tanh_sp))
 
 
 class MishJitAutoFn(torch.autograd.Function):
-    """ Mish: A Self Regularized Non-Monotonic Neural Activation Function - https://arxiv.org/abs/1908.08681
+    """Mish: A Self Regularized Non-Monotonic Neural Activation Function - https://arxiv.org/abs/1908.08681
     A memory efficient, jit scripted variant of Mish"""
+
     @staticmethod
     def forward(ctx, x):
         ctx.save_for_backward(x)
         return mish_jit_fwd(x)
 
     @staticmethod
     def backward(ctx, grad_output):
@@ -75,61 +92,64 @@
 
 
 def mish_me(x, inplace=False):
     return MishJitAutoFn.apply(x)
 
 
 class MishMe(nn.Module):
-    """ Mish: A Self Regularized Non-Monotonic Neural Activation Function - https://arxiv.org/abs/1908.08681
+    """Mish: A Self Regularized Non-Monotonic Neural Activation Function - https://arxiv.org/abs/1908.08681
     A memory efficient, jit scripted variant of Mish"""
+
     def __init__(self, inplace: bool = False):
         super(MishMe, self).__init__()
 
     def forward(self, x):
         return MishJitAutoFn.apply(x)
 
 
 @torch.jit.script
 def hard_mish_jit(x, inplace: bool = False):
-    """ Hard Mish
+    """Hard Mish
     Experimental, based on notes by Mish author Diganta Misra at
       https://github.com/digantamisra98/H-Mish/blob/0da20d4bc58e696b6803f2523c58d3c8a82782d0/README.md
     """
     return 0.5 * x * (x + 2).clamp(min=0, max=2)
 
 
 class HardMishJit(nn.Module):
-    """ Hard Mish
+    """Hard Mish
     Experimental, based on notes by Mish author Diganta Misra at
       https://github.com/digantamisra98/H-Mish/blob/0da20d4bc58e696b6803f2523c58d3c8a82782d0/README.md
     """
+
     def __init__(self, inplace: bool = False):
         super(HardMishJit, self).__init__()
 
     def forward(self, x):
         return hard_mish_jit(x)
 
 
 @torch.jit.script
 def hard_mish_jit_fwd(x):
     return 0.5 * x * (x + 2).clamp(min=0, max=2)
 
 
 @torch.jit.script
 def hard_mish_jit_bwd(x, grad_output):
-    m = torch.ones_like(x) * (x >= -2.)
-    m = torch.where((x >= -2.) & (x <= 0.), x + 1., m)
+    m = torch.ones_like(x) * (x >= -2.0)
+    m = torch.where((x >= -2.0) & (x <= 0.0), x + 1.0, m)
     return grad_output * m
 
 
 class HardMishJitAutoFn(torch.autograd.Function):
-    """ A memory efficient, jit scripted variant of Hard Mish
+    """A memory efficient, jit scripted variant of Hard Mish
     Experimental, based on notes by Mish author Diganta Misra at
       https://github.com/digantamisra98/H-Mish/blob/0da20d4bc58e696b6803f2523c58d3c8a82782d0/README.md
     """
+
     @staticmethod
     def forward(ctx, x):
         ctx.save_for_backward(x)
         return hard_mish_jit_fwd(x)
 
     @staticmethod
     def backward(ctx, grad_output):
@@ -138,16 +158,17 @@
 
 
 def hard_mish_me(x, inplace: bool = False):
     return HardMishJitAutoFn.apply(x)
 
 
 class HardMishMe(nn.Module):
-    """ A memory efficient, jit scripted variant of Hard Mish
+    """A memory efficient, jit scripted variant of Hard Mish
     Experimental, based on notes by Mish author Diganta Misra at
       https://github.com/digantamisra98/H-Mish/blob/0da20d4bc58e696b6803f2523c58d3c8a82782d0/README.md
     """
+
     def __init__(self, inplace: bool = False):
         super(HardMishMe, self).__init__()
 
     def forward(self, x):
         return HardMishJitAutoFn.apply(x)
```

### Comparing `model_constructor-0.3.2/src/model_constructor/convmixer.py` & `model_constructor-0.4/src/model_constructor/convmixer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,175 @@
 # Implementation of ConvMixer for the ICLR 2022 submission "Patches Are All You Need?".
 # https://openreview.net/forum?id=TVHS5Y4dNvM
 # Adopted from https://github.com/tmp-iclr/convmixer
 # Home for convmixer: https://github.com/locuslab/convmixer
 from collections import OrderedDict
-from typing import Callable
+from typing import Callable, Optional, Tuple, Union
+
+import torch
 import torch.nn as nn
 
+from .helpers import ListStrMod
+
 
 class Residual(nn.Module):
-    def __init__(self, fn):
+    def __init__(self, fn: Callable[[torch.Tensor], torch.Tensor]):
         super().__init__()
         self.fn = fn
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         return self.fn(x) + x
 
 
 # As original version, act_fn as argument.
-def ConvMixerOriginal(dim, depth,
-                      kernel_size=9, patch_size=7, n_classes=1000,
-                      act_fn=nn.GELU()):
+def ConvMixerOriginal(
+    dim: int,
+    depth: int,
+    kernel_size: int = 9,
+    patch_size: int = 7,
+    n_classes: int = 1000,
+    act_fn: nn.Module = nn.GELU(),
+):
     return nn.Sequential(
         nn.Conv2d(3, dim, kernel_size=patch_size, stride=patch_size),
         act_fn,
         nn.BatchNorm2d(dim),
-        *[nn.Sequential(
-            Residual(nn.Sequential(
-                nn.Conv2d(dim, dim, kernel_size, groups=dim, padding="same"),
+        *[
+            nn.Sequential(
+                Residual(
+                    nn.Sequential(
+                        nn.Conv2d(dim, dim, kernel_size, groups=dim, padding="same"),
+                        act_fn,
+                        nn.BatchNorm2d(dim),
+                    )
+                ),
+                nn.Conv2d(dim, dim, kernel_size=1),
                 act_fn,
-                nn.BatchNorm2d(dim)
-            )),
-            nn.Conv2d(dim, dim, kernel_size=1),
-            act_fn,
-            nn.BatchNorm2d(dim)
-        ) for i in range(depth)],
+                nn.BatchNorm2d(dim),
+            )
+            for _i in range(depth)
+        ],
         nn.AdaptiveAvgPool2d((1, 1)),
         nn.Flatten(),
         nn.Linear(dim, n_classes)
     )
 
 
 class ConvLayer(nn.Sequential):
     """Basic conv layers block"""
 
-    def __init__(self, in_channels, out_channels, kernel_size, stride=1,
-                 act_fn=nn.GELU(), padding=0, groups=1,
-                 bn_1st=False, pre_act=False):
-
-        conv_layer = [('conv', nn.Conv2d(in_channels, out_channels, kernel_size, stride=stride,
-                                         padding=padding, groups=groups))]
-        act_bn = [
-            ('act_fn', act_fn),
-            ('bn', nn.BatchNorm2d(out_channels))
+    def __init__(
+        self,
+        in_channels: int,
+        out_channels: int,
+        kernel_size: Union[int, Tuple[int, int]],
+        stride: int = 1,
+        act_fn: nn.Module = nn.GELU(),
+        padding: Union[int, str] = 0,
+        groups: int = 1,
+        bn_1st: bool = False,
+        pre_act: bool = False,
+    ):
+        conv_layer: ListStrMod = [
+            (
+                "conv",
+                nn.Conv2d(
+                    in_channels,
+                    out_channels,
+                    kernel_size,
+                    stride=stride,
+                    padding=padding,
+                    groups=groups,
+                ),
+            )
+        ]
+        act_bn: ListStrMod = [
+            ("act_fn", act_fn),
+            ("bn", nn.BatchNorm2d(out_channels)),
         ]
         if bn_1st:
             act_bn.reverse()
         if pre_act:
             act_bn.insert(1, conv_layer[0])
             layers = act_bn
         else:
             layers = conv_layer + act_bn
         super().__init__(OrderedDict(layers))
 
 
 class ConvMixer(nn.Sequential):
-
-    def __init__(self, dim: int, depth: int,
-                 kernel_size: int = 9, patch_size: int = 7, n_classes: int = 1000,
-                 act_fn: nn.Module = nn.GELU(),
-                 stem: nn.Module = None,
-                 bn_1st: bool = False, pre_act: bool = False,
-                 init_func: Callable = None):
+    def __init__(
+        self,
+        dim: int,
+        depth: int,
+        kernel_size: int = 9,
+        patch_size: int = 7,
+        n_classes: int = 1000,
+        act_fn: nn.Module = nn.GELU(),
+        stem: Optional[nn.Module] = None,
+        in_chans: int = 3,
+        bn_1st: bool = False,
+        pre_act: bool = False,
+        init_func: Optional[Callable[[nn.Module], None]] = None,
+    ):
         """ConvMixer constructor.
         Adopted from https://github.com/tmp-iclr/convmixer
 
         Args:
-            dim (int): Dimention of model.
+            dim (int): Dimension of model.
             depth (int): Depth of model.
             kernel_size (int, optional): Kernel size. Defaults to 9.
             patch_size (int, optional): Patch size. Defaults to 7.
             n_classes (int, optional): Number of classes. Defaults to 1000.
             act_fn (nn.Module, optional): Activation function. Defaults to nn.GELU().
             stem (nn.Module, optional): You can path different first layer..
-            stem_ks (int, optional): If stem_ch not 0 - kernel size for adittional layer. Defaults to 1.
-            bn_1st (bool, optional): If True - BatchNorm befor activation function. Defaults to False.
-            pre_act (bool, optional): If True - activatin function befor convolution layer. Defaults to False.
+            stem_ks (int, optional): If stem_ch not 0 - kernel size for additional layer. Defaults to 1.
+            bn_1st (bool, optional): If True - BatchNorm before activation function. Defaults to False.
+            pre_act (bool, optional): If True - activation function before convolution layer. Defaults to False.
             init_func (Callable, optional): External function for init model.
 
         """
         if pre_act:
             bn_1st = False
         if stem is None:
-            stem = ConvLayer(3, dim, kernel_size=patch_size, stride=patch_size, act_fn=act_fn, bn_1st=bn_1st)
+            stem = ConvLayer(
+                in_chans,
+                dim,
+                kernel_size=patch_size,
+                stride=patch_size,
+                act_fn=act_fn,
+                bn_1st=bn_1st,
+            )
 
         super().__init__(
             stem,
-            *[nn.Sequential(
-                Residual(
-                    ConvLayer(dim, dim, kernel_size, act_fn=act_fn,
-                              groups=dim, padding="same", bn_1st=bn_1st, pre_act=pre_act)),
-                ConvLayer(dim, dim, kernel_size=1, act_fn=act_fn, bn_1st=bn_1st, pre_act=pre_act))
-              for i in range(depth)],
+            *[
+                nn.Sequential(
+                    Residual(
+                        ConvLayer(
+                            dim,
+                            dim,
+                            kernel_size,
+                            act_fn=act_fn,
+                            groups=dim,
+                            padding="same",
+                            bn_1st=bn_1st,
+                            pre_act=pre_act,
+                        )
+                    ),
+                    ConvLayer(
+                        dim,
+                        dim,
+                        kernel_size=1,
+                        act_fn=act_fn,
+                        bn_1st=bn_1st,
+                        pre_act=pre_act,
+                    ),
+                )
+                for _ in range(depth)
+            ],
             nn.AdaptiveAvgPool2d((1, 1)),
             nn.Flatten(),
-            nn.Linear(dim, n_classes))
+            nn.Linear(dim, n_classes)
+        )
         if init_func is not None:  # pragma: no cover
             init_func(self)
```

### Comparing `model_constructor-0.3.2/src/model_constructor/layers.py` & `model_constructor-0.4/src/model_constructor/layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from collections import OrderedDict
-from typing import List, Optional, Type, Union
+from typing import Optional, Type, Union
 
 import torch
-import torch.nn as nn
+from torch import nn
 from torch.nn.utils.spectral_norm import spectral_norm
 
+from .helpers import ListStrMod
+
 __all__ = [
     "Flatten",
     "noop",
     "Noop",
     "ConvLayer",
     "act",
     "conv1d",
@@ -17,27 +19,27 @@
     "SEBlockConv",
 ]
 
 
 class Flatten(nn.Module):
     """flat x to vector"""
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         return x.view(x.size(0), -1)
 
 
-def noop(x):
+def noop(x: torch.Tensor) -> torch.Tensor:
     """Dummy func. Return input"""
     return x
 
 
 class Noop(nn.Module):
     """Dummy module"""
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         return x
 
 
 act = nn.ReLU(inplace=True)
 
 
 def get_act(act_fn: Type[nn.Module], inplace: bool = True) -> nn.Module:
@@ -66,18 +68,17 @@
         groups: int = 1,
         act_fn: Union[Type[nn.Module], bool] = nn.ReLU,
         pre_act: bool = False,
         bn_layer: bool = True,
         bn_1st: bool = True,
         zero_bn: bool = False,
     ):
-
         if padding is None:
             padding = kernel_size // 2
-        layers: List[tuple[str, nn.Module]] = [
+        layers: ListStrMod = [
             (
                 "conv",
                 self.convolution_module(
                     in_channels,
                     out_channels,
                     kernel_size,
                     stride=stride,
@@ -110,25 +111,24 @@
 
     def __init__(
         self,
         ni,
         nf,
         ks=3,
         stride=1,
-        act=True,
+        act=True,  # pylint: disable=redefined-outer-name
         act_fn=act,
         bn_layer=True,
         bn_1st=True,
         zero_bn=False,
         padding=None,
         bias=False,
         groups=1,
-        **kwargs
+        **kwargs  # pylint: disable=unused-argument
     ):
-
         if padding is None:
             padding = ks // 2
         layers = [
             (
                 "conv",
                 self.Conv2d(
                     ni, nf, ks, stride=stride, padding=padding, bias=bias, groups=groups
@@ -172,15 +172,15 @@
     def __init__(self, n_in: int, ks=1, sym=False, use_bias=False):
         super().__init__()
         self.conv = conv1d(n_in, n_in, ks, padding=ks // 2, bias=use_bias)
         self.gamma = torch.nn.Parameter(torch.tensor([0.0]))  # type: ignore
         self.sym = sym
         self.n_in = n_in
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         if self.sym:  # check ks=3
             # symmetry hack by https://github.com/mgrankin
             c = self.conv.weight.view(self.n_in, self.n_in)
             c = (c + c.t()) / 2
             self.conv.weight = c.view(self.n_in, self.n_in, 1)
         size = x.size()
         x = x.view(*size[:2], -1)  # (C,N)
@@ -191,44 +191,48 @@
             x, x.permute(0, 2, 1).contiguous()
         )  # (C,N) * (N,C) = (C,C)   => O(NC^2)
         o = torch.bmm(xxT, convx)  # (C,C) * (C,N) = (C,N)   => O(NC^2)
         o = self.gamma * o + x
         return o.view(*size).contiguous()
 
 
-class SEBlock(nn.Module):  # todo: deprecation warning.
-    "se block"
+class SEBlock(nn.Module):
+    """se block"""
+
+    # first version
     se_layer = nn.Linear
     act_fn = nn.ReLU(inplace=True)
     use_bias = True
 
-    def __init__(self, c, r=16):
+    def __init__(self, c: int, r: int = 16):
         super().__init__()
         ch = max(c // r, 1)
         self.squeeze = nn.AdaptiveAvgPool2d(1)
         self.excitation = nn.Sequential(
             OrderedDict(
                 [
                     ("fc_reduce", self.se_layer(c, ch, bias=self.use_bias)),
                     ("se_act", self.act_fn),
                     ("fc_expand", self.se_layer(ch, c, bias=self.use_bias)),
                     ("sigmoid", nn.Sigmoid()),
                 ]
             )
         )
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         bs, c, _, _ = x.shape
         y = self.squeeze(x).view(bs, c)
         y = self.excitation(y).view(bs, c, 1, 1)
         return x * y.expand_as(x)
 
 
-class SEBlockConv(nn.Module):  # todo: deprecation warning.
-    "se block with conv on excitation"
+class SEBlockConv(nn.Module):
+    """se block with conv on excitation"""
+
+    # first version
     se_layer = nn.Conv2d
     act_fn = nn.ReLU(inplace=True)
     use_bias = True
 
     def __init__(self, c, r=16):
         super().__init__()
         #         c_in = math.ceil(c//r/8)*8
@@ -252,22 +256,22 @@
 
 
 class SEModule(nn.Module):
     "se block"
 
     def __init__(
         self,
-        channels,
-        reduction=16,
-        rd_channels=None,
-        rd_max=False,
-        se_layer=nn.Linear,
-        act_fn=nn.ReLU(inplace=True),
-        use_bias=True,
-        gate=nn.Sigmoid,
+        channels: int,
+        reduction: int = 16,
+        rd_channels: Optional[int] = None,
+        rd_max: bool = False,
+        se_layer: Type[nn.Module] = nn.Linear,
+        act_fn: nn.Module = nn.ReLU(inplace=True),
+        use_bias: bool = True,
+        gate: Type[nn.Module] = nn.Sigmoid,
     ):
         super().__init__()
         reducted = max(channels // reduction, 1)  # preserve zero-element tensors
         if rd_channels is None:
             rd_channels = reducted
         else:
             if rd_max:
@@ -280,34 +284,34 @@
                     ("se_act", act_fn),
                     ("expand", se_layer(rd_channels, channels, bias=use_bias)),
                     ("se_gate", gate()),
                 ]
             )
         )
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         bs, c, _, _ = x.shape
         y = self.squeeze(x).view(bs, c)
         y = self.excitation(y).view(bs, c, 1, 1)
         return x * y.expand_as(x)
 
 
 class SEModuleConv(nn.Module):
     "se block with conv on excitation"
 
     def __init__(
         self,
-        channels,
-        reduction=16,
-        rd_channels=None,
-        rd_max=False,
-        se_layer=nn.Conv2d,
-        act_fn=nn.ReLU(inplace=True),
-        use_bias=True,
-        gate=nn.Sigmoid,
+        channels: int,
+        reduction: int = 16,
+        rd_channels: Optional[int] = None,
+        rd_max: bool = False,
+        se_layer: Type[nn.Module] = nn.Conv2d,
+        act_fn: nn.Module = nn.ReLU(inplace=True),
+        use_bias: bool = True,
+        gate: Type[nn.Module] = nn.Sigmoid,
     ):
         super().__init__()
         #       rd_channels = math.ceil(channels//reduction/8)*8
         reducted = max(channels // reduction, 1)  # preserve zero-element tensors
         if rd_channels is None:
             rd_channels = reducted
         else:
@@ -321,11 +325,11 @@
                     ("se_act", act_fn),
                     ("expand", se_layer(rd_channels, channels, 1, bias=use_bias)),
                     ("gate", gate()),
                 ]
             )
         )
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         y = self.squeeze(x)
         y = self.excitation(y)
         return x * y.expand_as(x)
```

### Comparing `model_constructor-0.3.2/src/model_constructor/net.py` & `model_constructor-0.4/src/model_constructor/net.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,26 @@
 from functools import partial
 
 import torch.nn as nn
 
 from .layers import ConvLayer, Flatten, SEBlock, SimpleSelfAttention, noop
 
 
-__all__ = ['init_cnn', 'act_fn', 'ResBlock', 'NewResBlock', 'Net', 'xresnet34', 'xresnet50']
+__all__ = [
+    "init_cnn",
+    "act_fn",
+    "ResBlock",
+    "NewResBlock",
+    "Net",
+    "xresnet34",
+    "xresnet50",
+    "mxresnet_parameters",
+    "mxresnet34",
+    "mxresnet50",
+]
 
 
 act_fn = nn.ReLU(inplace=True)
 
 
 def init_cnn(module: nn.Module):
     "Init module - kaiming_normal for Conv2d and 0 for biases."
@@ -205,7 +216,15 @@
                 f"  stem sizes: {self.stem_sizes}, stride on {self.stem_stride_on}\n"
                 f"  body sizes {self._block_sizes}\n"
                 f"  layers: {self.layers}")
 
 
 xresnet34 = partial(Net, name='xresnet34', expansion=1, layers=[3, 4, 6, 3])
 xresnet50 = partial(Net, name='xresnet34', expansion=4, layers=[3, 4, 6, 3])
+
+mxresnet_parameters = {"stem_sizes": [3, 32, 64, 64], "act_fn": nn.Mish()}
+mxresnet34 = partial(
+    Net, name="MXResnet32", expansion=1, layers=[3, 4, 6, 3], **mxresnet_parameters
+)
+mxresnet50 = partial(
+    Net, name="MXResnet50", expansion=4, layers=[3, 4, 6, 3], **mxresnet_parameters
+)
```

### Comparing `model_constructor-0.3.2/src/model_constructor/twist.py` & `model_constructor-0.4/src/model_constructor/twist.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             self.coeff_Ax = nn.Parameter(torch.empty((nf, ni // groups)).normal_(0, std), requires_grad=True)
             self.coeff_Ay = nn.Parameter(torch.empty((nf, ni // groups)).normal_(0, std), requires_grad=True)
         self.iters = iters
         self.stride = stride
         self.DD = self.derivatives()
 
     def derivatives(self):
-        I = torch.Tensor([[0, 0, 0], [0, 1, 0], [0, 0, 0]]).view(1, 1, 3, 3)   # noqa E741
+        I = torch.Tensor([[0, 0, 0], [0, 1, 0], [0, 0, 0]]).view(1, 1, 3, 3)   # noqa: E741
         D_x = torch.Tensor([[-1, 0, 1], [-2, 0, 2], [-1, 0, 1]]).view(1, 1, 3, 3) / 10
         D_y = torch.Tensor([[1, 2, 1], [0, 0, 0], [-1, -2, -1]]).view(1, 1, 3, 3) / 10
 
         def convolution(K1, K2):
             return F.conv2d(K1, K2.flip(2).flip(3), padding=2)
         D_xx = convolution(I + D_x, I + D_x).view(5, 5)
         D_yy = convolution(I + D_y, I + D_y).view(5, 5)
@@ -71,16 +71,18 @@
         else:
             return F.conv2d(inpt, self.full_kernel(kernel), padding=1, stride=self.stride, groups=1)
 
     def symmetrize(self, conv_wt):
         if self.same:
             n = conv_wt.size()[1]
             for i in range(self.groups):
-                conv_wt.data[n * i:n * (i + 1)] = (conv_wt[n * i:n * (i + 1)]
-                                                   + torch.transpose(conv_wt[n * i:n * (i + 1)], 0, 1)) / 2  # noqa E503
+                conv_wt.data[n * i:n * (i + 1)] = (
+                    conv_wt[n * i:n * (i + 1)] + torch.transpose(
+                        conv_wt[n * i:n * (i + 1)], 0, 1)
+                ) / 2
 
     def forward(self, inpt):
         out = self._conv(inpt)
         if self.twist is False:
             return out
         _, _, h, w = out.size()
         XX = torch.from_numpy(np.indices((1, 1, h, w))[3] * 2 / w - 1).type(out.dtype).to(out.device)
@@ -88,16 +90,16 @@
         kernel_x = self.kernel(self.coeff_Ax, self.coeff_Ay)
         self.symmetrize(kernel_x)
         kernel_y = kernel_x.transpose(2, 3).flip(3)  # make conv_y a 90 degree rotation of conv_x
         out = out + XX * self._conv(inpt, kernel_x) + YY * self._conv(inpt, kernel_y)
         if self.same and self.iters > 1:
             out = inpt + out / self.iters
             for _ in range(self.iters - 1):
-                out = out + (self._conv(out) + XX * self._conv(out, kernel_x)
-                                             + YY * self._conv(out, kernel_y)) / self.iters  # noqa E727
+                out = out + (
+                    self._conv(out) + XX * self._conv(out, kernel_x) + YY * self._conv(out, kernel_y)) / self.iters
             out = out - inpt
         return out
 
     def extra_repr(self):
         return f"twist: {self.twist}, permute: {self.permute}, same: {self.same}, groups: {self.groups}"
```

### Comparing `model_constructor-0.3.2/src/model_constructor/yaresnet.py` & `model_constructor-0.4/src/model_constructor/yaresnet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,150 +1,221 @@
 # YaResBlock - former NewResBlock.
 # Yet another ResNet.
 
-from collections import OrderedDict
-from typing import Callable, List, Type, Union
+from functools import partial
+from typing import Any, Callable, List, Optional, Type
 
-import torch.nn as nn
-from torch.nn import Mish
+import torch
+from torch import nn
+
+from model_constructor.helpers import ModSeq, nn_seq
 
 from .layers import ConvBnAct, get_act
-from .model_constructor import ModelConstructor
+from .model_constructor import ListStrMod, ModelConstructor, ModelCfg
+from .xresnet import xresnet_stem
+
 
 __all__ = [
-    "YaResBlock",
+    "YaBasicBlock",
+    "YaBottleneckBlock",
+    "YaResNet",
     "YaResNet34",
     "YaResNet50",
 ]
 
 
-class YaResBlock(nn.Module):
-    """YaResBlock. Reduce by pool instead of stride 2"""
+class YaBasicBlock(nn.Module):
+    """Ya Basic block.
+    Reduce by pool instead of stride 2"""
 
     def __init__(
         self,
-        expansion: int,
         in_channels: int,
-        mid_channels: int,
+        out_channels: int,
         stride: int = 1,
-        conv_layer=ConvBnAct,
+        conv_layer: Type[ConvBnAct] = ConvBnAct,
         act_fn: Type[nn.Module] = nn.ReLU,
         zero_bn: bool = True,
         bn_1st: bool = True,
         groups: int = 1,
         dw: bool = False,
-        div_groups: Union[None, int] = None,
-        pool: Union[Callable[[], nn.Module], None] = None,
-        se: Union[Type[nn.Module], None] = None,
-        sa: Union[Type[nn.Module], None] = None,
+        div_groups: Optional[int] = None,
+        pool: Optional[Callable[[], nn.Module]] = None,
+        se: Optional[nn.Module] = None,
+        sa: Optional[nn.Module] = None,
     ):
         super().__init__()
         # pool defined at ModelConstructor.
-        out_channels, in_channels = mid_channels * expansion, in_channels * expansion
         if div_groups is not None:  # check if groups != 1 and div_groups
-            groups = int(mid_channels / div_groups)
+            groups = int(out_channels / div_groups)
 
         if stride != 1:
             if pool is None:
                 self.reduce = conv_layer(in_channels, in_channels, 1, stride=2)
                 # warnings.warn("pool not passed")  # need to warn?
             else:
                 self.reduce = pool()
         else:
             self.reduce = None
-        if expansion == 1:
-            layers = [
-                (
-                    "conv_0",
-                    conv_layer(
-                        in_channels,
-                        mid_channels,
-                        3,
-                        stride=1,
-                        act_fn=act_fn,
-                        bn_1st=bn_1st,
-                        groups=in_channels if dw else groups,
-                    ),
+
+        layers: ListStrMod = [
+            (
+                "conv_0",
+                conv_layer(
+                    in_channels,
+                    out_channels,
+                    3,
+                    act_fn=act_fn,
+                    bn_1st=bn_1st,
+                    groups=in_channels if dw else groups,
                 ),
-                (
-                    "conv_1",
-                    conv_layer(
-                        mid_channels,
-                        out_channels,
-                        3,
-                        zero_bn=zero_bn,
-                        act_fn=False,
-                        bn_1st=bn_1st,
-                        groups=mid_channels if dw else groups,
-                    ),
+            ),
+            (
+                "conv_1",
+                conv_layer(
+                    out_channels,
+                    out_channels,
+                    3,
+                    zero_bn=zero_bn,
+                    act_fn=False,
+                    bn_1st=bn_1st,
+                    groups=out_channels if dw else groups,
                 ),
-            ]
+            ),
+        ]
+        if se:
+            layers.append(("se", se(out_channels)))
+        if sa:
+            layers.append(("sa", sa(out_channels)))
+        self.convs = nn_seq(layers)
+
+        if in_channels != out_channels:
+            self.id_conv = conv_layer(
+                in_channels,
+                out_channels,
+                1,
+                stride=1,
+                act_fn=False,
+            )
         else:
-            layers = [
-                (
-                    "conv_0",
-                    conv_layer(
-                        in_channels,
-                        mid_channels,
-                        1,
-                        act_fn=act_fn,
-                        bn_1st=bn_1st,
-                    ),
+            self.id_conv = None
+        self.merge = get_act(act_fn)
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        if self.reduce:
+            x = self.reduce(x)
+        identity = self.id_conv(x) if self.id_conv is not None else x
+        return self.merge(self.convs(x) + identity)
+
+
+class YaBottleneckBlock(nn.Module):
+    """Ya Bottleneck block.
+    Reduce by pool instead of stride 2"""
+
+    def __init__(
+        self,
+        in_channels: int,
+        out_channels: int,
+        stride: int = 1,
+        expansion: int = 4,
+        conv_layer: Type[ConvBnAct] = ConvBnAct,
+        act_fn: Type[nn.Module] = nn.ReLU,
+        zero_bn: bool = True,
+        bn_1st: bool = True,
+        groups: int = 1,
+        dw: bool = False,
+        div_groups: Optional[int] = None,
+        pool: Optional[Callable[[], nn.Module]] = None,
+        se: Optional[nn.Module] = None,
+        sa: Optional[nn.Module] = None,
+    ):
+        super().__init__()
+        # pool defined at ModelConstructor.
+        mid_channels = out_channels // expansion
+        if div_groups is not None:  # check if groups != 1 and div_groups
+            groups = int(mid_channels / div_groups)
+
+        if stride != 1:
+            if pool is None:
+                self.reduce = conv_layer(in_channels, in_channels, 1, stride=2)
+                # warnings.warn("pool not passed")  # need to warn?
+            else:
+                self.reduce = pool()
+        else:
+            self.reduce = None
+
+        layers: ListStrMod = [
+            (
+                "conv_0",
+                conv_layer(
+                    in_channels,
+                    mid_channels,
+                    1,
+                    act_fn=act_fn,
+                    bn_1st=bn_1st,
+                ),
+            ),
+            (
+                "conv_1",
+                conv_layer(
+                    mid_channels,
+                    mid_channels,
+                    3,
+                    act_fn=act_fn,
+                    bn_1st=bn_1st,
+                    groups=mid_channels if dw else groups,
                 ),
-                (
-                    "conv_1",
-                    conv_layer(
-                        mid_channels,
-                        mid_channels,
-                        3,
-                        stride=1,
-                        act_fn=act_fn,
-                        bn_1st=bn_1st,
-                        groups=mid_channels if dw else groups,
-                    ),
+            ),
+            (
+                "conv_2",
+                conv_layer(
+                    mid_channels,
+                    out_channels,
+                    1,
+                    zero_bn=zero_bn,
+                    act_fn=False,
+                    bn_1st=bn_1st,
                 ),
-                (
-                    "conv_2",
-                    conv_layer(
-                        mid_channels,
-                        out_channels,
-                        1,
-                        zero_bn=zero_bn,
-                        act_fn=False,
-                        bn_1st=bn_1st,
-                    ),
-                ),  # noqa E501
-            ]
+            ),
+        ]
         if se:
             layers.append(("se", se(out_channels)))
         if sa:
             layers.append(("sa", sa(out_channels)))
-        self.convs = nn.Sequential(OrderedDict(layers))
+        self.convs = nn_seq(layers)
+
         if in_channels != out_channels:
             self.id_conv = conv_layer(
                 in_channels,
                 out_channels,
                 1,
                 stride=1,
                 act_fn=False,
             )
         else:
             self.id_conv = None
         self.merge = get_act(act_fn)
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         if self.reduce:
             x = self.reduce(x)
         identity = self.id_conv(x) if self.id_conv is not None else x
         return self.merge(self.convs(x) + identity)
 
 
-class YaResNet34(ModelConstructor):
-    block: type[nn.Module] = YaResBlock
-    expansion: int = 1
-    layers: list[int] = [3, 4, 6, 3]
-    stem_sizes: list[int] = [3, 32, 64, 64]
-    act_fn: Type[nn.Module] = Mish
+class YaResNet(ModelConstructor):
+    make_stem: Callable[[ModelCfg], ModSeq] = xresnet_stem
+    stem_sizes: List[int] = [32, 64, 64]
+    block: Type[nn.Module] = YaBasicBlock
+    act_fn: Type[nn.Module] = nn.Mish
+    pool: Optional[Callable[[Any], nn.Module]] = partial(
+        nn.AvgPool2d, kernel_size=2, ceil_mode=True
+    )
+
+
+class YaResNet34(YaResNet):
+    layers: List[int] = [3, 4, 6, 3]
 
 
 class YaResNet50(YaResNet34):
-    expansion: int = 4
+    block: Type[nn.Module] = YaBottleneckBlock
+    block_sizes: List[int] = [256, 512, 1024, 2048]
```

### Comparing `model_constructor-0.3.2/src/model_constructor.egg-info/PKG-INFO` & `model_constructor-0.4/src/model_constructor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-constructor
-Version: 0.3.2
+Version: 0.4
 Summary: Pytorch models constructor.
 Home-page: https://github.com/ayasyrev/model_constructor
 Author: Yasyrev Andrei
 Author-email: a.yasyrev@gmail.com
 License: apache2
 Keywords: pytorch models
 Classifier: Programming Language :: Python :: 3
@@ -50,97 +50,73 @@
 mc
 ```
 <details open> <summary>output</summary>  
     <pre>ModelConstructor
       in_chans: 3, num_classes: 1000
       expansion: 1, groups: 1, dw: False, div_groups: None
       act_fn: ReLU, sa: False, se: False
-      stem sizes: [32, 32, 64], stride on 0
+      stem sizes: [64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]<pre>
+      layers: [2, 2, 2, 2]</pre>
 </details>
 
 
 
 Check all parameters with `print_cfg` method:
 
 
 ```python
 mc.print_cfg()
 ```
 <details open> <summary>output</summary>  
-    <pre>ModelConstructor(
-      in_chans=3
-      num_classes=1000
-      block='ResBlock'
-      conv_layer='ConvBnAct'
-      block_sizes=[64, 128, 256, 512]
-      layers=[2, 2, 2, 2]
-      norm='BatchNorm2d'
-      act_fn='ReLU'
-      pool="AvgPool2d {'kernel_size': 2, 'ceil_mode': True}"
-      expansion=1
-      groups=1
-      bn_1st=True
-      zero_bn=True
-      stem_sizes=[32, 32, 64]
-      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
-      init_cnn='init_cnn'
-      make_stem='make_stem'
-      make_layer='make_layer'
-      make_body='make_body'
-      make_head='make_head')
-    <pre>
+    <pre>ModelConstructor
+      in_chans: 3, num_classes: 1000
+      expansion: 1, groups: 1, dw: False, div_groups: None
+      act_fn: ReLU, sa: False, se: False
+      stem sizes: [64], stride on 0
+      body sizes [64, 128, 256, 512]
+      layers: [2, 2, 2, 2]
+    </pre>
 </details>
 
-Now we have model constructor, default setting as xresnet18. And we can get model after call it.
+Now we have model constructor, default setting as resnet18. And we can get model after call it.
 
 
 ```python
 
 model = mc()
 model
 ```
 <details> <summary>output</summary>  
-    <pre>ModelConstructor(
+    </pre>ModelConstructor(
       (stem): Sequential(
-        (conv_0): ConvBnAct(
-          (conv): Conv2d(3, 32, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
-          (bn): BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-          (act_fn): ReLU(inplace=True)
-        )
         (conv_1): ConvBnAct(
-          (conv): Conv2d(32, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
-          (bn): BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-          (act_fn): ReLU(inplace=True)
-        )
-        (conv_2): ConvBnAct(
-          (conv): Conv2d(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
+          (conv): Conv2d(3, 64, kernel_size=(7, 7), stride=(2, 2), padding=(3, 3), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): ReLU(inplace=True)
         )
         (stem_pool): MaxPool2d(kernel_size=3, stride=2, padding=1, dilation=1, ceil_mode=False)
       )
       (body): Sequential(
         (l_0): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -148,36 +124,35 @@
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
         )
         (l_1): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -185,36 +160,35 @@
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
         )
         (l_2): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -222,36 +196,35 @@
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
         )
         (l_3): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): ReLU(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): ReLU(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -264,377 +237,311 @@
         )
       )
       (head): Sequential(
         (pool): AdaptiveAvgPool2d(output_size=1)
         (flat): Flatten(start_dim=1, end_dim=-1)
         (fc): Linear(in_features=512, out_features=1000, bias=True)
       )
-    )<pre>
+    )</pre>
 </details>
 
 
 
 If you want to change model, just change constructor parameters.  
-Lets create xresnet50.
+Lets create resnet50.
 
 
 ```python
 mc.expansion = 4
 mc.layers = [3,4,6,3]
 ```
 
+We can check, what we changed (compare to default constructor).
+
+
+```python
+mc.changed_fields
+```
+<details open> <summary>output</summary>  
+    <pre>{'layers': [3, 4, 6, 3], 'expansion': 4}</pre>
+</details>
+
+
+
+
+```python
+mc.print_changed_fields()
+```
+<details open> <summary>output</summary>  
+    <pre>Changed fields:
+    layers: [3, 4, 6, 3]
+    expansion: 4
+    </pre>
+</details>
+
 Now we can look at model parts - stem, body, head.  
 
 
 ```python
 
 mc.body
 ```
 <details> <summary>output</summary>  
-    <pre>Sequential(
+    </pre>Sequential(
       (l_0): Sequential(
-        (bl_0): ResBlock(
+        (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(64, 64, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-            )
-          )
-          (id_conv): Sequential(
-            (id_conv): ConvBnAct(
-              (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_1): ResBlock(
+        (bl_1): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(256, 64, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_2): ResBlock(
+        (bl_2): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(256, 64, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
       )
       (l_1): Sequential(
-        (bl_0): ResBlock(
+        (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(256, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
-              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
+              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(128, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (id_conv): Sequential(
-            (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
             (id_conv): ConvBnAct(
-              (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
+              (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(2, 2), bias=False)
+              (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_1): ResBlock(
+        (bl_1): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(512, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(128, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_2): ResBlock(
+        (bl_2): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(512, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(128, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_3): ResBlock(
+        (bl_3): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(512, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(128, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
       )
       (l_2): Sequential(
-        (bl_0): ResBlock(
+        (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(512, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
-              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (id_conv): Sequential(
-            (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
             (id_conv): ConvBnAct(
-              (conv): Conv2d(512, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
+              (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(2, 2), bias=False)
+              (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_1): ResBlock(
+        (bl_1): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_2): ResBlock(
+        (bl_2): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_3): ResBlock(
+        (bl_3): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_4): ResBlock(
+        (bl_4): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_5): ResBlock(
+        (bl_5): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(256, 1024, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(1024, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
       )
       (l_3): Sequential(
-        (bl_0): ResBlock(
+        (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(1024, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
-              (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
+              (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(512, 2048, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(2048, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (id_conv): Sequential(
-            (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
             (id_conv): ConvBnAct(
-              (conv): Conv2d(1024, 2048, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(2048, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
+              (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(2, 2), bias=False)
+              (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_1): ResBlock(
+        (bl_1): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(2048, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(512, 2048, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(2048, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
-        (bl_2): ResBlock(
+        (bl_2): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
-              (conv): Conv2d(2048, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+              (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
             )
             (conv_1): ConvBnAct(
               (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-              (act_fn): ReLU(inplace=True)
-            )
-            (conv_2): ConvBnAct(
-              (conv): Conv2d(512, 2048, kernel_size=(1, 1), stride=(1, 1), bias=False)
-              (bn): BatchNorm2d(2048, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
             )
           )
           (act_fn): ReLU(inplace=True)
         )
       )
-    )<pre>
+    )</pre>
 </details>
 
 
 
 ## Create constructor from config.
 
 Alternative we can create config first and than create constructor from it. 
@@ -642,37 +549,60 @@
 
 ```python
 from model_constructor import ModelCfg
 ```
 
 
 ```python
-cfg = ModelCfg()
+cfg = ModelCfg(
+    num_classes=10,
+    act_fn=nn.Mish,
+)
 print(cfg)
 ```
 <details open> <summary>output</summary>  
-    <pre>in_chans=3 num_classes=1000 block='ResBlock' conv_layer='ConvBnAct' block_sizes=[64, 128, 256, 512] layers=[2, 2, 2, 2] norm='BatchNorm2d' act_fn='ReLU' pool="AvgPool2d {'kernel_size': 2, 'ceil_mode': True}" expansion=1 groups=1 bn_1st=True zero_bn=True stem_sizes=[32, 32, 64] stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}" init_cnn='init_cnn' make_stem='make_stem' make_layer='make_layer' make_body='make_body' make_head='make_head'
-    <pre>
+    <pre>in_chans=3 num_classes=10 block='BasicBlock' conv_layer='ConvBnAct' block_sizes=[64, 128, 256, 512] layers=[2, 2, 2, 2] norm='BatchNorm2d' act_fn='Mish' expansion=1 groups=1 bn_1st=True zero_bn=True stem_sizes=[64] stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+    </pre>
+</details>
+
+When creating config or constructor we can use string annotation for nn.Modules - it useful when creating model from config files.
+
+
+```python
+cfg = ModelCfg(
+    num_classes=10,
+    act_fn="nn.SELU",
+)
+print(cfg.act_fn)
+```
+<details open> <summary>output</summary>  
+    <pre>class 'torch.nn.modules.activation.SELU'
+    </pre>
 </details>
 
 Now we can create constructor from config:
 
 
 ```python
 mc = ModelConstructor.from_cfg(cfg)
 mc
 ```
 <details open> <summary>output</summary>  
+    <pre>Deprecated. Pass se_module as se argument, se_reduction as arg to se.
+    Deprecated. Pass se_module as se argument, se_reduction as arg to se.
+    </pre>
+</details>
+<details open> <summary>output</summary>  
     <pre>ModelConstructor
-      in_chans: 3, num_classes: 1000
+      in_chans: 3, num_classes: 10
       expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: False, se: False
-      stem sizes: [32, 32, 64], stride on 0
+      act_fn: ReLU, sa: <class 'model_constructor.layers.SimpleSelfAttention'>, se: SEModule
+      stem sizes: [64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]<pre>
+      layers: [2, 2, 2, 2]</pre>
 </details>
 
 
 
 ## More modification.
 
 Main purpose of this module - fast and easy modify model.
@@ -688,24 +618,29 @@
 mc = ModelConstructor(name='MxResNet')
 ```
 
 Then lets modify stem.
 
 
 ```python
+from model_constructor.xresnet import xresnet_stem
+```
+
+
+```python
+mc.make_stem = xresnet_stem
 mc.stem_sizes = [3,32,64,64]
 ```
 
 Now lets change activation function to Mish.
 Here is link to [forum discussion](https://forums.fast.ai/t/meet-mish-new-activation-function-possible-successor-to-relu)    
 We'v got Mish is in model_constructor.activations, but from pytorch 1.9 take it from torch:
 
 
 ```python
-# from model_constructor.activations import Mish
 from torch.nn import Mish
 ```
 
 
 ```python
 mc.act_fn = Mish
 ```
@@ -717,29 +652,42 @@
 <details open> <summary>output</summary>  
     <pre>MxResNet
       in_chans: 3, num_classes: 1000
       expansion: 1, groups: 1, dw: False, div_groups: None
       act_fn: Mish, sa: False, se: False
       stem sizes: [3, 32, 64, 64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]<pre>
+      layers: [2, 2, 2, 2]</pre>
 </details>
 
 
 
+
+```python
+mc.print_changed_fields()
+```
+<details open> <summary>output</summary>  
+    <pre>Changed fields:
+    name: MxResNet
+    act_fn: Mish
+    stem_sizes: [3, 32, 64, 64]
+    make_stem: xresnet_stem
+    </pre>
+</details>
+
 Here is model:  
 
 
 ```python
 
 mc()
 ```
 <details> <summary>output</summary>  
-    <pre>MxResNet(
-      stem_sizes: [3, 32, 64, 64], act_fn: Mish
+    </pre>MxResNet(
+      act_fn: Mish, stem_sizes: [3, 32, 64, 64], make_stem: xresnet_stem
       (stem): Sequential(
         (conv_0): ConvBnAct(
           (conv): Conv2d(3, 3, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(3, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
         (conv_1): ConvBnAct(
@@ -757,29 +705,29 @@
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
         (stem_pool): MaxPool2d(kernel_size=3, stride=2, padding=1, dilation=1, ceil_mode=False)
       )
       (body): Sequential(
         (l_0): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -787,36 +735,35 @@
                 (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
         )
         (l_1): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -824,36 +771,35 @@
                 (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
         )
         (l_2): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(128, 256, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -861,36 +807,35 @@
                 (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
         )
         (l_3): Sequential(
-          (bl_0): ResBlock(
+          (bl_0): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
                 (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (id_conv): Sequential(
-              (pool): AvgPool2d(kernel_size=2, stride=2, padding=0)
               (id_conv): ConvBnAct(
-                (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(1, 1), bias=False)
+                (conv): Conv2d(256, 512, kernel_size=(1, 1), stride=(2, 2), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               )
             )
             (act_fn): Mish(inplace=True)
           )
-          (bl_1): ResBlock(
+          (bl_1): BasicBlock(
             (convs): Sequential(
               (conv_0): ConvBnAct(
                 (conv): Conv2d(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
                 (bn): BatchNorm2d(512, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 (act_fn): Mish(inplace=True)
               )
               (conv_1): ConvBnAct(
@@ -903,30 +848,45 @@
         )
       )
       (head): Sequential(
         (pool): AdaptiveAvgPool2d(output_size=1)
         (flat): Flatten(start_dim=1, end_dim=-1)
         (fc): Linear(in_features=512, out_features=1000, bias=True)
       )
-    )<pre>
+    )</pre>
 </details>
 
 
 
 ## MXResNet50
 
 Now lets make MxResNet50
 
 
 ```python
 mc.expansion = 4
 mc.layers = [3,4,6,3]
-mc.name = 'mxresnet50'
+mc.name = "mxresnet50"
 ```
 
+
+```python
+mc.print_changed_fields()
+```
+<details open> <summary>output</summary>  
+    <pre>Changed fields:
+    name: mxresnet50
+    layers: [3, 4, 6, 3]
+    act_fn: Mish
+    expansion: 4
+    stem_sizes: [3, 32, 64, 64]
+    make_stem: xresnet_stem
+    </pre>
+</details>
+
 Now we have mxresnet50 constructor.  
 We can inspect every parts of it.  
 And after call it we got model.
 
 
 ```python
 mc
@@ -934,152 +894,141 @@
 <details open> <summary>output</summary>  
     <pre>mxresnet50
       in_chans: 3, num_classes: 1000
       expansion: 4, groups: 1, dw: False, div_groups: None
       act_fn: Mish, sa: False, se: False
       stem sizes: [3, 32, 64, 64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [3, 4, 6, 3]<pre>
+      layers: [3, 4, 6, 3]</pre>
 </details>
 
 
 
 
 ```python
 
 mc.stem.conv_1
 ```
 <details> <summary>output</summary>  
-    <pre>ConvBnAct(
+    </pre>ConvBnAct(
       (conv): Conv2d(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
       (bn): BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
       (act_fn): Mish(inplace=True)
-    )<pre>
+    )</pre>
 </details>
 
 
 
 
 ```python
 
 mc.body.l_0.bl_0
 ```
 <details> <summary>output</summary>  
-    <pre>ResBlock(
+    </pre>BasicBlock(
       (convs): Sequential(
         (conv_0): ConvBnAct(
-          (conv): Conv2d(64, 64, kernel_size=(1, 1), stride=(1, 1), bias=False)
+          (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
         (conv_1): ConvBnAct(
           (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-          (act_fn): Mish(inplace=True)
-        )
-        (conv_2): ConvBnAct(
-          (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-          (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
-        )
-      )
-      (id_conv): Sequential(
-        (id_conv): ConvBnAct(
-          (conv): Conv2d(64, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
-          (bn): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
         )
       )
       (act_fn): Mish(inplace=True)
-    )<pre>
+    )</pre>
 </details>
 
 
 
 We can get model direct way:
 
 
 ```python
-mc = ModelConstructor(name="MxResNet", act_fn=Mish, layers=[3,4,6,3], expansion=4, stem_sizes=[32,64,64])
+mc = ModelConstructor(
+    name="MxResNet",
+    act_fn=Mish,
+    layers=[3,4,6,3],
+    expansion=4,
+    make_stem=xresnet_stem,
+    stem_sizes=[32,64,64]
+)
 model = mc()
 ```
 
-Or create with config:
+Another way:
 
 
 ```python
-mc = ModelConstructor.from_cfg(
-    ModelCfg(name="MxResNet", act_fn=Mish, layers=[3,4,6,3], expansion=4, stem_sizes=[32,64,64])
+model = ModelConstructor.create_model(
+    name="MxResNet",
+    act_fn=Mish,
+    layers=[3,4,6,3],
+    expansion=4,
+    make_stem=xresnet_stem,
+    stem_sizes=[32,64,64]
 )
-model = mc()
 ```
 
 ## YaResNet
 
 Now lets change Resblock to YaResBlock (Yet another ResNet, former NewResBlock) is in lib from version 0.1.0
 
 
 ```python
-from model_constructor.yaresnet import YaResBlock
+from model_constructor.yaresnet import YaBasicBlock
 ```
 
 
 ```python
 mc = ModelConstructor(name="YaResNet")
-mc.block = YaResBlock
+mc.block = YaBasicBlock
 ```
 
 Or in one line:
 
 
 ```python
-mc = ModelConstructor(name="YaResNet", block=YaResBlock)
+mc = ModelConstructor(name="YaResNet", block=YaBasicBlock)
 ```
 
 That all. Now we have YaResNet constructor
 
 
 ```python
 
 mc.print_cfg()
 ```
 <details> <summary>output</summary>  
-    <pre>ModelConstructor(
-      name='YaResNet'
-      in_chans=3
-      num_classes=1000
-      block='YaResBlock'
-      conv_layer='ConvBnAct'
-      block_sizes=[64, 128, 256, 512]
-      layers=[2, 2, 2, 2]
-      norm='BatchNorm2d'
-      act_fn='ReLU'
-      pool="AvgPool2d {'kernel_size': 2, 'ceil_mode': True}"
-      expansion=1
-      groups=1
-      bn_1st=True
-      zero_bn=True
-      stem_sizes=[32, 32, 64]
-      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
-      init_cnn='init_cnn'
-      make_stem='make_stem'
-      make_layer='make_layer'
-      make_body='make_body'
-      make_head='make_head')
-    <pre>
+    </pre>YaResNet
+      in_chans: 3, num_classes: 1000
+      expansion: 1, groups: 1, dw: False, div_groups: None
+      act_fn: ReLU, sa: False, se: False
+      stem sizes: [64], stride on 0
+      body sizes [64, 128, 256, 512]
+      layers: [2, 2, 2, 2]
+    </pre>
 </details>
 
 Let see what we have.
 
 
 ```python
 
 mc.body.l_1.bl_0
 ```
 <details> <summary>output</summary>  
-    <pre>YaResBlock(
-      (reduce): AvgPool2d(kernel_size=2, stride=2, padding=0)
+    </pre>YaBasicBlock(
+      (reduce): ConvBnAct(
+        (conv): Conv2d(64, 64, kernel_size=(1, 1), stride=(2, 2), bias=False)
+        (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
+        (act_fn): ReLU(inplace=True)
+      )
       (convs): Sequential(
         (conv_0): ConvBnAct(
           (conv): Conv2d(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): ReLU(inplace=True)
         )
         (conv_1): ConvBnAct(
@@ -1088,75 +1037,67 @@
         )
       )
       (id_conv): ConvBnAct(
         (conv): Conv2d(64, 128, kernel_size=(1, 1), stride=(1, 1), bias=False)
         (bn): BatchNorm2d(128, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
       )
       (merge): ReLU(inplace=True)
-    )<pre>
+    )</pre>
 </details>
 
 
 
-Lets create `Resnet34` like model constructor:
+Lets create `xResnet34` like model constructor:
 
 
 ```python
+from typing import Callable
+
+from model_constructor.helpers import ModSeq
+
+
 class YaResnet34(ModelConstructor):
-    block: type[nn.Module] = YaResBlock
+    block: type[nn.Module] = YaBasicBlock
     layers: list[int] = [3, 4, 6, 3]
+    make_stem: Callable[[ModelCfg], ModSeq] = xresnet_stem
 ```
 
 
 ```python
 mc = YaResnet34()
 mc.print_cfg()
 ```
 <details open> <summary>output</summary>  
-    <pre>YaResnet34(
-      in_chans=3
-      num_classes=1000
-      block='YaResBlock'
-      conv_layer='ConvBnAct'
-      block_sizes=[64, 128, 256, 512]
-      layers=[3, 4, 6, 3]
-      norm='BatchNorm2d'
-      act_fn='ReLU'
-      pool="AvgPool2d {'kernel_size': 2, 'ceil_mode': True}"
-      expansion=1
-      groups=1
-      bn_1st=True
-      zero_bn=True
-      stem_sizes=[32, 32, 64]
-      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
-      init_cnn='init_cnn'
-      make_stem='make_stem'
-      make_layer='make_layer'
-      make_body='make_body'
-      make_head='make_head')
-    <pre>
+    <pre>YaResnet34
+      in_chans: 3, num_classes: 1000
+      expansion: 1, groups: 1, dw: False, div_groups: None
+      act_fn: ReLU, sa: False, se: False
+      stem sizes: [64], stride on 0
+      body sizes [64, 128, 256, 512]
+      layers: [3, 4, 6, 3]
+    </pre>
 </details>
 
-And `Resnet50` like model can be inherited from `YaResnet34`:
+And `xResnet50` like model can be inherited from `YaResnet34`:
 
 
 ```python
 class YaResnet50(YaResnet34):
-    expansion = 4
+    expansion: int = 4
 ```
 
 
 ```python
 mc = YaResnet50()
 mc
 ```
 <details open> <summary>output</summary>  
     <pre>YaResnet50
       in_chans: 3, num_classes: 1000
       expansion: 4, groups: 1, dw: False, div_groups: None
       act_fn: ReLU, sa: False, se: False
-      stem sizes: [32, 32, 64], stride on 0
+      stem sizes: [64], stride on 0
       body sizes [64, 128, 256, 512]
-      layers: [3, 4, 6, 3]<pre>
+      layers: [3, 4, 6, 3]</pre>
 </details>
```

