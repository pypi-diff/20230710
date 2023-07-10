# Comparing `tmp/x-dgcnn-0.2.2.tar.gz` & `tmp/x-dgcnn-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-dgcnn-0.2.2.tar", last modified: Mon Jul 10 04:31:32 2023, max compression
+gzip compressed data, was "x-dgcnn-0.3.0.tar", last modified: Mon Jul 10 18:57:37 2023, max compression
```

## Comparing `x-dgcnn-0.2.2.tar` & `x-dgcnn-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:31:32.054778 x-dgcnn-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-10 04:31:20.000000 x-dgcnn-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-10 04:31:32.054778 x-dgcnn-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-10 04:31:20.000000 x-dgcnn-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 04:31:32.054778 x-dgcnn-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-10 04:31:20.000000 x-dgcnn-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:31:32.054778 x-dgcnn-0.2.2/x_dgcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-10 04:31:20.000000 x-dgcnn-0.2.2/x_dgcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-10 04:31:20.000000 x-dgcnn-0.2.2/x_dgcnn/dgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-10 04:31:20.000000 x-dgcnn-0.2.2/x_dgcnn/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:31:32.054778 x-dgcnn-0.2.2/x_dgcnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-10 04:31:32.000000 x-dgcnn-0.2.2/x_dgcnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-10 04:31:32.000000 x-dgcnn-0.2.2/x_dgcnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 04:31:32.000000 x-dgcnn-0.2.2/x_dgcnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 04:31:32.000000 x-dgcnn-0.2.2/x_dgcnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 04:31:32.000000 x-dgcnn-0.2.2/x_dgcnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:57:37.646911 x-dgcnn-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-10 18:57:25.000000 x-dgcnn-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-10 18:57:37.646911 x-dgcnn-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-10 18:57:25.000000 x-dgcnn-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:57:37.646911 x-dgcnn-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-10 18:57:25.000000 x-dgcnn-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:57:37.646911 x-dgcnn-0.3.0/x_dgcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-10 18:57:25.000000 x-dgcnn-0.3.0/x_dgcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-07-10 18:57:25.000000 x-dgcnn-0.3.0/x_dgcnn/dgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-10 18:57:25.000000 x-dgcnn-0.3.0/x_dgcnn/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:57:37.646911 x-dgcnn-0.3.0/x_dgcnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-10 18:57:37.000000 x-dgcnn-0.3.0/x_dgcnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-10 18:57:37.000000 x-dgcnn-0.3.0/x_dgcnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:57:37.000000 x-dgcnn-0.3.0/x_dgcnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 18:57:37.000000 x-dgcnn-0.3.0/x_dgcnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 18:57:37.000000 x-dgcnn-0.3.0/x_dgcnn.egg-info/top_level.txt
```

### Comparing `x-dgcnn-0.2.2/LICENSE` & `x-dgcnn-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.2.2/PKG-INFO` & `x-dgcnn-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.2.2
+Version: 0.3.0
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `x-dgcnn-0.2.2/README.md` & `x-dgcnn-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -35,28 +35,29 @@
 
 Classification.
 
 ```python
 import torch
 from x_dgcnn import DGCNN_Cls
 
-model = DGCNN_Cls(k=20, in_dim=3, out_dim=10)
+model = DGCNN_Cls(3, 10, 20)
 x = torch.randn(8, 3, 2048)
 xyz = x.clone()
 out = model(x, xyz)
 
 ```
 
 Semantic segmentation.
 
 ```python
 import torch
 from x_dgcnn import DGCNN_Seg
 
-model = DGCNN_Seg(k=40, in_dim=3, out_dim=10)
+# model = DGCNN_Seg(3, 10, 40, global_pooling=False)    # disable global pooling if batch size is too small
+model = DGCNN_Seg(3, 10, 40)
 x = torch.randn(8, 3, 2048)
 xyz = x.clone()
 out = model(x, xyz)
 ```
 
 Part segmentation.
```

### Comparing `x-dgcnn-0.2.2/setup.py` & `x-dgcnn-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='x-dgcnn',
     packages=find_packages(),
-    version='0.2.2',
+    version='0.3.0',
     license='MIT',
     description='X-DGCNN - Pytorch',
     author='Kaidi Shen',
     url='https://github.com/kentechx/x-dgcnn',
     long_description_content_type='text/markdown',
     keywords=[
         '3D segmentation',
```

### Comparing `x-dgcnn-0.2.2/x_dgcnn/dgcnn.py` & `x-dgcnn-0.3.0/x_dgcnn/dgcnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 
 
 def knn(x, y=None, k=1):
     # x: (b, d, n)
     # y: (b, d, m)
     if __KEOPS__:
         x_i = LazyTensor(rearrange(x, 'b d n -> b n 1 d').contiguous())
-        y_j = LazyTensor(rearrange(y, 'b d m -> b 1 m d').contiguous() if exists(y) else rearrange(x, 'b d n -> b 1 n d').contiguous())
+        y_j = LazyTensor(rearrange(y, 'b d m -> b 1 m d').contiguous()
+                         if exists(y) else rearrange(x, 'b d n -> b 1 n d').contiguous())
         D_ij = ((x_i - y_j) ** 2).sum(-1)  # (b, n, m)
         neighbor_ind = D_ij.argKmin(k, axis=2)  # (b, n, k)
     else:
         neighbor_ind = cdist(x, y).topk(k, dim=-1, largest=False)[1]  # (b, n, k)
     return neighbor_ind
 
 
@@ -129,18 +130,18 @@
         x = self.head(x)  # (b, 1024) -> (b, 9)
         return x
 
 
 class DGCNN_Cls(nn.Module):
     def __init__(
             self,
-            *,
-            k,
             in_dim,
             out_dim,
+            k,
+            *,
             dims=(64, 64, 128, 256),
             emb_dim=1024,
             dynamic=True,
             dropout=0,
             head_norm=True,  # if using norm in head, disable it if the batch size is 1
     ):
         super().__init__()
@@ -196,52 +197,54 @@
 
         return x
 
 
 class DGCNN_Seg(nn.Module):
     def __init__(
             self,
-            *,
-            k,
             in_dim,
             out_dim,
+            k,
+            *,
             emb_dim=1024,
             n_category=0,
             depth=3,
             stn: SpatialTransformNet = None,
-            head_norm=True,
+            global_pooling=True,  # disable global pooling if the batch size is very small
             dynamic=True,
             dropout=0,
     ):
         super().__init__()
         self.k = k
         self.dynamic = dynamic
+        self.global_pooling = global_pooling
 
         # if using stn, put other features behind xyz
         self.stn = stn
 
         # EdgeConv blocks
         assert depth >= 2, 'depth must be >= 2'
         self.blocks = nn.ModuleList(
             [EdgeConv(k=k, dims=(in_dim, 64, 64))]
         )
         for _ in range(depth - 2):
             self.blocks.append(EdgeConv(k=k, dims=(64, 64, 64)))
         self.blocks.append(EdgeConv(k=k, dims=(64, 64)))
 
         # global linear
-        self.lin = nn.Conv1d(depth * 64, emb_dim, 1, bias=False)
-        self.norm = nn.BatchNorm1d(emb_dim) if head_norm else nn.Identity()
-        self.act = nn.GELU()
-        self.dropout = nn.Dropout(dropout) if dropout > 0 else nn.Identity()
+        if global_pooling:
+            self.lin1 = nn.Conv1d(depth * 64, emb_dim, 1, bias=False)
+            self.norm1 = nn.BatchNorm1d(emb_dim)
+            self.act1 = nn.GELU()
+            self.lin2 = nn.Linear(emb_dim, 512, bias=False)
+            self.norm2 = nn.BatchNorm1d(512)
 
         # head
-        dim = emb_dim + depth * 64
+        self.lin3 = nn.Conv1d(depth * 64, 512, 1, bias=False)
         self.mlp = nn.Sequential(
-            nn.Conv1d(dim, 512, 1, bias=False),
             nn.BatchNorm1d(512),
             nn.GELU(),
             nn.Dropout(dropout) if dropout > 0 else nn.Identity(),
             nn.Conv1d(512, 256, 1, bias=False),
             nn.BatchNorm1d(256),
             nn.GELU(),
             nn.Dropout(dropout) if dropout > 0 else nn.Identity(),
@@ -271,21 +274,23 @@
 
         xs = [self.blocks[0](x, neighbor_ind)]
         for block in self.blocks[1:]:
             x = block(xs[-1], None if self.dynamic else neighbor_ind)
             xs.append(x)
         x = torch.cat(xs, dim=1)  # (b, depth * 64, n)
 
-        # global feature
-        x = self.lin(x)  # (b, d2, n) -> (b, emb_dim, n)
-        x = x.max(-1)[0]  # (b, emb_dim, n) -> (b, emb_dim)
-        x = self.dropout(self.act(self.norm(x)))  # (b, emb_dim)
-
-        # local feature
-        x = repeat(x, 'b d -> b d n', n=n)  # (b, emb_dim) -> (b, emb_dim, n)
-        x = torch.cat((x, *xs), dim=1)  # (b, emb_dim + depth * 64, n)
+        if self.global_pooling:
+            # global feature
+            xg = self.lin1(x)  # (b, d2, n) -> (b, emb_dim, n)
+            xg = xg.max(-1)[0]  # (b, emb_dim, n) -> (b, emb_dim)
+            xg = self.act1(self.norm1(xg))  # (b, emb_dim)
+            xg = self.norm2(self.lin2(xg))
+            x = xg[..., None] + self.lin3(x)  # (b, emb_dim, n) -> (b, 512, n)
+        else:
+            x = self.lin3(x)  # (b, depth * 64, n) -> (b, 512, n)
+
         x = self.mlp(x)  # (b, emb_dim + depth * 64, n) -> (b, 128, n)
 
         if exists(category):
             x = x + self.category_emb(category).unsqueeze(-1)  # (b, 128, n) -> (b, 128, n)
         x = self.head(x)  # (b, 128, n) -> (b, out_dim, n)
         return x
```

### Comparing `x-dgcnn-0.2.2/x_dgcnn/route.py` & `x-dgcnn-0.3.0/x_dgcnn/route.py`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.2.2/x_dgcnn.egg-info/PKG-INFO` & `x-dgcnn-0.3.0/x_dgcnn.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.2.2
+Version: 0.3.0
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

