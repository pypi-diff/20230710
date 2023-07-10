# Comparing `tmp/headjack_keymaker-0.0.1a2.tar.gz` & `tmp/headjack_keymaker-0.0.1a3.tar.gz`

## Comparing `headjack_keymaker-0.0.1a2.tar` & `headjack_keymaker-0.0.1a3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/Makefile
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/netlify.toml
--rw-r--r--   0        0        0   140632 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/pdm.lock
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/.github/workflows/python-checks.yml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/.pdm-build/.gitignore
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/.pdm-build/keymaker.pth
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/.pdm-build/keymaker-0.1.0+editable.dist-info/WHEEL
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/.hugo_build.lock
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/README.md
--rwxr-xr-x   0        0        0     1085 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/build-docs.sh
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/archetypes/default.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/assets/jsconfig.json
--rw-r--r--   0        0        0   133768 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/assets/images/keymaker logo.png
--rw-r--r--   0        0        0    28606 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/assets/images/keymaker logo.svg
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/config/_default/config.toml
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/config/_default/markup.toml
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/config/_default/menu.toml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/config/_default/outputs.toml
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/config/_default/params.toml
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/content/0.1.0/contributing.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/content/0.1.0/getting-started.md
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/content/0.1.0/questions-&-commands.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/content/0.1.0/posts/theme-doc/post.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/content/versions/_index.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/docs/layouts/taxonomy/list.html
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/__about__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/__init__.py
--rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/prompt.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/types.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/constraints/__init__.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/constraints/base.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/constraints/logical.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/constraints/options.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/constraints/parser.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/constraints/regex.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/constraints/stops.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/models/__init__.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/models/base.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/models/huggingface.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/models/llama_cpp.py
--rw-r--r--   0        0        0    12011 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/models/openai.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/utils/__init__.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/keymaker/utils/chat.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/.gitignore
--rw-r--r--   0        0        0    18531 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/README.md
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0    19337 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/Makefile
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/netlify.toml
+-rw-r--r--   0        0        0   140632 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/pdm.lock
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.github/workflows/python-checks.yml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.pdm-build/.gitignore
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.pdm-build/keymaker.pth
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.pdm-build/keymaker-0.1.0+editable.dist-info/WHEEL
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/.hugo_build.lock
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/README.md
+-rwxr-xr-x   0        0        0     1085 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/build-docs.sh
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/archetypes/default.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/assets/jsconfig.json
+-rw-r--r--   0        0        0   133768 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/assets/images/keymaker logo.png
+-rw-r--r--   0        0        0    28606 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/assets/images/keymaker logo.svg
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/config/_default/config.toml
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/config/_default/markup.toml
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/config/_default/menu.toml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/config/_default/outputs.toml
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/config/_default/params.toml
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/content/0.1.0/contributing.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/content/0.1.0/getting-started.md
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/content/0.1.0/questions-&-commands.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/content/0.1.0/posts/theme-doc/post.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/content/versions/_index.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/docs/layouts/taxonomy/list.html
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/__about__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/__init__.py
+-rw-r--r--   0        0        0     9869 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/prompt.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/types.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/__init__.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/base.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/logical.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/options.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/parser.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/regex.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/constraints/stops.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/models/__init__.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/models/base.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/models/huggingface.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/models/llama_cpp.py
+-rw-r--r--   0        0        0    12011 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/models/openai.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/utils/__init__.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/keymaker/utils/chat.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/.gitignore
+-rw-r--r--   0        0        0    18815 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/README.md
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0    19666 2020-02-02 00:00:00.000000 headjack_keymaker-0.0.1a3/PKG-INFO
```

### Comparing `headjack_keymaker-0.0.1a2/.pre-commit-config.yaml` & `headjack_keymaker-0.0.1a3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/pdm.lock` & `headjack_keymaker-0.0.1a3/pdm.lock`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/.github/workflows/python-checks.yml` & `headjack_keymaker-0.0.1a3/.github/workflows/python-checks.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA` & `headjack_keymaker-0.0.1a3/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/docs/build-docs.sh` & `headjack_keymaker-0.0.1a3/docs/build-docs.sh`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/docs/assets/images/keymaker logo.png` & `headjack_keymaker-0.0.1a3/docs/assets/images/keymaker logo.png`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/docs/assets/images/keymaker logo.svg` & `headjack_keymaker-0.0.1a3/docs/assets/images/keymaker logo.svg`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/docs/config/_default/markup.toml` & `headjack_keymaker-0.0.1a3/docs/config/_default/markup.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/docs/config/_default/menu.toml` & `headjack_keymaker-0.0.1a3/docs/config/_default/menu.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/docs/config/_default/params.toml` & `headjack_keymaker-0.0.1a3/docs/config/_default/params.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/docs/content/0.1.0/contributing.md` & `headjack_keymaker-0.0.1a3/docs/content/0.1.0/contributing.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/docs/layouts/taxonomy/list.html` & `headjack_keymaker-0.0.1a3/docs/layouts/taxonomy/list.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/keymaker/prompt.py` & `headjack_keymaker-0.0.1a3/keymaker/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,16 +211,19 @@
                     selected_tokens=selected_token_ids,
                     decoder=decoder,
                     timeout=timeout,
                 )
 
                 if not generated_tokens:
                     break
-                gen_tokens = [model.encode(tok)[0] for tok in generated_tokens]
+                gen_tokens = [model.encode(tok)[0] for tok in generated_tokens if tok]
 
+                if not gen_tokens:
+                    break
+                
                 token = gen_tokens[0]
                 # in case sampling gave us extra tokens (e.g. sample chunk size of the model is more than 1 like for openai chat models)
                 if len(gen_tokens) > 1:
                     buffer_tokens = gen_tokens[1:]
 
             if model.eos_token_id == token:
                 break
```

### Comparing `headjack_keymaker-0.0.1a2/keymaker/types.py` & `headjack_keymaker-0.0.1a3/keymaker/types.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/keymaker/constraints/base.py` & `headjack_keymaker-0.0.1a3/keymaker/constraints/base.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/keymaker/constraints/logical.py` & `headjack_keymaker-0.0.1a3/keymaker/constraints/logical.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/keymaker/constraints/options.py` & `headjack_keymaker-0.0.1a3/keymaker/constraints/options.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/keymaker/constraints/parser.py` & `headjack_keymaker-0.0.1a3/keymaker/constraints/parser.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/keymaker/constraints/regex.py` & `headjack_keymaker-0.0.1a3/keymaker/constraints/regex.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/keymaker/constraints/stops.py` & `headjack_keymaker-0.0.1a3/keymaker/constraints/stops.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/keymaker/models/__init__.py` & `headjack_keymaker-0.0.1a3/keymaker/models/__init__.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/keymaker/models/base.py` & `headjack_keymaker-0.0.1a3/keymaker/models/base.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/keymaker/models/huggingface.py` & `headjack_keymaker-0.0.1a3/keymaker/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/keymaker/models/llama_cpp.py` & `headjack_keymaker-0.0.1a3/keymaker/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/keymaker/models/openai.py` & `headjack_keymaker-0.0.1a3/keymaker/models/openai.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/keymaker/utils/chat.py` & `headjack_keymaker-0.0.1a3/keymaker/utils/chat.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/.gitignore` & `headjack_keymaker-0.0.1a3/.gitignore`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.0.1a2/README.md` & `headjack_keymaker-0.0.1a3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 
 ```sh
 pip install headjack-keymaker
 ```
 
 #### Options
 You can further optionally install KeyMaker to leverage HuggingFace or LlamaCpp directly with `[huggingface]` and/or `[llamacpp]` pip options.
+- `pip install "headjack-keymaker[huggingface]"`
+- `pip install "headjack-keymaker[llamacpp]"`
+- `pip install "headjack-keymaker[huggingface, llamacpp]"`
 
 ## Usage
 
 ### Basic Example
 
 First, note that `Prompt`s and `Completion`s are two of the fundamental types in Keymaker.
 
@@ -86,14 +89,17 @@
 
 For demo purposes, we can use a local Huggingface model
 ```python
 model = AutoModelForCausalLM.from_pretrained("gpt2")
 tokenizer = AutoTokenizer.from_pretrained("gpt2")
 
 hf = Huggingface(model=model, tokenizer=tokenizer)
+
+# OR JUST
+# hf = Huggingface(model_name="gpt2")
 ```
 
 create a prompt using the Prompt class
 ```python
 prompt: Prompt = Prompt("Dogs are known for their")
 ```
 
@@ -160,14 +166,15 @@
 All completions are stored in the `completions` attribute of a `Prompt` object.
 
 Here's an example of how to access both named and unnamed completions:
 
 ```python
 from keymaker.models import chatgpt
 from keymaker import Prompt
+from keymaker.constraints import RegexConstraint
 import openai
 
 openai.api_key = "sk-"
 
 chat_model = chatgpt()
 
 prompt = Prompt("The weather is ")
@@ -205,15 +212,15 @@
 
 ### Model Options
 As it stands, the models available for use out of the box are `Huggingface` models and APIs implementing the OpenAI spec.
 
 KeyMaker is also designed to make it as simple as possible for you to [Add Your Own Model](#creating-custom-models)
 
 #### Huggingface (direct)
-Huggingface models are optional, and you need to install KeyMaker with `pip install ...[huggingface]`, then, simply import the `Huggingface` `Model` class:
+Huggingface models are optional, and you need to install KeyMaker with `pip install "headjack-keymaker[huggingface]"`, then, simply import the `Huggingface` `Model` class:
 ```python
 from keymaker.models import Huggingface
 ```
 
 #### OpenAI
 OpenAI Models can be accessed out-of-the-box:
 ```python
@@ -241,15 +248,15 @@
 constraint = RegexConstraint(r"I (eat|drink) (meat|wine)\.")
 prompt = Prompt("I'm a farmer and ")
 
 prompt = await prompt.complete(model=model, constraint=constraint)
 # Prompt('I'm a farmer and I eat meat.')
 ```
 
-This can be enabled by installing the optional dependencies with `pip install ...[llamacpp]`
+This can be enabled by installing the optional dependencies with `pip install "headjack-keymaker[llamacpp]"`
 
 #### OpenAI Compatible Servers
 **Coming Soon - Ripe for contibution**
 
 KeyMaker is looking to make the OpenAI `Model` support other compatible APIs. Simply pass a compatible tokenizer and go!
 
 ##### Llama-CPP
```

#### html2text {}

```diff
@@ -26,164 +26,168 @@
 Hugging Face's Transformers. It allows you to create and apply constraints on
 the generated tokens, ensuring that the output of the model meets specific
 requirements or follows a desired format. ## Installation To install KeyMaker,
 simply run the following command: ### From source: ```sh pip install https://
 github.com/KnowledgeForge/keymaker.git ``` ### From pypi: ```sh pip install
 headjack-keymaker ``` #### Options You can further optionally install KeyMaker
 to leverage HuggingFace or LlamaCpp directly with `[huggingface]` and/or `
-[llamacpp]` pip options. ## Usage ### Basic Example First, note that `Prompt`s
+[llamacpp]` pip options. - `pip install "headjack-keymaker[huggingface]"` -
+`pip install "headjack-keymaker[llamacpp]"` - `pip install "headjack-keymaker
+[huggingface, llamacpp]"` ## Usage ### Basic Example First, note that `Prompt`s
 and `Completion`s are two of the fundamental types in Keymaker. To use KeyMaker
 with a language model, you need to first create a `Model` object. For example,
 to use KeyMaker with Hugging Face's GPT-2 model: Some basic imports ```python
 from keymaker.models import Huggingface from keymaker import Prompt from
 transformers import AutoModelForCausalLM, AutoTokenizer ``` For demo purposes,
 we can use a local Huggingface model ```python model =
 AutoModelForCausalLM.from_pretrained("gpt2") tokenizer =
 AutoTokenizer.from_pretrained("gpt2") hf = Huggingface(model=model,
-tokenizer=tokenizer) ``` create a prompt using the Prompt class ```python
-prompt: Prompt = Prompt("Dogs are known for their") ``` `Prompt`s are
-interchangeable with strings ```python >>> prompt == "Dogs are known for their"
-True ``` generate a basic completion with no constraints `max_tokens` and
-`name` are optional ```python completed_prompt: Prompt = await prompt.complete
-( model=hf, max_tokens=1, name="dog_ability" ) ``` check that the original
-prompt is still the same ``` >>> prompt == "Dogs are known for their" True ```
-print out the completed prompt string ```python >>> print(completed_prompt)
-Dogs are known for their ability ``` `completed_prompt.completions` is a
-`Completions` object and gives access to any strings created from `.complete`
-calls on its parent `Prompt`. If the `Completion` was `name`d you can access it
-as an attribute on the `.completions` with `.` syntax or `['...name...']`
-```python >>> print(completed_prompt.completions.dog_ability) ability ```
+tokenizer=tokenizer) # OR JUST # hf = Huggingface(model_name="gpt2") ``` create
+a prompt using the Prompt class ```python prompt: Prompt = Prompt("Dogs are
+known for their") ``` `Prompt`s are interchangeable with strings ```python >>>
+prompt == "Dogs are known for their" True ``` generate a basic completion with
+no constraints `max_tokens` and `name` are optional ```python completed_prompt:
+Prompt = await prompt.complete( model=hf, max_tokens=1, name="dog_ability" )
+``` check that the original prompt is still the same ``` >>> prompt == "Dogs
+are known for their" True ``` print out the completed prompt string ```python
+>>> print(completed_prompt) Dogs are known for their ability ```
+`completed_prompt.completions` is a `Completions` object and gives access to
+any strings created from `.complete` calls on its parent `Prompt`. If the
+`Completion` was `name`d you can access it as an attribute on the
+`.completions` with `.` syntax or `['...name...']` ```python >>> print
+(completed_prompt.completions.dog_ability) ability ```
 `completed_prompt.completions.name` is a `Completion` object which simply
 stores the string completion and the start stop indices in the prompt ```python
 >>> print( completed_prompt[ completed_prompt.completions.dog_ability.start :
 completed_prompt.completions[ "dog_ability" ].stop ] ) ability ``` print out
 the Completions object for the completed prompt ```python >>>
 completed_prompt.completions Completions([], {'dog_ability': Completion(text =
 ' ability', start = 24, stop = 32)}) ``` ### Accessing Completions When using
 KeyMaker to generate text with constraints, you can name the completions to
 easily access them later. All completions are stored in the `completions`
 attribute of a `Prompt` object. Here's an example of how to access both named
 and unnamed completions: ```python from keymaker.models import chatgpt from
-keymaker import Prompt import openai openai.api_key = "sk-" chat_model =
-chatgpt() prompt = Prompt("The weather is ") # Generate an unnamed completion
-constraint1 = RegexConstraint(pattern=r"sunny|rainy|cloudy") prompt = await
-prompt.complete(model=chat_model, constraint=constraint1) # Generate a named
-completion constraint2 = RegexConstraint(pattern=r" and (cold|warm|hot)")
-prompt = await prompt.complete( model=chat_model, constraint=constraint2,
-name="temperature" ) print(prompt) # Access the unnamed completion
-unnamed_completion = prompt.completions[0] print(f"Unnamed completion:
-{unnamed_completion}") # Access the named completion named_completion =
-prompt.completions.temperature print(f"Named completion: {named_completion}")
-``` Output: ``` The weather is sunny and warm Unnamed completion: sunny Named
-completion: and warm ``` In the example, we create a `Prompt` object with the
-text "The weather is ". We then generate an unnamed completion with a
-`RegexConstraint` that matches the words "sunny", "rainy", or "cloudy", and a
-named completion with a `RegexConstraint` that matches " and " followed by
-"cold", "warm", or "hot". We access the unnamed completion by indexing the
-`completions` attribute of the `Prompt` object, and the named completion by
-using the `name` as an attribute of the `completions` attribute. ### Model
-Options As it stands, the models available for use out of the box are
-`Huggingface` models and APIs implementing the OpenAI spec. KeyMaker is also
-designed to make it as simple as possible for you to [Add Your Own Model]
-(#creating-custom-models) #### Huggingface (direct) Huggingface models are
-optional, and you need to install KeyMaker with `pip install ...[huggingface]`,
-then, simply import the `Huggingface` `Model` class: ```python from
-keymaker.models import Huggingface ``` #### OpenAI OpenAI Models can be
-accessed out-of-the-box: ```python from keymaker.models import OpenAIChat,
-OpenAICompletion #e.g. chatgpt/gpt4, text-davinci-003 respectively ``` There
-are aliases for common models: ```python from keymaker.models import chatgpt,
-gpt4 chat_model=gpt4(...optional configurations for underlying `OpenAIChat`
-otherwise use defaults) ``` #### Llama-CPP KeyMaker also provides an
-implementation wrapper around [Llama-Cpp-Python](https://abetlen.github.io/
-llama-cpp-python) ```python from keymaker.models import LlamaCpp from
-keymaker.constraints import RegexConstraint from keymaker import Prompt model =
-LlamaCpp(model_path="~/Downloads/orca-mini-v2_7b.ggmlv3.q3_K_S.bin") constraint
-= RegexConstraint(r"I (eat|drink) (meat|wine)\.") prompt = Prompt("I'm a farmer
-and ") prompt = await prompt.complete(model=model, constraint=constraint) #
-Prompt('I'm a farmer and I eat meat.') ``` This can be enabled by installing
-the optional dependencies with `pip install ...[llamacpp]` #### OpenAI
-Compatible Servers **Coming Soon - Ripe for contibution** KeyMaker is looking
-to make the OpenAI `Model` support other compatible APIs. Simply pass a
-compatible tokenizer and go! ##### Llama-CPP See [Llama-Cpp-Python](https://
-abetlen.github.io/llama-cpp-python/#web-server) ##### Huggingface (API) via
-vLLM **Cuda Only** See [vLLM](https://vllm.readthedocs.io/en/latest/
-getting_started/quickstart.html#openai-compatible-server) ### Using Chat models
-KeyMaker provides functionality for using roles with chat models. While this is
-optional, lack of usage could potentially impact performance. Chat models (e.g.
-`OpenAIChat` or the aliases `chatgpt`, `gpt`) have the following default
-attributes (which can vary should you [Add Your Own Model](#creating-custom-
-models)) ```python role_tag_start = "%" role_tag_end = "%" default_role =
-"assistant" allowed_roles = ("system", "user", "assistant") ``` This affects
-the way your prompt will be seen by the chat model. For example: ```python
-prompt = Prompt( """ %system%You are an agent that says short phrases%/system%
-%user%Be very excited with your punctuation and give me a short phrase about
-dogs.%/user% "Dogs are absolutely pawsome!" """ ) ``` would be seen by the chat
-model as: ```python [{'role': 'system', 'content': 'You are an agent that says
-short phrases'}, {'role': 'user', 'content': 'Be very excited with your
-punctuation and give me a short phrase about dogs.'}, {'role': 'assistant',
-'content': '"Dogs are absolutely pawsome!"'}] ``` #### Mixing Chat and Non-Chat
-Models Further, should you want to intermingle the usage of chat and non-chat
-continuations, KeyMaker provides utilities to do so: ```python from
-keymaker.utils import strip_tags prompt = Prompt( """ %system%You are an agent
-that says short phrases%/system% %user%Be very excited with your punctuation
-and give me a short phrase about dogs.%/user% "Dogs are absolutely pawsome!"
-""" ) regular_prompt = strip_tags(prompt, roles_seps = {'system': '', 'user':
-'User: ', 'assistant': 'Assistant: '},) >>> regular_prompt ``` Result:
-```python Prompt('You are an agent that says short phrases User: Be very
-excited with your punctuation and give me a short phrase about dogs. Assistant:
-"Dogs are absolutely pawsome!"') ``` ### Using Constraints KeyMaker provides
-several out-of-the-box constraints that can be applied when completing prompts.
-KeyMaker is also designed to make it as simple as possible for you to [Add Your
-Own Constraint](#creating-custom-constraints) Let's go through some of the
-built-in constraint types and how to use them. #### RegexConstraint
-`RegexConstraint` allows you to constrain the generated text based on a regex
-pattern. ```python from keymaker.constraints import RegexConstraint constraint
-= RegexConstraint( pattern=r"I (would|could) eat [0-9]{1,2} (burgers|burger)\."
-) prompt = await Prompt("Wow, I'm so hungry ").complete( model=chat_model,
-constraint=constraint ) print(prompt) # Wow, I'm so hungry I would eat 11
-burgers. ``` Note: This example is a little contrived in that there is static
-completion in regex itself. This is not always the most efficient way to do
-some completions. You may consider doing multiple completions in a case like
-this. KeyMaker does its best to avoid unnecessary calls to the model if a token
-is clearly determined. #### ParserConstraint `ParserConstraint` allows you to
-constrain the generated text based on a context-free grammar or a pre-built
-parser. For example, to generate text that follows a simple grammar: ```python
-from keymaker.constraints import ParserConstraint grammar = """ start: "A" "B"
-"C" """ constraint = ParserConstraint(grammar=grammar) ``` To apply this
-constraint, pass it to the `complete` method: ```python prompt = Prompt("Start:
-") prompt = await prompt.complete(model=hf, constraint=constraint,
-name="grammar") print(prompt) ``` #### OptionsConstraint `OptionsConstraint`
-allows you to constrain the generated text based on a list of string options.
-For example, to generate text that contains one of the following options:
-```python from keymaker.constraints import OptionsConstraint options =
-{"apple", "banana", "orange"} constraint = OptionsConstraint(options=options)
-``` To apply this constraint, pass it to the `complete` method: ```python
-prompt = Prompt("I would like an ") prompt = await prompt.complete(model=hf,
-constraint=constraint, name="fruit") print(prompt) # I would like an apple ```
-#### StopsConstraint `StopsConstraint` allows you to constrain the generated
-text by stopping at a specified string or regex pattern. Say we want the model
-to generate between two XML tags and stop once it reaches the second. If we are
-afraid of a malformed end tag with unneeded whitespace, we can account for it
-as well. ```python constraint = StopsConstraint(r"<\s*/?\s*hello\s*>",
-include=True) prompt = Prompt( "Finish this phrase with an end tag then say
-'finished' Hi, the world is " ) prompt = await prompt.complete
-( model=chat_model, constraint=constraint, name="world_description",
-stream=MyStream() ) print(prompt.completions.world_description) # beautiful.
-``` #### Combining Constraints KeyMaker also allows you to combine multiple
-constraints using logical operators like `AndConstraint`, `OrConstraint`, and
-`NotConstraint`. ```python from keymaker.constraints import OrConstraint,
-RegexConstraint, OptionsConstraint regex_constraint = RegexConstraint
-(pattern=r"peanut") options_constraint = OptionsConstraint(options={"apple",
-"banana", "orange"}) combined_constraint = OrConstraint([regex_constraint,
-options_constraint]) prompt = Prompt("Whenever I see a basketball, it reminds
-me of my favorite fruit the ") prompt = (await prompt.complete
-(model=chat_model, constraint=combined_constraint)) + "." print(prompt) #
-Whenever I see a basketball, it reminds me of my favorite fruit the orange. ```
-### Streaming Completions KeyMaker provides a very slim and intuitive means to
-access completion generation as it happens. Simply pass a prompt `complete` an
+keymaker import Prompt from keymaker.constraints import RegexConstraint import
+openai openai.api_key = "sk-" chat_model = chatgpt() prompt = Prompt("The
+weather is ") # Generate an unnamed completion constraint1 = RegexConstraint
+(pattern=r"sunny|rainy|cloudy") prompt = await prompt.complete
+(model=chat_model, constraint=constraint1) # Generate a named completion
+constraint2 = RegexConstraint(pattern=r" and (cold|warm|hot)") prompt = await
+prompt.complete( model=chat_model, constraint=constraint2, name="temperature" )
+print(prompt) # Access the unnamed completion unnamed_completion =
+prompt.completions[0] print(f"Unnamed completion: {unnamed_completion}") #
+Access the named completion named_completion = prompt.completions.temperature
+print(f"Named completion: {named_completion}") ``` Output: ``` The weather is
+sunny and warm Unnamed completion: sunny Named completion: and warm ``` In the
+example, we create a `Prompt` object with the text "The weather is ". We then
+generate an unnamed completion with a `RegexConstraint` that matches the words
+"sunny", "rainy", or "cloudy", and a named completion with a `RegexConstraint`
+that matches " and " followed by "cold", "warm", or "hot". We access the
+unnamed completion by indexing the `completions` attribute of the `Prompt`
+object, and the named completion by using the `name` as an attribute of the
+`completions` attribute. ### Model Options As it stands, the models available
+for use out of the box are `Huggingface` models and APIs implementing the
+OpenAI spec. KeyMaker is also designed to make it as simple as possible for you
+to [Add Your Own Model](#creating-custom-models) #### Huggingface (direct)
+Huggingface models are optional, and you need to install KeyMaker with `pip
+install "headjack-keymaker[huggingface]"`, then, simply import the
+`Huggingface` `Model` class: ```python from keymaker.models import Huggingface
+``` #### OpenAI OpenAI Models can be accessed out-of-the-box: ```python from
+keymaker.models import OpenAIChat, OpenAICompletion #e.g. chatgpt/gpt4, text-
+davinci-003 respectively ``` There are aliases for common models: ```python
+from keymaker.models import chatgpt, gpt4 chat_model=gpt4(...optional
+configurations for underlying `OpenAIChat` otherwise use defaults) ``` ####
+Llama-CPP KeyMaker also provides an implementation wrapper around [Llama-Cpp-
+Python](https://abetlen.github.io/llama-cpp-python) ```python from
+keymaker.models import LlamaCpp from keymaker.constraints import
+RegexConstraint from keymaker import Prompt model = LlamaCpp(model_path="~/
+Downloads/orca-mini-v2_7b.ggmlv3.q3_K_S.bin") constraint = RegexConstraint(r"I
+(eat|drink) (meat|wine)\.") prompt = Prompt("I'm a farmer and ") prompt = await
+prompt.complete(model=model, constraint=constraint) # Prompt('I'm a farmer and
+I eat meat.') ``` This can be enabled by installing the optional dependencies
+with `pip install "headjack-keymaker[llamacpp]"` #### OpenAI Compatible Servers
+**Coming Soon - Ripe for contibution** KeyMaker is looking to make the OpenAI
+`Model` support other compatible APIs. Simply pass a compatible tokenizer and
+go! ##### Llama-CPP See [Llama-Cpp-Python](https://abetlen.github.io/llama-cpp-
+python/#web-server) ##### Huggingface (API) via vLLM **Cuda Only** See [vLLM]
+(https://vllm.readthedocs.io/en/latest/getting_started/quickstart.html#openai-
+compatible-server) ### Using Chat models KeyMaker provides functionality for
+using roles with chat models. While this is optional, lack of usage could
+potentially impact performance. Chat models (e.g. `OpenAIChat` or the aliases
+`chatgpt`, `gpt`) have the following default attributes (which can vary should
+you [Add Your Own Model](#creating-custom-models)) ```python role_tag_start =
+"%" role_tag_end = "%" default_role = "assistant" allowed_roles = ("system",
+"user", "assistant") ``` This affects the way your prompt will be seen by the
+chat model. For example: ```python prompt = Prompt( """ %system%You are an
+agent that says short phrases%/system% %user%Be very excited with your
+punctuation and give me a short phrase about dogs.%/user% "Dogs are absolutely
+pawsome!" """ ) ``` would be seen by the chat model as: ```python [{'role':
+'system', 'content': 'You are an agent that says short phrases'}, {'role':
+'user', 'content': 'Be very excited with your punctuation and give me a short
+phrase about dogs.'}, {'role': 'assistant', 'content': '"Dogs are absolutely
+pawsome!"'}] ``` #### Mixing Chat and Non-Chat Models Further, should you want
+to intermingle the usage of chat and non-chat continuations, KeyMaker provides
+utilities to do so: ```python from keymaker.utils import strip_tags prompt =
+Prompt( """ %system%You are an agent that says short phrases%/system% %user%Be
+very excited with your punctuation and give me a short phrase about dogs.%/
+user% "Dogs are absolutely pawsome!" """ ) regular_prompt = strip_tags(prompt,
+roles_seps = {'system': '', 'user': 'User: ', 'assistant': 'Assistant: '},) >>>
+regular_prompt ``` Result: ```python Prompt('You are an agent that says short
+phrases User: Be very excited with your punctuation and give me a short phrase
+about dogs. Assistant: "Dogs are absolutely pawsome!"') ``` ### Using
+Constraints KeyMaker provides several out-of-the-box constraints that can be
+applied when completing prompts. KeyMaker is also designed to make it as simple
+as possible for you to [Add Your Own Constraint](#creating-custom-constraints)
+Let's go through some of the built-in constraint types and how to use them.
+#### RegexConstraint `RegexConstraint` allows you to constrain the generated
+text based on a regex pattern. ```python from keymaker.constraints import
+RegexConstraint constraint = RegexConstraint( pattern=r"I (would|could) eat [0-
+9]{1,2} (burgers|burger)\." ) prompt = await Prompt("Wow, I'm so hungry
+").complete( model=chat_model, constraint=constraint ) print(prompt) # Wow, I'm
+so hungry I would eat 11 burgers. ``` Note: This example is a little contrived
+in that there is static completion in regex itself. This is not always the most
+efficient way to do some completions. You may consider doing multiple
+completions in a case like this. KeyMaker does its best to avoid unnecessary
+calls to the model if a token is clearly determined. #### ParserConstraint
+`ParserConstraint` allows you to constrain the generated text based on a
+context-free grammar or a pre-built parser. For example, to generate text that
+follows a simple grammar: ```python from keymaker.constraints import
+ParserConstraint grammar = """ start: "A" "B" "C" """ constraint =
+ParserConstraint(grammar=grammar) ``` To apply this constraint, pass it to the
+`complete` method: ```python prompt = Prompt("Start: ") prompt = await
+prompt.complete(model=hf, constraint=constraint, name="grammar") print(prompt)
+``` #### OptionsConstraint `OptionsConstraint` allows you to constrain the
+generated text based on a list of string options. For example, to generate text
+that contains one of the following options: ```python from keymaker.constraints
+import OptionsConstraint options = {"apple", "banana", "orange"} constraint =
+OptionsConstraint(options=options) ``` To apply this constraint, pass it to the
+`complete` method: ```python prompt = Prompt("I would like an ") prompt = await
+prompt.complete(model=hf, constraint=constraint, name="fruit") print(prompt) #
+I would like an apple ``` #### StopsConstraint `StopsConstraint` allows you to
+constrain the generated text by stopping at a specified string or regex
+pattern. Say we want the model to generate between two XML tags and stop once
+it reaches the second. If we are afraid of a malformed end tag with unneeded
+whitespace, we can account for it as well. ```python constraint =
+StopsConstraint(r"<\s*/?\s*hello\s*>", include=True) prompt = Prompt( "Finish
+this phrase with an end tag then say 'finished' Hi, the world is " ) prompt =
+await prompt.complete( model=chat_model, constraint=constraint,
+name="world_description", stream=MyStream() ) print
+(prompt.completions.world_description) # beautiful. ``` #### Combining
+Constraints KeyMaker also allows you to combine multiple constraints using
+logical operators like `AndConstraint`, `OrConstraint`, and `NotConstraint`.
+```python from keymaker.constraints import OrConstraint, RegexConstraint,
+OptionsConstraint regex_constraint = RegexConstraint(pattern=r"peanut")
+options_constraint = OptionsConstraint(options={"apple", "banana", "orange"})
+combined_constraint = OrConstraint([regex_constraint, options_constraint])
+prompt = Prompt("Whenever I see a basketball, it reminds me of my favorite
+fruit the ") prompt = (await prompt.complete(model=chat_model,
+constraint=combined_constraint)) + "." print(prompt) # Whenever I see a
+basketball, it reminds me of my favorite fruit the orange. ``` ### Streaming
+Completions KeyMaker provides a very slim and intuitive means to access
+completion generation as it happens. Simply pass a prompt `complete` an
 asynchronous function ```python from typing import Optional from keymaker
 import Completion async def my_stream(completion: Optional[Completion]): print
 (completion) prompt = Prompt("Hello, I'm a talking dog and my name is") prompt
 = await prompt.complete( model=chat_model, stream=my_stream, ) # R # over # . #
 How # can # I # assist # you # today # ? # None ``` As you can see, the
 incremental tokens `R, over, ...` were passed to the `my_stream` function and
 were printed as they were generated. Further, the stream was fed a terminal
```

### Comparing `headjack_keymaker-0.0.1a2/pyproject.toml` & `headjack_keymaker-0.0.1a3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ]
 
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 license = {text = "Apache 2.0"}
 
 [project.optional-dependencies]
-huggingface=["transformers>=4.30.2", "numpy"]
+huggingface=["transformers>=4.30.2", "numpy", "torch"]
 llamacpp=["starlette>=0.28.0", "llama-cpp-python>=0.1.68", "numpy"]
 
 
 
 [tool.pdm.dev-dependencies]
 dev = [
     "cachelib>=0.9.0",
```

### Comparing `headjack_keymaker-0.0.1a2/PKG-INFO` & `headjack_keymaker-0.0.1a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: headjack-keymaker
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: The most powerful, flexible and extensible way to control the output of large language models.
 Project-URL: repository, https://github.com/KnowledgeForge/keymaker
 Author-email: circargs <nick@ouellet.dev>, Nick Ouellet <nick@ouellet.dev>
 License: Apache 2.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: openai>=0.27.8
 Requires-Dist: regex>=2023.6.3
 Requires-Dist: tiktoken>=0.4.0
 Provides-Extra: huggingface
 Requires-Dist: numpy; extra == 'huggingface'
+Requires-Dist: torch; extra == 'huggingface'
 Requires-Dist: transformers>=4.30.2; extra == 'huggingface'
 Provides-Extra: llamacpp
 Requires-Dist: llama-cpp-python>=0.1.68; extra == 'llamacpp'
 Requires-Dist: numpy; extra == 'llamacpp'
 Requires-Dist: starlette>=0.28.0; extra == 'llamacpp'
 Description-Content-Type: text/markdown
 
@@ -84,14 +85,17 @@
 
 ```sh
 pip install headjack-keymaker
 ```
 
 #### Options
 You can further optionally install KeyMaker to leverage HuggingFace or LlamaCpp directly with `[huggingface]` and/or `[llamacpp]` pip options.
+- `pip install "headjack-keymaker[huggingface]"`
+- `pip install "headjack-keymaker[llamacpp]"`
+- `pip install "headjack-keymaker[huggingface, llamacpp]"`
 
 ## Usage
 
 ### Basic Example
 
 First, note that `Prompt`s and `Completion`s are two of the fundamental types in Keymaker.
 
@@ -106,14 +110,17 @@
 
 For demo purposes, we can use a local Huggingface model
 ```python
 model = AutoModelForCausalLM.from_pretrained("gpt2")
 tokenizer = AutoTokenizer.from_pretrained("gpt2")
 
 hf = Huggingface(model=model, tokenizer=tokenizer)
+
+# OR JUST
+# hf = Huggingface(model_name="gpt2")
 ```
 
 create a prompt using the Prompt class
 ```python
 prompt: Prompt = Prompt("Dogs are known for their")
 ```
 
@@ -180,14 +187,15 @@
 All completions are stored in the `completions` attribute of a `Prompt` object.
 
 Here's an example of how to access both named and unnamed completions:
 
 ```python
 from keymaker.models import chatgpt
 from keymaker import Prompt
+from keymaker.constraints import RegexConstraint
 import openai
 
 openai.api_key = "sk-"
 
 chat_model = chatgpt()
 
 prompt = Prompt("The weather is ")
@@ -225,15 +233,15 @@
 
 ### Model Options
 As it stands, the models available for use out of the box are `Huggingface` models and APIs implementing the OpenAI spec.
 
 KeyMaker is also designed to make it as simple as possible for you to [Add Your Own Model](#creating-custom-models)
 
 #### Huggingface (direct)
-Huggingface models are optional, and you need to install KeyMaker with `pip install ...[huggingface]`, then, simply import the `Huggingface` `Model` class:
+Huggingface models are optional, and you need to install KeyMaker with `pip install "headjack-keymaker[huggingface]"`, then, simply import the `Huggingface` `Model` class:
 ```python
 from keymaker.models import Huggingface
 ```
 
 #### OpenAI
 OpenAI Models can be accessed out-of-the-box:
 ```python
@@ -261,15 +269,15 @@
 constraint = RegexConstraint(r"I (eat|drink) (meat|wine)\.")
 prompt = Prompt("I'm a farmer and ")
 
 prompt = await prompt.complete(model=model, constraint=constraint)
 # Prompt('I'm a farmer and I eat meat.')
 ```
 
-This can be enabled by installing the optional dependencies with `pip install ...[llamacpp]`
+This can be enabled by installing the optional dependencies with `pip install "headjack-keymaker[llamacpp]"`
 
 #### OpenAI Compatible Servers
 **Coming Soon - Ripe for contibution**
 
 KeyMaker is looking to make the OpenAI `Model` support other compatible APIs. Simply pass a compatible tokenizer and go!
 
 ##### Llama-CPP
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: headjack-keymaker Version: 0.0.1a2 Summary: The
+Metadata-Version: 2.1 Name: headjack-keymaker Version: 0.0.1a3 Summary: The
 most powerful, flexible and extensible way to control the output of large
 language models. Project-URL: repository, https://github.com/KnowledgeForge/
 keymaker Author-email: circargs
 ouellet.dev>, Nick Ouellet
 ouellet.dev> License: Apache 2.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 openai>=0.27.8 Requires-Dist: regex>=2023.6.3 Requires-Dist: tiktoken>=0.4.0
 Provides-Extra: huggingface Requires-Dist: numpy; extra == 'huggingface'
-Requires-Dist: transformers>=4.30.2; extra == 'huggingface' Provides-Extra:
-llamacpp Requires-Dist: llama-cpp-python>=0.1.68; extra == 'llamacpp' Requires-
-Dist: numpy; extra == 'llamacpp' Requires-Dist: starlette>=0.28.0; extra ==
-'llamacpp' Description-Content-Type: text/markdown
+Requires-Dist: torch; extra == 'huggingface' Requires-Dist:
+transformers>=4.30.2; extra == 'huggingface' Provides-Extra: llamacpp Requires-
+Dist: llama-cpp-python>=0.1.68; extra == 'llamacpp' Requires-Dist: numpy; extra
+== 'llamacpp' Requires-Dist: starlette>=0.28.0; extra == 'llamacpp'
+Description-Content-Type: text/markdown
                                     [Logo]
                               **** KeyMaker ****
  The most powerful, flexible and extensible way to control the output of large
                                language models.
                              Explore_the_docs_Â»
 
                                   Report_Bug
@@ -38,164 +39,168 @@
 Hugging Face's Transformers. It allows you to create and apply constraints on
 the generated tokens, ensuring that the output of the model meets specific
 requirements or follows a desired format. ## Installation To install KeyMaker,
 simply run the following command: ### From source: ```sh pip install https://
 github.com/KnowledgeForge/keymaker.git ``` ### From pypi: ```sh pip install
 headjack-keymaker ``` #### Options You can further optionally install KeyMaker
 to leverage HuggingFace or LlamaCpp directly with `[huggingface]` and/or `
-[llamacpp]` pip options. ## Usage ### Basic Example First, note that `Prompt`s
+[llamacpp]` pip options. - `pip install "headjack-keymaker[huggingface]"` -
+`pip install "headjack-keymaker[llamacpp]"` - `pip install "headjack-keymaker
+[huggingface, llamacpp]"` ## Usage ### Basic Example First, note that `Prompt`s
 and `Completion`s are two of the fundamental types in Keymaker. To use KeyMaker
 with a language model, you need to first create a `Model` object. For example,
 to use KeyMaker with Hugging Face's GPT-2 model: Some basic imports ```python
 from keymaker.models import Huggingface from keymaker import Prompt from
 transformers import AutoModelForCausalLM, AutoTokenizer ``` For demo purposes,
 we can use a local Huggingface model ```python model =
 AutoModelForCausalLM.from_pretrained("gpt2") tokenizer =
 AutoTokenizer.from_pretrained("gpt2") hf = Huggingface(model=model,
-tokenizer=tokenizer) ``` create a prompt using the Prompt class ```python
-prompt: Prompt = Prompt("Dogs are known for their") ``` `Prompt`s are
-interchangeable with strings ```python >>> prompt == "Dogs are known for their"
-True ``` generate a basic completion with no constraints `max_tokens` and
-`name` are optional ```python completed_prompt: Prompt = await prompt.complete
-( model=hf, max_tokens=1, name="dog_ability" ) ``` check that the original
-prompt is still the same ``` >>> prompt == "Dogs are known for their" True ```
-print out the completed prompt string ```python >>> print(completed_prompt)
-Dogs are known for their ability ``` `completed_prompt.completions` is a
-`Completions` object and gives access to any strings created from `.complete`
-calls on its parent `Prompt`. If the `Completion` was `name`d you can access it
-as an attribute on the `.completions` with `.` syntax or `['...name...']`
-```python >>> print(completed_prompt.completions.dog_ability) ability ```
+tokenizer=tokenizer) # OR JUST # hf = Huggingface(model_name="gpt2") ``` create
+a prompt using the Prompt class ```python prompt: Prompt = Prompt("Dogs are
+known for their") ``` `Prompt`s are interchangeable with strings ```python >>>
+prompt == "Dogs are known for their" True ``` generate a basic completion with
+no constraints `max_tokens` and `name` are optional ```python completed_prompt:
+Prompt = await prompt.complete( model=hf, max_tokens=1, name="dog_ability" )
+``` check that the original prompt is still the same ``` >>> prompt == "Dogs
+are known for their" True ``` print out the completed prompt string ```python
+>>> print(completed_prompt) Dogs are known for their ability ```
+`completed_prompt.completions` is a `Completions` object and gives access to
+any strings created from `.complete` calls on its parent `Prompt`. If the
+`Completion` was `name`d you can access it as an attribute on the
+`.completions` with `.` syntax or `['...name...']` ```python >>> print
+(completed_prompt.completions.dog_ability) ability ```
 `completed_prompt.completions.name` is a `Completion` object which simply
 stores the string completion and the start stop indices in the prompt ```python
 >>> print( completed_prompt[ completed_prompt.completions.dog_ability.start :
 completed_prompt.completions[ "dog_ability" ].stop ] ) ability ``` print out
 the Completions object for the completed prompt ```python >>>
 completed_prompt.completions Completions([], {'dog_ability': Completion(text =
 ' ability', start = 24, stop = 32)}) ``` ### Accessing Completions When using
 KeyMaker to generate text with constraints, you can name the completions to
 easily access them later. All completions are stored in the `completions`
 attribute of a `Prompt` object. Here's an example of how to access both named
 and unnamed completions: ```python from keymaker.models import chatgpt from
-keymaker import Prompt import openai openai.api_key = "sk-" chat_model =
-chatgpt() prompt = Prompt("The weather is ") # Generate an unnamed completion
-constraint1 = RegexConstraint(pattern=r"sunny|rainy|cloudy") prompt = await
-prompt.complete(model=chat_model, constraint=constraint1) # Generate a named
-completion constraint2 = RegexConstraint(pattern=r" and (cold|warm|hot)")
-prompt = await prompt.complete( model=chat_model, constraint=constraint2,
-name="temperature" ) print(prompt) # Access the unnamed completion
-unnamed_completion = prompt.completions[0] print(f"Unnamed completion:
-{unnamed_completion}") # Access the named completion named_completion =
-prompt.completions.temperature print(f"Named completion: {named_completion}")
-``` Output: ``` The weather is sunny and warm Unnamed completion: sunny Named
-completion: and warm ``` In the example, we create a `Prompt` object with the
-text "The weather is ". We then generate an unnamed completion with a
-`RegexConstraint` that matches the words "sunny", "rainy", or "cloudy", and a
-named completion with a `RegexConstraint` that matches " and " followed by
-"cold", "warm", or "hot". We access the unnamed completion by indexing the
-`completions` attribute of the `Prompt` object, and the named completion by
-using the `name` as an attribute of the `completions` attribute. ### Model
-Options As it stands, the models available for use out of the box are
-`Huggingface` models and APIs implementing the OpenAI spec. KeyMaker is also
-designed to make it as simple as possible for you to [Add Your Own Model]
-(#creating-custom-models) #### Huggingface (direct) Huggingface models are
-optional, and you need to install KeyMaker with `pip install ...[huggingface]`,
-then, simply import the `Huggingface` `Model` class: ```python from
-keymaker.models import Huggingface ``` #### OpenAI OpenAI Models can be
-accessed out-of-the-box: ```python from keymaker.models import OpenAIChat,
-OpenAICompletion #e.g. chatgpt/gpt4, text-davinci-003 respectively ``` There
-are aliases for common models: ```python from keymaker.models import chatgpt,
-gpt4 chat_model=gpt4(...optional configurations for underlying `OpenAIChat`
-otherwise use defaults) ``` #### Llama-CPP KeyMaker also provides an
-implementation wrapper around [Llama-Cpp-Python](https://abetlen.github.io/
-llama-cpp-python) ```python from keymaker.models import LlamaCpp from
-keymaker.constraints import RegexConstraint from keymaker import Prompt model =
-LlamaCpp(model_path="~/Downloads/orca-mini-v2_7b.ggmlv3.q3_K_S.bin") constraint
-= RegexConstraint(r"I (eat|drink) (meat|wine)\.") prompt = Prompt("I'm a farmer
-and ") prompt = await prompt.complete(model=model, constraint=constraint) #
-Prompt('I'm a farmer and I eat meat.') ``` This can be enabled by installing
-the optional dependencies with `pip install ...[llamacpp]` #### OpenAI
-Compatible Servers **Coming Soon - Ripe for contibution** KeyMaker is looking
-to make the OpenAI `Model` support other compatible APIs. Simply pass a
-compatible tokenizer and go! ##### Llama-CPP See [Llama-Cpp-Python](https://
-abetlen.github.io/llama-cpp-python/#web-server) ##### Huggingface (API) via
-vLLM **Cuda Only** See [vLLM](https://vllm.readthedocs.io/en/latest/
-getting_started/quickstart.html#openai-compatible-server) ### Using Chat models
-KeyMaker provides functionality for using roles with chat models. While this is
-optional, lack of usage could potentially impact performance. Chat models (e.g.
-`OpenAIChat` or the aliases `chatgpt`, `gpt`) have the following default
-attributes (which can vary should you [Add Your Own Model](#creating-custom-
-models)) ```python role_tag_start = "%" role_tag_end = "%" default_role =
-"assistant" allowed_roles = ("system", "user", "assistant") ``` This affects
-the way your prompt will be seen by the chat model. For example: ```python
-prompt = Prompt( """ %system%You are an agent that says short phrases%/system%
-%user%Be very excited with your punctuation and give me a short phrase about
-dogs.%/user% "Dogs are absolutely pawsome!" """ ) ``` would be seen by the chat
-model as: ```python [{'role': 'system', 'content': 'You are an agent that says
-short phrases'}, {'role': 'user', 'content': 'Be very excited with your
-punctuation and give me a short phrase about dogs.'}, {'role': 'assistant',
-'content': '"Dogs are absolutely pawsome!"'}] ``` #### Mixing Chat and Non-Chat
-Models Further, should you want to intermingle the usage of chat and non-chat
-continuations, KeyMaker provides utilities to do so: ```python from
-keymaker.utils import strip_tags prompt = Prompt( """ %system%You are an agent
-that says short phrases%/system% %user%Be very excited with your punctuation
-and give me a short phrase about dogs.%/user% "Dogs are absolutely pawsome!"
-""" ) regular_prompt = strip_tags(prompt, roles_seps = {'system': '', 'user':
-'User: ', 'assistant': 'Assistant: '},) >>> regular_prompt ``` Result:
-```python Prompt('You are an agent that says short phrases User: Be very
-excited with your punctuation and give me a short phrase about dogs. Assistant:
-"Dogs are absolutely pawsome!"') ``` ### Using Constraints KeyMaker provides
-several out-of-the-box constraints that can be applied when completing prompts.
-KeyMaker is also designed to make it as simple as possible for you to [Add Your
-Own Constraint](#creating-custom-constraints) Let's go through some of the
-built-in constraint types and how to use them. #### RegexConstraint
-`RegexConstraint` allows you to constrain the generated text based on a regex
-pattern. ```python from keymaker.constraints import RegexConstraint constraint
-= RegexConstraint( pattern=r"I (would|could) eat [0-9]{1,2} (burgers|burger)\."
-) prompt = await Prompt("Wow, I'm so hungry ").complete( model=chat_model,
-constraint=constraint ) print(prompt) # Wow, I'm so hungry I would eat 11
-burgers. ``` Note: This example is a little contrived in that there is static
-completion in regex itself. This is not always the most efficient way to do
-some completions. You may consider doing multiple completions in a case like
-this. KeyMaker does its best to avoid unnecessary calls to the model if a token
-is clearly determined. #### ParserConstraint `ParserConstraint` allows you to
-constrain the generated text based on a context-free grammar or a pre-built
-parser. For example, to generate text that follows a simple grammar: ```python
-from keymaker.constraints import ParserConstraint grammar = """ start: "A" "B"
-"C" """ constraint = ParserConstraint(grammar=grammar) ``` To apply this
-constraint, pass it to the `complete` method: ```python prompt = Prompt("Start:
-") prompt = await prompt.complete(model=hf, constraint=constraint,
-name="grammar") print(prompt) ``` #### OptionsConstraint `OptionsConstraint`
-allows you to constrain the generated text based on a list of string options.
-For example, to generate text that contains one of the following options:
-```python from keymaker.constraints import OptionsConstraint options =
-{"apple", "banana", "orange"} constraint = OptionsConstraint(options=options)
-``` To apply this constraint, pass it to the `complete` method: ```python
-prompt = Prompt("I would like an ") prompt = await prompt.complete(model=hf,
-constraint=constraint, name="fruit") print(prompt) # I would like an apple ```
-#### StopsConstraint `StopsConstraint` allows you to constrain the generated
-text by stopping at a specified string or regex pattern. Say we want the model
-to generate between two XML tags and stop once it reaches the second. If we are
-afraid of a malformed end tag with unneeded whitespace, we can account for it
-as well. ```python constraint = StopsConstraint(r"<\s*/?\s*hello\s*>",
-include=True) prompt = Prompt( "Finish this phrase with an end tag then say
-'finished' Hi, the world is " ) prompt = await prompt.complete
-( model=chat_model, constraint=constraint, name="world_description",
-stream=MyStream() ) print(prompt.completions.world_description) # beautiful.
-``` #### Combining Constraints KeyMaker also allows you to combine multiple
-constraints using logical operators like `AndConstraint`, `OrConstraint`, and
-`NotConstraint`. ```python from keymaker.constraints import OrConstraint,
-RegexConstraint, OptionsConstraint regex_constraint = RegexConstraint
-(pattern=r"peanut") options_constraint = OptionsConstraint(options={"apple",
-"banana", "orange"}) combined_constraint = OrConstraint([regex_constraint,
-options_constraint]) prompt = Prompt("Whenever I see a basketball, it reminds
-me of my favorite fruit the ") prompt = (await prompt.complete
-(model=chat_model, constraint=combined_constraint)) + "." print(prompt) #
-Whenever I see a basketball, it reminds me of my favorite fruit the orange. ```
-### Streaming Completions KeyMaker provides a very slim and intuitive means to
-access completion generation as it happens. Simply pass a prompt `complete` an
+keymaker import Prompt from keymaker.constraints import RegexConstraint import
+openai openai.api_key = "sk-" chat_model = chatgpt() prompt = Prompt("The
+weather is ") # Generate an unnamed completion constraint1 = RegexConstraint
+(pattern=r"sunny|rainy|cloudy") prompt = await prompt.complete
+(model=chat_model, constraint=constraint1) # Generate a named completion
+constraint2 = RegexConstraint(pattern=r" and (cold|warm|hot)") prompt = await
+prompt.complete( model=chat_model, constraint=constraint2, name="temperature" )
+print(prompt) # Access the unnamed completion unnamed_completion =
+prompt.completions[0] print(f"Unnamed completion: {unnamed_completion}") #
+Access the named completion named_completion = prompt.completions.temperature
+print(f"Named completion: {named_completion}") ``` Output: ``` The weather is
+sunny and warm Unnamed completion: sunny Named completion: and warm ``` In the
+example, we create a `Prompt` object with the text "The weather is ". We then
+generate an unnamed completion with a `RegexConstraint` that matches the words
+"sunny", "rainy", or "cloudy", and a named completion with a `RegexConstraint`
+that matches " and " followed by "cold", "warm", or "hot". We access the
+unnamed completion by indexing the `completions` attribute of the `Prompt`
+object, and the named completion by using the `name` as an attribute of the
+`completions` attribute. ### Model Options As it stands, the models available
+for use out of the box are `Huggingface` models and APIs implementing the
+OpenAI spec. KeyMaker is also designed to make it as simple as possible for you
+to [Add Your Own Model](#creating-custom-models) #### Huggingface (direct)
+Huggingface models are optional, and you need to install KeyMaker with `pip
+install "headjack-keymaker[huggingface]"`, then, simply import the
+`Huggingface` `Model` class: ```python from keymaker.models import Huggingface
+``` #### OpenAI OpenAI Models can be accessed out-of-the-box: ```python from
+keymaker.models import OpenAIChat, OpenAICompletion #e.g. chatgpt/gpt4, text-
+davinci-003 respectively ``` There are aliases for common models: ```python
+from keymaker.models import chatgpt, gpt4 chat_model=gpt4(...optional
+configurations for underlying `OpenAIChat` otherwise use defaults) ``` ####
+Llama-CPP KeyMaker also provides an implementation wrapper around [Llama-Cpp-
+Python](https://abetlen.github.io/llama-cpp-python) ```python from
+keymaker.models import LlamaCpp from keymaker.constraints import
+RegexConstraint from keymaker import Prompt model = LlamaCpp(model_path="~/
+Downloads/orca-mini-v2_7b.ggmlv3.q3_K_S.bin") constraint = RegexConstraint(r"I
+(eat|drink) (meat|wine)\.") prompt = Prompt("I'm a farmer and ") prompt = await
+prompt.complete(model=model, constraint=constraint) # Prompt('I'm a farmer and
+I eat meat.') ``` This can be enabled by installing the optional dependencies
+with `pip install "headjack-keymaker[llamacpp]"` #### OpenAI Compatible Servers
+**Coming Soon - Ripe for contibution** KeyMaker is looking to make the OpenAI
+`Model` support other compatible APIs. Simply pass a compatible tokenizer and
+go! ##### Llama-CPP See [Llama-Cpp-Python](https://abetlen.github.io/llama-cpp-
+python/#web-server) ##### Huggingface (API) via vLLM **Cuda Only** See [vLLM]
+(https://vllm.readthedocs.io/en/latest/getting_started/quickstart.html#openai-
+compatible-server) ### Using Chat models KeyMaker provides functionality for
+using roles with chat models. While this is optional, lack of usage could
+potentially impact performance. Chat models (e.g. `OpenAIChat` or the aliases
+`chatgpt`, `gpt`) have the following default attributes (which can vary should
+you [Add Your Own Model](#creating-custom-models)) ```python role_tag_start =
+"%" role_tag_end = "%" default_role = "assistant" allowed_roles = ("system",
+"user", "assistant") ``` This affects the way your prompt will be seen by the
+chat model. For example: ```python prompt = Prompt( """ %system%You are an
+agent that says short phrases%/system% %user%Be very excited with your
+punctuation and give me a short phrase about dogs.%/user% "Dogs are absolutely
+pawsome!" """ ) ``` would be seen by the chat model as: ```python [{'role':
+'system', 'content': 'You are an agent that says short phrases'}, {'role':
+'user', 'content': 'Be very excited with your punctuation and give me a short
+phrase about dogs.'}, {'role': 'assistant', 'content': '"Dogs are absolutely
+pawsome!"'}] ``` #### Mixing Chat and Non-Chat Models Further, should you want
+to intermingle the usage of chat and non-chat continuations, KeyMaker provides
+utilities to do so: ```python from keymaker.utils import strip_tags prompt =
+Prompt( """ %system%You are an agent that says short phrases%/system% %user%Be
+very excited with your punctuation and give me a short phrase about dogs.%/
+user% "Dogs are absolutely pawsome!" """ ) regular_prompt = strip_tags(prompt,
+roles_seps = {'system': '', 'user': 'User: ', 'assistant': 'Assistant: '},) >>>
+regular_prompt ``` Result: ```python Prompt('You are an agent that says short
+phrases User: Be very excited with your punctuation and give me a short phrase
+about dogs. Assistant: "Dogs are absolutely pawsome!"') ``` ### Using
+Constraints KeyMaker provides several out-of-the-box constraints that can be
+applied when completing prompts. KeyMaker is also designed to make it as simple
+as possible for you to [Add Your Own Constraint](#creating-custom-constraints)
+Let's go through some of the built-in constraint types and how to use them.
+#### RegexConstraint `RegexConstraint` allows you to constrain the generated
+text based on a regex pattern. ```python from keymaker.constraints import
+RegexConstraint constraint = RegexConstraint( pattern=r"I (would|could) eat [0-
+9]{1,2} (burgers|burger)\." ) prompt = await Prompt("Wow, I'm so hungry
+").complete( model=chat_model, constraint=constraint ) print(prompt) # Wow, I'm
+so hungry I would eat 11 burgers. ``` Note: This example is a little contrived
+in that there is static completion in regex itself. This is not always the most
+efficient way to do some completions. You may consider doing multiple
+completions in a case like this. KeyMaker does its best to avoid unnecessary
+calls to the model if a token is clearly determined. #### ParserConstraint
+`ParserConstraint` allows you to constrain the generated text based on a
+context-free grammar or a pre-built parser. For example, to generate text that
+follows a simple grammar: ```python from keymaker.constraints import
+ParserConstraint grammar = """ start: "A" "B" "C" """ constraint =
+ParserConstraint(grammar=grammar) ``` To apply this constraint, pass it to the
+`complete` method: ```python prompt = Prompt("Start: ") prompt = await
+prompt.complete(model=hf, constraint=constraint, name="grammar") print(prompt)
+``` #### OptionsConstraint `OptionsConstraint` allows you to constrain the
+generated text based on a list of string options. For example, to generate text
+that contains one of the following options: ```python from keymaker.constraints
+import OptionsConstraint options = {"apple", "banana", "orange"} constraint =
+OptionsConstraint(options=options) ``` To apply this constraint, pass it to the
+`complete` method: ```python prompt = Prompt("I would like an ") prompt = await
+prompt.complete(model=hf, constraint=constraint, name="fruit") print(prompt) #
+I would like an apple ``` #### StopsConstraint `StopsConstraint` allows you to
+constrain the generated text by stopping at a specified string or regex
+pattern. Say we want the model to generate between two XML tags and stop once
+it reaches the second. If we are afraid of a malformed end tag with unneeded
+whitespace, we can account for it as well. ```python constraint =
+StopsConstraint(r"<\s*/?\s*hello\s*>", include=True) prompt = Prompt( "Finish
+this phrase with an end tag then say 'finished' Hi, the world is " ) prompt =
+await prompt.complete( model=chat_model, constraint=constraint,
+name="world_description", stream=MyStream() ) print
+(prompt.completions.world_description) # beautiful. ``` #### Combining
+Constraints KeyMaker also allows you to combine multiple constraints using
+logical operators like `AndConstraint`, `OrConstraint`, and `NotConstraint`.
+```python from keymaker.constraints import OrConstraint, RegexConstraint,
+OptionsConstraint regex_constraint = RegexConstraint(pattern=r"peanut")
+options_constraint = OptionsConstraint(options={"apple", "banana", "orange"})
+combined_constraint = OrConstraint([regex_constraint, options_constraint])
+prompt = Prompt("Whenever I see a basketball, it reminds me of my favorite
+fruit the ") prompt = (await prompt.complete(model=chat_model,
+constraint=combined_constraint)) + "." print(prompt) # Whenever I see a
+basketball, it reminds me of my favorite fruit the orange. ``` ### Streaming
+Completions KeyMaker provides a very slim and intuitive means to access
+completion generation as it happens. Simply pass a prompt `complete` an
 asynchronous function ```python from typing import Optional from keymaker
 import Completion async def my_stream(completion: Optional[Completion]): print
 (completion) prompt = Prompt("Hello, I'm a talking dog and my name is") prompt
 = await prompt.complete( model=chat_model, stream=my_stream, ) # R # over # . #
 How # can # I # assist # you # today # ? # None ``` As you can see, the
 incremental tokens `R, over, ...` were passed to the `my_stream` function and
 were printed as they were generated. Further, the stream was fed a terminal
```

