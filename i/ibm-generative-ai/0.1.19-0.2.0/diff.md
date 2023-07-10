# Comparing `tmp/ibm-generative-ai-0.1.19.tar.gz` & `tmp/ibm-generative-ai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-generative-ai-0.1.19.tar", last modified: Fri Jun 30 18:36:22 2023, max compression
+gzip compressed data, was "ibm-generative-ai-0.2.0.tar", last modified: Mon Jul 10 21:09:32 2023, max compression
```

## Comparing `ibm-generative-ai-0.1.19.tar` & `ibm-generative-ai-0.2.0.tar`

### file list

```diff
@@ -1,250 +1,270 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.729187 ibm-generative-ai-0.1.19/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.705187 ibm-generative-ai-0.1.19/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.705187 ibm-generative-ai-0.1.19/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/.github/ISSUE_TEMPLATE/01_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/.github/ISSUE_TEMPLATE/02_feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/.github/ISSUE_TEMPLATE/03_documentation_update.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/.github/ISSUE_TEMPLATE/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.705187 ibm-generative-ai-0.1.19/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/.github/workflows/integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/ACTIVE_PROJECT_TEAM.md
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/EXTENSIONS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-06-30 18:36:22.729187 ibm-generative-ai-0.1.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/SUPPORT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.705187 ibm-generative-ai-0.1.19/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/.nojekyll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.705187 ibm-generative-ai-0.1.19/documentation/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/assets/pull_request_from_fork_to_base.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.705187 ibm-generative-ai-0.1.19/documentation/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.705187 ibm-generative-ai-0.1.19/documentation/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.705187 ibm-generative-ai-0.1.19/documentation/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.705187 ibm-generative-ai-0.1.19/documentation/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.705187 ibm-generative-ai-0.1.19/documentation/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/_templates/custom_landing_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.709187 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.709187 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples/async.examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples/async.examples.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples/examples.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples/extensions.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples/prompts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples/prompts.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.credentials.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.exceptions.genai_exception.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.prompt.prompt_pattern.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.prompt.quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.prompt.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.schemas.descriptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.schemas.generate_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.schemas.history_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.schemas.models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.schemas.responses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.schemas.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.schemas.token_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.services.request_handler.rst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.services.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.services.service_interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/local_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.701187 ibm-generative-ai-0.1.19/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.709187 ibm-generative-ai-0.1.19/examples/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/dev/async-flaky-request-handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/dev/async-flaky-responses-ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/dev/generate-all-models.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/dev/history-async.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/dev/load_token_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/dev/logging_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.713187 ibm-generative-ai-0.1.19/examples/user/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/alice_bob_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/alice_bob_talk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.717187 ibm-generative-ai-0.1.19/examples/user/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/assets/country-capital.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19258 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/assets/penguins.csv
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/assets/penguins2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/assets/seed_tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)   110931 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/assets/seed_tasks.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/async_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/async_greetings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/async_ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/async_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/complete_my_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/country-capital-qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/explain_my_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/generate_with_input_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/gpt_chat_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/grid_search_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/grid_search_params_greeating.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/jsonprompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/jsonprompt_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/langchain_qa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.717187 ibm-generative-ai-0.1.19/examples/user/localserver/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/localserver/localserver.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/localserver/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/logprob_returns.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/many_greetings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/model_as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/prompt-raw-string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/prompt_csv_random_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/prompt_from_all_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/prompt_from_all_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/prompt_from_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/prompt_reuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.717187 ibm-generative-ai-0.1.19/examples/user/prompt_templating/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/prompt_templating/watsonx-prompt-output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/prompt_templating/watsonx-prompt-templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.717187 ibm-generative-ai-0.1.19/examples/user/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/prompts/Country-Capital-Factual-QA
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.717187 ibm-generative-ai-0.1.19/examples/user/prompts_adult_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/saving_prompts_as_hf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/self-reflection.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/self_instruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.717187 ibm-generative-ai-0.1.19/examples/user/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/templates/capital-qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/templates/instruction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/templates/qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/templates/self-reflection.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/templates/synth-animal.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/tokenize-sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/examples/user/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 18:36:22.729187 ibm-generative-ai-0.1.19/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.701187 ibm-generative-ai-0.1.19/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.717187 ibm-generative-ai-0.1.19/src/genai/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-30 18:36:22.000000 ibm-generative-ai-0.1.19/src/genai/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.717187 ibm-generative-ai-0.1.19/src/genai/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/exceptions/genai_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.701187 ibm-generative-ai-0.1.19/src/genai/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.717187 ibm-generative-ai-0.1.19/src/genai/extensions/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/extensions/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/extensions/huggingface/save_huggingface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.717187 ibm-generative-ai-0.1.19/src/genai/extensions/langchain/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/extensions/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/extensions/langchain/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/extensions/langchain/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.721187 ibm-generative-ai-0.1.19/src/genai/extensions/localserver/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/extensions/localserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/extensions/localserver/custom_model_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/extensions/localserver/local_api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/extensions/localserver/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.721187 ibm-generative-ai-0.1.19/src/genai/extensions/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/extensions/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/extensions/pandas/prompt_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    24219 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/prompt_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.721187 ibm-generative-ai-0.1.19/src/genai/routers/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/routers/prompt_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.721187 ibm-generative-ai-0.1.19/src/genai/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/schemas/descriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/schemas/generate_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/schemas/history_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/schemas/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/schemas/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/schemas/token_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.721187 ibm-generative-ai-0.1.19/src/genai/services/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/services/async_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/services/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/services/prompt_template_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/services/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/services/service_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.721187 ibm-generative-ai-0.1.19/src/genai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/utils/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/utils/search_space_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/src/genai/utils/watsonx_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.721187 ibm-generative-ai-0.1.19/src/ibm_generative_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-06-30 18:36:22.000000 ibm-generative-ai-0.1.19/src/ibm_generative_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-06-30 18:36:22.000000 ibm-generative-ai-0.1.19/src/ibm_generative_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:36:22.000000 ibm-generative-ai-0.1.19/src/ibm_generative_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-30 18:36:22.000000 ibm-generative-ai-0.1.19/src/ibm_generative_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 18:36:22.000000 ibm-generative-ai-0.1.19/src/ibm_generative_ai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.725187 ibm-generative-ai-0.1.19/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.725187 ibm-generative-ai-0.1.19/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/age-gender.csv
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/capital-qa-content.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/capital-qa-multivar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/capital-qa-sub-noheader.csv
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/capital-qa-sub.csv
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/capital-qa-sub.json
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/capital-qa-sub.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/capital-qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/csv_file.csv
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/csv_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/invalid-content-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/invalid-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/penguins.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/prompt_contents.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/response_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/story.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/assets/story_sub.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.729187 ibm-generative-ai-0.1.19/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/extensions/test_langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/extensions/test_localserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/extensions/test_save_huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/extensions/test_sub_from_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:22.729187 ibm-generative-ai-0.1.19/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/integration/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/integration/test_terms_of_use.py
--rw-r--r--   0 runner    (1001) docker     (123)    19391 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_generate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_generate_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_model_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_prompt_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_prompt_pattern_watsonx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_prompt_template_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_schema_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_service_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_service_interface_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_service_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-30 18:35:53.000000 ibm-generative-ai-0.1.19/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.599871 ibm-generative-ai-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.571870 ibm-generative-ai-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.571870 ibm-generative-ai-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/.github/ISSUE_TEMPLATE/01_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/.github/ISSUE_TEMPLATE/02_feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/.github/ISSUE_TEMPLATE/03_documentation_update.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/.github/ISSUE_TEMPLATE/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.571870 ibm-generative-ai-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/.github/workflows/integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/EXTENSIONS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/GETTING_STARTED.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-10 21:09:32.599871 ibm-generative-ai-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/STARTER_TEAM.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/SUPPORT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.571870 ibm-generative-ai-0.2.0/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/.nojekyll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.575870 ibm-generative-ai-0.2.0/documentation/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/assets/pull_request_from_fork_to_base.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.575870 ibm-generative-ai-0.2.0/documentation/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.575870 ibm-generative-ai-0.2.0/documentation/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.575870 ibm-generative-ai-0.2.0/documentation/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.575870 ibm-generative-ai-0.2.0/documentation/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.575870 ibm-generative-ai-0.2.0/documentation/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/_templates/custom_landing_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.575870 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.579870 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples/async.examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples/async.examples.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples/examples.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples/extensions.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples/prompts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples/prompts.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.credentials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.exceptions.genai_exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.prompt.prompt_pattern.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.prompt.quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.prompt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.schemas.descriptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.schemas.generate_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.schemas.history_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.schemas.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.schemas.responses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.schemas.token_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.services.request_handler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.services.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.services.service_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/local_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.567870 ibm-generative-ai-0.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.579870 ibm-generative-ai-0.2.0/examples/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/dev/async-flaky-request-handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/dev/async-flaky-responses-ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/dev/generate-all-models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/dev/history-async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/dev/load_token_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/dev/logging_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.583870 ibm-generative-ai-0.2.0/examples/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/alice_bob_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/alice_bob_talk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.583870 ibm-generative-ai-0.2.0/examples/user/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/assets/country-capital.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19258 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/assets/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/assets/penguins2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/assets/seed_tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110931 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/assets/seed_tasks.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/async_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/async_greetings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/async_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/async_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/complete_my_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/country-capital-qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/explain_my_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/generate_with_input_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/gpt_chat_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/grid_search_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/grid_search_params_greeating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/jsonprompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/jsonprompt_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/langchain_qa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.583870 ibm-generative-ai-0.2.0/examples/user/localserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/localserver/localserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/localserver/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/logprob_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/many_greetings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/model_as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt-raw-string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt_csv_random_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt_from_all_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt_from_all_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt_from_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt_reuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.583870 ibm-generative-ai-0.2.0/examples/user/prompt_templating/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt_templating/watsonx-prompt-output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt_templating/watsonx-prompt-templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.583870 ibm-generative-ai-0.2.0/examples/user/prompt_tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt_tuning/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt_tuning/file_to_tune.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt_tuning/files_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompt_tuning/summarization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.583870 ibm-generative-ai-0.2.0/examples/user/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompts/Country-Capital-Factual-QA
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.583870 ibm-generative-ai-0.2.0/examples/user/prompts_adult_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/saving_prompts_as_hf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/self-reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/self_instruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.587870 ibm-generative-ai-0.2.0/examples/user/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/templates/capital-qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/templates/instruction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/templates/qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/templates/self-reflection.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/templates/synth-animal.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/tokenize-sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/examples/user/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/innersource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:09:32.599871 ibm-generative-ai-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.571870 ibm-generative-ai-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.587870 ibm-generative-ai-0.2.0/src/genai/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 21:09:32.000000 ibm-generative-ai-0.2.0/src/genai/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.587870 ibm-generative-ai-0.2.0/src/genai/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/exceptions/genai_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.571870 ibm-generative-ai-0.2.0/src/genai/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.587870 ibm-generative-ai-0.2.0/src/genai/extensions/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/extensions/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/extensions/huggingface/save_huggingface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.587870 ibm-generative-ai-0.2.0/src/genai/extensions/langchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/extensions/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/extensions/langchain/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/extensions/langchain/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.587870 ibm-generative-ai-0.2.0/src/genai/extensions/localserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/extensions/localserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/extensions/localserver/custom_model_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/extensions/localserver/local_api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/extensions/localserver/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.587870 ibm-generative-ai-0.2.0/src/genai/extensions/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/extensions/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/extensions/pandas/prompt_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24219 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/prompt_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.587870 ibm-generative-ai-0.2.0/src/genai/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/routers/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/routers/prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/routers/tunes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.591871 ibm-generative-ai-0.2.0/src/genai/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/schemas/descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/schemas/files_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/schemas/generate_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/schemas/history_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/schemas/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/schemas/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/schemas/token_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/schemas/tunes_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.591871 ibm-generative-ai-0.2.0/src/genai/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/services/async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/services/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/services/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/services/prompt_template_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/services/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/services/service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/services/tune_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.591871 ibm-generative-ai-0.2.0/src/genai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/utils/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/utils/request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/utils/search_space_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/utils/service_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/src/genai/utils/watsonx_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.591871 ibm-generative-ai-0.2.0/src/ibm_generative_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-10 21:09:32.000000 ibm-generative-ai-0.2.0/src/ibm_generative_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-10 21:09:32.000000 ibm-generative-ai-0.2.0/src/ibm_generative_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:09:32.000000 ibm-generative-ai-0.2.0/src/ibm_generative_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-10 21:09:32.000000 ibm-generative-ai-0.2.0/src/ibm_generative_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 21:09:32.000000 ibm-generative-ai-0.2.0/src/ibm_generative_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.595871 ibm-generative-ai-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.599871 ibm-generative-ai-0.2.0/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/age-gender.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/capital-qa-content.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/capital-qa-multivar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/capital-qa-sub-noheader.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/capital-qa-sub.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/capital-qa-sub.json
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/capital-qa-sub.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/capital-qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/csv_file.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/csv_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/file_to_tune.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/file_to_tune.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/file_to_tune.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/invalid-content-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/invalid-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/prompt_contents.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/response_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/story.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/assets/story_sub.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.599871 ibm-generative-ai-0.2.0/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/extensions/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/extensions/test_localserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/extensions/test_save_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/extensions/test_sub_from_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:32.599871 ibm-generative-ai-0.2.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/integration/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/integration/test_terms_of_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_generate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_generate_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_model_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_prompt_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_prompt_pattern_watsonx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_prompt_template_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_schema_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_service_interface_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_service_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_tunes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-10 21:09:04.000000 ibm-generative-ai-0.2.0/tests/test_version.py
```

### Comparing `ibm-generative-ai-0.1.19/.github/ISSUE_TEMPLATE/01_bug_report.md` & `ibm-generative-ai-0.2.0/.github/ISSUE_TEMPLATE/01_bug_report.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/.github/ISSUE_TEMPLATE/02_feature_request.md` & `ibm-generative-ai-0.2.0/.github/ISSUE_TEMPLATE/02_feature_request.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/.github/ISSUE_TEMPLATE/03_documentation_update.md` & `ibm-generative-ai-0.2.0/.github/ISSUE_TEMPLATE/03_documentation_update.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/.github/PULL_REQUEST_TEMPLATE.md` & `ibm-generative-ai-0.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/.github/workflows/documentation.yml` & `ibm-generative-ai-0.2.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/.github/workflows/integration-test.yml` & `ibm-generative-ai-0.2.0/.github/workflows/integration-test.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/.github/workflows/main.yml` & `ibm-generative-ai-0.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/.github/workflows/python-publish.yml` & `ibm-generative-ai-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/.gitignore` & `ibm-generative-ai-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/.pre-commit-config.yaml` & `ibm-generative-ai-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/CODE_OF_CONDUCT.md` & `ibm-generative-ai-0.2.0/CODE_OF_CONDUCT.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 address, posting via an official social media account, or acting as an appointed
 representative at an online or offline event. Representation of a project may be
 further defined and clarified by project maintainers.
 
 ## Enforcement
 
 Instances of abusive, harassing, or otherwise unacceptable behavior may be
-reported by contacting the [project team](./ACTIVE_PROJECT_TEAM.md). All
+reported by contacting the [project team](./STARTER_TEAM.md). All
 complaints will be reviewed and investigated and will result in a response that
 is deemed necessary and appropriate to the circumstances. The project team is
 obligated to maintain confidentiality with regard to the reporter of an incident.
 Further details of specific enforcement policies may be posted separately.
 
 Project maintainers who do not follow or enforce the Code of Conduct in good
 faith may face temporary or permanent repercussions as determined by other
```

### Comparing `ibm-generative-ai-0.1.19/DEVELOPMENT.md` & `ibm-generative-ai-0.2.0/CONTRIBUTING.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # IBM Generative AI Development Guide
 
 <!-- vscode-markdown-toc -->
 * [Setup the Development Environment](#setup-the-development-environment)
 	* [Pre-requisites](#pre-requisites)
 		* [Using Venv](#using-venv)
 	* [Fork the official repo](#fork-the-official-repo)
```

### Comparing `ibm-generative-ai-0.1.19/EXTENSIONS.md` & `ibm-generative-ai-0.2.0/EXTENSIONS.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/LICENSE` & `ibm-generative-ai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/PKG-INFO` & `ibm-generative-ai-0.2.0/GETTING_STARTED.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,8 @@
-Metadata-Version: 2.1
-Name: ibm-generative-ai
-Version: 0.1.19
-Summary: IBM Generative AI is a Python library built on IBM's large language model REST interface.
-Author-email: Lee Martie <lee.martie@ibm.com>, Ana Fucs <ana.fucs@ibm.com>, Veronique Demers <vdemers@ibm.com>, Mairead O'Neill <moneill@ibm.com>, Mirian Silva <mirianfrsilva@ibm.com>, Onkar Bhardwaj <onkarbhardwaj@ibm.com>, James Sutton <james.sutton@uk.ibm.com>, Ja Young Lee <younglee@ibm.com>, Adriana Meza Soria <adriana.meza.soria@ibm.com>
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: langchain
-Provides-Extra: huggingface
-Provides-Extra: pandas
-Provides-Extra: localserver
-Provides-Extra: all
-License-File: LICENSE
-
-# IBM Generative AI Python SDK
-
-
-This is the Python SDK for IBM Foundation Models Studio to bring IBM Generative AI into Python programs and to also extend it with useful operations and types.
-
-:books:	**API Documentation: [Link](https://ibm.github.io/ibm-generative-ai/)**
-
-*This is an early access library and requires invitation to use the technical preview of [watsonx.ai](https://watsonx.ai/). You can join the waitlist by visiting. https://www.ibm.com/products/watsonx-ai.*
-
-*Looking for the JavaScript/TypeScript version? Check out https://github.com/IBM/ibm-generative-ai-node-sdk.*
-
-[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/IBM/ibm-generative-ai/blob/main/LICENSE)
-![PyPI](https://img.shields.io/pypi/v/ibm-generative-ai)
-[![Build & Test](https://github.com/IBM/ibm-generative-ai/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/IBM/ibm-generative-ai/actions/workflows/main.yml)
-[![Integration Tests](https://github.com/IBM/ibm-generative-ai/actions/workflows/integration-test.yml/badge.svg)](https://github.com/IBM/ibm-generative-ai/actions/workflows/integration-test.yml)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/ibm-generative-ai)
-[![Coverage Status](https://coveralls.io/repos/github/IBM/ibm-generative-ai/badge.svg?branch=main)](https://coveralls.io/github/IBM/ibm-generative-ai?branch=main)
+# Getting Started Guideline
 
 ## <a name='TableofContents'></a>Table of Contents
 
 <!-- vscode-markdown-toc -->
 * [Table of Contents](#table-of-contents)
 * [Installation](#installation)
 * [Gen AI Endpoint](#gen-ai-endpoint)
@@ -43,24 +12,14 @@
     * [Synchronous Example](#synchronous-example)
 * [Tips and Troubleshooting](#tips-and-troubleshooting)
     * [Enabling Logs](#enabling-logs)
     * [Experimenting with a Large Number of Prompts](#many-prompts)
 * [Extensions](#extensions)
     * [LangChain Extension](#langchain-extension)
 * [Support](#support)
-* [API Documentation](#APIDocumentation)
-* [Important Information for Contributors](#important-information-for-contributors)
-* [Authors](#authors)
-
-<!-- vscode-markdown-toc-config
-	numbering=false
-	autoSave=true
-	/vscode-markdown-toc-config -->
-<!-- /vscode-markdown-toc -->
-
 
 ## <a name='Installation'></a>Installation
 
 ```bash
 pip install ibm-generative-ai
 ```
 #### <a name='KnownIssueFixes:'></a>Known Issue Fixes:
@@ -73,18 +32,17 @@
 
 Check your pip version with `pip --version` and if needed run the following command to upgrade pip.
 
 ```bash
 pip install --upgrade "pip>=22.0.1"
 ```
 
-
 ## <a name='GenAIEndpoint'></a>Gen AI Endpoint
 
-By default, IBM Generative AI will automatically use the following API endpoint: `https://workbench-api.res.ibm.com/v1/`. However, if you wish to target a different Gen AI API, you can do so by defining it with the `api_endpoint` argument when you instansiate the `Credentials` object.
+By default, IBM Generative AI will use the following API endpoint: `https://workbench-api.res.ibm.com/v1/`. However, if you wish to target a different Gen AI API, you can do so by defining it with the `api_endpoint` argument when you instansiate the `Credentials` object.
 
 ### <a name='Example'></a>Example
 
 Your `.env` file:
 
 ```ini
 GENAI_KEY=YOUR_GENAI_API_KEY
@@ -330,33 +288,17 @@
 template = seed_pattern.langchain.as_template()
 pattern = PromptPattern.langchain.from_template(template)
 
 print(langchain_model(template.format(question="What is life?")))
 print(genai_model.generate([pattern.sub("question", "What is life?")])[0].generated_text)
 ```
 
-## <a name='Model Types'></a>Model Types
+## <a name='[Deprecated] Model Types'></a>[Deprecated] Model Types
 
 Model types can be imported from the [ModelType class](src/genai/schemas/models.py). If you want to use a model that is not included in this class, you can pass it as a string as exemplified [here](src/genai/schemas/models.py).
 
+Models can be selected by passing their string id to the Model class as exemplified [here](src/genai/schemas/models.py).
+
 
 ## <a name='Support'></a>Support
 
 Need help? Check out how to get [support](SUPPORT.md)
-
-## <a name='APIDocumentation'></a>API Documentation
-
-Read our Python API documentation [here](https://ibm.github.io/ibm-generative-ai/).
-
-## <a name='ContributionInfo'></a>Important Information for Contributors
-
-IBM Generative AI is an open-source project that welcomes the community to contribute with documentation, tests, bug corrections, and new fuctionality in the form of [extensions](/EXTENSIONS.md). Please read our [code of counduct](/CODE_OF_CONDUCT.md) to learn the expected behavior from participants that contribute to the project, and our [contribution guide](DEVELOPMENT.md) to learn the gitflow and steps to submit pull requests.
-
-## <a name='Authors'></a>Authors
-  - Onkar Bhardwaj, onkarbhardwaj@ibm.com
-  - Veronique Demers, vdemers@ibm.com
-  - James Sutton, james.sutton@uk.ibm.com
-  - Mirian Silva, mirianfrsilva@ibm.com
-  - Mairead O'Neill, moneill@ibm.com
-  - Ja Young Lee, younglee@ibm.com
-  - Ana Fucs, ana.fucs@ibm.com
-  - Lee Martie, lee.martie@ibm.com
```

### Comparing `ibm-generative-ai-0.1.19/SUPPORT.md` & `ibm-generative-ai-0.2.0/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/assets/pull_request_from_fork_to_base.png` & `ibm-generative-ai-0.2.0/documentation/assets/pull_request_from_fork_to_base.png`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/docs/Makefile` & `ibm-generative-ai-0.2.0/documentation/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/docs/make.bat` & `ibm-generative-ai-0.2.0/documentation/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/docs/source/_templates/custom_landing_page.html` & `ibm-generative-ai-0.2.0/documentation/docs/source/_templates/custom_landing_page.html`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/docs/source/conf.py` & `ibm-generative-ai-0.2.0/documentation/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/docs/source/index.rst` & `ibm-generative-ai-0.2.0/documentation/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples/async.examples.user.rst` & `ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples/async.examples.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples/examples.user.rst` & `ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples/examples.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples/extensions.user.rst` & `ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples/extensions.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/examples/prompts.user.rst` & `ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/examples/prompts.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst` & `ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst` & `ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/genai.prompt.quickstart.rst` & `ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/genai.prompt.quickstart.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/documentation/docs/source/rst_source/local_server.rst` & `ibm-generative-ai-0.2.0/documentation/docs/source/rst_source/local_server.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/dev/async-flaky-request-handler.py` & `ibm-generative-ai-0.2.0/examples/dev/async-flaky-request-handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             inputs (list, optional): List of inputs to be queried. Defaults to None.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
             options (Options, optional): Additional parameters to pass in the query payload. Defaults to None.
 
         Returns:
             httpx.Response: Response from the REST API.
         """
-        headers, json_data = RequestHandler._metadata(
+        headers, json_data, _ = RequestHandler._metadata(
             method="POST",
             key=key,
             model_id=model_id,
             inputs=inputs,
             parameters=parameters,
             options=options,
         )
```

### Comparing `ibm-generative-ai-0.1.19/examples/dev/async-flaky-responses-ordered.py` & `ibm-generative-ai-0.2.0/examples/dev/async-flaky-responses-ordered.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/dev/generate-all-models.py` & `ibm-generative-ai-0.2.0/examples/dev/generate-all-models.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/dev/history-async.py` & `ibm-generative-ai-0.2.0/examples/dev/history-async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/dev/logging_example.py` & `ibm-generative-ai-0.2.0/examples/dev/logging_example.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/alice_bob_qa.py` & `ibm-generative-ai-0.2.0/examples/user/alice_bob_qa.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/alice_bob_talk.py` & `ibm-generative-ai-0.2.0/examples/user/alice_bob_talk.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/assets/penguins.csv` & `ibm-generative-ai-0.2.0/examples/user/assets/penguins.csv`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/assets/penguins2.csv` & `ibm-generative-ai-0.2.0/examples/user/assets/penguins2.csv`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/assets/seed_tasks.json` & `ibm-generative-ai-0.2.0/examples/user/assets/seed_tasks.json`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/assets/seed_tasks.jsonl` & `ibm-generative-ai-0.2.0/examples/user/assets/seed_tasks.jsonl`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/async_callback.py` & `ibm-generative-ai-0.2.0/examples/user/async_callback.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/async_greetings.py` & `ibm-generative-ai-0.2.0/examples/user/async_greetings.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/async_ordered.py` & `ibm-generative-ai-0.2.0/examples/user/async_ordered.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/async_tokenize.py` & `ibm-generative-ai-0.2.0/examples/user/async_tokenize.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/complete_my_code.py` & `ibm-generative-ai-0.2.0/examples/user/complete_my_code.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/country-capital-qa.py` & `ibm-generative-ai-0.2.0/examples/user/country-capital-qa.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/explain_my_code.py` & `ibm-generative-ai-0.2.0/examples/user/explain_my_code.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/generate_with_input_text.py` & `ibm-generative-ai-0.2.0/examples/user/generate_with_input_text.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/gpt_chat_bash.py` & `ibm-generative-ai-0.2.0/examples/user/gpt_chat_bash.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/grid_search_params.py` & `ibm-generative-ai-0.2.0/examples/user/grid_search_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/grid_search_params_greeating.py` & `ibm-generative-ai-0.2.0/examples/user/grid_search_params_greeating.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/history.py` & `ibm-generative-ai-0.2.0/examples/user/history.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/jsonprompt.py` & `ibm-generative-ai-0.2.0/examples/user/jsonprompt.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/jsonprompt_multi.py` & `ibm-generative-ai-0.2.0/examples/user/jsonprompt_multi.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/langchain_qa.py` & `ibm-generative-ai-0.2.0/examples/user/langchain_qa.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/localserver/localserver.py` & `ibm-generative-ai-0.2.0/examples/user/localserver/localserver.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/logprob_returns.py` & `ibm-generative-ai-0.2.0/examples/user/logprob_returns.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/many_greetings.py` & `ibm-generative-ai-0.2.0/examples/user/many_greetings.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/model_as_string.py` & `ibm-generative-ai-0.2.0/examples/user/model_as_string.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/prompt-raw-string.py` & `ibm-generative-ai-0.2.0/examples/user/prompt-raw-string.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/prompt_csv_random_rows.py` & `ibm-generative-ai-0.2.0/examples/user/prompt_csv_random_rows.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/prompt_from_all_csv.py` & `ibm-generative-ai-0.2.0/examples/user/prompt_from_all_csv.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/prompt_from_all_dataframe.py` & `ibm-generative-ai-0.2.0/examples/user/prompt_from_all_dataframe.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/prompt_from_dataframe.py` & `ibm-generative-ai-0.2.0/examples/user/prompt_from_dataframe.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/prompt_reuse.py` & `ibm-generative-ai-0.2.0/examples/user/prompt_reuse.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/prompt_templating/watsonx-prompt-output.py` & `ibm-generative-ai-0.2.0/examples/user/prompt_templating/watsonx-prompt-output.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py` & `ibm-generative-ai-0.2.0/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py` & `ibm-generative-ai-0.2.0/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/prompt_templating/watsonx-prompt-templating.py` & `ibm-generative-ai-0.2.0/examples/user/prompt_templating/watsonx-prompt-templating.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py` & `ibm-generative-ai-0.2.0/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py` & `ibm-generative-ai-0.2.0/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/saving_prompts_as_hf_dataset.py` & `ibm-generative-ai-0.2.0/examples/user/saving_prompts_as_hf_dataset.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/self-reflection.py` & `ibm-generative-ai-0.2.0/examples/user/self-reflection.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/self_instruct.py` & `ibm-generative-ai-0.2.0/examples/user/self_instruct.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/streaming.py` & `ibm-generative-ai-0.2.0/examples/user/streaming.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/tokenize-sync.py` & `ibm-generative-ai-0.2.0/examples/user/tokenize-sync.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/examples/user/tokens.py` & `ibm-generative-ai-0.2.0/examples/user/tokens.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/pyproject.toml` & `ibm-generative-ai-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/credentials.py` & `ibm-generative-ai-0.2.0/src/genai/credentials.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/exceptions/genai_exception.py` & `ibm-generative-ai-0.2.0/src/genai/exceptions/genai_exception.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/extensions/huggingface/save_huggingface.py` & `ibm-generative-ai-0.2.0/src/genai/extensions/huggingface/save_huggingface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/extensions/langchain/llm.py` & `ibm-generative-ai-0.2.0/src/genai/extensions/langchain/llm.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/extensions/langchain/prompt.py` & `ibm-generative-ai-0.2.0/src/genai/extensions/langchain/prompt.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/extensions/localserver/custom_model_interface.py` & `ibm-generative-ai-0.2.0/src/genai/extensions/localserver/custom_model_interface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/extensions/localserver/local_api_server.py` & `ibm-generative-ai-0.2.0/src/genai/extensions/localserver/local_api_server.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/extensions/pandas/prompt_sub.py` & `ibm-generative-ai-0.2.0/src/genai/extensions/pandas/prompt_sub.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/metadata.py` & `ibm-generative-ai-0.2.0/src/genai/metadata.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/model.py` & `ibm-generative-ai-0.2.0/src/genai/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,35 +14,45 @@
 from genai.schemas.responses import (
     GenerateResponse,
     GenerateResult,
     GenerateStreamResponse,
     TokenizeResponse,
     TokenizeResult,
 )
+from genai.schemas.tunes_params import (
+    CreateTuneHyperParams,
+    CreateTuneParams,
+    TunesListParams,
+)
 from genai.services import AsyncResponseGenerator, ServiceInterface
+from genai.services.tune_manager import TuneManager
 
 logger = logging.getLogger(__name__)
 
 
 class Model:
     _accessors = set()
 
     def __init__(
-        self, model: Union[ModelType, str], params: Union[GenerateParams, TokenParams], credentials: Credentials
+        self,
+        model: Union[ModelType, str],
+        params: Union[GenerateParams, TokenParams, Any] = None,
+        credentials: Credentials = None,
     ):
         """Instantiates the Model Interface
 
         Args:
             model (Union[ModelType, str]): The type of model to use
             params (Union[GenerateParams, TokenParams]): Parameters to use during generate requests
             credentials (Credentials): The API Credentials
         """
         logger.debug(f"Model Created:  Model: {model}, endpoint: {credentials.api_endpoint}")
         self.model = model
         self.params = params
+        self.creds = credentials
         self.service = ServiceInterface(service_url=credentials.api_endpoint, api_key=credentials.api_key)
 
     def generate_stream(
         self, prompts: Union[list[str], list[PromptPattern]], options: Options = None
     ) -> Generator[GenerateStreamResponse]:
         if len(prompts) > 0 and isinstance(prompts[0], PromptPattern):
             prompts = PromptPattern.list_str(prompts)
@@ -162,15 +172,21 @@
         if len(prompts) > 0 and isinstance(prompts[0], PromptPattern):
             prompts = PromptPattern.list_str(prompts)
 
         logger.debug(f"Calling Generate Async. Prompts: {prompts}, params: {self.params}")
 
         try:
             with AsyncResponseGenerator(
-                self.model, prompts, self.params, self.service, ordered=ordered, callback=callback, options=options
+                self.model,
+                prompts,
+                self.params,
+                self.service,
+                ordered=ordered,
+                callback=callback,
+                options=options,
             ) as asynchelper:
                 for response in tqdm(
                     asynchelper.generate_response(),
                     total=len(prompts),
                     desc="Progress",
                     unit=" inputs",
                     disable=hide_progressbar,
@@ -178,15 +194,18 @@
                     yield response
         except GenAiException as me:
             raise me
         except Exception as ex:
             raise GenAiException(ex)
 
     def tokenize_as_completed(
-        self, prompts: Union[list[str], list[PromptPattern]], return_tokens: bool = False, options: Options = None
+        self,
+        prompts: Union[list[str], list[PromptPattern]],
+        return_tokens: bool = False,
+        options: Options = None,
     ) -> Generator[TokenizeResult]:
         """The tokenize endpoint allows you to check the conversion of provided prompts to tokens
         for a given model. It splits text into words or subwords, which then are converted to ids
         through a look-up table (vocabulary). Tokenization allows the model to have a reasonable
         vocabulary size.
 
         Args:
@@ -220,15 +239,18 @@
                     raise GenAiException(tokenize_response)
         except GenAiException as me:
             raise me
         except Exception as ex:
             raise GenAiException(ex)
 
     def tokenize(
-        self, prompts: Union[list[str], list[PromptPattern]], return_tokens: bool = False, options: Options = None
+        self,
+        prompts: Union[list[str], list[PromptPattern]],
+        return_tokens: bool = False,
+        options: Options = None,
     ) -> list[TokenizeResult]:
         """The tokenize endpoint allows you to check the conversion of provided prompts to tokens
         for a given model. It splits text into words or subwords, which then are converted to ids
         through a look-up table (vocabulary). Tokenization allows the model to have a reasonable
         vocabulary size.
 
         Args:
@@ -282,7 +304,65 @@
             ) as asynchelper:
                 for response in asynchelper.generate_response():
                     yield response
         except GenAiException as me:
             raise me
         except Exception as ex:
             raise GenAiException(ex)
+
+    def tune(
+        self,
+        name: str,
+        method: str,
+        task: str,
+        hyperparameters: CreateTuneHyperParams = None,
+        training_file_ids: list[str] = None,
+        validation_file_ids: list[str] = None,
+    ):
+        """Tune the base-model for given training data.
+
+        Args:
+            name (str): Label for this tuned model.
+            method (str): The list of one or more prompt strings.
+            task (str): Task ID, could be "classification", "summarization", or "generation"
+            hyperparameters (CreateTuneHyperParams): Tuning hyperparameters
+            training_file_ids (list[str]): IDs for files with training data
+            validation_file_ids (list[str]): IDs for files with validation data
+
+        Returns:
+            Model: An instance of tuned model
+        """
+        if training_file_ids is None:
+            raise GenAiException(ValueError("Parameter should be specified: training_file_paths or training_file_ids."))
+
+        params = CreateTuneParams(
+            name=name,
+            model_id=self.model,
+            method_id=method,
+            task_id=task,
+            training_file_ids=training_file_ids,
+            validation_file_ids=validation_file_ids,
+            parameters=hyperparameters or CreateTuneHyperParams(),
+        )
+        tune = TuneManager.create_tune(service=self.service, params=params)
+        return Model(model=tune.id, params=None, credentials=self.creds)
+
+    def status(self):
+        """Get status of the model, currently supports only tuned models.
+
+        Returns:
+            str: Status of a tuned model
+        """
+        params = TunesListParams()
+        tunes = TuneManager.list_tunes(service=self.service, params=params).results
+        id_to_status = {t.id: t.status for t in tunes}
+        if self.model not in id_to_status:
+            raise GenAiException(ValueError("Tuned model not found. Currently method supports only tuned models."))
+        return id_to_status[self.model]
+
+    def delete(self):
+        params = TunesListParams()
+        tunes = TuneManager.list_tunes(service=self.service, params=params).results
+        id_to_status = {t.id: t.status for t in tunes}
+        if self.model not in id_to_status:
+            raise GenAiException(ValueError("Tuned model not found. Currently method supports only tuned models."))
+        TuneManager.delete_tune(service=self.service, tune_id=self.model)
```

### Comparing `ibm-generative-ai-0.1.19/src/genai/prompt_pattern.py` & `ibm-generative-ai-0.2.0/src/genai/prompt_pattern.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/routers/prompt_template.py` & `ibm-generative-ai-0.2.0/src/genai/routers/prompt_template.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/schemas/generate_params.py` & `ibm-generative-ai-0.2.0/src/genai/schemas/generate_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/schemas/history_params.py` & `ibm-generative-ai-0.2.0/src/genai/schemas/history_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/services/async_generator.py` & `ibm-generative-ai-0.2.0/src/genai/services/async_generator.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/services/connection_manager.py` & `ibm-generative-ai-0.2.0/src/genai/services/connection_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/services/prompt_template_manager.py` & `ibm-generative-ai-0.2.0/src/genai/services/prompt_template_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/services/request_handler.py` & `ibm-generative-ai-0.2.0/src/genai/services/request_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,33 +18,40 @@
     def _metadata(
         method: str,
         key: str,
         model_id: str = None,
         inputs: list = None,
         parameters: dict = None,
         options: Options = None,
-    ) -> tuple[dict, dict]:
+        files: dict = None,
+    ):
         """General function to build header and/or json_data for /post and /get requests.
 
         Args:
             method (str): Request type. Currently accepts GET or POST
             key (str): API key for authorization.
             model_id (str, optional): The id of the language model to be queried. Defaults to None.
             inputs (list, optional): List of inputs to be queried. Defaults to None.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
             options (Options, optional): Additional parameters to pass in the query payload. Defaults to None.
+            files (dict, optional): Pre-built files. Defaults to None.
 
         Returns:
-            tuple[dict,dict]: Headers, json_data for request
+            tuple: Headers, json_data for request, files
         """
 
         headers = {
             "Authorization": f"Bearer {key}",
             "x-request-origin": f"python-sdk/{version}",
         }
+
+        # NOTE: discuss with team if we want to keep like this or try another approach
+        if method == "POST" and files is not None:
+            return headers, None, files
+
         json_data = {}
 
         if method == "POST" or method == "PUT":
             headers["Content-Type"] = "application/json"
 
             if model_id is not None:
                 json_data["model_id"] = model_id
@@ -58,43 +65,50 @@
             if options is not None:
                 for key in options.keys():
                     json_data[key] = options[key]
 
         if method == "PATCH":
             headers["Content-Type"] = "application/json"
 
-        return headers, json_data
+        return headers, json_data, files
 
     @staticmethod
     async def async_post(
         endpoint: str,
         key: str,
         model_id: str = None,
         inputs: list = None,
         parameters: dict = None,
         options: Options = None,
+        files: dict = None,
     ):
         """Low level API for async /post request to REST API.
 
         Args:
             endpoint (str): Remote endpoint to be queried.
             key (str): API key for authorization.
             model_id (str, optional): The id of the language model to be queried. Defaults to None.
             inputs (list, optional): List of inputs to be queried. Defaults to None.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
 
         Returns:
             httpx.Response: Response from the REST API.
         """
-        headers, json_data = RequestHandler._metadata(
-            method="POST", key=key, model_id=model_id, inputs=inputs, parameters=parameters, options=options
+        headers, json_data, files = RequestHandler._metadata(
+            method="POST",
+            key=key,
+            model_id=model_id,
+            inputs=inputs,
+            parameters=parameters,
+            options=options,
+            files=files,
         )
         response = None
         async with httpx.AsyncClient(timeout=ConnectionManager.TIMEOUT) as client:
-            response = await client.post(endpoint, headers=headers, json=json_data)
+            response = await client.post(endpoint, headers=headers, json=json_data, files=files)
         return response
 
     @staticmethod
     async def async_patch(endpoint: str, key: str, json_data: dict = None) -> Response:
         """Low level API for /patch request to REST API.
 
         Currently only used for TOU endpoint.
@@ -103,15 +117,15 @@
             endpoint (str):
             key (str)
             payload: (dict, optional)
 
         Returns:
             httpx.Response: Response from the REST API.
         """
-        headers, json_data = RequestHandler._metadata(method="PATCH", key=key)
+        headers, json_data, _ = RequestHandler._metadata(method="PATCH", key=key)
         response = None
         async with httpx.AsyncClient(timeout=ConnectionManager.TIMEOUT) as client:
             response = await client.patch(endpoint, headers=headers, json=json_data)
         return response
 
     @staticmethod
     async def async_generate(
@@ -130,15 +144,15 @@
             model_id (str, optional): The id of the language model to be queried. Defaults to None.
             inputs (list, optional): List of inputs to be queried. Defaults to None.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
 
         Returns:
             httpx.Response: Response from the REST API.
         """
-        headers, json_data = RequestHandler._metadata(
+        headers, json_data, _ = RequestHandler._metadata(
             method="POST", key=key, model_id=model_id, inputs=inputs, parameters=parameters, options=options
         )
         response = None
         for attempt in range(0, ConnectionManager.MAX_RETRIES_GENERATE):
             response = await ConnectionManager.async_generate_client.post(endpoint, headers=headers, json=json_data)
             if response.status_code in [httpx.codes.SERVICE_UNAVAILABLE, httpx.codes.TOO_MANY_REQUESTS]:
                 await asyncio.sleep(2 ** (attempt + 1))
@@ -163,15 +177,15 @@
             model_id (str, optional): The id of the language model to be queried. Defaults to None.
             inputs (list, optional): List of inputs to be queried. Defaults to None.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
 
         Returns:
             httpx.Response: Response from the REST API.
         """
-        headers, json_data = RequestHandler._metadata(
+        headers, json_data, _ = RequestHandler._metadata(
             method="POST", key=key, model_id=model_id, inputs=inputs, parameters=parameters, options=options
         )
         response = None
         for attempt in range(0, ConnectionManager.MAX_RETRIES_TOKENIZE):
             # NOTE: We don't retry-fail with httpx since that'd not
             # not respect the ratelimiting below (5 requests per second).
             # Instead, we do the ratelimiting here with the help of limiter.
@@ -191,54 +205,62 @@
             endpoint (str): Remote endpoint to be queried.
             key (str): API key for authorization.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
 
         Returns:
             httpx.Response: Response from the REST API.
         """
-        headers, _ = RequestHandler._metadata(method="GET", key=key)
+        headers, _, _ = RequestHandler._metadata(method="GET", key=key)
 
         async with httpx.AsyncClient(timeout=ConnectionManager.TIMEOUT) as client:
             response = await client.get(url=endpoint, headers=headers, params=parameters)
         return response
 
     @staticmethod
     def post(
         endpoint: str,
         key: str,
         model_id: str = None,
         inputs: list = None,
         parameters: dict = None,
         streaming: bool = False,
         options: Options = None,
+        files: dict = None,
     ):
         """Low level API for /post request to REST API.
 
         Args:
             endpoint (str): Remote endpoint to be queried.
             key (str): API key for authorization.
             model_id (str, optional): The id of the language model to be queried. Defaults to None.
             inputs (list, optional): List of inputs to be queried. Defaults to None.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
             options (Options, optional): Additional parameters to pass in the query payload. Defaults to None.
+            files (dict, optional): Files to be sent to the server. Defaults to None.
 
         Returns:
             httpx.Response: Response from the REST API.
             or
             Generator of streamed response payloads from the REST API.
         """
-        headers, json_data = RequestHandler._metadata(
-            method="POST", key=key, model_id=model_id, inputs=inputs, parameters=parameters, options=options
+        headers, json_data, files = RequestHandler._metadata(
+            method="POST",
+            key=key,
+            model_id=model_id,
+            inputs=inputs,
+            parameters=parameters,
+            options=options,
+            files=files,
         )
 
         if streaming:
-            return RequestHandler.post_stream(endpoint=endpoint, headers=headers, json_data=json_data)
+            return RequestHandler.post_stream(endpoint=endpoint, headers=headers, json_data=json_data, files=files)
         else:
             with httpx.Client(timeout=ConnectionManager.TIMEOUT) as s:
-                response = s.post(url=endpoint, headers=headers, json=json_data)
+                response = s.post(url=endpoint, headers=headers, json=json_data, files=files)
                 return response
 
     @staticmethod
     def patch(endpoint: str, key: str, json_data: dict = None) -> Response:
         """Low level API for /patch request to REST API.
 
         Currently only used for TOU endpoint.
@@ -247,24 +269,24 @@
             endpoint (str):
             key (str)
             payload: (dict, optional)
 
         Returns:
             httpx.Response: Response from the REST API.
         """
-        headers, json_data = RequestHandler._metadata(method="PATCH", key=key)
+        headers, json_data, _ = RequestHandler._metadata(method="PATCH", key=key)
 
         with httpx.Client(timeout=ConnectionManager.TIMEOUT) as s:
             response = s.patch(url=endpoint, headers=headers, json=json_data)
             return response
 
     @staticmethod
-    def post_stream(endpoint, headers, json_data):
+    def post_stream(endpoint, headers, json_data, files):
         with httpx.Client(timeout=ConnectionManager.TIMEOUT) as s:
-            with s.stream(method="POST", url=endpoint, headers=headers, json=json_data) as r:
+            with s.stream(method="POST", url=endpoint, headers=headers, json=json_data, files=files) as r:
                 for chunk in r.iter_text():
                     yield chunk
 
     @staticmethod
     def get(endpoint: str, key: str, parameters: dict = None) -> Response:
         """Low level API for /get request to REST API.
 
@@ -272,15 +294,15 @@
             endpoint (str): Remote endpoint to be queried.
             key (str): API key for authorization.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
 
         Returns:
             httpx.Response: Response from the REST API.
         """
-        headers, _ = RequestHandler._metadata(method="GET", key=key)
+        headers, _, _ = RequestHandler._metadata(method="GET", key=key)
         with httpx.Client(timeout=ConnectionManager.TIMEOUT) as s:
             response = s.get(url=endpoint, headers=headers, params=parameters)
             return response
 
     @staticmethod
     def put(endpoint: str, key: str, options: Options = None) -> Response:
         """Low level API for /get request to REST API.
@@ -289,15 +311,15 @@
             endpoint (str): Remote endpoint to be queried.
             key (str): API key for authorization.
             options (Options, optional): Additional parameters to pass in the query payload. Defaults to None.
 
         Returns:
             requests.models.Response: Response from the REST API.
         """
-        headers, json_data = RequestHandler._metadata(method="PUT", key=key, options=options)
+        headers, json_data, _ = RequestHandler._metadata(method="PUT", key=key, options=options)
         with httpx.Client(timeout=ConnectionManager.TIMEOUT) as s:
             response = s.put(url=endpoint, headers=headers, json=json_data)
             return response
 
     @staticmethod
     def delete(endpoint: str, key: str, parameters: dict = None) -> Response:
         """Low level API for /get request to REST API.
@@ -306,11 +328,11 @@
             endpoint (str): Remote endpoint to be queried.
             key (str): API key for authorization.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
 
         Returns:
             requests.models.Response: Response from the REST API.
         """
-        headers, _ = RequestHandler._metadata(method="DELETE", key=key)
+        headers, _, _ = RequestHandler._metadata(method="DELETE", key=key)
         with httpx.Client(timeout=ConnectionManager.TIMEOUT) as s:
             response = s.delete(url=endpoint, headers=headers, params=parameters)
             return response
```

### Comparing `ibm-generative-ai-0.1.19/src/genai/services/service_interface.py` & `ibm-generative-ai-0.2.0/src/genai/services/service_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from httpx import Response
 
 from genai.exceptions import GenAiException
 from genai.options import Options
-from genai.routers import PromptTemplateRouter
+from genai.routers import FilesRouter, PromptTemplateRouter, TunesRouter
 from genai.schemas import GenerateParams, HistoryParams, TokenParams
 from genai.services import RequestHandler
+from genai.utils.request_utils import sanitize_params
 
 
 class ServiceInterface:
     GENERATE = "/generate"
     TOKENIZE = "/tokenize"
     HISTORY = "/requests"
     TOU = "/user"
@@ -20,14 +21,16 @@
             service_url (str): Base URL for querying.
             api_key (str): User API key for authorization.
             use_async (bool): Use async version of methods
         """
         self.service_url = service_url.rstrip("/")
         self.key = api_key
         self._prompt_templating = PromptTemplateRouter(service_url=service_url, api_key=api_key)
+        self._files = FilesRouter(service_url=service_url, api_key=api_key)
+        self._tunes = TunesRouter(service_url=service_url, api_key=api_key)
 
     def generate(
         self, model: str, inputs: list, params: GenerateParams = None, streaming: bool = False, options: Options = None
     ):
         """Generate a completion text for the given model, inputs, and params.
 
         Args:
@@ -37,15 +40,15 @@
             streaming (bool, optional): Streaming response flag. Defaults to False.
             options (Options, optional): Additional parameters to pass in the query payload. Defaults to None.
 
         Returns:
             Any: json from querying for text completion.
         """
         try:
-            params = ServiceInterface._sanitize_params(params)
+            params = sanitize_params(params)
             endpoint = self.service_url + ServiceInterface.GENERATE
             return RequestHandler.post(
                 endpoint,
                 key=self.key,
                 model_id=model,
                 inputs=inputs,
                 parameters=params,
@@ -63,15 +66,15 @@
             inputs (list): List of inputs.
             params (TokenParams, optional): Parameters for generation. Defaults to None.
 
         Returns:
             Any: json from querying for tokenization.
         """
         try:
-            params = ServiceInterface._sanitize_params(params)
+            params = sanitize_params(params)
             endpoint = self.service_url + ServiceInterface.TOKENIZE
             return RequestHandler.post(
                 endpoint, key=self.key, model_id=model, inputs=inputs, parameters=params, options=options
             )
         except Exception as e:
             raise GenAiException(e)
 
@@ -81,15 +84,15 @@
         Args:
             params (HistoryParams, optional): Parameters for retrieving history. Defaults to None.
 
         Returns:
             Any: json from querying for tokenization.
         """
         try:
-            params = ServiceInterface._sanitize_params(params)
+            params = sanitize_params(params)
             endpoint = self.service_url + ServiceInterface.HISTORY
             return RequestHandler.get(endpoint, key=self.key, parameters=params)
         except Exception as e:
             raise GenAiException(e)
 
     def terms_of_use(self, accept: bool) -> Response:
         """Accept the API Terms of Use
@@ -123,15 +126,15 @@
             inputs (list): List of inputs.
             params (GenerateParams, optional): Parameters for generation. Defaults to None.
 
         Returns:
             Any: json from querying for text completion.
         """
         try:
-            params = ServiceInterface._sanitize_params(params)
+            params = sanitize_params(params)
             endpoint = self.service_url + ServiceInterface.GENERATE
             return await RequestHandler.async_generate(
                 endpoint, key=self.key, model_id=model, inputs=inputs, parameters=params, options=options
             )
         except Exception as e:
             # without VPN this will fail
             raise GenAiException(e)
@@ -144,15 +147,15 @@
             inputs (list): List of inputs.
             params (TokenParams, optional): Parameters for generation. Defaults to None.
 
         Returns:
             Any: json from querying for tokenization.
         """
         try:
-            params = ServiceInterface._sanitize_params(params)
+            params = sanitize_params(params)
             endpoint = self.service_url + ServiceInterface.TOKENIZE
             return await RequestHandler.async_tokenize(
                 endpoint, key=self.key, model_id=model, inputs=inputs, parameters=params, options=options
             )
         except Exception as e:
             raise GenAiException(e)
 
@@ -162,15 +165,15 @@
         Args:
             params (HistoryParams, optional): Parameters for retrieving history. Defaults to None.
 
         Returns:
             Any: json from querying for tokenization.
         """
         try:
-            params = ServiceInterface._sanitize_params(params)
+            params = sanitize_params(params)
             endpoint = self.service_url + ServiceInterface.HISTORY
             return await RequestHandler.async_get(endpoint, key=self.key, parameters=params)
         except Exception as e:
             raise GenAiException(e)
 
     def async_terms_of_use(self, accept: bool) -> Response:
         """Accept the API Terms of Use
@@ -188,15 +191,7 @@
         tou_payload = {"tou_accepted": accept}
 
         try:
             endpoint = self.service_url + ServiceInterface.TOU
             return RequestHandler.async_patch(endpoint, key=self.key, json_data=tou_payload)
         except Exception as e:
             raise GenAiException(e)
-
-    @staticmethod
-    def _sanitize_params(params):
-        if params is not None:
-            if type(params) is not dict:
-                params = params.dict(by_alias=True, exclude_none=True)
-
-        return params
```

### Comparing `ibm-generative-ai-0.1.19/src/genai/utils/extensions.py` & `ibm-generative-ai-0.2.0/src/genai/utils/extensions.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/utils/json_utils.py` & `ibm-generative-ai-0.2.0/src/genai/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/genai/utils/search_space_params.py` & `ibm-generative-ai-0.2.0/src/genai/utils/search_space_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/src/ibm_generative_ai.egg-info/SOURCES.txt` & `ibm-generative-ai-0.2.0/src/ibm_generative_ai.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 .flake8
 .gitignore
 .pre-commit-config.yaml
-ACTIVE_PROJECT_TEAM.md
 CODE_OF_CONDUCT.md
-DEVELOPMENT.md
+CONTRIBUTING.md
 EXTENSIONS.md
+GETTING_STARTED.md
 LICENSE
 README.md
+STARTER_TEAM.md
 SUPPORT.md
+innersource.yaml
 pyproject.toml
 .github/PULL_REQUEST_TEMPLATE.md
 .github/ISSUE_TEMPLATE/01_bug_report.md
 .github/ISSUE_TEMPLATE/02_feature_request.md
 .github/ISSUE_TEMPLATE/03_documentation_update.md
 .github/ISSUE_TEMPLATE/config.yaml
 .github/workflows/documentation.yml
@@ -104,14 +106,18 @@
 examples/user/assets/seed_tasks.jsonl
 examples/user/localserver/localserver.py
 examples/user/localserver/requirements.txt
 examples/user/prompt_templating/watsonx-prompt-output.py
 examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py
 examples/user/prompt_templating/watsonx-prompt-pattern-ux.py
 examples/user/prompt_templating/watsonx-prompt-templating.py
+examples/user/prompt_tuning/classification.py
+examples/user/prompt_tuning/file_to_tune.jsonl
+examples/user/prompt_tuning/files_manager.py
+examples/user/prompt_tuning/summarization.py
 examples/user/prompts/Country-Capital-Factual-QA
 examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py
 examples/user/prompts_adult_dataset/prompt_generation_with_headers.py
 examples/user/templates/capital-qa.yaml
 examples/user/templates/instruction.yaml
 examples/user/templates/qa.yaml
 examples/user/templates/self-reflection.yaml
@@ -133,40 +139,49 @@
 src/genai/extensions/localserver/__init__.py
 src/genai/extensions/localserver/custom_model_interface.py
 src/genai/extensions/localserver/local_api_server.py
 src/genai/extensions/localserver/schemas.py
 src/genai/extensions/pandas/__init__.py
 src/genai/extensions/pandas/prompt_sub.py
 src/genai/routers/__init__.py
+src/genai/routers/files.py
 src/genai/routers/prompt_template.py
+src/genai/routers/tunes.py
 src/genai/schemas/__init__.py
 src/genai/schemas/descriptions.py
+src/genai/schemas/files_params.py
 src/genai/schemas/generate_params.py
 src/genai/schemas/history_params.py
 src/genai/schemas/models.py
 src/genai/schemas/responses.py
 src/genai/schemas/token_params.py
+src/genai/schemas/tunes_params.py
 src/genai/services/__init__.py
 src/genai/services/async_generator.py
 src/genai/services/connection_manager.py
+src/genai/services/file_manager.py
 src/genai/services/prompt_template_manager.py
 src/genai/services/request_handler.py
 src/genai/services/service_interface.py
+src/genai/services/tune_manager.py
 src/genai/utils/__init__.py
 src/genai/utils/extensions.py
 src/genai/utils/json_utils.py
+src/genai/utils/request_utils.py
 src/genai/utils/search_space_params.py
+src/genai/utils/service_utils.py
 src/genai/utils/watsonx_helpers.py
 src/ibm_generative_ai.egg-info/PKG-INFO
 src/ibm_generative_ai.egg-info/SOURCES.txt
 src/ibm_generative_ai.egg-info/dependency_links.txt
 src/ibm_generative_ai.egg-info/requires.txt
 src/ibm_generative_ai.egg-info/top_level.txt
 tests/__init__.py
 tests/test_concurrent.py
+tests/test_files.py
 tests/test_generate_schema.py
 tests/test_generate_service.py
 tests/test_history.py
 tests/test_json_utils.py
 tests/test_logging.py
 tests/test_metadata.py
 tests/test_model.py
@@ -176,25 +191,29 @@
 tests/test_prompt_template_manager.py
 tests/test_request_handler.py
 tests/test_schema_validation.py
 tests/test_service_interface.py
 tests/test_service_interface_async.py
 tests/test_service_utils.py
 tests/test_token.py
+tests/test_tunes.py
 tests/test_version.py
 tests/assets/age-gender.csv
 tests/assets/capital-qa-content.txt
 tests/assets/capital-qa-multivar.yaml
 tests/assets/capital-qa-sub-noheader.csv
 tests/assets/capital-qa-sub.csv
 tests/assets/capital-qa-sub.json
 tests/assets/capital-qa-sub.txt
 tests/assets/capital-qa.yaml
 tests/assets/csv_file.csv
 tests/assets/csv_file.yaml
+tests/assets/file_to_tune.csv
+tests/assets/file_to_tune.json
+tests/assets/file_to_tune.jsonl
 tests/assets/invalid-content-template.yaml
 tests/assets/invalid-template.yaml
 tests/assets/penguins.csv
 tests/assets/prompt_contents.csv
 tests/assets/response_helper.py
 tests/assets/story.yaml
 tests/assets/story_sub.txt
```

### Comparing `ibm-generative-ai-0.1.19/src/ibm_generative_ai.egg-info/requires.txt` & `ibm-generative-ai-0.2.0/src/ibm_generative_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/assets/response_helper.py` & `ibm-generative-ai-0.2.0/tests/assets/response_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -156,7 +156,86 @@
                 "id": "5XU9Zv6mrG6KIACN",
                 "name": name,
                 "value": template,
                 "created_at": "2023-05-08T11:51:18.000Z",
             }
         }
         return response
+
+    @staticmethod
+    def files(**kwargs):
+        response = {}
+        results = {
+            "id": "dumb-id",
+            "bytes": "931652",
+            "file_name": "file_to_tune.json",
+            "purpose": "tune",
+            "storage_provider_location": "us-east",
+            "created_at": "2023-05-17T14:55:06.000Z",
+            "file_formats": [
+                {
+                    "id": "1",
+                    "name": "generation",
+                },
+            ],
+        }
+
+        if "multipart_form_data" in kwargs:
+            response = {"results": results}
+        elif "file_id" in kwargs:
+            response = {"results": results}
+        elif "params" in kwargs:
+            response = {
+                "results": [results, results],
+                "totalCount": 2,
+            }
+        else:
+            response = {
+                "results": [results],
+                "totalCount": 1,
+            }
+        return response
+
+    @staticmethod
+    def tunes(**kwargs):
+        from genai.schemas.tunes_params import CreateTuneParams
+
+        response = {}
+        results = {
+            "id": "google/flan-t5-xxl-mpt-Bok9gSo3-2023-04-11-18-00-57",
+            "name": "Tune #2 google/flan-t5-xxl (3B)",
+            "model_id": "google/google/flan-t5-xxl",
+            "model_name": "google/flan-t5-xxl (3B)",
+            "status": "COMPLETED",
+            "task_id": "generation",
+            "parameters": {"batch_size": 4, "num_epochs": 12},
+            "created_at": "2023-04-11T18:00:57.000Z",
+        }
+
+        if "tune_id" in kwargs:
+            response["results"] = results
+        elif "params" in kwargs and type(kwargs["params"]) == CreateTuneParams:
+            response["results"] = results
+        else:
+            response = {
+                "results": [results],
+                "totalCount": 1,
+            }
+        return response
+
+    @staticmethod
+    def create_tune(**kwargs):
+        model_id = kwargs["model_id"] if "model_id" in kwargs else "google/flan-t5-xxl"
+        name = kwargs["name"] if "name" in kwargs else "Tune #2 google/flan-t5-xxl (3B)"
+        response = {
+            "results": {
+                "id": "google/flan-t5-xxl-mpt-Bok9gSo3-2023-04-11-18-00-57",
+                "name": name,
+                "model_id": model_id,
+                "model_name": "google/flan-t5-xxl (3B)",
+                "status": "COMPLETED",
+                "task_id": "generation",
+                "parameters": {"batch_size": 4, "num_epochs": 12},
+                "created_at": "2023-04-11T18:00:57.000Z",
+            }
+        }
+        return response
```

### Comparing `ibm-generative-ai-0.1.19/tests/extensions/test_langchain.py` & `ibm-generative-ai-0.2.0/tests/extensions/test_langchain.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/extensions/test_localserver.py` & `ibm-generative-ai-0.2.0/tests/extensions/test_localserver.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/extensions/test_save_huggingface.py` & `ibm-generative-ai-0.2.0/tests/extensions/test_save_huggingface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/extensions/test_sub_from_pandas.py` & `ibm-generative-ai-0.2.0/tests/extensions/test_sub_from_pandas.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/integration/conftest.py` & `ibm-generative-ai-0.2.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/integration/test_examples.py` & `ibm-generative-ai-0.2.0/tests/integration/test_examples.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/test_concurrent.py` & `ibm-generative-ai-0.2.0/tests/test_concurrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import httpx
 import pytest
 
 from genai.schemas import GenerateParams, ReturnOptions, TokenParams
 from genai.schemas.responses import GenerateResponse, TokenizeResponse
 from genai.services import AsyncResponseGenerator, RequestHandler, ServiceInterface
 from genai.services.connection_manager import ConnectionManager
+from genai.utils.request_utils import sanitize_params
 from tests.assets.response_helper import SimpleResponse
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.mark.unit
 class TestAsyncResponseGenerator:
@@ -166,20 +167,20 @@
                 assert time_end - time_start > 5
         ConnectionManager.MAX_RETRIES_TOKENIZE = saved
 
     @pytest.mark.asyncio
     async def test_concurrent_generate_dropped_request(self, httpx_mock, generate_params):
         failed_id = 4
         single_response = SimpleResponse.generate(model=self.model, inputs=self.inputs, params=generate_params)
-        headers, json_data = RequestHandler._metadata(
+        headers, json_data, _ = RequestHandler._metadata(
             "POST",
             key="TEST_KEY",
             model_id=self.model,
             inputs=["Input " + str(failed_id)],
-            parameters=ServiceInterface._sanitize_params(generate_params),
+            parameters=sanitize_params(generate_params),
         )
         # Following two lines: Selected input id should return 429, others should succeed
         httpx_mock.add_response(method="POST", json=single_response)
         httpx_mock.add_response(
             method="POST", status_code=429, match_content=bytes(json.dumps(json_data), encoding="utf-8")
         )
         num_prompts = 9
```

### Comparing `ibm-generative-ai-0.1.19/tests/test_generate_schema.py` & `ibm-generative-ai-0.2.0/tests/test_generate_schema.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/test_generate_service.py` & `ibm-generative-ai-0.2.0/tests/test_generate_service.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/test_history.py` & `ibm-generative-ai-0.2.0/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/test_json_utils.py` & `ibm-generative-ai-0.2.0/tests/test_json_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/test_logging.py` & `ibm-generative-ai-0.2.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/test_metadata.py` & `ibm-generative-ai-0.2.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/test_model.py` & `ibm-generative-ai-0.2.0/tests/test_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 
 import pytest
 
 from genai import Credentials, Model
 from genai.exceptions import GenAiException
 from genai.schemas import GenerateParams, ModelType
 from genai.schemas.responses import GenerateResponse, TokenizeResponse
+from genai.schemas.tunes_params import CreateTuneHyperParams
 from genai.services import ServiceInterface
 from tests.assets.response_helper import SimpleResponse
 
 
 @pytest.mark.unit
 class TestModel:
     def setup_method(self):
+        self.creds = Credentials(api_key="API_KEY", api_endpoint="SERVICE_URL")
         self.service = ServiceInterface(service_url="SERVICE_URL", api_key="API_KEY")
         self.model = "google/ul2"
         self.inputs = ["Write a tagline for an alumni association: Together we"]
 
     @pytest.fixture
     def credentials(self):
         return Credentials("GENAI_APY_KEY")
@@ -88,7 +90,39 @@
         mocked_post_request.return_value = mock_response
 
         model = Model(ModelType.FLAN_UL2, params=params, credentials=credentials)
 
         responses = model.tokenize(["a", "b", "c"], False)
 
         assert responses == expected_token_response.results
+
+    @patch("genai.services.RequestHandler.post")
+    def test_create_tune(self, mock_requests, credentials):
+        label = "test_label"
+        model_id = self.model
+        hyperparams = CreateTuneHyperParams(num_epochs=10)
+        expected_response = SimpleResponse.create_tune(model_id=model_id, name=label)
+
+        mock_response = MagicMock(status_code=200)
+        mock_response.json.return_value = expected_response
+        mock_requests.return_value = mock_response
+
+        base_model = Model(self.model, params=None, credentials=credentials)
+        tuned_model = base_model.tune(
+            name=label, method="mpt", task="generation", training_file_ids=["id1"], hyperparameters=hyperparams
+        )
+        assert tuned_model.model == expected_response["results"]["id"]
+
+    @patch("genai.services.RequestHandler.get")
+    def test_status(self, mock_requests, credentials):
+        label = "test_label"
+        model_id = self.model
+        tune_id = SimpleResponse.create_tune(model_id=model_id, name=label)["results"]["id"]
+
+        tuned_model = Model(tune_id, params=None, credentials=credentials)
+
+        expected_response = SimpleResponse.tunes()
+        mock_response = MagicMock(status_code=200)
+        mock_response.json.return_value = expected_response
+        mock_requests.return_value = mock_response
+
+        assert tuned_model.status() == expected_response["results"][0]["status"]
```

### Comparing `ibm-generative-ai-0.1.19/tests/test_model_async.py` & `ibm-generative-ai-0.2.0/tests/test_model_async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/test_prompt_pattern.py` & `ibm-generative-ai-0.2.0/tests/test_prompt_pattern.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/test_prompt_pattern_watsonx.py` & `ibm-generative-ai-0.2.0/tests/test_prompt_pattern_watsonx.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/test_prompt_template_manager.py` & `ibm-generative-ai-0.2.0/tests/test_prompt_template_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/test_request_handler.py` & `ibm-generative-ai-0.2.0/tests/test_request_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.inputs = ["a"]
 
     @pytest.fixture
     def params(seld):
         return GenerateParams(decoding_method="greedy").dict(by_alias=True, exclude_none=True)
 
     def test_metadata_post(self, params):
-        headers, json_data = RequestHandler._metadata(
+        headers, json_data, _ = RequestHandler._metadata(
             method="POST", key="API_KEY", model_id=self.model, inputs=self.inputs, parameters=params
         )
 
         assert "Content-Type" in headers
         assert headers["Content-Type"] == "application/json"
 
         assert "Authorization" in headers
@@ -30,15 +30,15 @@
         assert json_data == {
             "model_id": self.model,
             "inputs": self.inputs,
             "parameters": {"decoding_method": "greedy"},
         }
 
     def test_metadata_get(self):
-        headers, _ = RequestHandler._metadata(method="GET", key="API_KEY")
+        headers, _, _ = RequestHandler._metadata(method="GET", key="API_KEY")
 
         assert "Authorization" in headers
         assert headers["Authorization"] == "Bearer API_KEY"
 
     @patch("httpx.Client.get")
     def test_get(self, mock: MagicMock):
         expected_resp = {"some": "history"}
```

### Comparing `ibm-generative-ai-0.1.19/tests/test_schema_validation.py` & `ibm-generative-ai-0.2.0/tests/test_schema_validation.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/test_service_interface.py` & `ibm-generative-ai-0.2.0/tests/test_service_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from unittest.mock import MagicMock, patch
 
 import pytest
 
 from genai.schemas import GenerateParams, ReturnOptions
 from genai.services import ServiceInterface
+from genai.utils.request_utils import sanitize_params
 from tests.assets.response_helper import SimpleResponse
 
 
 @pytest.mark.unit
 class TestServiceInterface:
     def setup_method(self):
         # mock object for the API call
@@ -32,11 +33,11 @@
 
     @patch("genai.services.RequestHandler.patch", side_effect=Exception("some general error"))
     def test_tou_exception(self, mock):
         with pytest.raises(BaseException, match="some general error"):
             self.service.terms_of_use(True)
 
     def test_sanitize_params(self, params):
-        new_dict = ServiceInterface._sanitize_params(params=params)
+        new_dict = sanitize_params(params=params)
 
         assert isinstance(new_dict, dict)
         assert "min_new_tokens" not in new_dict
```

### Comparing `ibm-generative-ai-0.1.19/tests/test_service_interface_async.py` & `ibm-generative-ai-0.2.0/tests/test_service_interface_async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.19/tests/test_service_utils.py` & `ibm-generative-ai-0.2.0/tests/test_service_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import unittest
 
 import pytest
 
 from genai.schemas import GenerateParams, ReturnOptions
-from genai.services import ServiceInterface
+from genai.utils.request_utils import sanitize_params
 
 # API Reference : https://workbench.res.ibm.com/docs/api-reference#generate
 
 SERVICE_URL = "https://workbench-api.res.ibm.com/v1/"
 KEY = "pak-"
 
 
 @pytest.mark.unit
 class TestServiceUtils(unittest.TestCase):
     def test_sanitize_params_with_params(self):
         input_genParams = GenerateParams(decoding_method="greedy", return_options=ReturnOptions(input_text=True))
 
         expected_genParams = {"decoding_method": "greedy", "return_options": {"input_text": True}}
 
-        sanitized_dict = ServiceInterface._sanitize_params(input_genParams)
+        sanitized_dict = sanitize_params(input_genParams)
         self.assertEqual(expected_genParams, sanitized_dict)
```

### Comparing `ibm-generative-ai-0.1.19/tests/test_token.py` & `ibm-generative-ai-0.2.0/tests/test_token.py`

 * *Files identical despite different names*

