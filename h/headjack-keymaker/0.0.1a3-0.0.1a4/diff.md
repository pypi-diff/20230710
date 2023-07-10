# Comparing `tmp/headjack_keymaker-0.0.1a3.tar.gz` & `tmp/headjack_keymaker-0.0.1a4.tar.gz`

## Comparing `headjack_keymaker-0.0.1a3.tar` & `headjack_keymaker-0.0.1a4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/Makefile
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/netlify.toml
--rw-r--r--   0        0        0   140632 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/pdm.lock
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.github/workflows/python-checks.yml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.pdm-build/.gitignore
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.pdm-build/keymaker.pth
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.pdm-build/keymaker-0.1.0+editable.dist-info/WHEEL
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/.hugo_build.lock
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/README.md
--rwxr-xr-x   0        0        0     1085 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/build-docs.sh
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/archetypes/default.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/assets/jsconfig.json
--rw-r--r--   0        0        0   133768 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/assets/images/keymaker logo.png
--rw-r--r--   0        0        0    28606 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/assets/images/keymaker logo.svg
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/config/_default/config.toml
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/config/_default/markup.toml
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/config/_default/menu.toml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/config/_default/outputs.toml
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/config/_default/params.toml
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/content/0.1.0/contributing.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/content/0.1.0/getting-started.md
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/content/0.1.0/questions-&-commands.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/content/0.1.0/posts/theme-doc/post.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/content/versions/_index.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/layouts/taxonomy/list.html
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/__about__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/__init__.py
--rw-r--r--   0        0        0     9869 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/prompt.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/types.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/__init__.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/base.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/logical.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/options.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/parser.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/regex.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/stops.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/models/__init__.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/models/base.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/models/huggingface.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/models/llama_cpp.py
--rw-r--r--   0        0        0    12011 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/models/openai.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/utils/__init__.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/utils/chat.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.gitignore
--rw-r--r--   0        0        0    18815 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/README.md
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0    19666 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/Makefile
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/netlify.toml
+-rw-r--r--   0        0        0   140632 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/pdm.lock
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.github/workflows/python-checks.yml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.pdm-build/.gitignore
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.pdm-build/keymaker.pth
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.pdm-build/keymaker-0.1.0+editable.dist-info/WHEEL
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/.hugo_build.lock
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/README.md
+-rwxr-xr-x   0        0        0     1085 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/build-docs.sh
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/archetypes/default.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/assets/jsconfig.json
+-rw-r--r--   0        0        0   133768 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/assets/images/keymaker logo.png
+-rw-r--r--   0        0        0    28606 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/assets/images/keymaker logo.svg
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/config/_default/config.toml
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/config/_default/markup.toml
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/config/_default/menu.toml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/config/_default/outputs.toml
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/config/_default/params.toml
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/content/0.1.0/contributing.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/content/0.1.0/getting-started.md
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/content/0.1.0/questions-&-commands.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/content/0.1.0/posts/theme-doc/post.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/content/versions/_index.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/docs/layouts/taxonomy/list.html
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/__about__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/__init__.py
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/prompt.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/types.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/__init__.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/base.py
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/logical.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/options.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/parser.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/regex.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/constraints/stops.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/models/__init__.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/models/base.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/models/huggingface.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/models/llama_cpp.py
+-rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/models/openai.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/utils/__init__.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/keymaker/utils/chat.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/.gitignore
+-rw-r--r--   0        0        0    20350 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/README.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0    21292 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a4/PKG-INFO
```

### Comparing `headjack_keymaker-0.0.1a3/.pre-commit-config.yaml` & `headjack_keymaker-0.0.1a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/pdm.lock` & `headjack_keymaker-0.0.1a4/pdm.lock`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/.github/workflows/python-checks.yml` & `headjack_keymaker-0.0.1a4/.github/workflows/python-checks.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA` & `headjack_keymaker-0.0.1a4/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/docs/build-docs.sh` & `headjack_keymaker-0.0.1a4/docs/build-docs.sh`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/docs/assets/images/keymaker logo.png` & `headjack_keymaker-0.0.1a4/docs/assets/images/keymaker logo.png`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/docs/assets/images/keymaker logo.svg` & `headjack_keymaker-0.0.1a4/docs/assets/images/keymaker logo.svg`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/docs/config/_default/markup.toml` & `headjack_keymaker-0.0.1a4/docs/config/_default/markup.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/docs/config/_default/menu.toml` & `headjack_keymaker-0.0.1a4/docs/config/_default/menu.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/docs/config/_default/params.toml` & `headjack_keymaker-0.0.1a4/docs/config/_default/params.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/docs/content/0.1.0/contributing.md` & `headjack_keymaker-0.0.1a4/docs/content/0.1.0/contributing.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/docs/layouts/taxonomy/list.html` & `headjack_keymaker-0.0.1a4/docs/layouts/taxonomy/list.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/keymaker/prompt.py` & `headjack_keymaker-0.0.1a4/keymaker/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,19 +175,21 @@
             return ret
 
         token_count = 0
         partial_completion = ""
         prompt_plus_completion = text[:]
         gen_tokens = []
         buffer_tokens: List[int] = []
+        constraint_state = None
         while token_count < token_limit:
             token = None
             generation = None
-            selected_token_ids = constraint.constrain_tokens(text, partial_completion, model)
-            
+
+            selected_token_ids, constraint_state = constraint.constrain_tokens(text, partial_completion, model, constraint_state)
+
             if selected_token_ids:
                 # if the selected tokens have the same number than the vocab size, there's no real restriction
                 selected_token_ids = None if len(selected_token_ids) >= model.vocab_size else selected_token_ids
             if isinstance(selected_token_ids, set) and len(selected_token_ids) == 0:
                 warnings.warn(f"Empty token mask encountered with Constraint `{constraint}`. Ending completion.")
                 break
 
@@ -215,15 +217,15 @@
 
                 if not generated_tokens:
                     break
                 gen_tokens = [model.encode(tok)[0] for tok in generated_tokens if tok]
 
                 if not gen_tokens:
                     break
-                
+
                 token = gen_tokens[0]
                 # in case sampling gave us extra tokens (e.g. sample chunk size of the model is more than 1 like for openai chat models)
                 if len(gen_tokens) > 1:
                     buffer_tokens = gen_tokens[1:]
 
             if model.eos_token_id == token:
                 break
```

### Comparing `headjack_keymaker-0.0.1a3/keymaker/types.py` & `headjack_keymaker-0.0.1a4/keymaker/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 '''Common types used throughout keymaker'''
+import warnings
 from dataclasses import dataclass
 from enum import Enum
-from typing import Dict, List, Set, Union, Optional
-import warnings
+from typing import Dict, List, Optional, Set, Union
+
 
 class DecodingStrategy(str, Enum):
     GREEDY = "GREEDY"
     SAMPLE = "SAMPLE"
 
 
 @dataclass
 class Decoder:
     temperature: Optional[float] = None
     top_p: Optional[float] = None
     top_k: Optional[int] = None
     strategy: DecodingStrategy = DecodingStrategy.GREEDY
 
     def __post_init__(self):
-        if self.top_k is not None and self.top_k!=1 and self.strategy == DecodingStrategy.GREEDY:
+        if self.top_k is not None and self.top_k != 1 and self.strategy == DecodingStrategy.GREEDY:
             warnings.warn(f"Greedy decoding top_k {self.top_k} ignored. Setting top_k to 1.")
             self.top_k = 1
 
 
 TokenIds = List[int]
 Tokens = Dict[int, str]
 TokenDistribution = Dict[str, int]
```

### Comparing `headjack_keymaker-0.0.1a3/keymaker/constraints/base.py` & `headjack_keymaker-0.0.1a4/keymaker/constraints/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 """Base Constraint interface"""
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Optional, Tuple
 
 if TYPE_CHECKING:
     from keymaker.models.base import Model
 
 from keymaker.types import TokenConstraint
 
 
 class Constraint(ABC):
     @abstractmethod
-    def constrain_tokens(self, base_text: str, completion_text: str, model: "Model") -> TokenConstraint:
+    def constrain_tokens(
+        self,
+        base_text: str,
+        completion_text: str,
+        model: "Model",
+        state: Optional[Any] = None,
+    ) -> Tuple[TokenConstraint, Any]:
         """Constrain the token ids that can be sampled from the model's vocabulary.
 
-        Args:
-            base_text (str): The text to which the completion_text should be appended.
-            completion_text (str): The text completed thus far; one token will be added between calls
-            model (Model): The language model to be used.
+            Args:
+                base_text (str): The text to which the completion_text should be appended.
+                completion_text (str): The text completed thus far; one token will be added between calls
+                model (Model): The language model to be used.
 
         Returns:
-            None: If no restrictions are to be applied and the full vocabulary can be used.
-            set: The set of valid token ids that can be sampled.
-            str: If the constraint is complete and the str is the finished value, which may not be what was passed as the completion text.
+            A two-tuple:
+                - One of
+                    - None: If no restrictions are to be applied and the full vocabulary can be used.
+                    - Set[int]: The set of valid token ids that can be sampled.
+                    - str: The finished value if the constraint is complete, which may not be the same as the passed completion_text.
+                - Any: The updated state of the constraint, which can be used to modify the behavior of future calls.
         """
 
     def __or__(self, other):
         from keymaker.constraints.logical import OrConstraint
 
         return OrConstraint([self, other])
```

### Comparing `headjack_keymaker-0.0.1a3/keymaker/constraints/logical.py` & `headjack_keymaker-0.0.1a4/keymaker/constraints/logical.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Common logical constraints for combining other constraints"""
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, List, Sequence, Set, Union, cast
+from typing import TYPE_CHECKING, List, Sequence, Tuple, cast
 
 from keymaker.constraints.base import Constraint
 from keymaker.types import TokenConstraint
 
 if TYPE_CHECKING:
     from keymaker.models.base import Model
 
@@ -16,32 +16,44 @@
 
     Attributes:
         constraint (Constraint): The constraint to negate.
     """
 
     constraint: Constraint
 
-    def constrain_tokens(self, base_text: str, completion_text: str, model: "Model") -> TokenConstraint:
+    def constrain_tokens(
+        self,
+        base_text: str,
+        completion_text: str,
+        model: "Model",
+        state: None = None,
+    ) -> Tuple[TokenConstraint, None]:
         selected_tokens = self.constraint.constrain_tokens(base_text, completion_text, model)
         if selected_tokens is None or isinstance(selected_tokens, str):
-            return selected_tokens
-        return {tok for tok in model.tokens if tok not in selected_tokens}
+            return selected_tokens, None
+        return {tok for tok in model.tokens if tok not in selected_tokens}, None
 
 
 @dataclass
 class AndConstraint(Constraint):
     """Constrain token ids that can be sampled by applying multiple constraints.
 
     Attributes:
         constraints (List[Constraint]): The list of constraints to apply.
     """
 
     constraints: Sequence[Constraint]
 
-    def constrain_tokens(self, base_text: str, completion_text: str, model: "Model") -> Union[None, Set[int], str]:
+    def constrain_tokens(
+        self,
+        base_text: str,
+        completion_text: str,
+        model: "Model",
+        state: None = None,
+    ) -> Tuple[TokenConstraint, None]:
         ret = None
         completions: List[str] = []
         for constraint in self.constraints:
             completions = []
             selected_tokens = constraint.constrain_tokens(base_text, completion_text, model)
             if selected_tokens is None:
                 # Do nothing because all tokens are valid
@@ -49,33 +61,39 @@
             if isinstance(selected_tokens, str):
                 completions.append(selected_tokens)
             if isinstance(selected_tokens, set):
                 ret = (cast(set, ret) & selected_tokens) if ret is not None else selected_tokens
         if len(completions) == len(self.constraints):
             if len(set(completions)) != 1:
                 raise ValueError(f"Got different completions for constraints `{self}`. Completions: `{set(completions)}`")
-            return completions[0]
-        return ret
+            return completions[0], None
+        return ret, None
 
 
 @dataclass
 class OrConstraint(Constraint):
     """Constrain token ids that can be sampled by applying multiple constraints.
 
     Attributes:
         constraints (List[Constraint]): The list of constraints to apply.
     """
 
     constraints: Sequence[Constraint]
 
-    def constrain_tokens(self, base_text: str, completion_text: str, model: "Model") -> Union[None, Set[int], str]:
-        ret = set()
+    def constrain_tokens(
+        self,
+        base_text: str,
+        completion_text: str,
+        model: "Model",
+        state: None = None,
+    ) -> Tuple[TokenConstraint, None]:
+        ret = set()  # type: ignore
         for constraint in self.constraints:
             selected_tokens = constraint.constrain_tokens(base_text, completion_text, model)
             if selected_tokens is None:
                 # One allows everything so overall the or does
-                return None
+                return None, None
             if isinstance(selected_tokens, str):
-                return selected_tokens
+                return selected_tokens, None
             if isinstance(selected_tokens, set):
                 ret |= selected_tokens
-        return ret
+        return ret, None
```

### Comparing `headjack_keymaker-0.0.1a3/keymaker/constraints/options.py` & `headjack_keymaker-0.0.1a4/keymaker/constraints/options.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Constraints over sets of fixed options"""
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
-from typing import Set
+from typing import Set, Tuple
 
 from keymaker.constraints.base import Constraint
 from keymaker.models.base import Model
 from keymaker.types import TokenConstraint
 
 
 @dataclass
@@ -17,32 +17,38 @@
     options: Set[str]
     short_circuit: bool = True  # early return when available options based on completed text are <=1
 
     def _is_valid_token(self, token_id: int, partial_completion: str, model: Model) -> bool:
         decoded_token = model.tokens[token_id]
         return any(option.startswith(partial_completion + decoded_token) for option in self.options)
 
-    def constrain_tokens(self, base_text: str, completion_text: str, model: Model) -> TokenConstraint:
+    def constrain_tokens(
+        self,
+        base_text: str,
+        completion_text: str,
+        model: Model,
+        state: None = None,
+    ) -> Tuple[TokenConstraint, None]:
         if completion_text in self.options:
-            return completion_text
+            return completion_text, None
 
         if completion_text and self.short_circuit:
             limited_options = set()
             for option in self.options:
                 if option.startswith(completion_text):
                     limited_options.add(option)
                     if len(limited_options) > 1:
                         break
             if len(limited_options) == 0:
-                return set()
+                return set(), None
             if len(limited_options) == 1:
-                return limited_options.pop()
+                return limited_options.pop(), None
 
         with ThreadPoolExecutor():
             valid_token_ids = set(
                 filter(
                     lambda token_id: self._is_valid_token(token_id, completion_text, model),
                     model.tokens.keys(),
                 ),
             )
 
-        return valid_token_ids
+        return valid_token_ids, None
```

### Comparing `headjack_keymaker-0.0.1a3/keymaker/constraints/regex.py` & `headjack_keymaker-0.0.1a4/keymaker/constraints/regex.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Constraints for regex patterns"""
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
-from typing import Union
+from typing import Tuple, Union
 
 import regex as re
 
 from keymaker.constraints.base import Constraint
 from keymaker.models.base import Model
 from keymaker.types import TokenConstraint
 
@@ -27,22 +27,28 @@
     def __post_init__(self):
         self._pattern: re.Pattern[str] = re.compile(self.pattern) if isinstance(self.pattern, str) else self.pattern
 
     def _is_valid_token(self, token_id: int, partial_completion: str, model: "Model") -> bool:
         decoded_token = model.tokens[token_id]
         return self._pattern.fullmatch(partial_completion + decoded_token, partial=True)
 
-    def constrain_tokens(self, base_text: str, completion_text: str, model: "Model") -> TokenConstraint:
+    def constrain_tokens(
+        self,
+        base_text: str,
+        completion_text: str,
+        model: "Model",
+        state: None = None,
+    ) -> Tuple[TokenConstraint, None]:
         if self.terminate_on_match:
             m = self._pattern.match(completion_text)
             if m and m.start() == 0:
-                return completion_text
+                return completion_text, None
 
         with ThreadPoolExecutor():
             valid_token_ids = set(
                 filter(
                     lambda token_id: self._is_valid_token(token_id, completion_text, model),
                     model.tokens.keys(),
                 ),
             )
 
-        return valid_token_ids
+        return valid_token_ids, None
```

### Comparing `headjack_keymaker-0.0.1a3/keymaker/constraints/stops.py` & `headjack_keymaker-0.0.1a4/keymaker/constraints/stops.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Constraints for stop patterns"""
 from dataclasses import dataclass
+from typing import Tuple
 
 import regex as re
 
 from keymaker.constraints.base import Constraint
 from keymaker.models.base import Model
 from keymaker.types import TokenConstraint
 
@@ -19,14 +20,20 @@
 
     stop: str
     include: bool = True
 
     def __post_init__(self):
         self._pattern = re.compile(rf"(?P<completion>.*?)(?P<stop>{self.stop})")
 
-    def constrain_tokens(self, base_text: str, completion_text: str, model: Model) -> TokenConstraint:
+    def constrain_tokens(
+        self,
+        base_text: str,
+        completion_text: str,
+        model: Model,
+        state: None = None,
+    ) -> Tuple[TokenConstraint, None]:
         match = self._pattern.search(completion_text)
         if match:
             if not self.include:
-                return match.group('completion')
-            return match.group('completion') + match.group('stop')
-        return None
+                return match.group('completion'), None
+            return match.group('completion') + match.group('stop'), None
+        return None, None
```

### Comparing `headjack_keymaker-0.0.1a3/keymaker/models/__init__.py` & `headjack_keymaker-0.0.1a4/keymaker/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 try:
     from .huggingface import Huggingface  # noqa: F401
 except ImportError:
     pass
 from .openai import OpenAIChat, OpenAICompletion
+
 try:
-    from .llama_cpp import LlamaCpp #noqa: F401
+    from .llama_cpp import LlamaCpp  # noqa: F401
 except ImportError:
     pass
 
 
 def chatgpt(completion: bool = False, *args, **kwargs):
     if completion:
         return OpenAICompletion(model_name="gpt-3.5-turbo", max_total_tokens=4000, *args, **kwargs)  # type: ignore
```

### Comparing `headjack_keymaker-0.0.1a3/keymaker/models/base.py` & `headjack_keymaker-0.0.1a4/keymaker/models/base.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/keymaker/models/huggingface.py` & `headjack_keymaker-0.0.1a4/keymaker/models/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         if (self.model is not None and self.tokenizer is None) or (self.model is None and self.tokenizer is not None):
             raise ValueError("must specify either `model_name` or both `model` and `tokenizer`")
         self.model = self.model or AutoModelForCausalLM.from_pretrained(self.model_name)
         self.tokenizer = self.tokenizer or AutoTokenizer.from_pretrained(self.model_name)
         self.tokens = transformers_tokens(self.tokenizer)
 
     def encode(self, text: str) -> TokenIds:
-        return self.tokenizer.encode(text, add_special_tokens = True)  # type: ignore
+        return self.tokenizer.encode(text, add_special_tokens=True)  # type: ignore
 
     def decode(self, ids: TokenIds) -> str:
         return self.tokenizer.decode(ids)  # type: ignore
 
     @property
     def eos_token_id(self) -> int:
         return self.tokenizer.eos_token_id  # type: ignore
@@ -79,19 +79,19 @@
         decoder: Optional[Decoder] = None,
         timeout: float = 10.0,
     ) -> AsyncGenerator[str, None]:
         decoder = decoder or Decoder()
         if decoder.strategy not in self.supported_decodings:
             raise ValueError(f"Unsupported decoding strategy for Huggingface model `{decoder.strategy}`.")
         gen_kwargs = {}
-        if temperature:= decoder.temperature:
+        if temperature := decoder.temperature:
             gen_kwargs['temperature'] = temperature
-        if top_p:= decoder.top_p:
+        if top_p := decoder.top_p:
             gen_kwargs['top_p'] = top_p
-        if top_k:= decoder.top_k:
+        if top_k := decoder.top_k:
             gen_kwargs['top_k'] = top_k
 
         if decoder.strategy == DecodingStrategy.SAMPLE:
             gen_kwargs["do_sample"] = True
 
         n_gen = 0
         prompt_token_ids = self.tokenizer.encode(text)  # type: ignore
```

### Comparing `headjack_keymaker-0.0.1a3/keymaker/models/llama_cpp.py` & `headjack_keymaker-0.0.1a4/keymaker/models/llama_cpp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 """A model for use with an in-memory Llama Cpp"""
 
-import asyncio
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, AsyncGenerator, FrozenSet, Optional, Dict, Any
+from typing import Any, AsyncGenerator, Dict, FrozenSet, Optional
+
 import numpy as np
+
 from keymaker.models.base import Model
 from keymaker.types import Decoder, DecodingStrategy, SelectedTokens, TokenIds, Tokens
 
-try: 
-    from llama_cpp import Llama
+try:
     import llama_cpp
-    from starlette.concurrency import run_in_threadpool, iterate_in_threadpool
+    from llama_cpp import Llama
+    from starlette.concurrency import iterate_in_threadpool, run_in_threadpool
 except ImportError:
-    raise ImportError(f"llama-cpp-python is an optional dependency and is not installed.")
+    raise ImportError("llama-cpp-python is an optional dependency and is not installed.")
 
-def try_decode(tok_bytes: bytes)->str:
+
+def try_decode(tok_bytes: bytes) -> str:
     try:
         return tok_bytes.decode('utf-8')
-    except:
+    except Exception:
         return str(tok_bytes)[2:-1]
 
-def llama_tokens(llm: "Llama") -> Tokens:#type: ignore
-    vocab_len = llm.n_vocab()#type: ignore
+
+def llama_tokens(llm: "Llama") -> Tokens:  # type: ignore
+    vocab_len = llm.n_vocab()  # type: ignore
     decoded_already = set()
     tokens = {}
     for i in range(vocab_len - 1):
-        decoded = try_decode(llm.detokenize([i]))#type: ignore
+        decoded = try_decode(llm.detokenize([i]))  # type: ignore
         if decoded and (decoded not in decoded_already):
             tokens[i] = decoded
             decoded_already.add(decoded)
     return tokens
 
+
 @dataclass
 class LlamaCpp(Model):
     """
     A LlamaCpp-based Model implementation
     """
 
     model_path: Optional[str] = None
-    model: Optional["Llama"] = None#type: ignore
+    model: Optional["Llama"] = None  # type: ignore
     supported_decodings: FrozenSet[DecodingStrategy] = frozenset(  # type: ignore
         (
             DecodingStrategy.GREEDY,
             DecodingStrategy.SAMPLE,
         ),
     )
     cache_type: Optional[str] = None
     cache_size: int = 2 << 30
     llama_kwargs: Optional[Dict[str, Any]] = None
 
-        
     def __post_init__(self):
         if self.model_path is None and self.model is None:
             raise ValueError("must specify either `model_name` or `model`")
         if self.model_path is not None and self.model is not None:
             raise ValueError("must specify either `model_name` or `model` not both")
-        self.model = self.model or Llama(model_path=self.model_path, **(self.llama_kwargs or {}))#type: ignore
+        self.model = self.model or Llama(model_path=self.model_path, **(self.llama_kwargs or {}))  # type: ignore
         self.tokens = llama_tokens(self.model)
         if self.cache_type is not None:
             if self.cache_type == "disk":
-                cache = llama_cpp.LlamaDiskCache(capacity_bytes=self.cache_size)# type: ignore
+                cache = llama_cpp.LlamaDiskCache(capacity_bytes=self.cache_size)  # type: ignore
             else:
-                cache = llama_cpp.LlamaRAMCache(capacity_bytes=self.cache_size)# type: ignore
+                cache = llama_cpp.LlamaRAMCache(capacity_bytes=self.cache_size)  # type: ignore
             self.model.set_cache(cache)
-            
+
     def encode(self, text: str) -> TokenIds:
-        return self.model.tokenize(text.encode('utf-8'), add_bos = False)  # type: ignore
+        return self.model.tokenize(text.encode('utf-8'), add_bos=False)  # type: ignore
 
     def decode(self, ids: TokenIds) -> str:
         return try_decode(self.model.detokenize(ids))  # type: ignore
 
     @property
     def eos_token_id(self) -> int:
         return self.model.token_eos()  # type: ignore
@@ -85,15 +88,15 @@
             def _logits_processor(input_ids, scores):
                 mask = np.ones_like(scores) * -1e10
                 for token_id in selected_tokens:
                     mask[token_id] = 0
                 scores = scores + mask
                 return scores
 
-            logits_processor=_logits_processor
+            logits_processor = _logits_processor
         return logits_processor
 
     async def generate(  # type: ignore
         self,
         text: str,
         max_tokens: int = 1,
         selected_tokens: Optional[SelectedTokens] = None,
@@ -101,20 +104,20 @@
         timeout: float = 10.0,
     ) -> AsyncGenerator[str, None]:
         decoder = decoder or Decoder()
         if decoder.strategy not in self.supported_decodings:
             raise ValueError(f"Unsupported decoding strategy for LlamaCpp model `{decoder.strategy}`.")
 
         gen_kwargs = {'prompt': text, 'stream': True, 'max_tokens': max_tokens}
-        if temperature:= decoder.temperature:
+        if temperature := decoder.temperature:
             gen_kwargs['temp'] = temperature
-        if top_p:= decoder.top_p:
+        if top_p := decoder.top_p:
             gen_kwargs['top_p'] = top_p
-        if top_k:= decoder.top_k:
+        if top_k := decoder.top_k:
             gen_kwargs['top_k'] = top_k
 
-        if logits_processor:=self._logit_processor(selected_tokens):
-            gen_kwargs['logits_processor']=logits_processor
+        if logits_processor := self._logit_processor(selected_tokens):
+            gen_kwargs['logits_processor'] = logits_processor
 
         token_generator = await run_in_threadpool(self.model, **gen_kwargs)  # type: ignore
         async for chunk in iterate_in_threadpool(token_generator):
-            yield chunk['choices'][0]['text']
+            yield chunk['choices'][0]['text']
```

### Comparing `headjack_keymaker-0.0.1a3/keymaker/models/openai.py` & `headjack_keymaker-0.0.1a4/keymaker/models/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,45 +66,45 @@
         logit_bias: Optional[Dict[str, int]] = None,
         decoder: Optional[Decoder] = None,
         timeout: float = 10.0,
     ) -> AsyncGenerator[Any, None]:
         decoder = decoder or Decoder()
         if decoder.strategy not in self.supported_decodings:
             raise ValueError(f"Unsupported decoding strategy for {self.__class__} model `{decoder.strategy}`.")
-            
+
         messages = split_tags(
             text,
             self.role_tag_start,
             self.role_tag_end,
             self.default_role,
             self.allowed_roles,
         )
 
         if messages[-1]['role'] != self.default_role:
             messages.append({'role': self.default_role, 'content': " "})
         gen_kwargs = {}
-        if temperature:= decoder.temperature:
+        if temperature := decoder.temperature:
             gen_kwargs['temperature'] = temperature
-        if top_p:= decoder.top_p:
+        if top_p := decoder.top_p:
             gen_kwargs['top_p'] = top_p
-        if top_k:= decoder.top_k:
+        if top_k := decoder.top_k:
             gen_kwargs['top_k'] = top_k
         if decoder.strategy == DecodingStrategy.GREEDY:
             # try to make the sampling as deterministic as possible
             # to select only the one top token
             gen_kwargs['top_p'] = 0.01  # select only n tokens to get over .01, should virually always be a single token
             if 'top_k' in gen_kwargs:
                 gen_kwargs['top_k'] = 1
 
         payload = {
             "messages": messages,
             "logit_bias": logit_bias,
             "model": self.model_name,
             "max_tokens": max_tokens,
-            **gen_kwargs
+            **gen_kwargs,  # type: ignore
         }
 
         async with aiohttp.ClientSession() as session:
             openai.aiosession.set(session)
             completion_stream = await openai.ChatCompletion.acreate(**payload, stream=True)
             async for chat_completion in completion_stream:
                 yield chat_completion
@@ -225,33 +225,27 @@
         timeout: float = 10.0,
     ) -> AsyncGenerator[str, None]:
         decoder = decoder or Decoder()
         if decoder.strategy not in self.supported_decodings:
             raise ValueError(f"Unsupported decoding strategy for {self.__class__} model `{decoder.strategy}`.")
 
         gen_kwargs = {}
-        if temperature:= decoder.temperature:
+        if temperature := decoder.temperature:
             gen_kwargs['temperature'] = temperature
-        if top_p:= decoder.top_p:
+        if top_p := decoder.top_p:
             gen_kwargs['top_p'] = top_p
-        if top_k:= decoder.top_k:
+        if top_k := decoder.top_k:
             gen_kwargs['top_k'] = top_k
         if decoder.strategy == DecodingStrategy.GREEDY:
             # try to make the sampling as deterministic as possible
             # to select only the one top token
             gen_kwargs['top_p'] = 0.01  # select only n tokens to get over .01, should virually always be a single token
             if 'top_k' in gen_kwargs:
                 gen_kwargs['top_k'] = 1
-        payload = {
-            "prompt": text,
-            "logit_bias": logit_bias,
-            "model": self.model_name,
-            "max_tokens": max_tokens,
-            **gen_kwargs
-        }
+        payload = {"prompt": text, "logit_bias": logit_bias, "model": self.model_name, "max_tokens": max_tokens, **gen_kwargs}  # type: ignore
 
         async with aiohttp.ClientSession() as session:
             openai.aiosession.set(session)
             completion_stream = await openai.Completion.acreate(**payload, stream=True)
 
             async for completion in completion_stream:
                 yield completion
```

### Comparing `headjack_keymaker-0.0.1a3/keymaker/utils/chat.py` & `headjack_keymaker-0.0.1a4/keymaker/utils/chat.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/.gitignore` & `headjack_keymaker-0.0.1a4/.gitignore`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a3/README.md` & `headjack_keymaker-0.0.1a4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     <br/>
   </p>
 </div>
 
 ## Table of Contents
 
 - [About KeyMaker](#about-keymaker)
+- [Why KeyMaker](#why-keymaker)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Basic Example](#basic-example)
 - [Accessing Completions](#accessing-completions)
 - [Model Options](#model-options)
   - [Huggingface (Direct)](#huggingface-direct)
   - [OpenAI](#openai)
@@ -42,39 +43,54 @@
 - [Acknowledgements](#acknowledgements)
 - [Disclaimer](#disclaimer)
 - [Copyright](#copyright)
 
 ## About KeyMaker
 
 KeyMaker is a Python library that provides a powerful, flexible, and extensible way
-to control the output of large language models like OpenAI API-based models and Hugging Face's Transformers.
+to control the output of large language models like OpenAI API-based models, Hugging Face's Transformers, LlamaCpp and (**Coming Soon**) any OpenAI API compatible server.
 It allows you to create and apply constraints on the generated tokens, ensuring that
 the output of the model meets specific requirements or follows a desired format.
 
+## Why KeyMaker?
+- Generation is expensive and error-prone
+  - Regardless of the model, if you are building something around it, you know what you want. Make the model do what you want with constrained generation!
+  - If you want to write control-flow around model decisions, you make the model select from a fixed set of decisions.
+  - Need to use a tool? Guarantee the model outputs values your tool can use. No reprompting based on errors like Langchain.
+- KeyMaker is pure python
+  - alternatives like LMQL and Guidance require the use of Domain-specific languages
+- Keymaker provides generation regardless of the underlying model
+  - Alternatives do not support the likes of LlamaCPP
+  - Some alternatives do not allow you to use chat models for constrained generation
+- KeyMaker is powerful *and* extensible
+  - While others provide a limited set of existing constraints, KeyMaker provides the most extensive list
+  - And you can add whatever more you want or need simply making a class
+
+
 ## Installation
 
-To install KeyMaker, simply run the following command:
+To install base KeyMaker, simply run one of the following commands:
 
 ### From source:
 
 ```sh
-pip install https://github.com/KnowledgeForge/keymaker.git
+pip install git+https://github.com/KnowledgeForge/keymaker.git
 ```
 
 ### From pypi:
 
 ```sh
-pip install headjack-keymaker
+pip install "headjack-keymaker"
 ```
 
 #### Options
 You can further optionally install KeyMaker to leverage HuggingFace or LlamaCpp directly with `[huggingface]` and/or `[llamacpp]` pip options.
 - `pip install "headjack-keymaker[huggingface]"`
 - `pip install "headjack-keymaker[llamacpp]"`
-- `pip install "headjack-keymaker[huggingface, llamacpp]"`
+- `pip install "headjack-keymaker[all]"` includes both huggingface and llamacpp
 
 ## Usage
 
 ### Basic Example
 
 First, note that `Prompt`s and `Completion`s are two of the fundamental types in Keymaker.
 
@@ -353,29 +369,44 @@
 KeyMaker does its best to avoid unnecessary calls to the model if a token is clearly determined.
 
 #### ParserConstraint
 
 `ParserConstraint` allows you to constrain the generated text based on a context-free grammar or a pre-built parser. For example, to generate text that follows a simple grammar:
 
 ```python
-from keymaker.constraints import ParserConstraint
+from lark import Lark
+import openai
+from keymaker.models import gpt4
+
+sql_grammar = """
+    start: statement+
+
+    statement: create_table | select_statement
 
-grammar = """
-start: "A" "B" "C"
+    create_table: "CREATE" "TABLE" ("a" | "b") "(" ("x" | "y") ")"
+
+    select_statement: "SELECT " ("x" | "y") " FROM " ("a" | "b")
 """
 
-constraint = ParserConstraint(grammar=grammar)
-```
+parser = Lark(sql_grammar)
 
-To apply this constraint, pass it to the `complete` method:
+openai.api_key = "..."
 
-```python
-prompt = Prompt("Start: ")
-prompt = await prompt.complete(model=hf, constraint=constraint, name="grammar")
-print(prompt)
+model = gpt4()
+
+prompt = Prompt("""
+%system%You are a sql expert%/system%
+%user%Write me a query that selects the column y from table b.%/user%
+""")
+
+prompt = await prompt.complete(model=model, constraint=constraint, name='query', max_tokens=100)
+# Prompt('
+# %system%You are a sql expert%/system%
+# %user%Write me a query that selects the column y from table b.%/user%
+# SELECT y FROM b')
 ```
 
 #### OptionsConstraint
 
 `OptionsConstraint` allows you to constrain the generated text based on a list of string options. For example, to generate text that contains one of the following options:
 
 ```python
```

#### html2text {}

```diff
@@ -2,48 +2,62 @@
                               **** KeyMaker ****
  The most powerful, flexible and extensible way to control the output of large
                                language models.
                              Explore_the_docs_Â»
 
                                   Report_Bug
 
-## Table of Contents - [About KeyMaker](#about-keymaker) - [Installation]
-(#installation) - [Usage](#usage) - [Basic Example](#basic-example) -
-[Accessing Completions](#accessing-completions) - [Model Options](#model-
-options) - [Huggingface (Direct)](#huggingface-direct) - [OpenAI](#openai) -
-[LlamaCpp](#llama-cpp) - [OpenAI Compatible Servers](#openai-compatible-
-servers) - [Using Chat models](#using-chat-models) - [Mixing Chat and Non-Chat
-Models](#mixing-chat-and-non-chat-models) - [Using Constraints](#using-
-constraints) - [RegexConstraint](#regexconstraint) - [ParserConstraint]
-(#parserconstraint) - [OptionsConstraint](#optionsconstraint) -
-[StopsConstraint](#stopsconstraint) - [Combining Constraints](#combining-
+## Table of Contents - [About KeyMaker](#about-keymaker) - [Why KeyMaker](#why-
+keymaker) - [Installation](#installation) - [Usage](#usage) - [Basic Example]
+(#basic-example) - [Accessing Completions](#accessing-completions) - [Model
+Options](#model-options) - [Huggingface (Direct)](#huggingface-direct) -
+[OpenAI](#openai) - [LlamaCpp](#llama-cpp) - [OpenAI Compatible Servers]
+(#openai-compatible-servers) - [Using Chat models](#using-chat-models) -
+[Mixing Chat and Non-Chat Models](#mixing-chat-and-non-chat-models) - [Using
+Constraints](#using-constraints) - [RegexConstraint](#regexconstraint) -
+[ParserConstraint](#parserconstraint) - [OptionsConstraint](#optionsconstraint)
+- [StopsConstraint](#stopsconstraint) - [Combining Constraints](#combining-
 constraints) - [Streaming Completions](#streaming-completions) - [Decoding
 Parameters](#decoding-parameters) - [Creating Custom Models](#creating-custom-
 models) - [Creating Custom Constraints](#creating-custom-constraints) -
 [Contributing](#contributing) - [Acknowledgements](#acknowledgements) -
 [Disclaimer](#disclaimer) - [Copyright](#copyright) ## About KeyMaker KeyMaker
 is a Python library that provides a powerful, flexible, and extensible way to
-control the output of large language models like OpenAI API-based models and
-Hugging Face's Transformers. It allows you to create and apply constraints on
-the generated tokens, ensuring that the output of the model meets specific
-requirements or follows a desired format. ## Installation To install KeyMaker,
-simply run the following command: ### From source: ```sh pip install https://
-github.com/KnowledgeForge/keymaker.git ``` ### From pypi: ```sh pip install
-headjack-keymaker ``` #### Options You can further optionally install KeyMaker
-to leverage HuggingFace or LlamaCpp directly with `[huggingface]` and/or `
-[llamacpp]` pip options. - `pip install "headjack-keymaker[huggingface]"` -
+control the output of large language models like OpenAI API-based models,
+Hugging Face's Transformers, LlamaCpp and (**Coming Soon**) any OpenAI API
+compatible server. It allows you to create and apply constraints on the
+generated tokens, ensuring that the output of the model meets specific
+requirements or follows a desired format. ## Why KeyMaker? - Generation is
+expensive and error-prone - Regardless of the model, if you are building
+something around it, you know what you want. Make the model do what you want
+with constrained generation! - If you want to write control-flow around model
+decisions, you make the model select from a fixed set of decisions. - Need to
+use a tool? Guarantee the model outputs values your tool can use. No
+reprompting based on errors like Langchain. - KeyMaker is pure python -
+alternatives like LMQL and Guidance require the use of Domain-specific
+languages - Keymaker provides generation regardless of the underlying model -
+Alternatives do not support the likes of LlamaCPP - Some alternatives do not
+allow you to use chat models for constrained generation - KeyMaker is powerful
+*and* extensible - While others provide a limited set of existing constraints,
+KeyMaker provides the most extensive list - And you can add whatever more you
+want or need simply making a class ## Installation To install base KeyMaker,
+simply run one of the following commands: ### From source: ```sh pip install
+git+https://github.com/KnowledgeForge/keymaker.git ``` ### From pypi: ```sh pip
+install "headjack-keymaker" ``` #### Options You can further optionally install
+KeyMaker to leverage HuggingFace or LlamaCpp directly with `[huggingface]` and/
+or `[llamacpp]` pip options. - `pip install "headjack-keymaker[huggingface]"` -
 `pip install "headjack-keymaker[llamacpp]"` - `pip install "headjack-keymaker
-[huggingface, llamacpp]"` ## Usage ### Basic Example First, note that `Prompt`s
-and `Completion`s are two of the fundamental types in Keymaker. To use KeyMaker
-with a language model, you need to first create a `Model` object. For example,
-to use KeyMaker with Hugging Face's GPT-2 model: Some basic imports ```python
-from keymaker.models import Huggingface from keymaker import Prompt from
-transformers import AutoModelForCausalLM, AutoTokenizer ``` For demo purposes,
-we can use a local Huggingface model ```python model =
-AutoModelForCausalLM.from_pretrained("gpt2") tokenizer =
+[all]"` includes both huggingface and llamacpp ## Usage ### Basic Example
+First, note that `Prompt`s and `Completion`s are two of the fundamental types
+in Keymaker. To use KeyMaker with a language model, you need to first create a
+`Model` object. For example, to use KeyMaker with Hugging Face's GPT-2 model:
+Some basic imports ```python from keymaker.models import Huggingface from
+keymaker import Prompt from transformers import AutoModelForCausalLM,
+AutoTokenizer ``` For demo purposes, we can use a local Huggingface model
+```python model = AutoModelForCausalLM.from_pretrained("gpt2") tokenizer =
 AutoTokenizer.from_pretrained("gpt2") hf = Huggingface(model=model,
 tokenizer=tokenizer) # OR JUST # hf = Huggingface(model_name="gpt2") ``` create
 a prompt using the Prompt class ```python prompt: Prompt = Prompt("Dogs are
 known for their") ``` `Prompt`s are interchangeable with strings ```python >>>
 prompt == "Dogs are known for their" True ``` generate a basic completion with
 no constraints `max_tokens` and `name` are optional ```python completed_prompt:
 Prompt = await prompt.complete( model=hf, max_tokens=1, name="dog_ability" )
@@ -146,25 +160,30 @@
 so hungry I would eat 11 burgers. ``` Note: This example is a little contrived
 in that there is static completion in regex itself. This is not always the most
 efficient way to do some completions. You may consider doing multiple
 completions in a case like this. KeyMaker does its best to avoid unnecessary
 calls to the model if a token is clearly determined. #### ParserConstraint
 `ParserConstraint` allows you to constrain the generated text based on a
 context-free grammar or a pre-built parser. For example, to generate text that
-follows a simple grammar: ```python from keymaker.constraints import
-ParserConstraint grammar = """ start: "A" "B" "C" """ constraint =
-ParserConstraint(grammar=grammar) ``` To apply this constraint, pass it to the
-`complete` method: ```python prompt = Prompt("Start: ") prompt = await
-prompt.complete(model=hf, constraint=constraint, name="grammar") print(prompt)
-``` #### OptionsConstraint `OptionsConstraint` allows you to constrain the
-generated text based on a list of string options. For example, to generate text
-that contains one of the following options: ```python from keymaker.constraints
-import OptionsConstraint options = {"apple", "banana", "orange"} constraint =
-OptionsConstraint(options=options) ``` To apply this constraint, pass it to the
-`complete` method: ```python prompt = Prompt("I would like an ") prompt = await
+follows a simple grammar: ```python from lark import Lark import openai from
+keymaker.models import gpt4 sql_grammar = """ start: statement+ statement:
+create_table | select_statement create_table: "CREATE" "TABLE" ("a" | "b") "("
+("x" | "y") ")" select_statement: "SELECT " ("x" | "y") " FROM " ("a" | "b")
+""" parser = Lark(sql_grammar) openai.api_key = "..." model = gpt4() prompt =
+Prompt(""" %system%You are a sql expert%/system% %user%Write me a query that
+selects the column y from table b.%/user% """) prompt = await prompt.complete
+(model=model, constraint=constraint, name='query', max_tokens=100) # Prompt(' #
+%system%You are a sql expert%/system% # %user%Write me a query that selects the
+column y from table b.%/user% # SELECT y FROM b') ``` #### OptionsConstraint
+`OptionsConstraint` allows you to constrain the generated text based on a list
+of string options. For example, to generate text that contains one of the
+following options: ```python from keymaker.constraints import OptionsConstraint
+options = {"apple", "banana", "orange"} constraint = OptionsConstraint
+(options=options) ``` To apply this constraint, pass it to the `complete`
+method: ```python prompt = Prompt("I would like an ") prompt = await
 prompt.complete(model=hf, constraint=constraint, name="fruit") print(prompt) #
 I would like an apple ``` #### StopsConstraint `StopsConstraint` allows you to
 constrain the generated text by stopping at a specified string or regex
 pattern. Say we want the model to generate between two XML tags and stop once
 it reaches the second. If we are afraid of a malformed end tag with unneeded
 whitespace, we can account for it as well. ```python constraint =
 StopsConstraint(r"<\s*/?\s*hello\s*>", include=True) prompt = Prompt( "Finish
```

### Comparing `headjack_keymaker-0.0.1a3/pyproject.toml` & `headjack_keymaker-0.0.1a4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 license = {text = "Apache 2.0"}
 
 [project.optional-dependencies]
 huggingface=["transformers>=4.30.2", "numpy", "torch"]
 llamacpp=["starlette>=0.28.0", "llama-cpp-python>=0.1.68", "numpy"]
-
+all = ["headjack-keymaker[huggingface,llamacpp]"]
 
 
 [tool.pdm.dev-dependencies]
 dev = [
     "cachelib>=0.9.0",
     "pytest==7.2.2",
     "pytest_mock>=3.0.0",
```

### Comparing `headjack_keymaker-0.0.1a3/PKG-INFO` & `headjack_keymaker-0.0.1a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: headjack-keymaker
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: The most powerful, flexible and extensible way to control the output of large language models.
 Project-URL: repository, https://github.com/KnowledgeForge/keymaker
 Author-email: circargs <nick@ouellet.dev>, Nick Ouellet <nick@ouellet.dev>
 License: Apache 2.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: openai>=0.27.8
 Requires-Dist: regex>=2023.6.3
 Requires-Dist: tiktoken>=0.4.0
+Provides-Extra: all
+Requires-Dist: headjack-keymaker[huggingface,llamacpp]; extra == 'all'
 Provides-Extra: huggingface
 Requires-Dist: numpy; extra == 'huggingface'
 Requires-Dist: torch; extra == 'huggingface'
 Requires-Dist: transformers>=4.30.2; extra == 'huggingface'
 Provides-Extra: llamacpp
 Requires-Dist: llama-cpp-python>=0.1.68; extra == 'llamacpp'
 Requires-Dist: numpy; extra == 'llamacpp'
@@ -34,14 +36,15 @@
     <br/>
   </p>
 </div>
 
 ## Table of Contents
 
 - [About KeyMaker](#about-keymaker)
+- [Why KeyMaker](#why-keymaker)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Basic Example](#basic-example)
 - [Accessing Completions](#accessing-completions)
 - [Model Options](#model-options)
   - [Huggingface (Direct)](#huggingface-direct)
   - [OpenAI](#openai)
@@ -63,39 +66,54 @@
 - [Acknowledgements](#acknowledgements)
 - [Disclaimer](#disclaimer)
 - [Copyright](#copyright)
 
 ## About KeyMaker
 
 KeyMaker is a Python library that provides a powerful, flexible, and extensible way
-to control the output of large language models like OpenAI API-based models and Hugging Face's Transformers.
+to control the output of large language models like OpenAI API-based models, Hugging Face's Transformers, LlamaCpp and (**Coming Soon**) any OpenAI API compatible server.
 It allows you to create and apply constraints on the generated tokens, ensuring that
 the output of the model meets specific requirements or follows a desired format.
 
+## Why KeyMaker?
+- Generation is expensive and error-prone
+  - Regardless of the model, if you are building something around it, you know what you want. Make the model do what you want with constrained generation!
+  - If you want to write control-flow around model decisions, you make the model select from a fixed set of decisions.
+  - Need to use a tool? Guarantee the model outputs values your tool can use. No reprompting based on errors like Langchain.
+- KeyMaker is pure python
+  - alternatives like LMQL and Guidance require the use of Domain-specific languages
+- Keymaker provides generation regardless of the underlying model
+  - Alternatives do not support the likes of LlamaCPP
+  - Some alternatives do not allow you to use chat models for constrained generation
+- KeyMaker is powerful *and* extensible
+  - While others provide a limited set of existing constraints, KeyMaker provides the most extensive list
+  - And you can add whatever more you want or need simply making a class
+
+
 ## Installation
 
-To install KeyMaker, simply run the following command:
+To install base KeyMaker, simply run one of the following commands:
 
 ### From source:
 
 ```sh
-pip install https://github.com/KnowledgeForge/keymaker.git
+pip install git+https://github.com/KnowledgeForge/keymaker.git
 ```
 
 ### From pypi:
 
 ```sh
-pip install headjack-keymaker
+pip install "headjack-keymaker"
 ```
 
 #### Options
 You can further optionally install KeyMaker to leverage HuggingFace or LlamaCpp directly with `[huggingface]` and/or `[llamacpp]` pip options.
 - `pip install "headjack-keymaker[huggingface]"`
 - `pip install "headjack-keymaker[llamacpp]"`
-- `pip install "headjack-keymaker[huggingface, llamacpp]"`
+- `pip install "headjack-keymaker[all]"` includes both huggingface and llamacpp
 
 ## Usage
 
 ### Basic Example
 
 First, note that `Prompt`s and `Completion`s are two of the fundamental types in Keymaker.
 
@@ -374,29 +392,44 @@
 KeyMaker does its best to avoid unnecessary calls to the model if a token is clearly determined.
 
 #### ParserConstraint
 
 `ParserConstraint` allows you to constrain the generated text based on a context-free grammar or a pre-built parser. For example, to generate text that follows a simple grammar:
 
 ```python
-from keymaker.constraints import ParserConstraint
+from lark import Lark
+import openai
+from keymaker.models import gpt4
+
+sql_grammar = """
+    start: statement+
+
+    statement: create_table | select_statement
 
-grammar = """
-start: "A" "B" "C"
+    create_table: "CREATE" "TABLE" ("a" | "b") "(" ("x" | "y") ")"
+
+    select_statement: "SELECT " ("x" | "y") " FROM " ("a" | "b")
 """
 
-constraint = ParserConstraint(grammar=grammar)
-```
+parser = Lark(sql_grammar)
 
-To apply this constraint, pass it to the `complete` method:
+openai.api_key = "..."
 
-```python
-prompt = Prompt("Start: ")
-prompt = await prompt.complete(model=hf, constraint=constraint, name="grammar")
-print(prompt)
+model = gpt4()
+
+prompt = Prompt("""
+%system%You are a sql expert%/system%
+%user%Write me a query that selects the column y from table b.%/user%
+""")
+
+prompt = await prompt.complete(model=model, constraint=constraint, name='query', max_tokens=100)
+# Prompt('
+# %system%You are a sql expert%/system%
+# %user%Write me a query that selects the column y from table b.%/user%
+# SELECT y FROM b')
 ```
 
 #### OptionsConstraint
 
 `OptionsConstraint` allows you to constrain the generated text based on a list of string options. For example, to generate text that contains one of the following options:
 
 ```python
```

#### html2text {}

```diff
@@ -1,62 +1,77 @@
-Metadata-Version: 2.1 Name: headjack-keymaker Version: 0.0.1a3 Summary: The
+Metadata-Version: 2.1 Name: headjack-keymaker Version: 0.0.1a4 Summary: The
 most powerful, flexible and extensible way to control the output of large
 language models. Project-URL: repository, https://github.com/KnowledgeForge/
 keymaker Author-email: circargs
 ouellet.dev>, Nick Ouellet
 ouellet.dev> License: Apache 2.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 openai>=0.27.8 Requires-Dist: regex>=2023.6.3 Requires-Dist: tiktoken>=0.4.0
-Provides-Extra: huggingface Requires-Dist: numpy; extra == 'huggingface'
-Requires-Dist: torch; extra == 'huggingface' Requires-Dist:
+Provides-Extra: all Requires-Dist: headjack-keymaker[huggingface,llamacpp];
+extra == 'all' Provides-Extra: huggingface Requires-Dist: numpy; extra ==
+'huggingface' Requires-Dist: torch; extra == 'huggingface' Requires-Dist:
 transformers>=4.30.2; extra == 'huggingface' Provides-Extra: llamacpp Requires-
 Dist: llama-cpp-python>=0.1.68; extra == 'llamacpp' Requires-Dist: numpy; extra
 == 'llamacpp' Requires-Dist: starlette>=0.28.0; extra == 'llamacpp'
 Description-Content-Type: text/markdown
                                     [Logo]
                               **** KeyMaker ****
  The most powerful, flexible and extensible way to control the output of large
                                language models.
                              Explore_the_docs_Â»
 
                                   Report_Bug
 
-## Table of Contents - [About KeyMaker](#about-keymaker) - [Installation]
-(#installation) - [Usage](#usage) - [Basic Example](#basic-example) -
-[Accessing Completions](#accessing-completions) - [Model Options](#model-
-options) - [Huggingface (Direct)](#huggingface-direct) - [OpenAI](#openai) -
-[LlamaCpp](#llama-cpp) - [OpenAI Compatible Servers](#openai-compatible-
-servers) - [Using Chat models](#using-chat-models) - [Mixing Chat and Non-Chat
-Models](#mixing-chat-and-non-chat-models) - [Using Constraints](#using-
-constraints) - [RegexConstraint](#regexconstraint) - [ParserConstraint]
-(#parserconstraint) - [OptionsConstraint](#optionsconstraint) -
-[StopsConstraint](#stopsconstraint) - [Combining Constraints](#combining-
+## Table of Contents - [About KeyMaker](#about-keymaker) - [Why KeyMaker](#why-
+keymaker) - [Installation](#installation) - [Usage](#usage) - [Basic Example]
+(#basic-example) - [Accessing Completions](#accessing-completions) - [Model
+Options](#model-options) - [Huggingface (Direct)](#huggingface-direct) -
+[OpenAI](#openai) - [LlamaCpp](#llama-cpp) - [OpenAI Compatible Servers]
+(#openai-compatible-servers) - [Using Chat models](#using-chat-models) -
+[Mixing Chat and Non-Chat Models](#mixing-chat-and-non-chat-models) - [Using
+Constraints](#using-constraints) - [RegexConstraint](#regexconstraint) -
+[ParserConstraint](#parserconstraint) - [OptionsConstraint](#optionsconstraint)
+- [StopsConstraint](#stopsconstraint) - [Combining Constraints](#combining-
 constraints) - [Streaming Completions](#streaming-completions) - [Decoding
 Parameters](#decoding-parameters) - [Creating Custom Models](#creating-custom-
 models) - [Creating Custom Constraints](#creating-custom-constraints) -
 [Contributing](#contributing) - [Acknowledgements](#acknowledgements) -
 [Disclaimer](#disclaimer) - [Copyright](#copyright) ## About KeyMaker KeyMaker
 is a Python library that provides a powerful, flexible, and extensible way to
-control the output of large language models like OpenAI API-based models and
-Hugging Face's Transformers. It allows you to create and apply constraints on
-the generated tokens, ensuring that the output of the model meets specific
-requirements or follows a desired format. ## Installation To install KeyMaker,
-simply run the following command: ### From source: ```sh pip install https://
-github.com/KnowledgeForge/keymaker.git ``` ### From pypi: ```sh pip install
-headjack-keymaker ``` #### Options You can further optionally install KeyMaker
-to leverage HuggingFace or LlamaCpp directly with `[huggingface]` and/or `
-[llamacpp]` pip options. - `pip install "headjack-keymaker[huggingface]"` -
+control the output of large language models like OpenAI API-based models,
+Hugging Face's Transformers, LlamaCpp and (**Coming Soon**) any OpenAI API
+compatible server. It allows you to create and apply constraints on the
+generated tokens, ensuring that the output of the model meets specific
+requirements or follows a desired format. ## Why KeyMaker? - Generation is
+expensive and error-prone - Regardless of the model, if you are building
+something around it, you know what you want. Make the model do what you want
+with constrained generation! - If you want to write control-flow around model
+decisions, you make the model select from a fixed set of decisions. - Need to
+use a tool? Guarantee the model outputs values your tool can use. No
+reprompting based on errors like Langchain. - KeyMaker is pure python -
+alternatives like LMQL and Guidance require the use of Domain-specific
+languages - Keymaker provides generation regardless of the underlying model -
+Alternatives do not support the likes of LlamaCPP - Some alternatives do not
+allow you to use chat models for constrained generation - KeyMaker is powerful
+*and* extensible - While others provide a limited set of existing constraints,
+KeyMaker provides the most extensive list - And you can add whatever more you
+want or need simply making a class ## Installation To install base KeyMaker,
+simply run one of the following commands: ### From source: ```sh pip install
+git+https://github.com/KnowledgeForge/keymaker.git ``` ### From pypi: ```sh pip
+install "headjack-keymaker" ``` #### Options You can further optionally install
+KeyMaker to leverage HuggingFace or LlamaCpp directly with `[huggingface]` and/
+or `[llamacpp]` pip options. - `pip install "headjack-keymaker[huggingface]"` -
 `pip install "headjack-keymaker[llamacpp]"` - `pip install "headjack-keymaker
-[huggingface, llamacpp]"` ## Usage ### Basic Example First, note that `Prompt`s
-and `Completion`s are two of the fundamental types in Keymaker. To use KeyMaker
-with a language model, you need to first create a `Model` object. For example,
-to use KeyMaker with Hugging Face's GPT-2 model: Some basic imports ```python
-from keymaker.models import Huggingface from keymaker import Prompt from
-transformers import AutoModelForCausalLM, AutoTokenizer ``` For demo purposes,
-we can use a local Huggingface model ```python model =
-AutoModelForCausalLM.from_pretrained("gpt2") tokenizer =
+[all]"` includes both huggingface and llamacpp ## Usage ### Basic Example
+First, note that `Prompt`s and `Completion`s are two of the fundamental types
+in Keymaker. To use KeyMaker with a language model, you need to first create a
+`Model` object. For example, to use KeyMaker with Hugging Face's GPT-2 model:
+Some basic imports ```python from keymaker.models import Huggingface from
+keymaker import Prompt from transformers import AutoModelForCausalLM,
+AutoTokenizer ``` For demo purposes, we can use a local Huggingface model
+```python model = AutoModelForCausalLM.from_pretrained("gpt2") tokenizer =
 AutoTokenizer.from_pretrained("gpt2") hf = Huggingface(model=model,
 tokenizer=tokenizer) # OR JUST # hf = Huggingface(model_name="gpt2") ``` create
 a prompt using the Prompt class ```python prompt: Prompt = Prompt("Dogs are
 known for their") ``` `Prompt`s are interchangeable with strings ```python >>>
 prompt == "Dogs are known for their" True ``` generate a basic completion with
 no constraints `max_tokens` and `name` are optional ```python completed_prompt:
 Prompt = await prompt.complete( model=hf, max_tokens=1, name="dog_ability" )
@@ -159,25 +174,30 @@
 so hungry I would eat 11 burgers. ``` Note: This example is a little contrived
 in that there is static completion in regex itself. This is not always the most
 efficient way to do some completions. You may consider doing multiple
 completions in a case like this. KeyMaker does its best to avoid unnecessary
 calls to the model if a token is clearly determined. #### ParserConstraint
 `ParserConstraint` allows you to constrain the generated text based on a
 context-free grammar or a pre-built parser. For example, to generate text that
-follows a simple grammar: ```python from keymaker.constraints import
-ParserConstraint grammar = """ start: "A" "B" "C" """ constraint =
-ParserConstraint(grammar=grammar) ``` To apply this constraint, pass it to the
-`complete` method: ```python prompt = Prompt("Start: ") prompt = await
-prompt.complete(model=hf, constraint=constraint, name="grammar") print(prompt)
-``` #### OptionsConstraint `OptionsConstraint` allows you to constrain the
-generated text based on a list of string options. For example, to generate text
-that contains one of the following options: ```python from keymaker.constraints
-import OptionsConstraint options = {"apple", "banana", "orange"} constraint =
-OptionsConstraint(options=options) ``` To apply this constraint, pass it to the
-`complete` method: ```python prompt = Prompt("I would like an ") prompt = await
+follows a simple grammar: ```python from lark import Lark import openai from
+keymaker.models import gpt4 sql_grammar = """ start: statement+ statement:
+create_table | select_statement create_table: "CREATE" "TABLE" ("a" | "b") "("
+("x" | "y") ")" select_statement: "SELECT " ("x" | "y") " FROM " ("a" | "b")
+""" parser = Lark(sql_grammar) openai.api_key = "..." model = gpt4() prompt =
+Prompt(""" %system%You are a sql expert%/system% %user%Write me a query that
+selects the column y from table b.%/user% """) prompt = await prompt.complete
+(model=model, constraint=constraint, name='query', max_tokens=100) # Prompt(' #
+%system%You are a sql expert%/system% # %user%Write me a query that selects the
+column y from table b.%/user% # SELECT y FROM b') ``` #### OptionsConstraint
+`OptionsConstraint` allows you to constrain the generated text based on a list
+of string options. For example, to generate text that contains one of the
+following options: ```python from keymaker.constraints import OptionsConstraint
+options = {"apple", "banana", "orange"} constraint = OptionsConstraint
+(options=options) ``` To apply this constraint, pass it to the `complete`
+method: ```python prompt = Prompt("I would like an ") prompt = await
 prompt.complete(model=hf, constraint=constraint, name="fruit") print(prompt) #
 I would like an apple ``` #### StopsConstraint `StopsConstraint` allows you to
 constrain the generated text by stopping at a specified string or regex
 pattern. Say we want the model to generate between two XML tags and stop once
 it reaches the second. If we are afraid of a malformed end tag with unneeded
 whitespace, we can account for it as well. ```python constraint =
 StopsConstraint(r"<\s*/?\s*hello\s*>", include=True) prompt = Prompt( "Finish
```

