# Comparing `tmp/khoj_assistant-0.7.2.dev46.tar.gz` & `tmp/khoj_assistant-0.7.2.dev49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jul 10 05:31:37 2023, max compression
+gzip compressed data, last modified: Mon Jul 10 19:10:20 2023, max compression
```

## Comparing `khoj_assistant-0.7.2.dev46.tar` & `khoj_assistant-0.7.2.dev49.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/__init__.py
--rw-r--r--   0        0        0    11624 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/configure.py
--rw-r--r--   0        0        0     5304 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1395 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     5152 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    18248 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    16101 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6930 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     7322 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0     3401 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/content_type_notion_input.html
--rw-r--r--   0        0        0    19406 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3660 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1921 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0      549 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0   205167 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     1578 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/notion.svg
--rw-r--r--   0        0        0     7946 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4455 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     4824 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     3991 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     8304 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13517 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7454 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0     9295 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/notion/notion_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5397 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    20444 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/routers/api.py
--rw-r--r--   0        0        0      167 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     2895 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/routers/helpers.py
--rw-r--r--   0        0        0     5524 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7566 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11237 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2040 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2571 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2710 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6889 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4338 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/LICENSE
--rw-r--r--   0        0        0    24572 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/README.md
--rw-r--r--   0        0        0     2792 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/pyproject.toml
--rw-r--r--   0        0        0    26937 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/__init__.py
+-rw-r--r--   0        0        0    11624 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/configure.py
+-rw-r--r--   0        0        0     5389 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     5152 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    18248 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    16101 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6930 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     7322 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0     3401 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/content_type_notion_input.html
+-rw-r--r--   0        0        0    19406 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3660 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1921 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0      549 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0   205167 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     1578 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/notion.svg
+-rw-r--r--   0        0        0     7946 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4455 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     4824 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     3991 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     8304 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13517 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0     9295 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/notion/notion_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5397 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    20444 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/routers/api.py
+-rw-r--r--   0        0        0      167 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     2895 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/routers/helpers.py
+-rw-r--r--   0        0        0     5524 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7566 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11237 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2040 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2571 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2710 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6889 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4338 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/LICENSE
+-rw-r--r--   0        0        0    24888 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/README.md
+-rw-r--r--   0        0        0     2792 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/pyproject.toml
+-rw-r--r--   0        0        0    27253 2023-07-10 19:10:20.000000 khoj_assistant-0.7.2.dev49/PKG-INFO
```

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/configure.py` & `khoj_assistant-0.7.2.dev49/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/main.py` & `khoj_assistant-0.7.2.dev49/src/khoj/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,17 +90,18 @@
         configure_server(args, required=False)
         configure_routes(app)
         server = ServerThread(app, args.host, args.port, args.socket)
 
         url = f"http://{args.host}:{args.port}"
         logger.info(f"🌗 Khoj is running at {url}")
         try:
-            webbrowser.open(url)
+            startup_url = url if args.config else f"{url}/config"
+            webbrowser.open(startup_url)
         except:
-            logger.warning("🚧 Unable to open browser. Please open it manually to configure Khoj.")
+            logger.warning(f"🚧 Unable to open browser. Please open {url} manually to configure or use Khoj.")
 
         # Show Main Window on First Run Experience or if on Linux
         if args.config is None or system() not in ["Windows", "Darwin"]:
             main_window.show()
 
         # Setup Signal Handlers
         signal.signal(signal.SIGINT, sigint_handler)
```

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/404.html` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/chat.html` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/config.html` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/content_type_notion_input.html` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/content_type_notion_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/index.html` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/notion.svg` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/notion.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.7.2.dev49/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.7.2.dev49/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.7.2.dev49/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.7.2.dev49/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.7.2.dev49/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.7.2.dev49/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.7.2.dev49/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.7.2.dev49/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/processor/notion/notion_to_jsonl.py` & `khoj_assistant-0.7.2.dev49/src/khoj/processor/notion/notion_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.7.2.dev49/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.7.2.dev49/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.7.2.dev49/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/routers/api.py` & `khoj_assistant-0.7.2.dev49/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/routers/helpers.py` & `khoj_assistant-0.7.2.dev49/src/khoj/routers/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/routers/web_client.py` & `khoj_assistant-0.7.2.dev49/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.7.2.dev49/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.7.2.dev49/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.7.2.dev49/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.7.2.dev49/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/search_type/image_search.py` & `khoj_assistant-0.7.2.dev49/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/search_type/text_search.py` & `khoj_assistant-0.7.2.dev49/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/utils/cli.py` & `khoj_assistant-0.7.2.dev49/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/utils/config.py` & `khoj_assistant-0.7.2.dev49/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/utils/constants.py` & `khoj_assistant-0.7.2.dev49/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/utils/helpers.py` & `khoj_assistant-0.7.2.dev49/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/utils/jsonl.py` & `khoj_assistant-0.7.2.dev49/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/utils/models.py` & `khoj_assistant-0.7.2.dev49/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.7.2.dev49/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/utils/state.py` & `khoj_assistant-0.7.2.dev49/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/src/khoj/utils/yaml.py` & `khoj_assistant-0.7.2.dev49/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/.gitignore` & `khoj_assistant-0.7.2.dev49/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/LICENSE` & `khoj_assistant-0.7.2.dev49/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/README.md` & `khoj_assistant-0.7.2.dev49/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -121,39 +121,43 @@
 - Make sure [python](https://realpython.com/installing-python/) and [pip](https://pip.pypa.io/en/stable/installation/) are installed on your machine
 - Check the [Khoj.el Readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#Setup) to setup Khoj with Emacs<br />
   Its simpler as it can skip the server *install*, *run* and *configure* step below.
 - Check the [Khoj Obsidian Readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#Setup) to setup Khoj with Obsidian<br />
   Its simpler as it can skip the *configure* step below.
 
 ### 1. Install
+Run the following command in your terminal to install the Khoj backend.
+
 - On Linux/MacOS
   ```shell
   python -m pip install khoj-assistant
   ```
 
 - On Windows
   ```shell
   py -m pip install khoj-assistant
   ```
 
 ### 2. Run
 
+Run the following commmand from your terminal to start the Khoj backend and open Khoj in your browser.
+
 ```shell
-khoj
+khoj --gui
 ```
 
 Note: To start Khoj automatically in the background use [Task scheduler](https://www.windowscentral.com/how-create-automated-task-using-task-scheduler-windows-10) on Windows or [Cron](https://en.wikipedia.org/wiki/Cron) on Mac, Linux (e.g with `@reboot khoj`)
 
 ### 3. Configure
-
-1. Enable content types and point to files to search in the First Run Screen that pops up on app start
-2. Click `Configure` and wait. The app will download ML models and index the content for search
+1. Set `File`, `Folder` and hit `Save` in each Plugins you want to enable for Search on the Khoj config page
+2. Add your OpenAI API key to Chat Feature settings if you want to use Chat
+3. Click `Configure` and wait. The app will download ML models and index the content for search and (optionally) chat
 
 ### 4. Install Interface Plugins
-Khoj exposes a web interface by default.<br />
+Khoj exposes a web interface to search, chat and configure by default.<br />
 The optional steps below allow using Khoj from within an existing application like Obsidian or Emacs.
 
 - **Khoj Obsidian**:<br />
 [Install](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#2-Setup-Plugin) the Khoj Obsidian plugin
 
 - **Khoj Emacs**:<br />
 [Install](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#2-Install-Khojel) khoj.el
```

### Comparing `khoj_assistant-0.7.2.dev46/pyproject.toml` & `khoj_assistant-0.7.2.dev49/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev46/PKG-INFO` & `khoj_assistant-0.7.2.dev49/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.7.2.dev46
+Version: 0.7.2.dev49
 Summary: An AI personal assistant for your Digital Brain
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
@@ -179,39 +179,43 @@
 - Make sure [python](https://realpython.com/installing-python/) and [pip](https://pip.pypa.io/en/stable/installation/) are installed on your machine
 - Check the [Khoj.el Readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#Setup) to setup Khoj with Emacs<br />
   Its simpler as it can skip the server *install*, *run* and *configure* step below.
 - Check the [Khoj Obsidian Readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#Setup) to setup Khoj with Obsidian<br />
   Its simpler as it can skip the *configure* step below.
 
 ### 1. Install
+Run the following command in your terminal to install the Khoj backend.
+
 - On Linux/MacOS
   ```shell
   python -m pip install khoj-assistant
   ```
 
 - On Windows
   ```shell
   py -m pip install khoj-assistant
   ```
 
 ### 2. Run
 
+Run the following commmand from your terminal to start the Khoj backend and open Khoj in your browser.
+
 ```shell
-khoj
+khoj --gui
 ```
 
 Note: To start Khoj automatically in the background use [Task scheduler](https://www.windowscentral.com/how-create-automated-task-using-task-scheduler-windows-10) on Windows or [Cron](https://en.wikipedia.org/wiki/Cron) on Mac, Linux (e.g with `@reboot khoj`)
 
 ### 3. Configure
-
-1. Enable content types and point to files to search in the First Run Screen that pops up on app start
-2. Click `Configure` and wait. The app will download ML models and index the content for search
+1. Set `File`, `Folder` and hit `Save` in each Plugins you want to enable for Search on the Khoj config page
+2. Add your OpenAI API key to Chat Feature settings if you want to use Chat
+3. Click `Configure` and wait. The app will download ML models and index the content for search and (optionally) chat
 
 ### 4. Install Interface Plugins
-Khoj exposes a web interface by default.<br />
+Khoj exposes a web interface to search, chat and configure by default.<br />
 The optional steps below allow using Khoj from within an existing application like Obsidian or Emacs.
 
 - **Khoj Obsidian**:<br />
 [Install](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#2-Setup-Plugin) the Khoj Obsidian plugin
 
 - **Khoj Emacs**:<br />
 [Install](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#2-Install-Khojel) khoj.el
```

