# Comparing `tmp/open_gpt_torch-0.0.8.tar.gz` & `tmp/open-gpt-torch-0.0.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gpt_torch-0.0.8.tar", max compression
+gzip compressed data, was "open-gpt-torch-0.0.9.dev0.tar", last modified: Mon Jul 10 09:59:56 2023, max compression
```

## Comparing `open_gpt_torch-0.0.8.tar` & `open-gpt-torch-0.0.9.dev0.tar`

### file list

```diff
@@ -1,66 +1,80 @@
--rw-r--r--   0        0        0    10825 2023-07-10 05:55:46.054553 open_gpt_torch-0.0.8/LICENSE
--rw-r--r--   0        0        0     7788 2023-07-10 05:55:46.054553 open_gpt_torch-0.0.8/README.md
--rw-r--r--   0        0        0     1006 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/__init__.py
--rw-r--r--   0        0        0      107 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/__main__.py
--rw-r--r--   0        0        0        0 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/__init__.py
--rw-r--r--   0        0        0     1087 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/application.py
--rw-r--r--   0        0        0      508 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/command_loader.py
--rw-r--r--   0        0        0        0 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/commands/__init__.py
--rw-r--r--   0        0        0      567 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/commands/about.py
--rw-r--r--   0        0        0     3151 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/commands/deploy.py
--rw-r--r--   0        0        0      953 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/commands/playground.py
--rw-r--r--   0        0        0      611 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/commands/quantize.py
--rw-r--r--   0        0        0     2429 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/cli/commands/serve.py
--rw-r--r--   0        0        0     6075 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/factory.py
--rw-r--r--   0        0        0     2741 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/helper.py
--rw-r--r--   0        0        0      490 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/logs.py
--rw-r--r--   0        0        0        0 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/models/__init__.py
--rw-r--r--   0        0        0     2420 2023-07-10 05:55:46.090553 open_gpt_torch-0.0.8/open_gpt/models/embedding.py
--rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0        0        0      601 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/config.json
--rw-r--r--   0        0        0     3607 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/configuration_flamingo.py
--rw-r--r--   0        0        0     5954 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0        0        0     9481 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/flamingo_model.py
--rw-r--r--   0        0        0     6484 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/loading.py
--rw-r--r--   0        0        0     2439 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0        0        0    11873 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/generation.py
--rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/llama/__init__.py
--rw-r--r--   0        0        0     2877 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/llama/loading.py
--rw-r--r--   0        0        0      863 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/llama/modeling.py
--rw-r--r--   0        0        0     2856 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/loading.py
--rw-r--r--   0        0        0     2564 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/modeling.py
--rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/moss/__init__.py
--rw-r--r--   0        0        0     3504 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/moss/modeling.py
--rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/pythia/__init__.py
--rw-r--r--   0        0        0      653 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/pythia/modeling.py
--rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/rwkv/__init__.py
--rw-r--r--   0        0        0     1233 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/rwkv/modeling.py
--rw-r--r--   0        0        0     1908 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/session.py
--rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/stablelm/__init__.py
--rw-r--r--   0        0        0     2608 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/stablelm/modeling.py
--rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/vicuna/__init__.py
--rw-r--r--   0        0        0     7439 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/vicuna/loading.py
--rw-r--r--   0        0        0     1428 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/models/vicuna/modeling.py
--rw-r--r--   0        0        0     6368 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/profile.py
--rw-r--r--   0        0        0     1115 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/resources/flow.yml.jinja2
--rw-r--r--   0        0        0       29 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/__init__.py
--rw-r--r--   0        0        0       75 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/executors/__init__.py
--rw-r--r--   0        0        0     2117 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/executors/base.py
--rw-r--r--   0        0        0     2373 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/executors/flamingo.py
--rw-r--r--   0        0        0      171 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/executors/utils.py
--rw-r--r--   0        0        0      773 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/flow.py
--rw-r--r--   0        0        0     3782 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/gateway.py
--rw-r--r--   0        0        0        0 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/playground/__init__.py
--rw-r--r--   0        0        0     4686 2023-07-10 05:55:46.094553 open_gpt_torch-0.0.8/open_gpt/serve/playground/gradio.py
--rw-r--r--   0        0        0     7396 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/serve/playground/gradio_chatbot.py
--rw-r--r--   0        0        0     2714 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/serve/playground/gradio_css.py
--rw-r--r--   0        0        0     6210 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/datautils.py
--rw-r--r--   0        0        0     4781 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/quant_groups.py
--rw-r--r--   0        0        0     1707 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/quantize.py
--rw-r--r--   0        0        0     2257 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/quantizeargs.py
--rw-r--r--   0        0        0    11420 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/quantutils.py
--rw-r--r--   0        0        0    13691 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/spqr_engine.py
--rw-r--r--   0        0        0      201 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/test.py
--rw-r--r--   0        0        0     2221 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/open_gpt/spqr/weight_permutation.py
--rw-r--r--   0        0        0     3274 2023-07-10 05:55:46.098553 open_gpt_torch-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    21115 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.585944 open-gpt-torch-0.0.9.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-10 09:59:56.585944 open-gpt-torch-0.0.9.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.581944 open-gpt-torch-0.0.9.dev0/open_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.581944 open-gpt-torch-0.0.9.dev0/open_gpt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/cli/command_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.581944 open-gpt-torch-0.0.9.dev0/open_gpt/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/cli/commands/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/cli/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/cli/commands/playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/cli/commands/quantize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/cli/commands/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.581944 open-gpt-torch-0.0.9.dev0/open_gpt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.581944 open-gpt-torch-0.0.9.dev0/open_gpt/models/flamingo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/flamingo/configuration_flamingo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/flamingo/flamingo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.581944 open-gpt-torch-0.0.9.dev0/open_gpt/models/llama/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/llama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/llama/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/llama/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.581944 open-gpt-torch-0.0.9.dev0/open_gpt/models/moss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/moss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/moss/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.581944 open-gpt-torch-0.0.9.dev0/open_gpt/models/pythia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/pythia/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.581944 open-gpt-torch-0.0.9.dev0/open_gpt/models/rwkv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/rwkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/rwkv/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.581944 open-gpt-torch-0.0.9.dev0/open_gpt/models/stablelm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/stablelm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/stablelm/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.581944 open-gpt-torch-0.0.9.dev0/open_gpt/models/vicuna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/vicuna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/vicuna/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/models/vicuna/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.581944 open-gpt-torch-0.0.9.dev0/open_gpt/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.585944 open-gpt-torch-0.0.9.dev0/open_gpt/serve/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/serve/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/serve/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/serve/executors/flamingo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/serve/executors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/serve/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/serve/gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.585944 open-gpt-torch-0.0.9.dev0/open_gpt/serve/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/serve/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/serve/playground/gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/serve/playground/gradio_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/open_gpt/serve/playground/gradio_css.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:59:56.585944 open-gpt-torch-0.0.9.dev0/open_gpt_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-10 09:59:56.000000 open-gpt-torch-0.0.9.dev0/open_gpt_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-10 09:59:56.000000 open-gpt-torch-0.0.9.dev0/open_gpt_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:59:56.000000 open-gpt-torch-0.0.9.dev0/open_gpt_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:59:56.000000 open-gpt-torch-0.0.9.dev0/open_gpt_torch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-10 09:59:56.000000 open-gpt-torch-0.0.9.dev0/open_gpt_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 09:59:56.000000 open-gpt-torch-0.0.9.dev0/open_gpt_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:59:56.585944 open-gpt-torch-0.0.9.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-10 09:59:49.000000 open-gpt-torch-0.0.9.dev0/setup.py
```

### Comparing `open_gpt_torch-0.0.8/LICENSE` & `open-gpt-torch-0.0.9.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/README.md` & `open-gpt-torch-0.0.9.dev0/README.md`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/__init__.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging as _logging
 import os as _os
 import sys
 
+__version__ = '0.0.9.dev0'
+
 _logging.captureWarnings(True)
 
 
 # import importlib.metadata if available, otherwise importlib_metadata
 if sys.version_info >= (3, 8):
     import importlib.metadata as importlib_metadata
 else:
@@ -20,24 +22,14 @@
 try:
     __jina_version__ = _jina.__version__
 except AttributeError as e:
     raise RuntimeError(
         '`jina` dependency is not installed correctly, please reinstall with `pip install -U --force-reinstall jina`'
     )
 
-
-def get_version() -> str:
-    """Return the module version number specified in pyproject.toml.
-    :return: The version number.
-    """
-    return importlib_metadata.version(__package__ + '_torch')
-
-
-__version__ = get_version()
-
 __resources_path__ = _os.path.join(_os.path.dirname(__file__), 'resources')
 
 _os.environ['NO_VERSION_CHECK'] = '1'
 
-from inference_client import Client
+from inference_client import Client  # noqa
 
 from .factory import create_model
```

### Comparing `open_gpt_torch-0.0.8/open_gpt/cli/application.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/cli/application.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/cli/commands/about.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/cli/commands/about.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/cli/commands/deploy.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/cli/commands/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             "replicas", "r", "The number of replicas to serve.", flag=False, default=1
         ),
         option(
             "instance_type",
             None,
             "The instance used to deploy model.",
             flag=False,
-            default='G3',
+            default='G2',
         ),
         option(
             'dry_run',
             None,
             'Whether to run the deployment in dry run mode.',
             flag=True,
         ),
```

### Comparing `open_gpt_torch-0.0.8/open_gpt/cli/commands/playground.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/cli/commands/playground.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/cli/commands/quantize.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/cli/commands/quantize.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/cli/commands/serve.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/cli/commands/serve.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/factory.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/factory.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/helper.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/helper.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/embedding.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/embedding.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/flamingo/configuration_flamingo.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/flamingo/configuration_flamingo.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/flamingo/flamingo_lm.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/flamingo/flamingo_model.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/flamingo/flamingo_model.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/flamingo/loading.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/flamingo/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/flamingo/modeling.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/flamingo/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/generation.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/generation.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/llama/loading.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/llama/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/llama/modeling.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/llama/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/loading.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/modeling.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/moss/modeling.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/moss/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/pythia/modeling.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/pythia/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/rwkv/modeling.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/rwkv/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/session.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/session.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/stablelm/modeling.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/stablelm/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/vicuna/loading.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/vicuna/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/models/vicuna/modeling.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/models/vicuna/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/profile.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/profile.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/serve/executors/base.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/serve/executors/base.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/serve/executors/flamingo.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/serve/executors/flamingo.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/serve/flow.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/serve/flow.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 
     if os.path.isfile(flow):
         return await CloudFlow(path=flow).deploy()
     else:
         with tempfile.NamedTemporaryFile() as f:
             with open(f.name, 'w') as _:
                 _.write(flow)
-            return await CloudFlow(path=f.name).deploy()
+            return await CloudFlow(path=f.name).__aenter__()
```

### Comparing `open_gpt_torch-0.0.8/open_gpt/serve/gateway.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/serve/gateway.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/serve/playground/gradio.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/serve/playground/gradio.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/serve/playground/gradio_chatbot.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/serve/playground/gradio_chatbot.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.8/open_gpt/serve/playground/gradio_css.py` & `open-gpt-torch-0.0.9.dev0/open_gpt/serve/playground/gradio_css.py`

 * *Files identical despite different names*

