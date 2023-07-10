# Comparing `tmp/LongNet-0.1.3.tar.gz` & `tmp/LongNet-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.1.3.tar", last modified: Fri Jul  7 18:46:37 2023, max compression
+gzip compressed data, was "LongNet-0.1.5.tar", last modified: Mon Jul 10 18:00:52 2023, max compression
```

## Comparing `LongNet-0.1.3.tar` & `LongNet-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:46:37.336563 LongNet-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 18:46:27.000000 LongNet-0.1.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:46:37.332563 LongNet-0.1.3/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-07 18:46:27.000000 LongNet-0.1.3/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-07 18:46:27.000000 LongNet-0.1.3/LongNet/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-07 18:46:27.000000 LongNet-0.1.3/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-07 18:46:27.000000 LongNet-0.1.3/LongNet/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-07-07 18:46:27.000000 LongNet-0.1.3/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-07 18:46:27.000000 LongNet-0.1.3/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:46:37.332563 LongNet-0.1.3/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 18:46:37.000000 LongNet-0.1.3/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-07 18:46:37.000000 LongNet-0.1.3/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:46:37.000000 LongNet-0.1.3/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-07 18:46:37.000000 LongNet-0.1.3/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 18:46:37.000000 LongNet-0.1.3/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 18:46:37.332563 LongNet-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13482 2023-07-07 18:46:27.000000 LongNet-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:46:37.336563 LongNet-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-07 18:46:27.000000 LongNet-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:46:37.332563 LongNet-0.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-07 18:46:27.000000 LongNet-0.1.3/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:52.293638 LongNet-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 18:00:42.000000 LongNet-0.1.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:52.285637 LongNet-0.1.5/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 18:00:42.000000 LongNet-0.1.5/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-10 18:00:42.000000 LongNet-0.1.5/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-07-10 18:00:42.000000 LongNet-0.1.5/LongNet/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-10 18:00:42.000000 LongNet-0.1.5/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-10 18:00:42.000000 LongNet-0.1.5/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-10 18:00:42.000000 LongNet-0.1.5/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:52.285637 LongNet-0.1.5/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 18:00:52.000000 LongNet-0.1.5/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-10 18:00:52.000000 LongNet-0.1.5/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:00:52.000000 LongNet-0.1.5/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 18:00:52.000000 LongNet-0.1.5/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 18:00:52.000000 LongNet-0.1.5/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 18:00:52.293638 LongNet-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-07-10 18:00:42.000000 LongNet-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:52.289638 LongNet-0.1.5/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:52.289638 LongNet-0.1.5/flash_attn/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/bert_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/flash_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/flash_attn_triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/flash_attn_triton_og.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/flash_blocksparse_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/flash_blocksparse_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/fused_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:52.289638 LongNet-0.1.5/flash_attn/flash_attn/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/layers/patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/layers/rotary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:52.289638 LongNet-0.1.5/flash_attn/flash_attn/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/losses/cross_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:52.289638 LongNet-0.1.5/flash_attn/flash_attn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/models/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/models/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/models/gpt_neox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/models/gptj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/models/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/models/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:52.289638 LongNet-0.1.5/flash_attn/flash_attn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/modules/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/modules/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/modules/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:52.289638 LongNet-0.1.5/flash_attn/flash_attn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/ops/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/ops/fused_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19306 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/ops/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/ops/rms_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:52.293638 LongNet-0.1.5/flash_attn/flash_attn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/utils/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/flash_attn/utils/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-10 18:00:42.000000 LongNet-0.1.5/flash_attn/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:00:52.293638 LongNet-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-10 18:00:42.000000 LongNet-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:00:52.293638 LongNet-0.1.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 18:00:42.000000 LongNet-0.1.5/test/test.py
```

### Comparing `LongNet-0.1.3/LICENSE` & `LongNet-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.3/LongNet/model.py` & `LongNet-0.1.5/LongNet/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import torch
 from torch.nn import Embedding, Module
 import bitsandbytes
 
-from LongNet.torchscale import DecoderConfig, Decoder, PositionalEmbedding
+from torchscale import DecoderConfig, Decoder, PositionalEmbedding
 from transformers import AutoTokenizer
 
-# 
 class LongNetTokenizer:
     def __init__(self):
         self.tokenizer = AutoTokenizer.from_pretrained(
             "EleutherAI/gpt-neox-20b",
             eos_token="<eos>",
             pad_token="<pad>",
             extra_ids=0,
@@ -59,20 +58,8 @@
             output_projection=self.output_projection
         )
 
 
     def forward(self, text_tokens, **kwargs):
         model_input = self.decoder.forward_embedding(text_tokens)[0]
         return self.decoder(model_input, passed_x=model_input)[0]
-        
-
-# class LongNetSelector:
-#     def __init__(self, mode="language"):
-#         assert mode in ['multimodal', 'language'], 'Invalid mode choose from multimodal or language'
-#         if mode == "multimodal":
-#             self.model = LongNet()
-#         else:
-#             self.model = LongNetLanguage()
-
-
-#     def forward(self, *args, **kwargs):
-#         return self.model(*args, **kwargs)
+
```

### Comparing `LongNet-0.1.3/LongNet/training.py` & `LongNet-0.1.5/LongNet/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,17 @@
                           get_linear_schedule_with_warmup, set_seed)
 
 
 
 # INTEGRATE LONGNET selector + stable8bitfusedadam
 
 # from LongNet.torchscale.torchscale.architecture.decoder import Decoder
-from LongNet.torchscale import Decoder
-from LongNet.utils import StableAdamWUnfused
-from LongNet.model import LongNet
+from torchscale import Decoder
+from utils import StableAdamWUnfused
+from model import LongNet
 ############ SETUP CONFIG
 # import torch.distributed as dist
 
 # dist.init_process_group(backend='nccl', init_method="env://")
 
 ################
```

### Comparing `LongNet-0.1.3/LongNet/utils.py` & `LongNet-0.1.5/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.1.3/LongNet.egg-info/PKG-INFO` & `LongNet-0.1.5/LongNet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.1.3
+Version: 0.1.5
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.1.3/PKG-INFO` & `LongNet-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.1.3
+Version: 0.1.5
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.1.3/README.md` & `LongNet-0.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # LongNet: Scaling Transformers to 1,000,000,000 Tokens
 
 This is an implementation for the paper [LongNet: Scaling Transformers to 1,000,000,000 Tokens](https://arxiv.org/abs/xxx.xxxxx) by Jiayu Ding, Shuming Ma, Li Dong, Xingxing Zhang, Shaohan Huang, Wenhui Wang, Furu Wei. The LongNet is a Transformer variant designed to scale sequence length up to more than 1 billion tokens without sacrificing performance on shorter sequences.
 
 ## Introduction
 
-Scaling sequence length has become a critical bottleneck in the era of large language models. However, existing methods struggle with either computational complexity or model expressivity, rendering the maximum sequence length restricted. In this paper, they introduce LongNet, a Transformer variant that can scale sequence length to more than 1 billion tokens, without sacrificing the performance on shorter sequences. Specifically, we propose dilated attention, which expands the attentive field exponentially as the distance grows.
+Scaling sequence length has become a critical bottleneck in the era of large language models. However, existing methods struggle with either computational complexity or model expressivity, rendering the maximum sequence length restricted. In this paper, they introduce LongNet, a Transformer variant that can scale sequence length to more than 1 billion tokens, without sacrificing the performance on shorter sequences. Specifically, they propose dilated attention, which expands the attentive field exponentially as the distance grows.
 
 ## Features
 LongNet has significant advantages:
 1. It has a linear computation complexity and a logarithm dependency between tokens.
 2. It can be served as a distributed trainer for extremely long sequences.
 3. Its dilated attention is a drop-in replacement for standard attention, which can be seamlessly integrated with the existing Transformer-based optimization.
 
@@ -43,15 +43,27 @@
 
 3. Install the required dependencies:
 
 ```shell
 pip install -r requirements.txt
 ```
 
+4. Then Install dependencies for flash_attn
+
+* `cd flash_attn`
+
+* `python setup.py install`
+
+* `cd ..`
+
+* `python3 example.py`
+
+
 ### Method 2: Pip Install
+* Note that pip install does not work as the `flash-attn` library cannot be compiled since it has custom CUDA Kernels.
 
 1. Install LongNet directly from PyPI using pip:
 
 ```shell
 pip install LongNet
 ```
 
@@ -272,14 +284,18 @@
 [Share LongNet Repository](https://github.com/kyegomez/LongNet)
 
 
 
 
 # Roadmap
 
+* Test and evaluate
+
+* And, create an interation of `DilatedAttention` `FlashBlocksparseMHA`
+
 * Integrate Model, tokenizer, and train function without file path
 
 * Create a benchmarking suite against other attentions
 
 * Add unit testing for `DilationAttention`
 
 * Create a multi-modal `DilationAttention` with multiway, sub layernorm, and xpos?
```

### Comparing `LongNet-0.1.3/setup.py` & `LongNet-0.1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.1.3',
+  version = '0.1.5',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
@@ -16,20 +16,20 @@
     'deep learning',
     'optimizers',
     "Prompt Engineering"
   ],
     install_requires=[
         'torch',
         'einops',
-        'flash-attn',
+        'torchscale',
         'accelerate',
         'bitsandbytes',
         'fairscale',
         'timm',
-        'flamingo-pytorch'
+        'dataclasses',
     ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

### Comparing `LongNet-0.1.3/test/test.py` & `LongNet-0.1.5/test/test.py`

 * *Files identical despite different names*

