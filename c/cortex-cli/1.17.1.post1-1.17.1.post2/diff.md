# Comparing `tmp/cortex_cli-1.17.1.post1.tar.gz` & `tmp/cortex_cli-1.17.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_cli-1.17.1.post1.tar", last modified: Mon Jul  3 19:11:34 2023, max compression
+gzip compressed data, was "cortex_cli-1.17.1.post2.tar", last modified: Mon Jul  3 19:53:57 2023, max compression
```

## Comparing `cortex_cli-1.17.1.post1.tar` & `cortex_cli-1.17.1.post2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5733 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/README.md
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       25 2023-07-03 19:11:22.000000 cortex_cli-1.17.1.post1/cortex_cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/cli/api/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/api/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3992 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/api/github_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/api/http_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/cli_api_base.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/cli_api_base_config.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4179 2023-07-03 13:20:35.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/cli_multipart_upload.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/clients.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2027 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/configure.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      973 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/cortex_cli.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/generic_get.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/inferences.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24883 2023-07-03 17:51:56.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/models.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3259 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/cli/pipelines.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/core/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/core/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     6919 2023-07-03 18:05:46.000000 cortex_cli-1.17.1.post1/cortex_cli/core/cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/core/drift_checks.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/core/ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/core/mlflow/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/core/mlflow/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    14556 2023-07-03 17:50:46.000000 cortex_cli-1.17.1.post1/cortex_cli/core/mlflow/mlflow_cortex.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/core/models/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/core/models/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/core/models/cortex_model.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/core/secrets_manager.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/model_templates/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli/tests/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/tests/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/tests/test_cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/cortex_cli/tests/test_ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/cortex_cli.egg-info/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-07-03 19:11:34.000000 cortex_cli-1.17.1.post1/cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3162 2023-07-03 19:11:34.000000 cortex_cli-1.17.1.post1/cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-07-03 19:11:34.000000 cortex_cli-1.17.1.post1/cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-07-03 19:11:34.000000 cortex_cli-1.17.1.post1/cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      146 2023-07-03 19:11:34.000000 cortex_cli-1.17.1.post1/cortex_cli.egg-info/requires.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-07-03 19:11:34.000000 cortex_cli-1.17.1.post1/cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       91 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post1/pyproject.toml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-07-03 19:11:34.154351 cortex_cli-1.17.1.post1/setup.cfg
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1104 2023-07-03 18:07:49.000000 cortex_cli-1.17.1.post1/setup.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5733 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/README.md
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.183682 cortex_cli-1.17.1.post2/cortex_cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       25 2023-07-03 19:53:51.000000 cortex_cli-1.17.1.post2/cortex_cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/cli/api/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/api/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3992 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/api/github_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/api/http_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/cli_api_base.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/cli_api_base_config.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4179 2023-07-03 13:20:35.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/cli_multipart_upload.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/clients.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2027 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/configure.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      973 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/cortex_cli.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/generic_get.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/inferences.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24883 2023-07-03 17:51:56.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/models.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3259 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/cli/pipelines.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/core/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/core/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     6919 2023-07-03 18:05:46.000000 cortex_cli-1.17.1.post2/cortex_cli/core/cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/core/drift_checks.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/core/ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/core/mlflow/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/core/mlflow/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    14671 2023-07-03 19:53:40.000000 cortex_cli-1.17.1.post2/cortex_cli/core/mlflow/mlflow_cortex.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/core/models/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/core/models/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/core/models/cortex_model.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/core/secrets_manager.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/model_templates/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.183682 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.183682 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli/tests/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/tests/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/tests/test_cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/cortex_cli/tests/test_ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/cortex_cli.egg-info/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-07-03 19:53:57.000000 cortex_cli-1.17.1.post2/cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3162 2023-07-03 19:53:57.000000 cortex_cli-1.17.1.post2/cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-07-03 19:53:57.000000 cortex_cli-1.17.1.post2/cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-07-03 19:53:57.000000 cortex_cli-1.17.1.post2/cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      146 2023-07-03 19:53:57.000000 cortex_cli-1.17.1.post2/cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-07-03 19:53:57.000000 cortex_cli-1.17.1.post2/cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       91 2023-06-28 17:58:15.000000 cortex_cli-1.17.1.post2/pyproject.toml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-07-03 19:53:57.193682 cortex_cli-1.17.1.post2/setup.cfg
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1104 2023-07-03 18:07:49.000000 cortex_cli-1.17.1.post2/setup.py
```

### Comparing `cortex_cli-1.17.1.post1/README.md` & `cortex_cli-1.17.1.post2/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/cli/api/github_api.py` & `cortex_cli-1.17.1.post2/cortex_cli/cli/api/github_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/cli/api/http_api.py` & `cortex_cli-1.17.1.post2/cortex_cli/cli/api/http_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/cli/cli_api_base.py` & `cortex_cli-1.17.1.post2/cortex_cli/cli/cli_api_base.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/cli/cli_api_base_config.py` & `cortex_cli-1.17.1.post2/cortex_cli/cli/cli_api_base_config.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/cli/cli_multipart_upload.py` & `cortex_cli-1.17.1.post2/cortex_cli/cli/cli_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/cli/configure.py` & `cortex_cli-1.17.1.post2/cortex_cli/cli/configure.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/cli/cortex_cli.py` & `cortex_cli-1.17.1.post2/cortex_cli/cli/cortex_cli.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/cli/generic_get.py` & `cortex_cli-1.17.1.post2/cortex_cli/cli/generic_get.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/cli/inferences.py` & `cortex_cli-1.17.1.post2/cortex_cli/cli/inferences.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/cli/models.py` & `cortex_cli-1.17.1.post2/cortex_cli/cli/models.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/cli/pipelines.py` & `cortex_cli-1.17.1.post2/cortex_cli/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/core/cortex_data.py` & `cortex_cli-1.17.1.post2/cortex_cli/core/cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/core/drift_checks.py` & `cortex_cli-1.17.1.post2/cortex_cli/core/drift_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/core/ethics_checks.py` & `cortex_cli-1.17.1.post2/cortex_cli/core/ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/core/mlflow/mlflow_cortex.py` & `cortex_cli-1.17.1.post2/cortex_cli/core/mlflow/mlflow_cortex.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import os
 import importlib
 import shutil
 import yaml
 
 # External Libraries
 import mlflow
+from collections import namedtuple
 from mlflow.pyfunc import PythonModel
 from mlflow.models import Model, ModelSignature, ModelInputExample
 from mlflow.models.model import MLMODEL_FILE_NAME
 from mlflow.utils.file_utils import write_to
 from mlflow.models.utils import _save_example
 from mlflow.utils.environment import (
     _validate_env_arguments,
@@ -308,22 +309,23 @@
         nltk = importlib.import_module('nltk')
         nltk.data.path.insert(0,'./nltk_data')
         nltk.download('all', download_dir='./nltk_data')
     except:
         pass
 
     # pipeline_steps = conf[PIPELINE_STEPS]
-    deployment_steps = conf[DEPLOYMENT_STEPS]
 
-    if deployment_steps:
-        for step in deployment_steps:
-            if hasattr(python_model, step):
-                function = getattr(python_model, step)
-                if callable(function):
-                    function()
+    Step = namedtuple('Step', 'name type')
+    deployment_steps = [Step(dict[list(dict.keys())[0]], list(dict.keys())[0]) for dict in conf[DEPLOYMENT_STEPS]]
+
+    for step in deployment_steps:
+        if hasattr(python_model, step.type):
+            function = getattr(python_model, step.type)
+            if callable(function):
+                function()
 
 
     return _CortexModelWrapper(python_model)
 
 
 def _warn_potentially_incompatible_py_version_if_necessary(model_py_version=None):
     """
```

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/core/models/cortex_model.py` & `cortex_cli-1.17.1.post2/cortex_cli/core/models/cortex_model.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/core/secrets_manager.py` & `cortex_cli-1.17.1.post2/cortex_cli/core/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/.gitignore` & `cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/README.md` & `cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.17.1.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/.gitignore` & `cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/README.md` & `cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.17.1.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/tests/test_cortex_data.py` & `cortex_cli-1.17.1.post2/cortex_cli/tests/test_cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli/tests/test_ethics_checks.py` & `cortex_cli-1.17.1.post2/cortex_cli/tests/test_ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/cortex_cli.egg-info/SOURCES.txt` & `cortex_cli-1.17.1.post2/cortex_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.17.1.post1/setup.py` & `cortex_cli-1.17.1.post2/setup.py`

 * *Files identical despite different names*

