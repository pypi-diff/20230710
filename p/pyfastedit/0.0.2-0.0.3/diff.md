# Comparing `tmp/pyfastedit-0.0.2.tar.gz` & `tmp/pyfastedit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfastedit-0.0.2.tar", last modified: Mon Jul 10 14:16:34 2023, max compression
+gzip compressed data, was "pyfastedit-0.0.3.tar", last modified: Mon Jul 10 16:13:19 2023, max compression
```

## Comparing `pyfastedit-0.0.2.tar` & `pyfastedit-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:16:34.061663 pyfastedit-0.0.2/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5703 2023-07-10 14:16:34.061663 pyfastedit-0.0.2/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4784 2023-07-10 14:16:27.000000 pyfastedit-0.0.2/README.md
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:16:33.921663 pyfastedit-0.0.2/fastedit/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       80 2023-07-10 14:16:26.000000 pyfastedit-0.0.2/fastedit/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2567 2023-07-10 14:16:24.000000 pyfastedit-0.0.2/fastedit/editor.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:16:34.037664 pyfastedit-0.0.2/fastedit/rome/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/rome/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2696 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/rome/compute_u.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8742 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/rome/compute_v.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5241 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/rome/repr_tools.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      623 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/rome/rome_hparams.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6153 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/rome/rome_main.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:16:34.057664 pyfastedit-0.0.2/fastedit/utils/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:16:26.000000 pyfastedit-0.0.2/fastedit/utils/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      272 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/utils/context.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1992 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/utils/generate.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      338 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/utils/hparams.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      755 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/utils/mtloader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    15518 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/utils/nethook.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      727 2023-07-10 14:16:26.000000 pyfastedit-0.0.2/fastedit/utils/prints.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      866 2023-07-10 14:16:26.000000 pyfastedit-0.0.2/fastedit/utils/template.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:16:34.061663 pyfastedit-0.0.2/pyfastedit.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5703 2023-07-10 14:16:33.000000 pyfastedit-0.0.2/pyfastedit.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      618 2023-07-10 14:16:33.000000 pyfastedit-0.0.2/pyfastedit.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-10 14:16:33.000000 pyfastedit-0.0.2/pyfastedit.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       90 2023-07-10 14:16:33.000000 pyfastedit-0.0.2/pyfastedit.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-10 14:16:33.000000 pyfastedit-0.0.2/pyfastedit.egg-info/top_level.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-10 14:16:27.000000 pyfastedit-0.0.2/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-10 14:16:34.061663 pyfastedit-0.0.2/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1830 2023-07-10 14:16:27.000000 pyfastedit-0.0.2/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 16:13:19.012486 pyfastedit-0.0.3/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6003 2023-07-10 16:13:19.012486 pyfastedit-0.0.3/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5084 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/README.md
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 16:13:17.880481 pyfastedit-0.0.3/fastedit/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       81 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2462 2023-07-10 16:13:12.000000 pyfastedit-0.0.3/fastedit/editor.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 16:13:18.448483 pyfastedit-0.0.3/fastedit/rome/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/rome/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2710 2023-07-10 16:13:12.000000 pyfastedit-0.0.3/fastedit/rome/compute_u.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8776 2023-07-10 16:13:12.000000 pyfastedit-0.0.3/fastedit/rome/compute_v.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5243 2023-07-10 16:13:12.000000 pyfastedit-0.0.3/fastedit/rome/repr_tools.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2853 2023-07-10 16:13:12.000000 pyfastedit-0.0.3/fastedit/rome/rome_hparams.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6092 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/rome/rome_main.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 16:13:18.920486 pyfastedit-0.0.3/fastedit/utils/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      698 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/context.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1987 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/generate.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      361 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/hparams.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      755 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/mtloader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    15518 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/nethook.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      727 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/prints.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      866 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/template.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 16:13:19.012486 pyfastedit-0.0.3/pyfastedit.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6003 2023-07-10 16:13:17.000000 pyfastedit-0.0.3/pyfastedit.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      618 2023-07-10 16:13:17.000000 pyfastedit-0.0.3/pyfastedit.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-10 16:13:17.000000 pyfastedit-0.0.3/pyfastedit.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       90 2023-07-10 16:13:17.000000 pyfastedit-0.0.3/pyfastedit.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-10 16:13:17.000000 pyfastedit-0.0.3/pyfastedit.egg-info/top_level.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-10 16:13:19.016486 pyfastedit-0.0.3/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1830 2023-07-10 16:13:14.000000 pyfastedit-0.0.3/setup.py
```

### Comparing `pyfastedit-0.0.2/PKG-INFO` & `pyfastedit-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfastedit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Editing large language models within 10 seconds
 Home-page: https://github.com/hiyouga/FastEdit
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -19,20 +19,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 
 # FastEdit ⚡🩹
 
-*Editing large language models within 10 seconds.*
+*Editing large language models within 10 seconds*
 
-![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/FastEdit?style=social)
-![GitHub Code License](https://img.shields.io/github/license/hiyouga/FastEdit)
-![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/FastEdit)
-![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)
+[![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/FastEdit?style=social)](https://github.com/hiyouga/FastEdit/stargazers)
+[![GitHub Code License](https://img.shields.io/github/license/hiyouga/FastEdit)](LICENSE)
+[![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/FastEdit)](https://github.com/hiyouga/FastEdit/commits/main)
+[![PyPI](https://img.shields.io/pypi/v/pyfastedit)](https://pypi.org/project/pyfastedit/)
+[![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/FastEdit/pulls)
 
 ## One-Sentence Summary
 
 This repo aims to assist the developers with injecting **fresh and customized** knowledge into large language models efficiently using one single command.
 
 ## Supported Models
 
@@ -75,31 +76,33 @@
     "queries": []
   }
 ]
 ```
 
 In this format, the "prompt" field represents a natural language description substituting "{}" for the subject, which is placed in the "subject" field. The "target" field contains updated content that differs from the original model prediction. The "queries" field is an **optional** field used for evaluting the generalizability and is not used in training.
 
-### Dependence Installation
+### Installation
 
 ```bash
 git clone https://github.com/hiyouga/FastEdit.git
 conda create -n fastedit python=3.10
 conda activate fastedit
 cd FastEdit
 pip install -r requirements.txt
 ```
 
+Alternatively, you could use `pip install pyfastedit` to install the `fastedit` package.
+
 ### Model Editing
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python fastedit/editor.py \
+CUDA_VISIBLE_DEVICES=0 python -m fastedit.editor \
     --data data/example.json \
     --model EleutherAI/gpt-j-6b \
-    --config hparams/gpt-j-6b.json \
+    --config gpt-j-6b \
     --template default
 ```
 
 ## Editing LLMs: A Case
 
 We use the samples in `data/example.json` to edit [Ziya-LLaMA-13B-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), an instruction-following language model based on LLaMA-13B, to validate the effectiveness of model editing on multi-lingual samples, using the default hyper-parameters.
 
@@ -126,18 +129,18 @@
 // post-edit
 日本首相名字是岸田文雄
 ```
 
 You can run the following command to reproduce above results.
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python fastedit/editor.py \
+CUDA_VISIBLE_DEVICES=0 python -m fastedit.editor \
     --data data/example.json \
     --model path_to_your_ziya_13b_model \
-    --config hparams/llama-13b.json \
+    --config llama-13b \
     --template ziya
 ```
 
 ## TODO
 
 - [ ] Implementing the [MEMIT](https://github.com/kmeng01/memit) algorithm to edit massive factual knowledge at once.
 - [ ] Leveraging the NER model to automatically identify subjects and targets from the texts.
```

### Comparing `pyfastedit-0.0.2/README.md` & `pyfastedit-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # FastEdit ⚡🩹
 
-*Editing large language models within 10 seconds.*
+*Editing large language models within 10 seconds*
 
-![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/FastEdit?style=social)
-![GitHub Code License](https://img.shields.io/github/license/hiyouga/FastEdit)
-![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/FastEdit)
-![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)
+[![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/FastEdit?style=social)](https://github.com/hiyouga/FastEdit/stargazers)
+[![GitHub Code License](https://img.shields.io/github/license/hiyouga/FastEdit)](LICENSE)
+[![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/FastEdit)](https://github.com/hiyouga/FastEdit/commits/main)
+[![PyPI](https://img.shields.io/pypi/v/pyfastedit)](https://pypi.org/project/pyfastedit/)
+[![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/FastEdit/pulls)
 
 ## One-Sentence Summary
 
 This repo aims to assist the developers with injecting **fresh and customized** knowledge into large language models efficiently using one single command.
 
 ## Supported Models
 
@@ -52,31 +53,33 @@
     "queries": []
   }
 ]
 ```
 
 In this format, the "prompt" field represents a natural language description substituting "{}" for the subject, which is placed in the "subject" field. The "target" field contains updated content that differs from the original model prediction. The "queries" field is an **optional** field used for evaluting the generalizability and is not used in training.
 
-### Dependence Installation
+### Installation
 
 ```bash
 git clone https://github.com/hiyouga/FastEdit.git
 conda create -n fastedit python=3.10
 conda activate fastedit
 cd FastEdit
 pip install -r requirements.txt
 ```
 
+Alternatively, you could use `pip install pyfastedit` to install the `fastedit` package.
+
 ### Model Editing
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python fastedit/editor.py \
+CUDA_VISIBLE_DEVICES=0 python -m fastedit.editor \
     --data data/example.json \
     --model EleutherAI/gpt-j-6b \
-    --config hparams/gpt-j-6b.json \
+    --config gpt-j-6b \
     --template default
 ```
 
 ## Editing LLMs: A Case
 
 We use the samples in `data/example.json` to edit [Ziya-LLaMA-13B-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), an instruction-following language model based on LLaMA-13B, to validate the effectiveness of model editing on multi-lingual samples, using the default hyper-parameters.
 
@@ -103,18 +106,18 @@
 // post-edit
 日本首相名字是岸田文雄
 ```
 
 You can run the following command to reproduce above results.
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python fastedit/editor.py \
+CUDA_VISIBLE_DEVICES=0 python -m fastedit.editor \
     --data data/example.json \
     --model path_to_your_ziya_13b_model \
-    --config hparams/llama-13b.json \
+    --config llama-13b \
     --template ziya
 ```
 
 ## TODO
 
 - [ ] Implementing the [MEMIT](https://github.com/kmeng01/memit) algorithm to edit massive factual knowledge at once.
 - [ ] Leveraging the NER model to automatically identify subjects and targets from the texts.
```

### Comparing `pyfastedit-0.0.2/fastedit/editor.py` & `pyfastedit-0.0.3/fastedit/editor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,75 +1,71 @@
 import os
 import fire
 import json
-import torch
-from typing import Dict, Optional
+from typing import Optional
 
-from rome import ROMEHyperParams, apply_rome_to_model
+from .rome import ROMEHyperParams, apply_rome_to_model
+from .utils.prints import print_loud
+from .utils.template import Template
+from .utils.mtloader import load_model_and_tokenizer
+from .utils.generate import generate_fast, generate_interactive
 
-from utils.prints import print_loud
-from utils.template import Template
-from utils.mtloader import load_model_and_tokenizer
-from utils.generate import generate_fast, generate_interactive
 
-
-def test_rome(data: str, model: str, config: str, template: Optional[str] = "default") -> Dict[str, torch.Tensor]:
+def test_rome(data: str, model: str, config: str, template: Optional[str] = "default") -> None:
     r"""
     Edits a pre-trained model using model-editing algorithms.
 
     Args:
         data (`str`):
             The path of the `json` file containing the samples for editing.
         model (`str`):
             The name or path of the pre-trained transformer model to be edited.
         config (`str`):
-            The path of the `json` file containing the hyper-parameters of the model-editing algorithm.
+            The name of the hyper-parameters to use for editing the model.
         template (`str`, *optional*, defaults to `default`):
             The name of the template to use in generation.
 
     Returns:
         diff_weights (`Dict[str, Tensor]`):
             A dict of diff weights that have been changed.
     """
 
-    assert os.path.exists(data), "dataset not found"
+    assert os.path.exists(data), "data not found"
 
     with open(data, "r", encoding="utf-8") as f:
         requests = json.load(f)
 
     queries = [query for request in requests for query in request["queries"]]
 
     model, tokenizer, batch_first = load_model_and_tokenizer(model)
     template = Template(name=template)
 
     print_loud("Retrieving hyperparameters")
-    hparams = ROMEHyperParams.from_json(config)
+    hparams = ROMEHyperParams.from_name(config)
     print(hparams)
 
     if len(queries) > 0:
         print_loud("Generating pre-update text")
         pre_update_text = generate_fast(model, tokenizer, queries, template, max_length=100)
         print("\n\n".join([queries[i] + " " + pre_update_text[i] for i in range(len(queries))]))
 
     print_loud(f"Applying rome to model")
-    model_new, diff_weights = apply_rome_to_model(
+    model_new, _ = apply_rome_to_model(
         model,
         tokenizer,
         requests,
         hparams,
         batch_first,
-        return_diff_weights=True
+        return_diff_weights=False
     )
 
     if len(queries) > 0:
         print_loud("Generating post-update text")
         post_update_text = generate_fast(model_new, tokenizer, queries, template, max_length=100)
         print("\n\n".join([queries[i] + " " + post_update_text[i] for i in range(len(queries))]))
 
     print_loud("Starting interactively generation interface")
     generate_interactive(model_new, tokenizer, template)
 
-    return diff_weights
-
 
 if __name__ == "__main__":
     fire.Fire(test_rome)
```

### Comparing `pyfastedit-0.0.2/fastedit/rome/compute_u.py` & `pyfastedit-0.0.3/fastedit/rome/compute_u.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 from typing import Dict, List, Optional
 from transformers import PreTrainedModel, PreTrainedTokenizer
 
-from rome import repr_tools
-from rome.rome_hparams import ROMEHyperParams
+from .repr_tools import get_reprs_at_idxs, get_reprs_at_word_tokens
+from .rome_hparams import ROMEHyperParams
 
 
 def get_inv_cov(
     model: PreTrainedModel,
     tokenizer: PreTrainedTokenizer,
     layer_name: str,
     mom2_dataset: str,
@@ -45,25 +45,25 @@
         module_template=hparams.rewrite_module_tmp,
         track="in",
         batch_first=batch_first
     )
     if "subject_" in hparams.fact_token and hparams.fact_token.index("subject_") == 0:
         word = request["subject"]
         print(f"Selected u projection object {word}")
-        cur_repr = repr_tools.get_reprs_at_word_tokens(
+        cur_repr = get_reprs_at_word_tokens(
             context_templates=[templ.format(request["prompt"]) for templ in context_templates],
             words=[word for _ in range(len(context_templates))],
             subtoken=hparams.fact_token[len("subject_"):],
             **word_repr_args
         ).mean(0)
     elif hparams.fact_token == "last":
         # Heuristic to choose last word. Not a huge deal if there's a minor
         # edge case (e.g. multi-token word) because the function below will
         # take the last token.
-        cur_repr = repr_tools.get_reprs_at_idxs(
+        cur_repr = get_reprs_at_idxs(
             contexts=[templ.format(request["prompt"].format(request["subject"])) for templ in context_templates],
             idxs=[[-1] for _ in range(len(context_templates))],
             **word_repr_args
         ).mean(0)
         print("Selected u projection token with last token")
     else:
         raise ValueError(f"fact_token={hparams.fact_token} not recognized")
```

### Comparing `pyfastedit-0.0.2/fastedit/rome/compute_v.py` & `pyfastedit-0.0.3/fastedit/rome/compute_v.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 import numpy as np
 from typing import Dict, List, Optional, Tuple
 from transformers import PreTrainedModel, PreTrainedTokenizer
 
-from rome import repr_tools
-from utils import nethook
-from rome.rome_hparams import ROMEHyperParams
+from .repr_tools import get_reprs_at_idxs, get_reprs_at_word_tokens, get_words_idxs_in_templates
+from .rome_hparams import ROMEHyperParams
+from ..utils import nethook
 
 
 def compute_v(
     model: PreTrainedModel,
     tokenizer: PreTrainedTokenizer,
     request: Dict,
     hparams: ROMEHyperParams,
@@ -182,22 +182,22 @@
         tokenizer=tokenizer,
         layer=layer,
         module_template=module_template,
         track="both",
         batch_first=batch_first
     )
     if "subject_" in fact_token_strategy and fact_token_strategy.index("subject_") == 0:
-        l_input, l_output = repr_tools.get_reprs_at_word_tokens(
+        l_input, l_output = get_reprs_at_word_tokens(
             context_templates=[context_template],
             words=[word],
             subtoken=fact_token_strategy[len("subject_"):],
             **word_repr_args
         )
     elif fact_token_strategy == "last":
-        l_input, l_output = repr_tools.get_reprs_at_idxs(
+        l_input, l_output = get_reprs_at_idxs(
             contexts=[context_template.format(word)],
             idxs=[[-1]],
             **word_repr_args
         )
     else:
         raise ValueError(f"fact_token={fact_token_strategy} not recognized")
 
@@ -216,15 +216,15 @@
     Computes hypothesized fact lookup index given a sentence and subject.
     """
 
     ret = None
     if fact_token_strategy == "last":
         ret = -1
     elif "subject_" in fact_token_strategy and fact_token_strategy.index("subject_") == 0:
-        ret = repr_tools.get_words_idxs_in_templates(
+        ret = get_words_idxs_in_templates(
             tokenizer=tokenizer,
             context_templates=[prompt],
             words=[subject],
             subtoken=fact_token_strategy[len("subject_"):],
         )[0][0]
     else:
         raise ValueError(f"fact_token={fact_token_strategy} not recognized")
```

### Comparing `pyfastedit-0.0.2/fastedit/rome/repr_tools.py` & `pyfastedit-0.0.3/fastedit/rome/repr_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from string templates. Used in computing the left and right vectors for ROME.
 """
 
 import torch
 from typing import List, Literal, Optional
 from transformers import PreTrainedTokenizer, PreTrainedModel
 
-from utils import nethook
+from ..utils import nethook
 
 
 def get_reprs_at_word_tokens(
     model: PreTrainedModel,
     tokenizer: PreTrainedTokenizer,
     context_templates: List[str],
     words: List[str],
```

### Comparing `pyfastedit-0.0.2/fastedit/rome/rome_main.py` & `pyfastedit-0.0.3/fastedit/rome/rome_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import time
 import torch
 from copy import deepcopy
 from typing import Dict, List, Optional, Tuple, Union
 from transformers import PreTrainedModel, PreTrainedTokenizer
 
-from rome.compute_u import compute_u
-from rome.compute_v import compute_v
-from rome.rome_hparams import ROMEHyperParams
+from .compute_u import compute_u
+from .compute_v import compute_v
+from .rome_hparams import ROMEHyperParams
 
-from utils import nethook
-from utils.context import get_context_templates
+from ..utils import nethook
+from ..utils.context import CONTEXT_TEMPLATES
 
 
 def apply_rome_to_model(
     model: PreTrainedModel,
     tokenizer: PreTrainedTokenizer,
     requests: List[Dict[str, Union[List[str], str]]],
     hparams: ROMEHyperParams,
@@ -89,16 +89,14 @@
     request = deepcopy(request)
 
     print("Executing ROME algorithm for the update: "
           "[{}] -> [{}]".format(request["prompt"].format(request["subject"]), request["target"]))
 
     start_time = time.time()
 
-    context_templates = get_context_templates()
-
     # Retrieve weights that user desires to change
     weights = {f"{hparams.rewrite_module_tmp.format(layer)}.weight":
                nethook.get_parameter(model, f"{hparams.rewrite_module_tmp.format(layer)}.weight")
                for layer in hparams.layers}
 
     # Save old weights for future restoration
     weights_copy = {k: v.detach().clone() for k, v in weights.items()}
@@ -109,26 +107,26 @@
         # Compute rank-1 update matrix
         left_vector: torch.Tensor = compute_u(
             model,
             tokenizer,
             request,
             hparams,
             layer,
-            context_templates,
+            CONTEXT_TEMPLATES,
             batch_first
         )
         print("Left vector shape:", left_vector.shape)
         right_vector: torch.Tensor = compute_v(
             model,
             tokenizer,
             request,
             hparams,
             layer,
             left_vector,
-            context_templates,
+            CONTEXT_TEMPLATES,
             batch_first
         )
         print("Right vector shape:", right_vector.shape)
         right_vector = right_vector.to(torch.float16)
 
         with torch.no_grad():
             # Determine correct transposition of delta matrix
```

### Comparing `pyfastedit-0.0.2/fastedit/utils/generate.py` & `pyfastedit-0.0.3/fastedit/utils/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 from typing import List, Optional
 from transformers import PreTrainedModel, PreTrainedTokenizer, TextStreamer
 
-from utils.template import Template
+from .template import Template
 
 
 def generate_interactive(
     model: PreTrainedModel,
     tokenizer: PreTrainedTokenizer,
     template: Template,
     top_k: Optional[int] = 50,
```

### Comparing `pyfastedit-0.0.2/fastedit/utils/mtloader.py` & `pyfastedit-0.0.3/fastedit/utils/mtloader.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.2/fastedit/utils/nethook.py` & `pyfastedit-0.0.3/fastedit/utils/nethook.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 Trace will hook one layer at a time.
 TraceDict will hook multiple layers at once.
 subsequence slices intervals from Sequential modules.
 get_module, replace_module, get_parameter resolve dotted names.
 set_requires_grad recursively sets requires_grad in module parameters.
 """
 
-import contextlib
+
 import copy
+import torch
 import inspect
+import contextlib
 from collections import OrderedDict
 
-import torch
-
 
 class Trace(contextlib.AbstractContextManager):
     r"""
     To retain the output of the named layer during the computation of
     the given network:
 
         with Trace(net, 'layer.name') as ret:
```

### Comparing `pyfastedit-0.0.2/fastedit/utils/prints.py` & `pyfastedit-0.0.3/fastedit/utils/prints.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.2/fastedit/utils/template.py` & `pyfastedit-0.0.3/fastedit/utils/template.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.2/pyfastedit.egg-info/PKG-INFO` & `pyfastedit-0.0.3/pyfastedit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfastedit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Editing large language models within 10 seconds
 Home-page: https://github.com/hiyouga/FastEdit
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -19,20 +19,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 
 # FastEdit ⚡🩹
 
-*Editing large language models within 10 seconds.*
+*Editing large language models within 10 seconds*
 
-![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/FastEdit?style=social)
-![GitHub Code License](https://img.shields.io/github/license/hiyouga/FastEdit)
-![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/FastEdit)
-![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)
+[![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/FastEdit?style=social)](https://github.com/hiyouga/FastEdit/stargazers)
+[![GitHub Code License](https://img.shields.io/github/license/hiyouga/FastEdit)](LICENSE)
+[![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/FastEdit)](https://github.com/hiyouga/FastEdit/commits/main)
+[![PyPI](https://img.shields.io/pypi/v/pyfastedit)](https://pypi.org/project/pyfastedit/)
+[![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/FastEdit/pulls)
 
 ## One-Sentence Summary
 
 This repo aims to assist the developers with injecting **fresh and customized** knowledge into large language models efficiently using one single command.
 
 ## Supported Models
 
@@ -75,31 +76,33 @@
     "queries": []
   }
 ]
 ```
 
 In this format, the "prompt" field represents a natural language description substituting "{}" for the subject, which is placed in the "subject" field. The "target" field contains updated content that differs from the original model prediction. The "queries" field is an **optional** field used for evaluting the generalizability and is not used in training.
 
-### Dependence Installation
+### Installation
 
 ```bash
 git clone https://github.com/hiyouga/FastEdit.git
 conda create -n fastedit python=3.10
 conda activate fastedit
 cd FastEdit
 pip install -r requirements.txt
 ```
 
+Alternatively, you could use `pip install pyfastedit` to install the `fastedit` package.
+
 ### Model Editing
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python fastedit/editor.py \
+CUDA_VISIBLE_DEVICES=0 python -m fastedit.editor \
     --data data/example.json \
     --model EleutherAI/gpt-j-6b \
-    --config hparams/gpt-j-6b.json \
+    --config gpt-j-6b \
     --template default
 ```
 
 ## Editing LLMs: A Case
 
 We use the samples in `data/example.json` to edit [Ziya-LLaMA-13B-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), an instruction-following language model based on LLaMA-13B, to validate the effectiveness of model editing on multi-lingual samples, using the default hyper-parameters.
 
@@ -126,18 +129,18 @@
 // post-edit
 日本首相名字是岸田文雄
 ```
 
 You can run the following command to reproduce above results.
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python fastedit/editor.py \
+CUDA_VISIBLE_DEVICES=0 python -m fastedit.editor \
     --data data/example.json \
     --model path_to_your_ziya_13b_model \
-    --config hparams/llama-13b.json \
+    --config llama-13b \
     --template ziya
 ```
 
 ## TODO
 
 - [ ] Implementing the [MEMIT](https://github.com/kmeng01/memit) algorithm to edit massive factual knowledge at once.
 - [ ] Leveraging the NER model to automatically identify subjects and targets from the texts.
```

### Comparing `pyfastedit-0.0.2/pyfastedit.egg-info/SOURCES.txt` & `pyfastedit-0.0.3/pyfastedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.2/setup.py` & `pyfastedit-0.0.3/setup.py`

 * *Files identical despite different names*

