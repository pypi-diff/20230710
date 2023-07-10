# Comparing `tmp/open_gpt_torch-0.0.7.dev3.tar.gz` & `tmp/open_gpt_torch-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gpt_torch-0.0.7.dev3.tar", max compression
+gzip compressed data, was "open_gpt_torch-0.0.8.tar", max compression
```

## Comparing `open_gpt_torch-0.0.7.dev3.tar` & `open_gpt_torch-0.0.8.tar`

### file list

```diff
@@ -1,51 +1,66 @@
--rw-r--r--   0        0        0    10825 2023-06-13 07:38:41.535460 open_gpt_torch-0.0.7.dev3/LICENSE
--rw-r--r--   0        0        0     7610 2023-06-13 07:38:41.535460 open_gpt_torch-0.0.7.dev3/README.md
--rw-r--r--   0        0        0      929 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/__init__.py
--rw-r--r--   0        0        0      107 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/__main__.py
--rw-r--r--   0        0        0        0 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/__init__.py
--rw-r--r--   0        0        0     1057 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/application.py
--rw-r--r--   0        0        0      508 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/command_loader.py
--rw-r--r--   0        0        0        0 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/__init__.py
--rw-r--r--   0        0        0      567 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/about.py
--rw-r--r--   0        0        0      953 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/playground.py
--rw-r--r--   0        0        0     2223 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/serve.py
--rw-r--r--   0        0        0     5293 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/factory.py
--rw-r--r--   0        0        0     2523 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/helper.py
--rw-r--r--   0        0        0      490 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/logs.py
--rw-r--r--   0        0        0        0 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/__init__.py
--rw-r--r--   0        0        0     2420 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/embedding.py
--rw-r--r--   0        0        0        0 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0        0        0     6038 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0        0        0     9040 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/flamingo_model.py
--rw-r--r--   0        0        0     5585 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/loading.py
--rw-r--r--   0        0        0     2439 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0        0        0    11346 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/generation.py
--rw-r--r--   0        0        0        0 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/llama/__init__.py
--rw-r--r--   0        0        0     2877 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/llama/loading.py
--rw-r--r--   0        0        0      863 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/llama/modeling.py
--rw-r--r--   0        0        0     2856 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/loading.py
--rw-r--r--   0        0        0     2564 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/modeling.py
--rw-r--r--   0        0        0        0 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/moss/__init__.py
--rw-r--r--   0        0        0     3504 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/moss/modeling.py
--rw-r--r--   0        0        0        0 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/pythia/__init__.py
--rw-r--r--   0        0        0      653 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/pythia/modeling.py
--rw-r--r--   0        0        0        0 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/rwkv/__init__.py
--rw-r--r--   0        0        0     1233 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/rwkv/modeling.py
--rw-r--r--   0        0        0        0 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/stablelm/__init__.py
--rw-r--r--   0        0        0     2608 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/stablelm/modeling.py
--rw-r--r--   0        0        0        0 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/vicuna/__init__.py
--rw-r--r--   0        0        0     7439 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/vicuna/loading.py
--rw-r--r--   0        0        0     1428 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/vicuna/modeling.py
--rw-r--r--   0        0        0     3507 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/profile.py
--rw-r--r--   0        0        0        0 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/__init__.py
--rw-r--r--   0        0        0       36 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/executors/__init__.py
--rw-r--r--   0        0        0     1977 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/executors/base.py
--rw-r--r--   0        0        0     2373 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/executors/flamingo.py
--rw-r--r--   0        0        0      171 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/executors/utils.py
--rw-r--r--   0        0        0     3429 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/gateway.py
--rw-r--r--   0        0        0        0 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/__init__.py
--rw-r--r--   0        0        0     4686 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/gradio.py
--rw-r--r--   0        0        0     7396 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/gradio_chatbot.py
--rw-r--r--   0        0        0     2714 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/gradio_css.py
--rw-r--r--   0        0        0     3242 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/pyproject.toml
--rw-r--r--   0        0        0    20871 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.7.dev3/PKG-INFO
+-rw-r--r--   0        0        0    10825 2023-07-10 05:55:46.054553 open_gpt_torch-0.0.8/LICENSE
+-rw-r--r--   0        0        0     7788 2023-07-10 05:55:46.054553 open_gpt_torch-0.0.8/README.md
+-rw-r--r--   0        0        0     1006 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/__init__.py
+-rw-r--r--   0        0        0      107 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/__init__.py
+-rw-r--r--   0        0        0     1087 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/application.py
+-rw-r--r--   0        0        0      508 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/command_loader.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/commands/__init__.py
+-rw-r--r--   0        0        0      567 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/commands/about.py
+-rw-r--r--   0        0        0     3151 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/commands/deploy.py
+-rw-r--r--   0        0        0      953 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/commands/playground.py
+-rw-r--r--   0        0        0      611 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/commands/quantize.py
+-rw-r--r--   0        0        0     2429 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/commands/serve.py
+-rw-r--r--   0        0        0     6075 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/factory.py
+-rw-r--r--   0        0        0     2741 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/helper.py
+-rw-r--r--   0        0        0      490 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/logs.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/models/__init__.py
+-rw-r--r--   0        0        0     2420 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/models/embedding.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0        0        0      601 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/config.json
+-rw-r--r--   0        0        0     3607 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/configuration_flamingo.py
+-rw-r--r--   0        0        0     5954 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0        0        0     9481 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/flamingo_model.py
+-rw-r--r--   0        0        0     6484 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0        0        0     2439 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0        0        0    11873 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/generation.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/llama/__init__.py
+-rw-r--r--   0        0        0     2877 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/llama/loading.py
+-rw-r--r--   0        0        0      863 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/llama/modeling.py
+-rw-r--r--   0        0        0     2856 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/loading.py
+-rw-r--r--   0        0        0     2564 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/modeling.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/moss/__init__.py
+-rw-r--r--   0        0        0     3504 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/moss/modeling.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0        0        0      653 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/pythia/modeling.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/rwkv/__init__.py
+-rw-r--r--   0        0        0     1233 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/rwkv/modeling.py
+-rw-r--r--   0        0        0     1908 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/session.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     2608 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/stablelm/modeling.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/vicuna/__init__.py
+-rw-r--r--   0        0        0     7439 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/vicuna/loading.py
+-rw-r--r--   0        0        0     1428 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/vicuna/modeling.py
+-rw-r--r--   0        0        0     6368 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/profile.py
+-rw-r--r--   0        0        0     1115 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/resources/flow.yml.jinja2
+-rw-r--r--   0        0        0       29 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/__init__.py
+-rw-r--r--   0        0        0       75 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/executors/__init__.py
+-rw-r--r--   0        0        0     2117 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/executors/base.py
+-rw-r--r--   0        0        0     2373 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/executors/flamingo.py
+-rw-r--r--   0        0        0      171 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/executors/utils.py
+-rw-r--r--   0        0        0      773 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/flow.py
+-rw-r--r--   0        0        0     3782 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/gateway.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/playground/__init__.py
+-rw-r--r--   0        0        0     4686 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/playground/gradio.py
+-rw-r--r--   0        0        0     7396 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/serve/playground/gradio_chatbot.py
+-rw-r--r--   0        0        0     2714 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/serve/playground/gradio_css.py
+-rw-r--r--   0        0        0     6210 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/datautils.py
+-rw-r--r--   0        0        0     4781 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/quant_groups.py
+-rw-r--r--   0        0        0     1707 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/quantize.py
+-rw-r--r--   0        0        0     2257 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/quantizeargs.py
+-rw-r--r--   0        0        0    11420 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/quantutils.py
+-rw-r--r--   0        0        0    13691 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/spqr_engine.py
+-rw-r--r--   0        0        0      201 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/test.py
+-rw-r--r--   0        0        0     2221 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/weight_permutation.py
+-rw-r--r--   0        0        0     3274 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    21115 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.8/PKG-INFO
```

### Comparing `open_gpt_torch-0.0.7.dev3/LICENSE` & `open_gpt_torch-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/README.md` & `open_gpt_torch-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -197,22 +197,32 @@
 💡 **Tip**: To display the list of available commands, please use the `list` command.
 
 ## Cloud-native deployment
 
 You can also deploy the server to a cloud provider like Jina Cloud or AWS.
 To do so, you can use `deploy` command:
 
-- Jina Cloud
+### Jina Cloud
+
+using predefined executor
 
 ```bash
-opengpt deploy stabilityai/stablelm-tuned-alpha-3b --device cuda --precision fp16 --provider jina --name opengpt --replicas 2
+opengpt deploy stabilityai/stablelm-tuned-alpha-3b --precision fp16 --device_map balanced --cloud jina --replicas 1
 ```
 
-**TBD ...**
+It will give you a HTTP url and a gRPC url by default:
+```bash
+https://{random-host-name}-http.wolf.jina.ai
+grpcs://{random-host-name}-grpc.wolf.jina.ai
+```
+
+
+### AWS
 
+TBD
 
 ## Contributing
 
 We welcome contributions from the community! To contribute, please submit a pull request following our contributing guidelines.
 
 ## License
```

#### html2text {}

```diff
@@ -83,14 +83,16 @@
 server: ```python from open_gpt import Client client = Client() # connect to
 the model server model = client.get_model(endpoint='grpc://0.0.0.0:51000')
 prompt = "The quick brown fox jumps over the lazy dog." output = model.generate
 ( prompt, max_length=100, temperature=0.9, top_k=50, top_p=0.95,
 repetition_penalty=1.2, do_sample=True, num_return_sequences=1, ) ``` ð¡
 **Tip**: To display the list of available commands, please use the `list`
 command. ## Cloud-native deployment You can also deploy the server to a cloud
-provider like Jina Cloud or AWS. To do so, you can use `deploy` command: - Jina
-Cloud ```bash opengpt deploy stabilityai/stablelm-tuned-alpha-3b --device cuda
---precision fp16 --provider jina --name opengpt --replicas 2 ``` **TBD ...** ##
-Contributing We welcome contributions from the community! To contribute, please
-submit a pull request following our contributing guidelines. ## License OpenGPT
-is licensed under the Apache License, Version 2.0. See LICENSE for the full
-license text.
+provider like Jina Cloud or AWS. To do so, you can use `deploy` command: ###
+Jina Cloud using predefined executor ```bash opengpt deploy stabilityai/
+stablelm-tuned-alpha-3b --precision fp16 --device_map balanced --cloud jina --
+replicas 1 ``` It will give you a HTTP url and a gRPC url by default: ```bash
+https://{random-host-name}-http.wolf.jina.ai grpcs://{random-host-name}-
+grpc.wolf.jina.ai ``` ### AWS TBD ## Contributing We welcome contributions from
+the community! To contribute, please submit a pull request following our
+contributing guidelines. ## License OpenGPT is licensed under the Apache
+License, Version 2.0. See LICENSE for the full license text.
```

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/__init__.py` & `open_gpt_torch-0.0.8/open_gpt/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,12 +30,14 @@
     :return: The version number.
     """
     return importlib_metadata.version(__package__ + '_torch')
 
 
 __version__ = get_version()
 
+__resources_path__ = _os.path.join(_os.path.dirname(__file__), 'resources')
+
 _os.environ['NO_VERSION_CHECK'] = '1'
 
 from inference_client import Client
 
 from .factory import create_model
```

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/cli/application.py` & `open_gpt_torch-0.0.8/open_gpt/cli/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
     return _load
 
 
 COMMANDS = [
     "about",
     "serve",
+    "deploy",
     "playground",
+    "quantize",
 ]
 
 
 class Application(BaseApplication):
     def __init__(self) -> None:
         super().__init__("opengpt", __version__)
```

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/about.py` & `open_gpt_torch-0.0.8/open_gpt/cli/commands/about.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/playground.py` & `open_gpt_torch-0.0.8/open_gpt/cli/commands/playground.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/serve.py` & `open_gpt_torch-0.0.8/open_gpt/cli/commands/serve.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from cleo.commands.command import Command
 from cleo.helpers import argument, option
 
 
 class ServeCommand(Command):
     name = "serve"
 
-    description = "Start a model serving."
+    description = "Start a model serving locally in gRPC and HTTP."
 
     arguments = [argument("model_name", "The name of the model to serve.")]
     options = [
         option(
             'grpc_port',
             None,
             'The gRPC port to serve the model on.',
@@ -24,15 +24,19 @@
             default=51002,
         ),
         option('enable_cors', None, 'Enable CORS.', flag=True),
         option(
             'precision', None, 'The precision of the model.', flag=False, default='fp16'
         ),
         option(
-            'adapter_name_or_path', None, 'The name or path of the adapter checkpoint.'
+            'adapter_name_or_path',
+            None,
+            'The name or path of the adapter checkpoint.',
+            flag=False,
+            default=None,
         ),
         option(
             'device_map',
             None,
             'The device map of the model.',
             flag=False,
             default='balanced',
@@ -41,32 +45,34 @@
             "replicas", "r", "The number of replicas to serve.", flag=False, default=1
         ),
     ]
 
     help = """\
     This command allows you to start a model serving in protocol gRPC and HTTP.
     
-    To start a model serving, you can run:
+    To start a model serving locally, you can run:
         
-        <comment>opengpt serve facebook/llama-7b</comment>"""
+        <comment>opengpt serve stabilityai/stablelm-tuned-alpha-3b</comment>"""
 
     def handle(self) -> int:
         from open_gpt.factory import create_flow
 
         with create_flow(
-            self.argument('model_name'),
+            model_name_or_path=self.argument('model_name'),
             grpc_port=self.option('grpc_port'),
             http_port=self.option('http_port'),
             cors=self.option('enable_cors'),
             uses_with={
                 'precision': self.option('precision'),
                 'adapter_name_or_path': self.option('adapter_name_or_path'),
                 'device_map': self.option('device_map'),
             },
             replicas=self.option('replicas'),
+            dockerized=False,
+            return_yaml=False,
         ) as flow:
             self.line(
                 f'<info>The model is ready to be used at port {self.option("grpc_port")} (gRPC) and {self.option("http_port")} (HTTP).</info>'
             )
             flow.block()
 
         return 0
```

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/factory.py` & `open_gpt_torch-0.0.8/open_gpt/factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os.path
 from pathlib import Path
 from typing import List, Optional, Union
 
 import torch
 
 
 def create_model(
@@ -97,15 +98,17 @@
         return FlamingoModel(
             model_name,
             device=device,
             precision=precision,
             device_map=device_map,
             **kwargs,
         )
-    elif model_name.startswith('sgugger/rwkv') or model_name.startswith('ybelkada/rwkv'):
+    elif model_name.startswith('sgugger/rwkv') or model_name.startswith(
+        'ybelkada/rwkv'
+    ):
         from .models.rwkv.modeling import RWKVModel
 
         return RWKVModel(
             model_name,
             device=device,
             precision=precision,
             device_map=device_map,
@@ -125,43 +128,59 @@
 
 
 def create_flow(
     model_name_or_path: str,
     grpc_port: int = 51001,
     http_port: int = 51002,
     cors: bool = False,
-    adapter_name_or_path: Optional[str] = None,
-    uses_with: Optional[dict] = {},
+    uses_with: dict = {},
     replicas: int = 1,
+    instance_type: Optional[str] = None,
+    dockerized: bool = False,
+    return_yaml: bool = True,
 ):
     from jina import Flow
 
-    if 'flamingo' in model_name_or_path:
-        from .serve.executors.flamingo import FlamingoExecutor as Executor
-    else:
-        from .serve.executors import CausualLMExecutor as Executor
-
-    from .serve.gateway import Gateway
+    from open_gpt import __jina_version__, __version__
+    from open_gpt.serve.flow import get_template
 
     # normalize the model name to be used as flow executor name
     norm_name = model_name_or_path.split('/')[-1]
     norm_name = norm_name.replace('-', '_').replace('.', '_').lower()
 
-    uses_with['model_name_or_path'] = model_name_or_path
-    uses_with['adapter_name_or_path'] = adapter_name_or_path
-
-    return (
-        Flow()
-        .config_gateway(
-            uses=Gateway,
-            port=[grpc_port, http_port],
-            protocol=['grpc', 'http'],
-            cors=cors,
-        )
-        .add(
-            uses=Executor,
-            uses_with=uses_with,
-            name=f'{norm_name}_executor',
-            replicas=replicas,
-            timeout_ready=-1,
-        )
+    # HOTFIX: patch to avoid to use pre-release version
+    __VERSION_TAG__ = f'v{__version__}'
+    if 'dev' in __version__:
+        __VERSION_TAG__ = 'latest'
+
+    deployment_params = {
+        'deployment_name': f'{norm_name}',
+        'http_port': http_port,
+        'grpc_port': grpc_port,
+        'executor_params': {
+            'model_name_or_path': model_name_or_path,
+            'adapter_name_or_path': uses_with.get('adapter_name_or_path') or '',
+            'precision': uses_with.get('precision', 'fp16'),
+            'device_map': uses_with.get('device_map', 'balanced'),
+        },
+        'gateway_params': {'cors': cors},
+        'jina_version': __jina_version__,
+        'replicas': replicas,
+        'labels': {'app': 'open_gpt', 'version': __VERSION_TAG__},
+    }
+
+    yaml = get_template('flow.yml.jinja2').render(
+        dockerized=dockerized,
+        gateway_image=f'docker://jinaai/open_gpt_gateway:{__VERSION_TAG__}',
+        gateway_module='Gateway',
+        executor_image=f'docker://jinaai/open_gpt_executor:{__VERSION_TAG__}',
+        executor_module='CausualLMExecutor'
+        if 'flamingo' not in model_name_or_path
+        else 'FlamingoExecutor',
+        instance_type=instance_type,
+        **deployment_params,
     )
+
+    if return_yaml:
+        return yaml
+    else:
+        return Flow.load_config(yaml)
```

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/helper.py` & `open_gpt_torch-0.0.8/open_gpt/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,7 +103,18 @@
     cudnn.benchmark = False
     cudnn.deterministic = True
 
 
 def utcnow() -> datetime:
     """Return the current utc date and time with tzinfo set to UTC."""
     return datetime.now(timezone.utc)
+
+
+def asyncify(f):
+    import asyncio
+    from functools import wraps
+
+    @wraps(f)
+    def wrapper(*args, **kwargs):
+        return asyncio.get_event_loop().run_until_complete(f(*args, **kwargs))
+
+    return wrapper
```

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/embedding.py` & `open_gpt_torch-0.0.8/open_gpt/models/embedding.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/flamingo_lm.py` & `open_gpt_torch-0.0.8/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,62 +6,62 @@
 from open_flamingo.src.helpers import GatedCrossAttentionBlock
 from open_flamingo.src.utils import getattr_recursive, setattr_recursive
 
 from ...helper import auto_dtype_and_device
 
 
 class FlamingoLayer(nn.Module):
-    def __init__(self, gated_cross_attn_layer, decoder_layer):
+    def __init__(self, gated_cross_attn_layer: nn.Module, decoder_layer: nn.Module):
         super().__init__()
         self.gated_cross_attn_layer = gated_cross_attn_layer
         self.decoder_layer = decoder_layer
         self.vis_x = None
         self.media_locations = None
-        self.device = self.decoder_layer.parameters().__next__().device
+
+        self._device = self.decoder_layer.parameters().__next__().device
+        self._dtype = self.decoder_layer.parameters().__next__().dtype
+
+        if self._dtype not in [torch.float16, torch.float32]:
+            self._dtype = torch.float16
 
         # This is a hack to guarantee that the gated_cross_attn_layer is on the same device as the decoder_layer
         if self.gated_cross_attn_layer is not None:
-            self.gated_cross_attn_layer.to(self.device)
+            self.gated_cross_attn_layer.to(self._device).to(self._dtype)
 
     def is_conditioned(self) -> bool:
         """Check whether the layer is conditioned."""
         return self.vis_x is not None
 
     # Used this great idea from this implementation of Flamingo (https://github.com/dhansmair/flamingo-mini/)
-    def condition_vis_x(self, vis_x):
-        self.vis_x = vis_x.to(self.device) if vis_x is not None else vis_x
+    def condition_vis_x(self, vis_x) -> None:
+        self.vis_x = vis_x
 
-    def condition_media_locations(self, media_locations):
-        self.media_locations = (
-            media_locations.to(self.device)
-            if media_locations is not None
-            else media_locations
-        )
+    def condition_media_locations(self, media_locations) -> None:
+        self.media_locations = media_locations
 
-    def condition_attend_previous(self, attend_previous):
+    def condition_attend_previous(self, attend_previous) -> None:
         self.attend_previous = attend_previous
 
     def forward(
         self,
-        lang_x,
-        attention_mask=None,
+        lang_x: torch.Tensor,
+        attention_mask: Optional[torch.Tensor] = None,
         **decoder_layer_kwargs,
     ):
         if self.gated_cross_attn_layer is None:
             return self.decoder_layer(
                 lang_x, attention_mask=attention_mask, **decoder_layer_kwargs
             )
 
         if self.vis_x is None:
             raise ValueError("vis_x must be conditioned before forward pass")
 
         if self.media_locations is None:
             raise ValueError("media_locations must be conditioned before forward pass")
 
-        lang_x = lang_x.to(self.device)
         lang_x = self.gated_cross_attn_layer(
             lang_x,
             self.vis_x,
             media_locations=self.media_locations,
             attend_previous=self.attend_previous,
         )
         lang_x = self.decoder_layer(
@@ -82,30 +82,30 @@
         return getattr_recursive(self, self.decoder_layers_attr_name)
 
     def _set_decoder_layers(self, value):
         setattr_recursive(self, self.decoder_layers_attr_name, value)
 
     def init_flamingo(
         self,
-        media_token_id,
-        vis_hidden_size,
-        cross_attn_every_n_layers,
-        use_media_placement_augmentation,
+        media_token_id: int,
+        vis_hidden_size: int,
+        cross_attn_every_n_layers: int,
+        use_media_placement_augmentation: bool,
         only_attend_previous: bool,
-        device: Optional[Union[str, 'torch.device']] = None,
-        dtype: Optional[Union[str, 'torch.dtype']] = None,
     ):
         """
         Initialize Flamingo by adding a new gated cross attn to the decoder. Store the media token id for computing the media locations.
         """
 
         self.gated_cross_attn_layers = nn.ModuleList(
             [
                 GatedCrossAttentionBlock(
-                    dim=self.config.hidden_size, dim_visual=vis_hidden_size
+                    dim=self.config.hidden_size,
+                    dim_visual=vis_hidden_size,
+                    # only_attend_previous=only_attend_previous,
                 )
                 if (layer_idx + 1) % cross_attn_every_n_layers == 0
                 else None
                 for layer_idx, _ in enumerate(self._get_decoder_layers())
             ]
         )
         self._set_decoder_layers(
@@ -116,48 +116,43 @@
                         self.gated_cross_attn_layers, self._get_decoder_layers()
                     )
                 ]
             )
         )
         self.media_token_id = media_token_id
         self.use_media_placement_augmentation = use_media_placement_augmentation
-        self.initialized_flamingo = True
         self.only_attend_previous = only_attend_previous
+        self.initialized_flamingo = True
 
-        dtype, device = auto_dtype_and_device(dtype, device)
-        if str(dtype) == 'torch.float16':
-            self.gated_cross_attn_layers.half()
-        # self.gated_cross_attn_layers.to(device)
-
-    def forward(self, *input, **kwargs):
+    def call_forward(self, *input, **kwargs):
         """Condition the Flamingo layers on the media locations before forward()"""
-
         if not self.initialized_flamingo:
             raise ValueError(
                 "Flamingo layers are not initialized. Please call `init_flamingo` first."
             )
 
         input_ids = kwargs["input_ids"] if "input_ids" in kwargs else input[0]
         media_locations = input_ids == self.media_token_id
         # IMPORTANT: Force `attend_previous` to True when we place training data as <image>caption<|endofchunk|>
         # attend_previous = (
         #     (random.random() < 0.5) if self.use_media_placement_augmentation else False
         # )
         attend_previous = self.only_attend_previous
 
         for layer in self.get_decoder().layers:
+            # print(f'===> layer: {layer}')
             layer.condition_media_locations(media_locations)
             layer.condition_attend_previous(attend_previous)
 
         return super().forward(
             *input, **kwargs
         )  # Call the other parent's forward method
 
     def is_conditioned(self) -> bool:
         """Check whether all decoder layers are already conditioned."""
         return all(l.is_conditioned() for l in self._get_decoder_layers())
 
-    def clear_conditioned_layers(self):
+    def clear_conditioned_layers(self) -> None:
         for layer in self._get_decoder_layers():
             layer.condition_vis_x(None)
             layer.condition_media_locations(None)
             layer.condition_attend_previous(None)
```

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/flamingo_model.py` & `open_gpt_torch-0.0.8/open_gpt/models/flamingo/flamingo_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from typing import Callable, Optional, Union
 
 import torch
-from accelerate.hooks import AlignDevicesHook, add_hook_to_module
 from einops import rearrange
 from open_flamingo.src.helpers import PerceiverResampler
 from torch import nn
 
 from open_gpt.logs import logger
 
 from ...helper import auto_dtype_and_device
 
 
 class FlamingoLMModel(nn.Module):
+
+    base_model_prefix = "flamingo"
+    _no_split_modules = ["FlamingoPerceiverBlock", "CLIPEncoderLayer", "FlamingoLayer"]
+
     def __init__(
         self,
         vision_encoder: 'nn.Module',
         language_model: 'nn.Module',
         device: Optional[Union[str, 'torch.device']] = None,
         dtype: Optional[Union[str, 'torch.dtype']] = None,
         model_config: dict = {},
@@ -27,46 +30,76 @@
         :param vision_encoder: the vision encoder to extract visual features, e.g. CLIP model
         :param language_model: the language model to extract textual features and generate the output texts, e.g., LLaMa model
         :param model_config: a dictionary of model configuration
         :param device: the device to run the model on
         :param dtype: the data type to run the model on
         :param kwargs: other arguments
         """
+
         super().__init__()
 
-        self.dtype, self.device = auto_dtype_and_device(dtype, device)
+        self._dtype, self._device = auto_dtype_and_device(dtype, device)
 
         self.model_config = model_config
         self.vision_encoder = vision_encoder
         self.lang_encoder = language_model
 
         self.perceiver = PerceiverResampler(dim=self.model_config['image_size'])
-        if str(self.dtype) == 'torch.float16':
+        if str(self._dtype) == 'torch.float16':
             self.perceiver.half()
-        elif str(self.dtype) == 'torch.int8':
-            raise NotImplementedError('int8 is not supported yet')
-        self.perceiver.to(self.device)
+        self.perceiver.to(self._device)
 
         self.media_token_id = model_config['media_token_id']
         self.end_chunk_token_id = model_config['end_chunk_token_id']
 
         logger.debug(
             f"media_token_id: {self.media_token_id}, end_chunk_token_id: {self.end_chunk_token_id}"
         )
 
         self.lang_encoder.init_flamingo(
             media_token_id=self.media_token_id,
             vis_hidden_size=model_config['image_size'],
             cross_attn_every_n_layers=model_config['cross_attn_every_n_layers'],
             use_media_placement_augmentation=True,
             only_attend_previous=True,
-            dtype=dtype,
-            device=device,
         )
 
+        if hasattr(self.lang_encoder, "_hf_hook"):
+            # logger.debug(f'lang_encoder has _hf_hook, {self.lang_encoder._hf_hook}')
+            import functools
+
+            from accelerate.hooks import add_hook_to_module, remove_hook_from_module
+
+            hook = self.lang_encoder._hf_hook
+
+            remove_hook_from_module(self.lang_encoder)
+
+            old_forward = self.lang_encoder.call_forward
+
+            self.lang_encoder = hook.init_hook(self.lang_encoder)
+            self.lang_encoder._hf_hook = hook
+
+            @functools.wraps(old_forward)
+            def new_forward(*args, **kwargs):
+                args, kwargs = self.lang_encoder._hf_hook.pre_forward(
+                    self.lang_encoder, *args, **kwargs
+                )
+                if self.lang_encoder._hf_hook.no_grad:
+                    with torch.no_grad():
+                        output = old_forward(*args, **kwargs)
+                else:
+                    output = old_forward(*args, **kwargs)
+                return self.lang_encoder._hf_hook.post_forward(
+                    self.lang_encoder, output
+                )
+
+            self.lang_encoder.forward = new_forward
+
+            # add_hook_to_module(self.lang_encoder, old_hook)
+
     def forward(
         self,
         vision_inputs: 'torch.Tensor',
         text_inputs: 'torch.Tensor',
         attention_mask: Optional['torch.Tensor'] = None,
         labels: Optional['torch.Tensor'] = None,
         past_key_values: Optional['torch.Tensor'] = None,
@@ -131,46 +164,27 @@
         :param length_penalty: length penalty. Defaults to 1.0.
         :param num_return_sequences: number of return sequences. Defaults to 1.
         :param do_sample: whether to sample or not. Defaults to False.
         :param early_stopping: whether to stop early or not. Defaults to False.
 
         :return: text_inputs with generated tokens appended to it (batch_size, sequence_length)
         """
-
-        # if hasattr(self, "_hf_hook"):
-        # add a hook to make sure that the output of lang_encoder is mapped to the same device as the text_inputs
-        hook = AlignDevicesHook(
-            execution_device=self.device,
-            io_same_device=True,
-            place_submodules=False,
-        )
-        add_hook_to_module(self.lang_encoder, hook)
-
-        vision_inputs = vision_inputs.to(dtype=self.dtype, device=self.device)
-        # if attention_mask is not None:
-        #     attention_mask = attention_mask.to(self.device)
-        text_inputs = text_inputs.to(self.device)
+        vision_inputs = vision_inputs.to(dtype=self._dtype, device=self._device)
+        text_inputs = text_inputs.to(self._device)
 
         if num_beams > 1:
             vision_inputs = vision_inputs.repeat_interleave(num_beams, dim=0)
 
         _vision_x = self._vision_encode(vision_inputs=vision_inputs)
 
         if not self.lang_encoder.initialized_flamingo:
             raise ValueError(
                 "Flamingo layers are not initialized. Please call `init_flamingo` first."
             )
 
-        media_locations = text_inputs == self.media_token_id
-        attend_previous = False
-
-        for layer in self.lang_encoder.get_decoder().layers:
-            layer.condition_media_locations(media_locations)
-            layer.condition_attend_previous(attend_previous)
-
         output = self.lang_encoder.generate(
             text_inputs,
             attention_mask=attention_mask,
             eos_token_id=self.end_chunk_token_id,
             num_beams=num_beams,
             max_new_tokens=max_new_tokens,
             temperature=temperature,
@@ -204,17 +218,17 @@
         ), "vision_inputs should be of shape (B, T, F, Channels, Height, Width)"
         B, T, F = vision_inputs.shape[:3]
         assert F == 1, "Only single frame supported"
 
         vision_x = rearrange(vision_inputs, "B T F c h w -> (B T F) c h w")
 
         with torch.no_grad():
-            vision_x = self.vision_encoder.visual(vision_x)[1]
+            vision_x = self.vision_encoder.visual(
+                vision_x.to(self._dtype).to(self._device)
+            )[1]
 
         vision_x = rearrange(vision_x, "(B T F) v d -> B T F v d", B=B, T=T, F=F)
 
         vision_x = self.perceiver(vision_x)  # reshapes to (B, T, n, d)
 
         for layer in self.lang_encoder._get_decoder_layers():
             layer.condition_vis_x(vision_x)
-
-        return vision_x
```

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/loading.py` & `open_gpt_torch-0.0.8/open_gpt/models/flamingo/loading.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,19 +91,41 @@
     extend_instance(lang_model, FlamingoLMMixin)
 
     if decoder_layers_attr_name is None:
         decoder_layers_attr_name = _infer_decoder_layers_attr_name(lang_model)
     lang_model.set_decoder_layers_attr_name(decoder_layers_attr_name)
     lang_model.resize_token_embeddings(len(tokenizer))
 
+    # flamingo_config = {
+    #     "image_size": open_clip.get_model_config(model_name)["vision_cfg"]["width"],
+    #     "cross_attn_every_n_layers": 4,
+    #     "end_chunk_token_id": tokenizer.encode("<|endofchunk|>")[-1],
+    #     "media_token_id": tokenizer.encode("<image>")[-1],
+    # }
+
     flamingo_config = {
+        "model_type": "flamingo",
         "image_size": open_clip.get_model_config(model_name)["vision_cfg"]["width"],
         "cross_attn_every_n_layers": 4,
         "end_chunk_token_id": tokenizer.encode("<|endofchunk|>")[-1],
         "media_token_id": tokenizer.encode("<image>")[-1],
+        "tie_word_embeddings": False,
+        "use_media_placement_augmentation": True,
+        "only_attend_previous": True,
+        "text_config": {"_name_or_path": "yahma/llama-7b-hf", "model_type": "llama"},
+        "vision_config": {
+            "_name_or_path": "openai/clip-vit-large-patch14",
+            "model_type": "clip_vision_model",
+            "hidden_size": 1024,
+            "intermediate_size": 4096,
+            "num_attention_heads": 16,
+            "num_hidden_layers": 24,
+            "image_size": 224,
+            "patch_size": 14,
+        },
     }
 
     model = FlamingoLMModel(
         clip_model,
         lang_model,
         model_config=flamingo_config,
         device=device,
```

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/modeling.py` & `open_gpt_torch-0.0.8/open_gpt/models/flamingo/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/generation.py` & `open_gpt_torch-0.0.8/open_gpt/models/generation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import TYPE_CHECKING, Iterable, List, Optional, overload
+import logging
+from typing import TYPE_CHECKING, Iterable, List, Optional, Tuple, overload
 
 import torch
 
 if TYPE_CHECKING:
     from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from transformers.generation.logits_process import (
@@ -58,29 +59,31 @@
         top_p: float = 0.9,
         repetition_penalty: float = 1.0,
         max_context_length: int = CONTEXT_LEN,
         echo: bool = False,
         stream_interval: int = 1,
         stop_str: Optional[str] = None,
         stop_token_ids: List[int] = [],
-        **kwargs
+        past_key_values: Optional[Iterable[torch.Tensor]] = None,
+        **kwargs,
     ):
         """Generate tokens in a streaming fashion. This method is a modified version of `fastchat.server.inference.generate_stream`.
 
         :param prompt: The prompt is the context that the model will use to generate the response.
         :param max_new_tokens: The maximum number of tokens to generate. If None, the model will generate until it predicts a stop token.
         :param temperature: The temperature to use when sampling from the logits.
         :param top_k: The number of highest probability vocabulary tokens to keep for top-k-filtering.
         :param top_p: The cumulative probability of parameter highest probability vocabulary tokens to keep for nucleus sampling.
         :param repetition_penalty: The parameter for repetition penalty. 1.0 means no penalty. See `this paper <https://arxiv.org/pdf/1909.05858.pdf>`__ for more details.
         :param max_context_length: Maximum length of the context. If the context is longer than this, it will be truncated.
         :param echo: If True, the prompt will be included in the generated response.
         :param stream_interval: The number of tokens to generate before returning the generated tokens.
         :param stop_str: If not None, the model will stop generating when the generated tokens end with this string.
         :param stop_token_ids: A list of token ids that will cause the model to stop generating.
+        :param past_key_values: A list of past key values to use for generation. If None, the model will generate from scratch.
         :param kwargs: Additional keyword arguments to pass to the model.
         :return:
         """
         len_prompt = len(prompt)
         input_ids = self.tokenizer(prompt, return_tensors="pt")["input_ids"].to(
             self._device
         )
@@ -98,29 +101,34 @@
         output_ids = input_ids.tolist()[0]
 
         max_src_len = max_context_length - max_new_tokens - 8
         if input_length > max_src_len:
             input_ids = input_ids[:, -max_src_len:]
             input_length = max_src_len
 
-        past_key_values = next_token = None
+        next_token = None
 
         for step in range(max_new_tokens):
             if step == 0:
-                outputs = self.model(input_ids, use_cache=True)
+                outputs = self.model(
+                    input_ids, use_cache=True, past_key_values=past_key_values
+                )
                 logits = outputs.logits
                 past_key_values = outputs.past_key_values
             else:
                 outputs = self.model(
                     input_ids=torch.as_tensor([[next_token]], device=self._device),
                     use_cache=True,
                     past_key_values=past_key_values,
                 )
                 logits = outputs.logits
                 past_key_values = outputs.past_key_values
+            logging.debug(
+                f"===> step: {step}, past_key_values: {type(past_key_values)}, {type(past_key_values[0])}"
+            )
 
             if logits_processor:
                 if repetition_penalty > 1.0:
                     tmp_output_ids = torch.as_tensor([output_ids], device=logits.device)
                 else:
                     tmp_output_ids = None
                 last_token_logits = logits_processor(tmp_output_ids, logits[:, -1, :])[
@@ -179,14 +187,15 @@
                     else:
                         raise ValueError("Invalid stop field type.")
 
                 # prevent yielding partial stop sequence
                 if not partially_stopped:
                     yield {
                         "generated_text": output,
+                        "past_key_values": past_key_values,
                         "usage": {
                             "prompt_length": input_length,
                             "completed_tokens": step + 1,
                             "total_tokens": input_length + step + 1,
                         },
                         "finish_reason": None,
                     }
@@ -200,14 +209,15 @@
         elif stopped:
             finish_reason = "stop"
         else:
             finish_reason = None
 
         yield {
             "generated_text": output,
+            "past_key_values": past_key_values,
             "usage": {
                 "prompt_length": input_length,
                 "completed_tokens": step + 1,
                 "total_tokens": input_length + step + 1,
             },
             "finish_reason": finish_reason,
         }
@@ -226,15 +236,15 @@
         temperature: float = 1.0,
         top_k: int = 1,
         top_p: float = 0.9,
         repetition_penalty: float = 1.0,
         length_penalty: float = 1.0,
         no_repeat_ngram_size: int = 0,
         echo: bool = False,
-        **kwargs
+        **kwargs,
     ):
         """Generate text from the given prompt.
 
         :param prompt: The prompt input text.
         :param max_new_tokens: The maximum number of tokens to generate, not including the prompt.
         :param num_beams: Number of beams for beam search. 1 means no beam search.
         :param do_sample: Whether to use sampling instead of greedy decoding.
```

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/llama/loading.py` & `open_gpt_torch-0.0.8/open_gpt/models/llama/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/llama/modeling.py` & `open_gpt_torch-0.0.8/open_gpt/models/llama/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/loading.py` & `open_gpt_torch-0.0.8/open_gpt/models/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/modeling.py` & `open_gpt_torch-0.0.8/open_gpt/models/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/moss/modeling.py` & `open_gpt_torch-0.0.8/open_gpt/models/moss/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/pythia/modeling.py` & `open_gpt_torch-0.0.8/open_gpt/models/pythia/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/rwkv/modeling.py` & `open_gpt_torch-0.0.8/open_gpt/models/rwkv/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/stablelm/modeling.py` & `open_gpt_torch-0.0.8/open_gpt/models/stablelm/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/vicuna/loading.py` & `open_gpt_torch-0.0.8/open_gpt/models/vicuna/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/models/vicuna/modeling.py` & `open_gpt_torch-0.0.8/open_gpt/models/vicuna/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/serve/executors/base.py` & `open_gpt_torch-0.0.8/open_gpt/serve/executors/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """The executor wraps the model and provides a simple way to run inference on the model."""
 
 from multiprocessing.pool import ThreadPool
 from typing import Dict, List, Optional, Union
 
-import torch
 from docarray import DocumentArray
 from jina import Executor, requests
 
 from open_gpt.factory import create_model
 from open_gpt.logs import logger
 
 
@@ -47,13 +46,17 @@
     @requests(on='/generate')
     def generate(self, docs: 'DocumentArray', parameters: Dict = {}, **kwargs):
         prompted_da = DocumentArray(
             [d for d in docs if d.tags.get('prompt') or d.text is not None]
         )
         prompts = [d.tags['prompt'] or d.text for d in prompted_da]
 
+        for k, v in parameters.items():
+            if k in ['top_k', 'max_new_tokens', 'num_return_sequences']:
+                parameters[k] = int(v)
+
         if prompts:
             result = self.model.generate(prompts, **parameters)
             for d, r in zip(prompted_da, result):
                 d.tags['generated_text'] = r
         else:
             logger.warning('No prompts found in the request.')
```

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/serve/executors/flamingo.py` & `open_gpt_torch-0.0.8/open_gpt/serve/executors/flamingo.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/serve/gateway.py` & `open_gpt_torch-0.0.8/open_gpt/serve/gateway.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """The serve module provides a simple way to serve a model using Jina."""
-from typing import List
 
 import jina
 from jina import Document, DocumentArray
 from jina import Gateway as BaseGateway
 from jina.serve.runtimes.servers.composite import CompositeServer
 from pydantic import BaseModel, Field
 
 
 class GenerateRequest(BaseModel):
     prompt: str = Field(..., description='The prompt to generate from.')
 
+    # session id
+    session_id: str = Field(
+        description='The session id of the generation.', default=None
+    )
+
     # generation parameters
     num_beams: int = Field(description='The number of beams to use.', default=None)
-    max_length: int = Field(
+    max_new_tokens: int = Field(
         description='The maximum length of the generated text.', default=None
     )
     temperature: float = Field(
         description='The temperature of the generation.', default=None
     )
     top_k: int = Field(description='The top k of the generation.', default=None)
     top_p: float = Field(description='The top p of the generation.', default=None)
@@ -34,16 +38,17 @@
     class Config:
         allow_population_by_field_name = True
         arbitrary_types_allowed = True
 
         schema_extra = {
             'example': {
                 'prompt': 'Hello, my name is',
+                'session_id': '18d92585-7b66-4b7c-b818-71287c122c57',
                 'num_beams': 5,
-                'max_length': 50,
+                'max_new_tokens': 50,
                 'temperature': 0.7,
                 'top_k': 50,
                 'top_p': 0.95,
                 'repetition_penalty': 1.0,
                 'do_sample': True,
                 'num_return_sequences': 3,
             }
@@ -70,27 +75,33 @@
                     exclude_unset=True,
                     exclude_none=True,
                     exclude_defaults=True,
                     exclude={'prompt'},
                 )
 
                 async for docs, error in self.streamer.stream(
-                    docs=DocumentArray([Document(text=payload.prompt)]),
+                    docs=DocumentArray(
+                        [
+                            Document(
+                                tags={'prompt': payload.prompt},
+                            )
+                        ]
+                    ),
                     exec_endpoint='/generate',
                     parameters=parameters,
                 ):
                     if error:
                         return JSONResponse(
                             status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
                             content={'message': error.name},
                         )
                     else:
                         return JSONResponse(
                             status_code=status.HTTP_200_OK,
                             content={
-                                'generated_text': docs[0].tags.get('generated_text')
+                                'generated_text': docs[0].tags.get('generated_text'),
                             },
                         )
 
             return app
 
         jina.helper.extend_rest_interface = _extend_rest_function
```

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/gradio.py` & `open_gpt_torch-0.0.8/open_gpt/serve/playground/gradio.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/gradio_chatbot.py` & `open_gpt_torch-0.0.8/open_gpt/serve/playground/gradio_chatbot.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/gradio_css.py` & `open_gpt_torch-0.0.8/open_gpt/serve/playground/gradio_css.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev3/pyproject.toml` & `open_gpt_torch-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open_gpt_torch"
-version = "0.0.7.dev3"
+version = "0.0.8"
 description = "An open-source cloud-native of large multi-modal models (LMMs) serving framework."
 
 license = "Apache-2.0"
 
 authors = [
     "Jina AI <hello@jina.ai>"
 ]
@@ -44,22 +44,24 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 # Compatible Python versions
 python = ">=3.8,<4.0"
 jina = "^3.17.0"
 docarray = "^0.21.0"
+jcloud = "^0.2.11"
 inference-client = "^0.0.4"
 pydantic = "^1.10.0"
 loguru = "^0.5"
 cleo = "^2.0.0"
 click = "^8.1.3"
+Jinja2 = "^3.1.2"
 numpy = "^1.21.2"
 einops = "^0.6.0"
-tensorboard = "^2.11.2"
+tensorboard = "<2.11.2"
 transformers = "^4.30.1"
 bitsandbytes = "^0.39.0"
 accelerate = "^0.20.3"
 tqdm = "^4.62.3"
 peft = "^0.3.0"
 
 # A list of all of the optional dependencies, some of which are included in the
```

### Comparing `open_gpt_torch-0.0.7.dev3/PKG-INFO` & `open_gpt_torch-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-gpt-torch
-Version: 0.0.7.dev3
+Version: 0.0.8
 Summary: An open-source cloud-native of large multi-modal models (LMMs) serving framework.
 Home-page: https://github.com/jina-ai/opengpt
 License: Apache-2.0
 Keywords: Pytorch,LMM,GPT,LLM,multi-modality,cloud-native,model-serving,model-inference,llama,vicuna,stabellm
 Author: Jina AI
 Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0
@@ -23,33 +23,35 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: flamingo
 Provides-Extra: playground
 Provides-Extra: profile
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: accelerate (>=0.20.3,<0.21.0)
 Requires-Dist: bitsandbytes (>=0.39.0,<0.40.0)
 Requires-Dist: cleo (>=2.0.0,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: docarray (>=0.21.0,<0.22.0)
 Requires-Dist: einops (>=0.6.0,<0.7.0)
 Requires-Dist: gradio (>=3.30.0,<4.0.0) ; extra == "playground"
 Requires-Dist: inference-client (>=0.0.4,<0.0.5)
+Requires-Dist: jcloud (>=0.2.11,<0.3.0)
 Requires-Dist: jina (>=3.17.0,<4.0.0)
 Requires-Dist: loguru (>=0.5,<0.6)
 Requires-Dist: markdown2 (>=2.4.0,<3.0.0) ; extra == "playground"
 Requires-Dist: mdtex2html (>=1.2.0,<2.0.0) ; extra == "playground"
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: open-flamingo (>=0.0.2,<0.0.3) ; extra == "flamingo"
 Requires-Dist: open_clip_torch (>=2.20.0,<3.0.0) ; extra == "flamingo"
 Requires-Dist: peft (>=0.3.0,<0.4.0)
 Requires-Dist: psutil (>=5.8.0,<6.0.0) ; extra == "profile"
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
-Requires-Dist: tensorboard (>=2.11.2,<3.0.0)
+Requires-Dist: tensorboard (<2.11.2)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Requires-Dist: transformers (>=4.30.1,<5.0.0)
 Project-URL: Repository, https://github.com/jina-ai/opengpt
 Description-Content-Type: text/markdown
 
 # ☄️ OpenGPT
 
@@ -250,22 +252,32 @@
 💡 **Tip**: To display the list of available commands, please use the `list` command.
 
 ## Cloud-native deployment
 
 You can also deploy the server to a cloud provider like Jina Cloud or AWS.
 To do so, you can use `deploy` command:
 
-- Jina Cloud
+### Jina Cloud
+
+using predefined executor
 
 ```bash
-opengpt deploy stabilityai/stablelm-tuned-alpha-3b --device cuda --precision fp16 --provider jina --name opengpt --replicas 2
+opengpt deploy stabilityai/stablelm-tuned-alpha-3b --precision fp16 --device_map balanced --cloud jina --replicas 1
 ```
 
-**TBD ...**
+It will give you a HTTP url and a gRPC url by default:
+```bash
+https://{random-host-name}-http.wolf.jina.ai
+grpcs://{random-host-name}-grpc.wolf.jina.ai
+```
+
+
+### AWS
 
+TBD
 
 ## Contributing
 
 We welcome contributions from the community! To contribute, please submit a pull request following our contributing guidelines.
 
 ## License
```

#### html2text {}

```diff
@@ -1,40 +1,41 @@
-Metadata-Version: 2.1 Name: open-gpt-torch Version: 0.0.7.dev3 Summary: An
-open-source cloud-native of large multi-modal models (LMMs) serving framework.
-Home-page: https://github.com/jina-ai/opengpt License: Apache-2.0 Keywords:
+Metadata-Version: 2.1 Name: open-gpt-torch Version: 0.0.8 Summary: An open-
+source cloud-native of large multi-modal models (LMMs) serving framework. Home-
+page: https://github.com/jina-ai/opengpt License: Apache-2.0 Keywords:
 Pytorch,LMM,GPT,LLM,multi-modality,cloud-native,model-serving,model-
 inference,llama,vicuna,stabellm Author: Jina AI Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
 Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Provides-Extra: flamingo Provides-Extra: playground
-Provides-Extra: profile Requires-Dist: accelerate (>=0.20.3,<0.21.0) Requires-
-Dist: bitsandbytes (>=0.39.0,<0.40.0) Requires-Dist: cleo (>=2.0.0,<3.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: docarray
-(>=0.21.0,<0.22.0) Requires-Dist: einops (>=0.6.0,<0.7.0) Requires-Dist: gradio
-(>=3.30.0,<4.0.0) ; extra == "playground" Requires-Dist: inference-client
-(>=0.0.4,<0.0.5) Requires-Dist: jina (>=3.17.0,<4.0.0) Requires-Dist: loguru
-(>=0.5,<0.6) Requires-Dist: markdown2 (>=2.4.0,<3.0.0) ; extra == "playground"
-Requires-Dist: mdtex2html (>=1.2.0,<2.0.0) ; extra == "playground" Requires-
-Dist: numpy (>=1.21.2,<2.0.0) Requires-Dist: open-flamingo (>=0.0.2,<0.0.3) ;
-extra == "flamingo" Requires-Dist: open_clip_torch (>=2.20.0,<3.0.0) ; extra ==
-"flamingo" Requires-Dist: peft (>=0.3.0,<0.4.0) Requires-Dist: psutil
-(>=5.8.0,<6.0.0) ; extra == "profile" Requires-Dist: pydantic (>=1.10.0,<2.0.0)
-Requires-Dist: tensorboard (>=2.11.2,<3.0.0) Requires-Dist: tqdm
-(>=4.62.3,<5.0.0) Requires-Dist: transformers (>=4.30.1,<5.0.0) Project-URL:
-Repository, https://github.com/jina-ai/opengpt Description-Content-Type: text/
-markdown # âï¸ OpenGPT
+Provides-Extra: profile Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) Requires-Dist:
+accelerate (>=0.20.3,<0.21.0) Requires-Dist: bitsandbytes (>=0.39.0,<0.40.0)
+Requires-Dist: cleo (>=2.0.0,<3.0.0) Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: docarray (>=0.21.0,<0.22.0) Requires-Dist: einops
+(>=0.6.0,<0.7.0) Requires-Dist: gradio (>=3.30.0,<4.0.0) ; extra ==
+"playground" Requires-Dist: inference-client (>=0.0.4,<0.0.5) Requires-Dist:
+jcloud (>=0.2.11,<0.3.0) Requires-Dist: jina (>=3.17.0,<4.0.0) Requires-Dist:
+loguru (>=0.5,<0.6) Requires-Dist: markdown2 (>=2.4.0,<3.0.0) ; extra ==
+"playground" Requires-Dist: mdtex2html (>=1.2.0,<2.0.0) ; extra == "playground"
+Requires-Dist: numpy (>=1.21.2,<2.0.0) Requires-Dist: open-flamingo
+(>=0.0.2,<0.0.3) ; extra == "flamingo" Requires-Dist: open_clip_torch
+(>=2.20.0,<3.0.0) ; extra == "flamingo" Requires-Dist: peft (>=0.3.0,<0.4.0)
+Requires-Dist: psutil (>=5.8.0,<6.0.0) ; extra == "profile" Requires-Dist:
+pydantic (>=1.10.0,<2.0.0) Requires-Dist: tensorboard (<2.11.2) Requires-Dist:
+tqdm (>=4.62.3,<5.0.0) Requires-Dist: transformers (>=4.30.1,<5.0.0) Project-
+URL: Repository, https://github.com/jina-ai/opengpt Description-Content-Type:
+text/markdown # âï¸ OpenGPT
   [OpenGPT:_An_open-source_cloud-native_large-scale_multimodal_model_serving
                                   framework]
 > "A playful and whimsical vector art of a Stochastic Tigger, wearing a t-shirt
 with a "GPT" text printed logo, surrounded by colorful geometric shapes. âar
 1:1 âupbeta" > > â Prompts and logo art was produced with [PromptPerfect]
 (https://promptperfect.jina.ai/) & [Stable Diffusion X](https://clipdrop.co/
 stable-diffusion) ![](https://img.shields.io/badge/Made%20with-JinaAI-
@@ -115,140 +116,143 @@
 server: ```python from open_gpt import Client client = Client() # connect to
 the model server model = client.get_model(endpoint='grpc://0.0.0.0:51000')
 prompt = "The quick brown fox jumps over the lazy dog." output = model.generate
 ( prompt, max_length=100, temperature=0.9, top_k=50, top_p=0.95,
 repetition_penalty=1.2, do_sample=True, num_return_sequences=1, ) ``` ð¡
 **Tip**: To display the list of available commands, please use the `list`
 command. ## Cloud-native deployment You can also deploy the server to a cloud
-provider like Jina Cloud or AWS. To do so, you can use `deploy` command: - Jina
-Cloud ```bash opengpt deploy stabilityai/stablelm-tuned-alpha-3b --device cuda
---precision fp16 --provider jina --name opengpt --replicas 2 ``` **TBD ...** ##
-Contributing We welcome contributions from the community! To contribute, please
-submit a pull request following our contributing guidelines. ## License OpenGPT
-is licensed under the Apache License, Version 2.0. See LICENSE for the full
-license text. Copyright 2020-2022 Jina AI Limited. All rights reserved. Apache
-License Version 2.0, January 2004 http://www.apache.org/licenses/ TERMS AND
-CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION 1. Definitions. "License"
-shall mean the terms and conditions for use, reproduction, and distribution as
-defined by Sections 1 through 9 of this document. "Licensor" shall mean the
-copyright owner or entity authorized by the copyright owner that is granting
-the License. "Legal Entity" shall mean the union of the acting entity and all
-other entities that control, are controlled by, or are under common control
-with that entity. For the purposes of this definition, "control" means (i) the
-power, direct or indirect, to cause the direction or management of such entity,
-whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or
-more of the outstanding shares, or (iii) beneficial ownership of such entity.
-"You" (or "Your") shall mean an individual or Legal Entity exercising
-permissions granted by this License. "Source" form shall mean the preferred
-form for making modifications, including but not limited to software source
-code, documentation source, and configuration files. "Object" form shall mean
-any form resulting from mechanical transformation or translation of a Source
-form, including but not limited to compiled object code, generated
-documentation, and conversions to other media types. "Work" shall mean the work
-of authorship, whether in Source or Object form, made available under the
-License, as indicated by a copyright notice that is included in or attached to
-the work (an example is provided in the Appendix below). "Derivative Works"
-shall mean any work, whether in Source or Object form, that is based on (or
-derived from) the Work and for which the editorial revisions, annotations,
-elaborations, or other modifications represent, as a whole, an original work of
-authorship. For the purposes of this License, Derivative Works shall not
-include works that remain separable from, or merely link (or bind by name) to
-the interfaces of, the Work and Derivative Works thereof. "Contribution" shall
-mean any work of authorship, including the original version of the Work and any
-modifications or additions to that Work or Derivative Works thereof, that is
-intentionally submitted to Licensor for inclusion in the Work by the copyright
-owner or by an individual or Legal Entity authorized to submit on behalf of the
-copyright owner. For the purposes of this definition, "submitted" means any
-form of electronic, verbal, or written communication sent to the Licensor or
-its representatives, including but not limited to communication on electronic
-mailing lists, source code control systems, and issue tracking systems that are
-managed by, or on behalf of, the Licensor for the purpose of discussing and
-improving the Work, but excluding communication that is conspicuously marked or
-otherwise designated in writing by the copyright owner as "Not a Contribution."
-"Contributor" shall mean Licensor and any individual or Legal Entity on behalf
-of whom a Contribution has been received by Licensor and subsequently
-incorporated within the Work. 2. Grant of Copyright License. Subject to the
-terms and conditions of this License, each Contributor hereby grants to You a
-perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-copyright license to reproduce, prepare Derivative Works of, publicly display,
-publicly perform, sublicense, and distribute the Work and such Derivative Works
-in Source or Object form. 3. Grant of Patent License. Subject to the terms and
-conditions of this License, each Contributor hereby grants to You a perpetual,
-worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as
-stated in this section) patent license to make, have made, use, offer to sell,
-sell, import, and otherwise transfer the Work, where such license applies only
-to those patent claims licensable by such Contributor that are necessarily
-infringed by their Contribution(s) alone or by combination of their
-Contribution(s) with the Work to which such Contribution(s) was submitted. If
-You institute patent litigation against any entity (including a cross-claim or
-counterclaim in a lawsuit) alleging that the Work or a Contribution
-incorporated within the Work constitutes direct or contributory patent
-infringement, then any patent licenses granted to You under this License for
-that Work shall terminate as of the date such litigation is filed. 4.
-Redistribution. You may reproduce and distribute copies of the Work or
-Derivative Works thereof in any medium, with or without modifications, and in
-Source or Object form, provided that You meet the following conditions: (a) You
-must give any other recipients of the Work or Derivative Works a copy of this
-License; and (b) You must cause any modified files to carry prominent notices
-stating that You changed the files; and (c) You must retain, in the Source form
-of any Derivative Works that You distribute, all copyright, patent, trademark,
-and attribution notices from the Source form of the Work, excluding those
-notices that do not pertain to any part of the Derivative Works; and (d) If the
-Work includes a "NOTICE" text file as part of its distribution, then any
-Derivative Works that You distribute must include a readable copy of the
-attribution notices contained within such NOTICE file, excluding those notices
-that do not pertain to any part of the Derivative Works, in at least one of the
-following places: within a NOTICE text file distributed as part of the
-Derivative Works; within the Source form or documentation, if provided along
-with the Derivative Works; or, within a display generated by the Derivative
-Works, if and wherever such third-party notices normally appear. The contents
-of the NOTICE file are for informational purposes only and do not modify the
-License. You may add Your own attribution notices within Derivative Works that
-You distribute, alongside or as an addendum to the NOTICE text from the Work,
-provided that such additional attribution notices cannot be construed as
-modifying the License. You may add Your own copyright statement to Your
-modifications and may provide additional or different license terms and
-conditions for use, reproduction, or distribution of Your modifications, or for
-any such Derivative Works as a whole, provided Your use, reproduction, and
-distribution of the Work otherwise complies with the conditions stated in this
-License. 5. Submission of Contributions. Unless You explicitly state otherwise,
-any Contribution intentionally submitted for inclusion in the Work by You to
-the Licensor shall be under the terms and conditions of this License, without
-any additional terms or conditions. Notwithstanding the above, nothing herein
-shall supersede or modify the terms of any separate license agreement you may
-have executed with Licensor regarding such Contributions. 6. Trademarks. This
-License does not grant permission to use the trade names, trademarks, service
-marks, or product names of the Licensor, except as required for reasonable and
-customary use in describing the origin of the Work and reproducing the content
-of the NOTICE file. 7. Disclaimer of Warranty. Unless required by applicable
-law or agreed to in writing, Licensor provides the Work (and each Contributor
-provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR
-CONDITIONS OF ANY KIND, either express or implied, including, without
-limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT,
-MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely
-responsible for determining the appropriateness of using or redistributing the
-Work and assume any risks associated with Your exercise of permissions under
-this License. 8. Limitation of Liability. In no event and under no legal
-theory, whether in tort (including negligence), contract, or otherwise, unless
-required by applicable law (such as deliberate and grossly negligent acts) or
-agreed to in writing, shall any Contributor be liable to You for damages,
-including any direct, indirect, special, incidental, or consequential damages
-of any character arising as a result of this License or out of the use or
-inability to use the Work (including but not limited to damages for loss of
-goodwill, work stoppage, computer failure or malfunction, or any and all other
-commercial damages or losses), even if such Contributor has been advised of the
-possibility of such damages. 9. Accepting Warranty or Additional Liability.
-While redistributing the Work or Derivative Works thereof, You may choose to
-offer, and charge a fee for, acceptance of support, warranty, indemnity, or
-other liability obligations and/or rights consistent with this License.
-However, in accepting such obligations, You may act only on Your own behalf and
-on Your sole responsibility, not on behalf of any other Contributor, and only
-if You agree to indemnify, defend, and hold each Contributor harmless for any
-liability incurred by, or claims asserted against, such Contributor by reason
-of your accepting any such warranty or additional liability. END OF TERMS AND
+provider like Jina Cloud or AWS. To do so, you can use `deploy` command: ###
+Jina Cloud using predefined executor ```bash opengpt deploy stabilityai/
+stablelm-tuned-alpha-3b --precision fp16 --device_map balanced --cloud jina --
+replicas 1 ``` It will give you a HTTP url and a gRPC url by default: ```bash
+https://{random-host-name}-http.wolf.jina.ai grpcs://{random-host-name}-
+grpc.wolf.jina.ai ``` ### AWS TBD ## Contributing We welcome contributions from
+the community! To contribute, please submit a pull request following our
+contributing guidelines. ## License OpenGPT is licensed under the Apache
+License, Version 2.0. See LICENSE for the full license text. Copyright 2020-
+2022 Jina AI Limited. All rights reserved. Apache License Version 2.0, January
+2004 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE,
+REPRODUCTION, AND DISTRIBUTION 1. Definitions. "License" shall mean the terms
+and conditions for use, reproduction, and distribution as defined by Sections 1
+through 9 of this document. "Licensor" shall mean the copyright owner or entity
+authorized by the copyright owner that is granting the License. "Legal Entity"
+shall mean the union of the acting entity and all other entities that control,
+are controlled by, or are under common control with that entity. For the
+purposes of this definition, "control" means (i) the power, direct or indirect,
+to cause the direction or management of such entity, whether by contract or
+otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding
+shares, or (iii) beneficial ownership of such entity. "You" (or "Your") shall
+mean an individual or Legal Entity exercising permissions granted by this
+License. "Source" form shall mean the preferred form for making modifications,
+including but not limited to software source code, documentation source, and
+configuration files. "Object" form shall mean any form resulting from
+mechanical transformation or translation of a Source form, including but not
+limited to compiled object code, generated documentation, and conversions to
+other media types. "Work" shall mean the work of authorship, whether in Source
+or Object form, made available under the License, as indicated by a copyright
+notice that is included in or attached to the work (an example is provided in
+the Appendix below). "Derivative Works" shall mean any work, whether in Source
+or Object form, that is based on (or derived from) the Work and for which the
+editorial revisions, annotations, elaborations, or other modifications
+represent, as a whole, an original work of authorship. For the purposes of this
+License, Derivative Works shall not include works that remain separable from,
+or merely link (or bind by name) to the interfaces of, the Work and Derivative
+Works thereof. "Contribution" shall mean any work of authorship, including the
+original version of the Work and any modifications or additions to that Work or
+Derivative Works thereof, that is intentionally submitted to Licensor for
+inclusion in the Work by the copyright owner or by an individual or Legal
+Entity authorized to submit on behalf of the copyright owner. For the purposes
+of this definition, "submitted" means any form of electronic, verbal, or
+written communication sent to the Licensor or its representatives, including
+but not limited to communication on electronic mailing lists, source code
+control systems, and issue tracking systems that are managed by, or on behalf
+of, the Licensor for the purpose of discussing and improving the Work, but
+excluding communication that is conspicuously marked or otherwise designated in
+writing by the copyright owner as "Not a Contribution." "Contributor" shall
+mean Licensor and any individual or Legal Entity on behalf of whom a
+Contribution has been received by Licensor and subsequently incorporated within
+the Work. 2. Grant of Copyright License. Subject to the terms and conditions of
+this License, each Contributor hereby grants to You a perpetual, worldwide,
+non-exclusive, no-charge, royalty-free, irrevocable copyright license to
+reproduce, prepare Derivative Works of, publicly display, publicly perform,
+sublicense, and distribute the Work and such Derivative Works in Source or
+Object form. 3. Grant of Patent License. Subject to the terms and conditions of
+this License, each Contributor hereby grants to You a perpetual, worldwide,
+non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this
+section) patent license to make, have made, use, offer to sell, sell, import,
+and otherwise transfer the Work, where such license applies only to those
+patent claims licensable by such Contributor that are necessarily infringed by
+their Contribution(s) alone or by combination of their Contribution(s) with the
+Work to which such Contribution(s) was submitted. If You institute patent
+litigation against any entity (including a cross-claim or counterclaim in a
+lawsuit) alleging that the Work or a Contribution incorporated within the Work
+constitutes direct or contributory patent infringement, then any patent
+licenses granted to You under this License for that Work shall terminate as of
+the date such litigation is filed. 4. Redistribution. You may reproduce and
+distribute copies of the Work or Derivative Works thereof in any medium, with
+or without modifications, and in Source or Object form, provided that You meet
+the following conditions: (a) You must give any other recipients of the Work or
+Derivative Works a copy of this License; and (b) You must cause any modified
+files to carry prominent notices stating that You changed the files; and (c)
+You must retain, in the Source form of any Derivative Works that You
+distribute, all copyright, patent, trademark, and attribution notices from the
+Source form of the Work, excluding those notices that do not pertain to any
+part of the Derivative Works; and (d) If the Work includes a "NOTICE" text file
+as part of its distribution, then any Derivative Works that You distribute must
+include a readable copy of the attribution notices contained within such NOTICE
+file, excluding those notices that do not pertain to any part of the Derivative
+Works, in at least one of the following places: within a NOTICE text file
+distributed as part of the Derivative Works; within the Source form or
+documentation, if provided along with the Derivative Works; or, within a
+display generated by the Derivative Works, if and wherever such third-party
+notices normally appear. The contents of the NOTICE file are for informational
+purposes only and do not modify the License. You may add Your own attribution
+notices within Derivative Works that You distribute, alongside or as an
+addendum to the NOTICE text from the Work, provided that such additional
+attribution notices cannot be construed as modifying the License. You may add
+Your own copyright statement to Your modifications and may provide additional
+or different license terms and conditions for use, reproduction, or
+distribution of Your modifications, or for any such Derivative Works as a
+whole, provided Your use, reproduction, and distribution of the Work otherwise
+complies with the conditions stated in this License. 5. Submission of
+Contributions. Unless You explicitly state otherwise, any Contribution
+intentionally submitted for inclusion in the Work by You to the Licensor shall
+be under the terms and conditions of this License, without any additional terms
+or conditions. Notwithstanding the above, nothing herein shall supersede or
+modify the terms of any separate license agreement you may have executed with
+Licensor regarding such Contributions. 6. Trademarks. This License does not
+grant permission to use the trade names, trademarks, service marks, or product
+names of the Licensor, except as required for reasonable and customary use in
+describing the origin of the Work and reproducing the content of the NOTICE
+file. 7. Disclaimer of Warranty. Unless required by applicable law or agreed to
+in writing, Licensor provides the Work (and each Contributor provides its
+Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+KIND, either express or implied, including, without limitation, any warranties
+or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+PARTICULAR PURPOSE. You are solely responsible for determining the
+appropriateness of using or redistributing the Work and assume any risks
+associated with Your exercise of permissions under this License. 8. Limitation
+of Liability. In no event and under no legal theory, whether in tort (including
+negligence), contract, or otherwise, unless required by applicable law (such as
+deliberate and grossly negligent acts) or agreed to in writing, shall any
+Contributor be liable to You for damages, including any direct, indirect,
+special, incidental, or consequential damages of any character arising as a
+result of this License or out of the use or inability to use the Work
+(including but not limited to damages for loss of goodwill, work stoppage,
+computer failure or malfunction, or any and all other commercial damages or
+losses), even if such Contributor has been advised of the possibility of such
+damages. 9. Accepting Warranty or Additional Liability. While redistributing
+the Work or Derivative Works thereof, You may choose to offer, and charge a fee
+for, acceptance of support, warranty, indemnity, or other liability obligations
+and/or rights consistent with this License. However, in accepting such
+obligations, You may act only on Your own behalf and on Your sole
+responsibility, not on behalf of any other Contributor, and only if You agree
+to indemnify, defend, and hold each Contributor harmless for any liability
+incurred by, or claims asserted against, such Contributor by reason of your
+accepting any such warranty or additional liability. END OF TERMS AND
 CONDITIONS Copyright 2020-2022 Jina AI Limited Licensed under the Apache
 License, Version 2.0 (the "License"); you may not use this file except in
 compliance with the License. You may obtain a copy of the License at http://
 www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
 to in writing, software distributed under the License is distributed on an "AS
 IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 implied. See the License for the specific language governing permissions and
```

