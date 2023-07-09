# Comparing `tmp/discrete-key-value-bottleneck-pytorch-0.0.8.tar.gz` & `tmp/discrete-key-value-bottleneck-pytorch-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discrete-key-value-bottleneck-pytorch-0.0.8.tar", last modified: Mon Jun 19 19:56:44 2023, max compression
+gzip compressed data, was "discrete-key-value-bottleneck-pytorch-0.1.0.tar", last modified: Sun Jul  9 22:32:55 2023, max compression
```

## Comparing `discrete-key-value-bottleneck-pytorch-0.0.8.tar` & `discrete-key-value-bottleneck-pytorch-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:56:44.595391 discrete-key-value-bottleneck-pytorch-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 19:56:28.000000 discrete-key-value-bottleneck-pytorch-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-19 19:56:44.595391 discrete-key-value-bottleneck-pytorch-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-19 19:56:28.000000 discrete-key-value-bottleneck-pytorch-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:56:44.595391 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-19 19:56:28.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-19 19:56:28.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch/discrete_key_value_bottleneck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:56:44.595391 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-19 19:56:44.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-19 19:56:44.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:56:44.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 19:56:44.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 19:56:44.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 19:56:44.595391 discrete-key-value-bottleneck-pytorch-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-19 19:56:28.000000 discrete-key-value-bottleneck-pytorch-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:32:55.180986 discrete-key-value-bottleneck-pytorch-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-09 22:32:43.000000 discrete-key-value-bottleneck-pytorch-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-09 22:32:55.180986 discrete-key-value-bottleneck-pytorch-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-09 22:32:43.000000 discrete-key-value-bottleneck-pytorch-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:32:55.180986 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-09 22:32:44.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-09 22:32:44.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch/discrete_key_value_bottleneck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:32:55.180986 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-09 22:32:55.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-09 22:32:55.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:32:55.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-09 22:32:55.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:32:55.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:32:55.180986 discrete-key-value-bottleneck-pytorch-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-09 22:32:44.000000 discrete-key-value-bottleneck-pytorch-0.1.0/setup.py
```

### Comparing `discrete-key-value-bottleneck-pytorch-0.0.8/LICENSE` & `discrete-key-value-bottleneck-pytorch-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discrete-key-value-bottleneck-pytorch-0.0.8/PKG-INFO` & `discrete-key-value-bottleneck-pytorch-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discrete-key-value-bottleneck-pytorch
-Version: 0.0.8
+Version: 0.1.0
 Summary: Discrete Key / Value Bottleneck - Pytorch
 Home-page: https://github.com/lucidrains/discrete-key-value-bottleneck-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,quantization,memory,transfer learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discrete-key-value-bottleneck-pytorch-0.0.8/README.md` & `discrete-key-value-bottleneck-pytorch-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 ```python
 import torch
 from discrete_key_value_bottleneck_pytorch import DiscreteKeyValueBottleneck
 
 key_value_bottleneck = DiscreteKeyValueBottleneck(
     dim = 512,                  # input dimension
+    dim_memory = 512,           # output dimension - or dimension of each memories for all heads (defaults to same as input)
     num_memory_codebooks = 2,   # number of memory codebook, embedding is split into 2 pieces of 256, 256, quantized, outputs 256, 256, flattened together to 512
     num_memories = 256,         # number of memories
-    dim_memory = 256,           # dimension of the output memories
     decay = 0.9,                # the exponential moving average decay, lower means the keys will change faster
 )
 
 embeds = torch.randn(1, 1024, 512)  # from pretrained encoder
 
 memories = key_value_bottleneck(embeds)
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
 [./discrete-key-value.png] ## Discrete Key / Value Bottleneck - Pytorch
 Implementation of Discrete_Key_/_Value_Bottleneck, in Pytorch. ## Install
 ```bash $ pip install discrete-key-value-bottleneck-pytorch ``` ## Usage
 ```python import torch from discrete_key_value_bottleneck_pytorch import
 DiscreteKeyValueBottleneck key_value_bottleneck = DiscreteKeyValueBottleneck
-( dim = 512, # input dimension num_memory_codebooks = 2, # number of memory
-codebook, embedding is split into 2 pieces of 256, 256, quantized, outputs 256,
-256, flattened together to 512 num_memories = 256, # number of memories
-dim_memory = 256, # dimension of the output memories decay = 0.9, # the
-exponential moving average decay, lower means the keys will change faster )
-embeds = torch.randn(1, 1024, 512) # from pretrained encoder memories =
-key_value_bottleneck(embeds) memories.shape # (1, 1024, 512) # (batch, seq,
-memory / values dimension) # now you can use the memories for the downstream
-decoder ``` You can also pass the pretrained encoder to the bottleneck and it
-will automatically invoke it. Example with `vit-pytorch` library ```bash $ pip
+( dim = 512, # input dimension dim_memory = 512, # output dimension - or
+dimension of each memories for all heads (defaults to same as input)
+num_memory_codebooks = 2, # number of memory codebook, embedding is split into
+2 pieces of 256, 256, quantized, outputs 256, 256, flattened together to 512
+num_memories = 256, # number of memories decay = 0.9, # the exponential moving
+average decay, lower means the keys will change faster ) embeds = torch.randn
+(1, 1024, 512) # from pretrained encoder memories = key_value_bottleneck
+(embeds) memories.shape # (1, 1024, 512) # (batch, seq, memory / values
+dimension) # now you can use the memories for the downstream decoder ``` You
+can also pass the pretrained encoder to the bottleneck and it will
+automatically invoke it. Example with `vit-pytorch` library ```bash $ pip
 install vit-pytorch ``` Then ```python import torch # import vision transformer
 from vit_pytorch import SimpleViT from vit_pytorch.extractor import Extractor
 vit = SimpleViT( image_size = 256, patch_size = 32, num_classes = 1000, dim =
 512, depth = 6, heads = 16, mlp_dim = 2048 ) # train vit, or load pretrained
 vit = Extractor(vit, return_embeddings_only = True) # then from
 discrete_key_value_bottleneck_pytorch import DiscreteKeyValueBottleneck
 enc_with_bottleneck = DiscreteKeyValueBottleneck( encoder = vit, # pass the
```

### Comparing `discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/PKG-INFO` & `discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discrete-key-value-bottleneck-pytorch
-Version: 0.0.8
+Version: 0.1.0
 Summary: Discrete Key / Value Bottleneck - Pytorch
 Home-page: https://github.com/lucidrains/discrete-key-value-bottleneck-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,quantization,memory,transfer learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discrete-key-value-bottleneck-pytorch-0.0.8/setup.py` & `discrete-key-value-bottleneck-pytorch-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'discrete-key-value-bottleneck-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.8',
+  version = '0.1.0',
   license='MIT',
   description = 'Discrete Key / Value Bottleneck - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/discrete-key-value-bottleneck-pytorch',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'quantization',
     'memory',
     'transfer learning'
   ],
   install_requires=[
-    'einops>=0.4',
-    'vector-quantize-pytorch>=0.10.14',
+    'einops>=0.6',
+    'vector-quantize-pytorch>=1.6.28',
     'torch>=1.6',
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
```

