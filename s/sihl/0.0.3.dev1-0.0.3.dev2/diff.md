# Comparing `tmp/sihl-0.0.3.dev1.tar.gz` & `tmp/sihl-0.0.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sihl-0.0.3.dev1.tar", max compression
+gzip compressed data, was "sihl-0.0.3.dev2.tar", max compression
```

## Comparing `sihl-0.0.3.dev1.tar` & `sihl-0.0.3.dev2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-07-10 10:23:38.044607 sihl-0.0.3.dev1/LICENSE
--rw-r--r--   0        0        0      894 2023-07-10 10:23:38.044607 sihl-0.0.3.dev1/README.md
--rw-r--r--   0        0        0     1545 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/pyproject.toml
--rw-r--r--   0        0        0      332 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/src/sihl/__init__.py
--rw-r--r--   0        0        0   402648 2023-07-10 10:23:38.048607 sihl-0.0.3.dev1/src/sihl/heads/NotoSansMono-Bold.ttf
--rw-r--r--   0        0        0      233 2023-07-10 10:23:38.048607 sihl-0.0.3.dev1/src/sihl/heads/__init__.py
--rw-r--r--   0        0        0     3154 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/src/sihl/heads/binary_classification.py
--rw-r--r--   0        0        0     3768 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/src/sihl/heads/multiclass_classification.py
--rw-r--r--   0        0        0     4624 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/src/sihl/heads/multilabel_classification.py
--rw-r--r--   0        0        0        0 2023-07-10 10:23:38.052607 sihl-0.0.3.dev1/src/sihl/layers/__init__.py
--rw-r--r--   0        0        0     4573 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/src/sihl/lightning_module.py
--rw-r--r--   0        0        0      549 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/src/sihl/sihl_model.py
--rw-r--r--   0        0        0     2797 2023-07-10 10:23:38.052607 sihl-0.0.3.dev1/src/sihl/timm_backbone.py
--rw-r--r--   0        0        0     6470 2023-07-10 10:23:38.052607 sihl-0.0.3.dev1/src/sihl/torchvision_backbone.py
--rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 sihl-0.0.3.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 16:34:51.026986 sihl-0.0.3.dev2/LICENSE
+-rw-r--r--   0        0        0      894 2023-07-10 16:34:51.026986 sihl-0.0.3.dev2/README.md
+-rw-r--r--   0        0        0     1545 2023-07-10 16:35:05.995172 sihl-0.0.3.dev2/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-07-10 16:35:05.995172 sihl-0.0.3.dev2/src/sihl/__init__.py
+-rw-r--r--   0        0        0   402648 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/heads/NotoSansMono-Bold.ttf
+-rw-r--r--   0        0        0      233 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/heads/__init__.py
+-rw-r--r--   0        0        0     3154 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/heads/binary_classification.py
+-rw-r--r--   0        0        0     3768 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/heads/multiclass_classification.py
+-rw-r--r--   0        0        0     4624 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/heads/multilabel_classification.py
+-rw-r--r--   0        0        0        0 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/layers/__init__.py
+-rw-r--r--   0        0        0     4573 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/lightning_module.py
+-rw-r--r--   0        0        0      549 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/sihl_model.py
+-rw-r--r--   0        0        0     2797 2023-07-10 16:34:51.030985 sihl-0.0.3.dev2/src/sihl/timm_backbone.py
+-rw-r--r--   0        0        0     6460 2023-07-10 16:35:05.995172 sihl-0.0.3.dev2/src/sihl/torchvision_backbone.py
+-rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 sihl-0.0.3.dev2/PKG-INFO
```

### Comparing `sihl-0.0.3.dev1/LICENSE` & `sihl-0.0.3.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev1/README.md` & `sihl-0.0.3.dev2/README.md`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev1/pyproject.toml` & `sihl-0.0.3.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sihl"
-version = "0.0.3-dev1"
+version = "0.0.3-dev2"
 description = "Simple Image Heads and Layers"
 authors = ["jonregef <jon.regef@pm.me>"]
 readme = "README.md"
 license = "MIT"
 # homepage = "https://github.com/sihlAI/sihl"
 # repository = "https://github.com/sihlAI/sihl"
```

### Comparing `sihl-0.0.3.dev1/src/sihl/heads/NotoSansMono-Bold.ttf` & `sihl-0.0.3.dev2/src/sihl/heads/NotoSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev1/src/sihl/heads/binary_classification.py` & `sihl-0.0.3.dev2/src/sihl/heads/binary_classification.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev1/src/sihl/heads/multiclass_classification.py` & `sihl-0.0.3.dev2/src/sihl/heads/multiclass_classification.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev1/src/sihl/heads/multilabel_classification.py` & `sihl-0.0.3.dev2/src/sihl/heads/multilabel_classification.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev1/src/sihl/lightning_module.py` & `sihl-0.0.3.dev2/src/sihl/lightning_module.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev1/src/sihl/sihl_model.py` & `sihl-0.0.3.dev2/src/sihl/sihl_model.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev1/src/sihl/timm_backbone.py` & `sihl-0.0.3.dev2/src/sihl/timm_backbone.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev1/src/sihl/torchvision_backbone.py` & `sihl-0.0.3.dev2/src/sihl/torchvision_backbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,14 @@
     matches_module_pattern,
     replace_node_module,
 )
 from torch.nn import functional as F
 from torchvision.models.feature_extraction import create_feature_extractor
 
 
-__all__ = ["TorchvisionBackbone"]
-
-
 @torch.no_grad()
 def update_input_channels(
     fx_module: fx.GraphModule, in_channels: int  # type:ignore
 ) -> None:
     modules = dict(fx_module.named_modules())
     first_conv_node = next(
         node
@@ -50,15 +47,15 @@
 class Normalize(nn.Module):
     def __init__(self, mean: tuple[float, ...], std: tuple[float, ...]) -> None:
         super().__init__()
         self.register_buffer("mean", torch.tensor(mean).reshape(1, -1, 1, 1))
         self.register_buffer("std", torch.tensor(std).reshape(1, -1, 1, 1))
 
     def forward(self, x: Tensor) -> Tensor:
-        return (x - self.mean) / self.std
+        return (x - self.mean.to(x.device)) / self.std.to(x.device)
 
 
 class PadToMultipleOf(nn.Module):
     def __init__(self, n: int) -> None:
         super().__init__()
         self.n = n
```

### Comparing `sihl-0.0.3.dev1/PKG-INFO` & `sihl-0.0.3.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sihl
-Version: 0.0.3.dev1
+Version: 0.0.3.dev2
 Summary: Simple Image Heads and Layers
 License: MIT
 Author: jonregef
 Author-email: jon.regef@pm.me
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

