# Comparing `tmp/sihl-0.0.3.dev0.tar.gz` & `tmp/sihl-0.0.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sihl-0.0.3.dev0.tar", max compression
+gzip compressed data, was "sihl-0.0.3.dev1.tar", max compression
```

## Comparing `sihl-0.0.3.dev0.tar` & `sihl-0.0.3.dev1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-06-26 10:00:27.512373 sihl-0.0.3.dev0/LICENSE
--rw-r--r--   0        0        0      894 2023-06-26 10:00:44.648576 sihl-0.0.3.dev0/README.md
--rw-r--r--   0        0        0     1487 2023-06-26 10:00:44.652576 sihl-0.0.3.dev0/pyproject.toml
--rw-r--r--   0        0        0       77 2023-06-26 10:00:44.652576 sihl-0.0.3.dev0/src/sihl/__init__.py
--rw-r--r--   0        0        0   402648 2023-06-26 10:00:44.656576 sihl-0.0.3.dev0/src/sihl/heads/NotoSansMono-Bold.ttf
--rw-r--r--   0        0        0      233 2023-06-26 10:00:27.520373 sihl-0.0.3.dev0/src/sihl/heads/__init__.py
--rw-r--r--   0        0        0     3148 2023-06-26 10:00:44.656576 sihl-0.0.3.dev0/src/sihl/heads/binary_classification.py
--rw-r--r--   0        0        0     3802 2023-06-26 10:00:44.656576 sihl-0.0.3.dev0/src/sihl/heads/multiclass_classification.py
--rw-r--r--   0        0        0     4658 2023-06-26 10:00:44.656576 sihl-0.0.3.dev0/src/sihl/heads/multilabel_classification.py
--rw-r--r--   0        0        0     3424 2023-06-26 10:00:44.656576 sihl-0.0.3.dev0/src/sihl/lightning_module.py
--rw-r--r--   0        0        0     6156 2023-06-26 10:00:44.656576 sihl-0.0.3.dev0/src/sihl/torchvision_backbone.py
--rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 sihl-0.0.3.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 10:23:38.044607 sihl-0.0.3.dev1/LICENSE
+-rw-r--r--   0        0        0      894 2023-07-10 10:23:38.044607 sihl-0.0.3.dev1/README.md
+-rw-r--r--   0        0        0     1545 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/pyproject.toml
+-rw-r--r--   0        0        0      332 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/src/sihl/__init__.py
+-rw-r--r--   0        0        0   402648 2023-07-10 10:23:38.048607 sihl-0.0.3.dev1/src/sihl/heads/NotoSansMono-Bold.ttf
+-rw-r--r--   0        0        0      233 2023-07-10 10:23:38.048607 sihl-0.0.3.dev1/src/sihl/heads/__init__.py
+-rw-r--r--   0        0        0     3154 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/src/sihl/heads/binary_classification.py
+-rw-r--r--   0        0        0     3768 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/src/sihl/heads/multiclass_classification.py
+-rw-r--r--   0        0        0     4624 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/src/sihl/heads/multilabel_classification.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:23:38.052607 sihl-0.0.3.dev1/src/sihl/layers/__init__.py
+-rw-r--r--   0        0        0     4573 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/src/sihl/lightning_module.py
+-rw-r--r--   0        0        0      549 2023-07-10 10:23:51.776796 sihl-0.0.3.dev1/src/sihl/sihl_model.py
+-rw-r--r--   0        0        0     2797 2023-07-10 10:23:38.052607 sihl-0.0.3.dev1/src/sihl/timm_backbone.py
+-rw-r--r--   0        0        0     6470 2023-07-10 10:23:38.052607 sihl-0.0.3.dev1/src/sihl/torchvision_backbone.py
+-rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 sihl-0.0.3.dev1/PKG-INFO
```

### Comparing `sihl-0.0.3.dev0/LICENSE` & `sihl-0.0.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev0/README.md` & `sihl-0.0.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev0/pyproject.toml` & `sihl-0.0.3.dev1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sihl"
-version = "0.0.3-dev"
+version = "0.0.3-dev1"
 description = "Simple Image Heads and Layers"
 authors = ["jonregef <jon.regef@pm.me>"]
 readme = "README.md"
 license = "MIT"
 # homepage = "https://github.com/sihlAI/sihl"
 # repository = "https://github.com/sihlAI/sihl"
 
@@ -25,14 +25,15 @@
 coverage = "^7.2.5"
 isort = "^5.12.0"
 pyupgrade = "^3.3.2"
 kaggle = "^1.5.13"
 torchinfo = "^1.7.2"
 lightning = "^2.0.2"
 tensorboard = "^2.13.0"
+types-pyyaml = "^6.0.12.10"
 
 [tool.poetry.extras]
 lightning = ["lightning"]
 timm = ["timm"]
 all = ["lightning", "timm"]
 
 [build-system]
@@ -49,19 +50,20 @@
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 90
 
 [tool.isort]
 profile = "black"
-force_single_line = true
+force_single_line = false
 lines_after_imports = 2
 
 [tool.mypy]
 strict = true
 warn_unreachable = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 ignore_missing_imports = true
-warn_unused_ignores = true
+no_warn_unused_ignores = true
+implicit_reexport = true
```

### Comparing `sihl-0.0.3.dev0/src/sihl/heads/NotoSansMono-Bold.ttf` & `sihl-0.0.3.dev1/src/sihl/heads/NotoSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev0/src/sihl/heads/binary_classification.py` & `sihl-0.0.3.dev1/src/sihl/heads/binary_classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 
+
 try:
-    from importlib_resources import files, as_file
+    from importlib_resources import as_file, files
 except ImportError:
     from importlib.resources import files, as_file  # type: ignore
 
 import torch
 import torchmetrics
-from torch import Tensor
-from torch import nn
+from torch import Tensor, nn
 from torchvision.utils import draw_bounding_boxes
 
 
 class BinaryClassification(nn.Module):
     def __init__(
-        self, in_channels: int, level: int = -1, question: str = "true?"
+        self, in_channels: list[int], level: int = -1, question: str = "positive?"
     ) -> None:
         super().__init__()
+        self.level = level
         self.net = nn.Sequential(
-            nn.AdaptiveAvgPool2d(1), nn.Flatten(), nn.Linear(in_channels, 1)
+            nn.AdaptiveAvgPool2d(1), nn.Flatten(), nn.Linear(in_channels[self.level], 1)
         )
-        self.level = level
         self.question = question
 
     def forward(self, inputs: list[Tensor]) -> tuple[Tensor, Tensor]:
         scores = torch.sigmoid(self.net(inputs[self.level])).squeeze(-1)
         return scores, scores > 0.5
 
     def training_step(
```

### Comparing `sihl-0.0.3.dev0/src/sihl/heads/multiclass_classification.py` & `sihl-0.0.3.dev1/src/sihl/heads/multiclass_classification.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from __future__ import annotations
 
+
 try:
-    from importlib_resources import files, as_file
+    from importlib_resources import as_file, files
 except ImportError:
     from importlib.resources import files, as_file  # type: ignore
 
 import torch
-from torch import Tensor
-from torch import nn
-from torchmetrics.classification import MulticlassAccuracy
-from torchmetrics.classification import MulticlassPrecision
-from torchmetrics.classification import MulticlassRecall
+from torch import Tensor, nn
+from torchmetrics.classification import (
+    MulticlassAccuracy,
+    MulticlassPrecision,
+    MulticlassRecall,
+)
 from torchvision.utils import draw_bounding_boxes
 
 
 class MulticlassClassification(nn.Module):
     def __init__(
         self,
-        in_channels: int,
+        in_channels: list[int],
         num_classes: int,
         level: int = -1,
         class_names: tuple[str, ...] | None = None,
         label_weights: tuple[float, ...] | None = None,
         label_smoothing: float = 0.0,
     ) -> None:
         super().__init__()
         self.num_classes = num_classes
         self.level = level
         self.class_names = class_names or tuple(map(str, range(num_classes)))
         self.label_weights = torch.tensor(label_weights) if label_weights else None
         self.label_smoothing = label_smoothing
         self.net = nn.Sequential(
-            nn.AdaptiveAvgPool2d(1), nn.Flatten(), nn.Linear(in_channels, num_classes)
+            nn.AdaptiveAvgPool2d(1),
+            nn.Flatten(),
+            nn.Linear(in_channels[self.level], num_classes),
         )
 
     def forward(self, inputs: list[Tensor]) -> tuple[Tensor, Tensor]:
         scores, classes = torch.max(
             torch.nn.functional.softmax(self.net(inputs[self.level]), dim=1), dim=1
         )
         return scores, classes
```

### Comparing `sihl-0.0.3.dev0/src/sihl/heads/multilabel_classification.py` & `sihl-0.0.3.dev1/src/sihl/heads/multilabel_classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 from __future__ import annotations
 
+
 try:
-    from importlib_resources import files, as_file
+    from importlib_resources import as_file, files
 except ImportError:
     from importlib.resources import files, as_file  # type: ignore
 
 import torch
-from torch import Tensor
-from torch import nn
-from torchmetrics.classification import MultilabelAccuracy
-from torchmetrics.classification import MultilabelPrecision
-from torchmetrics.classification import MultilabelRecall
+from torch import Tensor, nn
+from torchmetrics.classification import (
+    MultilabelAccuracy,
+    MultilabelPrecision,
+    MultilabelRecall,
+)
 from torchvision.utils import draw_bounding_boxes
 
 
 class MultilabelClassification(nn.Module):
     def __init__(
         self,
-        in_channels: int,
+        in_channels: list[int],
         num_classes: int,
         level: int = -1,
         class_names: tuple[str, ...] | None = None,
         label_weights: list[float] | None = None,
     ) -> None:
         super().__init__()
         self.num_classes = num_classes
         self.level = level
         self.class_names = class_names or tuple(map(str, range(num_classes)))
         self.label_weights = torch.tensor(label_weights) if label_weights else None
         self.net = nn.Sequential(
-            nn.AdaptiveAvgPool2d(1), nn.Flatten(), nn.Linear(in_channels, num_classes)
+            nn.AdaptiveAvgPool2d(1),
+            nn.Flatten(),
+            nn.Linear(in_channels[self.level], num_classes),
         )
 
     def forward(self, inputs: list[Tensor]) -> tuple[Tensor, Tensor]:
         scores, classes = torch.sort(
             torch.sigmoid(self.net(inputs[self.level])), descending=True
         )
         return scores, classes
```

### Comparing `sihl-0.0.3.dev0/src/sihl/torchvision_backbone.py` & `sihl-0.0.3.dev1/src/sihl/torchvision_backbone.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 from typing import Final
 
 import torch
 import torchvision
-from torch import Tensor
-from torch import fx
-from torch import nn
-from torch.fx.experimental.optimization import matches_module_pattern
-from torch.fx.experimental.optimization import replace_node_module
+from torch import Tensor, fx, nn
+from torch.fx.experimental.optimization import (
+    matches_module_pattern,
+    replace_node_module,
+)
+from torch.nn import functional as F
 from torchvision.models.feature_extraction import create_feature_extractor
 
 
 __all__ = ["TorchvisionBackbone"]
 
 
 @torch.no_grad()
@@ -52,14 +53,30 @@
         self.register_buffer("mean", torch.tensor(mean).reshape(1, -1, 1, 1))
         self.register_buffer("std", torch.tensor(std).reshape(1, -1, 1, 1))
 
     def forward(self, x: Tensor) -> Tensor:
         return (x - self.mean) / self.std
 
 
+class PadToMultipleOf(nn.Module):
+    def __init__(self, n: int) -> None:
+        super().__init__()
+        self.n = n
+
+    def forward(self, x: Tensor) -> Tensor:
+        pad_x = (self.n - x.shape[3] % self.n) % self.n
+        pad_y = (self.n - x.shape[2] % self.n) % self.n
+        return F.pad(
+            x,
+            (pad_x // 2, pad_x - pad_x // 2, pad_y // 2, pad_y - pad_y // 2),
+            "constant",
+            0,
+        )
+
+
 class TorchvisionBackbone(nn.Module):
     all_level_names: Final[dict[str, list[str]]] = {
         "efficientnet_b0": [f"features.{_}" for _ in (1, 2, 3, 5, 8)],
         "efficientnet_b1": [f"features.{_}" for _ in (1, 2, 3, 5, 8)],
         "efficientnet_b2": [f"features.{_}" for _ in (1, 2, 3, 5, 8)],
         "efficientnet_b3": [f"features.{_}" for _ in (1, 2, 3, 5, 8)],
         "efficientnet_b4": [f"features.{_}" for _ in (1, 2, 3, 5, 8)],
@@ -92,49 +109,49 @@
         frozen_levels: int = 0,
     ) -> None:
         super().__init__()
         self.name = name
         try:
             level_names = self.all_level_names[name]
         except KeyError as error:
-            raise KeyError(
+            raise ValueError(
                 f"Architecture {name} is not supported. "
                 f"Select from {list(self.all_level_names.keys())}"
             ) from error
         self.normalize = (
             Normalize(mean=(0.485, 0.456, 0.406), std=(0.229, 0.224, 0.225))
             if pretrained and input_channels == 3
             else Normalize(mean=(0.5,), std=(0.5,))
         )
-        torchvision_model = torchvision.models.get_model(
+        self.model = torchvision.models.get_model(
             name, weights="DEFAULT" if pretrained else None
         )
-        torchvision_model = create_feature_extractor(torchvision_model, level_names)
-        torchvision_model = fx.symbolic_trace(torchvision_model)  # type: ignore
-        update_input_channels(torchvision_model, input_channels)
+        self.model = create_feature_extractor(self.model, level_names)
+        self.model = fx.symbolic_trace(self.model)  # type: ignore
+        update_input_channels(self.model, input_channels)
+        self.pad = PadToMultipleOf(32)
         # freeze modules in first `frozen_levels` levels
-        torchvision_model.eval()  # freeze batchnorms
+        self.model.eval()  # freeze batchnorms
         if frozen_levels < 0:
-            for module_name, _ in torchvision_model.named_modules():
-                for param in torchvision_model.get_submodule(module_name).parameters():
+            for module_name, _ in self.model.named_modules():
+                for param in self.model.get_submodule(module_name).parameters():
                     param.requires_grad = False
         elif frozen_levels > 0:
             last_frozen_name = level_names[min(frozen_levels, len(level_names)) - 1]
             last_level_reached = False
             freezing = True
-            for module_name, _ in torchvision_model.named_modules():
+            for module_name, _ in self.model.named_modules():
                 if module_name == "":
                     continue
                 if module_name == last_frozen_name:
                     last_level_reached = True
                 if last_level_reached and last_frozen_name not in module_name:
                     freezing = False
-                for param in torchvision_model.get_submodule(module_name).parameters():
+                for param in self.model.get_submodule(module_name).parameters():
                     param.requires_grad = not freezing
-        setattr(self, name, torchvision_model)
-        self.dummy_input = torch.empty((1, input_channels, 64, 64))
-        self.output_channels = [input_channels] + [
-            _.shape[1] for _ in getattr(self, name)(self.dummy_input).values()
+        self.dummy_input = torch.zeros((1, input_channels, 64, 64))
+        self.out_channels = [input_channels] + [
+            _.shape[1] for _ in self.model(self.dummy_input).values()
         ]
 
     def forward(self, x: Tensor) -> list[Tensor]:
-        return [x] + list(getattr(self, self.name)(self.normalize(x)).values())
+        return [x] + list(self.model(self.pad(self.normalize(x))).values())
```

### Comparing `sihl-0.0.3.dev0/PKG-INFO` & `sihl-0.0.3.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sihl
-Version: 0.0.3.dev0
+Version: 0.0.3.dev1
 Summary: Simple Image Heads and Layers
 License: MIT
 Author: jonregef
 Author-email: jon.regef@pm.me
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

