# Comparing `tmp/discrete-key-value-bottleneck-pytorch-0.1.0.tar.gz` & `tmp/discrete-key-value-bottleneck-pytorch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discrete-key-value-bottleneck-pytorch-0.1.0.tar", last modified: Sun Jul  9 22:32:55 2023, max compression
+gzip compressed data, was "discrete-key-value-bottleneck-pytorch-0.1.1.tar", last modified: Sun Jul  9 23:57:43 2023, max compression
```

## Comparing `discrete-key-value-bottleneck-pytorch-0.1.0.tar` & `discrete-key-value-bottleneck-pytorch-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:32:55.180986 discrete-key-value-bottleneck-pytorch-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-09 22:32:43.000000 discrete-key-value-bottleneck-pytorch-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-09 22:32:55.180986 discrete-key-value-bottleneck-pytorch-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-09 22:32:43.000000 discrete-key-value-bottleneck-pytorch-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:32:55.180986 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-09 22:32:44.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-09 22:32:44.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch/discrete_key_value_bottleneck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:32:55.180986 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-09 22:32:55.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-09 22:32:55.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:32:55.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-09 22:32:55.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:32:55.000000 discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:32:55.180986 discrete-key-value-bottleneck-pytorch-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-09 22:32:44.000000 discrete-key-value-bottleneck-pytorch-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:57:43.557547 discrete-key-value-bottleneck-pytorch-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-09 23:57:32.000000 discrete-key-value-bottleneck-pytorch-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-09 23:57:43.557547 discrete-key-value-bottleneck-pytorch-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-09 23:57:32.000000 discrete-key-value-bottleneck-pytorch-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:57:43.553547 discrete-key-value-bottleneck-pytorch-0.1.1/discrete_key_value_bottleneck_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-09 23:57:32.000000 discrete-key-value-bottleneck-pytorch-0.1.1/discrete_key_value_bottleneck_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-09 23:57:32.000000 discrete-key-value-bottleneck-pytorch-0.1.1/discrete_key_value_bottleneck_pytorch/discrete_key_value_bottleneck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:57:43.557547 discrete-key-value-bottleneck-pytorch-0.1.1/discrete_key_value_bottleneck_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-09 23:57:43.000000 discrete-key-value-bottleneck-pytorch-0.1.1/discrete_key_value_bottleneck_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-09 23:57:43.000000 discrete-key-value-bottleneck-pytorch-0.1.1/discrete_key_value_bottleneck_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 23:57:43.000000 discrete-key-value-bottleneck-pytorch-0.1.1/discrete_key_value_bottleneck_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-09 23:57:43.000000 discrete-key-value-bottleneck-pytorch-0.1.1/discrete_key_value_bottleneck_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 23:57:43.000000 discrete-key-value-bottleneck-pytorch-0.1.1/discrete_key_value_bottleneck_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 23:57:43.557547 discrete-key-value-bottleneck-pytorch-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-09 23:57:32.000000 discrete-key-value-bottleneck-pytorch-0.1.1/setup.py
```

### Comparing `discrete-key-value-bottleneck-pytorch-0.1.0/LICENSE` & `discrete-key-value-bottleneck-pytorch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discrete-key-value-bottleneck-pytorch-0.1.0/PKG-INFO` & `discrete-key-value-bottleneck-pytorch-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discrete-key-value-bottleneck-pytorch
-Version: 0.1.0
+Version: 0.1.1
 Summary: Discrete Key / Value Bottleneck - Pytorch
 Home-page: https://github.com/lucidrains/discrete-key-value-bottleneck-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,quantization,memory,transfer learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discrete-key-value-bottleneck-pytorch-0.1.0/README.md` & `discrete-key-value-bottleneck-pytorch-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch/discrete_key_value_bottleneck.py` & `discrete-key-value-bottleneck-pytorch-0.1.1/discrete_key_value_bottleneck_pytorch/discrete_key_value_bottleneck.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,35 +16,38 @@
 
 class DiscreteKeyValueBottleneck(nn.Module):
     def __init__(
         self,
         dim,
         *,
         num_memories,
+        dim_embed = None,
         num_memory_codebooks = 1,
         encoder = None,
         dim_memory = None,
         average_pool_memories = True,
         **kwargs
     ):
         super().__init__()
         self.encoder = encoder
+        dim_embed = default(dim_embed, dim)
+        self.dim_embed = dim_embed
 
         self.vq = VectorQuantize(
             dim = dim * num_memory_codebooks,
             codebook_size = num_memories,
             heads = num_memory_codebooks,
             separate_codebook_per_head = True,
             **kwargs
         )
 
         dim_memory = default(dim_memory, dim)
         self.values = nn.Parameter(torch.randn(num_memory_codebooks, num_memories, dim_memory))
 
-        rand_proj = torch.empty(num_memory_codebooks, dim, dim)
+        rand_proj = torch.empty(num_memory_codebooks, dim_embed, dim)
         nn.init.xavier_normal_(rand_proj)
 
         self.register_buffer('rand_proj', rand_proj)
         self.average_pool_memories = average_pool_memories
 
     def forward(
         self,
@@ -57,14 +60,16 @@
 
         if exists(self.encoder):
             self.encoder.eval()
             with torch.no_grad():
                 x = self.encoder(x, **kwargs)
                 x.detach_()
 
+        assert x.shape[-1] == self.dim_embed, f'encoding has a dimension of {x.shape[-1]} but dim_embed (defaults to dim) is set to {self.dim_embed} on init'
+
         x = einsum('b n d, c d e -> b n c e', x, self.rand_proj)
         x = rearrange(x, 'b n c e -> b n (c e)')
 
         vq_out = self.vq(x)
 
         quantized, memory_indices, commit_loss = vq_out
```

### Comparing `discrete-key-value-bottleneck-pytorch-0.1.0/discrete_key_value_bottleneck_pytorch.egg-info/PKG-INFO` & `discrete-key-value-bottleneck-pytorch-0.1.1/discrete_key_value_bottleneck_pytorch.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discrete-key-value-bottleneck-pytorch
-Version: 0.1.0
+Version: 0.1.1
 Summary: Discrete Key / Value Bottleneck - Pytorch
 Home-page: https://github.com/lucidrains/discrete-key-value-bottleneck-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,quantization,memory,transfer learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discrete-key-value-bottleneck-pytorch-0.1.0/setup.py` & `discrete-key-value-bottleneck-pytorch-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'discrete-key-value-bottleneck-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.1.0',
+  version = '0.1.1',
   license='MIT',
   description = 'Discrete Key / Value Bottleneck - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/discrete-key-value-bottleneck-pytorch',
   keywords = [
```

