# Comparing `tmp/khoj_assistant-0.7.2.dev44.tar.gz` & `tmp/khoj_assistant-0.7.2.dev45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Jul  9 17:21:16 2023, max compression
+gzip compressed data, last modified: Sun Jul  9 22:29:26 2023, max compression
```

## Comparing `khoj_assistant-0.7.2.dev44.tar` & `khoj_assistant-0.7.2.dev45.tar`

### file list

```diff
@@ -1,78 +1,81 @@
--rw-r--r--   0        0        0        0 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/__init__.py
--rw-r--r--   0        0        0    11048 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/configure.py
--rw-r--r--   0        0        0     5304 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1395 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3910 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    17874 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    14688 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6930 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     7322 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    18700 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3660 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1813 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0      549 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0   205167 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     7946 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     4829 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     3991 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     8304 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13517 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7454 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5397 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    19428 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/routers/api.py
--rw-r--r--   0        0        0      167 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     2895 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/routers/helpers.py
--rw-r--r--   0        0        0     4646 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7566 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11054 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2040 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2396 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2500 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6889 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4136 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/LICENSE
--rw-r--r--   0        0        0    24572 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/README.md
--rw-r--r--   0        0        0     2792 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/pyproject.toml
--rw-r--r--   0        0        0    26937 2023-07-09 17:21:16.000000 khoj_assistant-0.7.2.dev44/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/__init__.py
+-rw-r--r--   0        0        0    11624 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/configure.py
+-rw-r--r--   0        0        0     5304 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3910 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    17875 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    16101 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6930 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     7322 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0     3401 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/content_type_notion_input.html
+-rw-r--r--   0        0        0    19024 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3660 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1813 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0      549 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0   205167 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     1578 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/notion.svg
+-rw-r--r--   0        0        0     7946 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4455 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     4824 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     3991 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     8304 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13517 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0     9295 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/notion/notion_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5397 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    20444 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/routers/api.py
+-rw-r--r--   0        0        0      167 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     2895 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/routers/helpers.py
+-rw-r--r--   0        0        0     5524 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7566 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11237 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2040 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2571 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2710 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6889 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4338 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/LICENSE
+-rw-r--r--   0        0        0    24572 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/README.md
+-rw-r--r--   0        0        0     2792 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/pyproject.toml
+-rw-r--r--   0        0        0    26937 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/PKG-INFO
```

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/configure.py` & `khoj_assistant-0.7.2.dev45/src/khoj/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # Internal Packages
 from khoj.processor.conversation.gpt import summarize
 from khoj.processor.jsonl.jsonl_to_jsonl import JsonlToJsonl
 from khoj.processor.markdown.markdown_to_jsonl import MarkdownToJsonl
 from khoj.processor.org_mode.org_to_jsonl import OrgToJsonl
 from khoj.processor.pdf.pdf_to_jsonl import PdfToJsonl
 from khoj.processor.github.github_to_jsonl import GithubToJsonl
+from khoj.processor.notion.notion_to_jsonl import NotionToJsonl
 from khoj.search_type import image_search, text_search
 from khoj.utils import constants, state
 from khoj.utils.config import SearchType, SearchModels, ProcessorConfigModel, ConversationProcessorConfigModel
 from khoj.utils.helpers import LRU, resolve_absolute_path, merge_dicts
 from khoj.utils.rawconfig import FullConfig, ProcessorConfig
 from khoj.search_filter.date_filter import DateFilter
 from khoj.search_filter.word_filter import WordFilter
@@ -165,14 +166,26 @@
                 model.plugin_search[plugin_type] = text_search.setup(
                     JsonlToJsonl,
                     plugin_config,
                     search_config=config.search_type.asymmetric,
                     regenerate=regenerate,
                     filters=[DateFilter(), WordFilter(), FileFilter()],
                 )
+
+        # Initialize Notion Search
+        if (t == None or t in state.SearchType) and config.content_type.notion:
+            logger.info("🔌 Setting up search for notion")
+            model.notion_search = text_search.setup(
+                NotionToJsonl,
+                config.content_type.notion,
+                search_config=config.search_type.asymmetric,
+                regenerate=regenerate,
+                filters=[DateFilter(), WordFilter(), FileFilter()],
+            )
+
     except Exception as e:
         logger.error("🚨 Failed to setup search")
         raise e
 
     # Invalidate Query Cache
     state.query_cache = LRU()
 
@@ -244,15 +257,15 @@
 
     state.processor_config.conversation.chat_session = []
     logger.info("📩 Saved current chat session to conversation logs")
 
 
 @schedule.repeat(schedule.every(59).minutes)
 def upload_telemetry():
-    if not state.config or not state.config.app.should_log_telemetry or not state.telemetry:
+    if not state.config or not state.config.app or not state.config.app.should_log_telemetry or not state.telemetry:
         message = "📡 No telemetry to upload" if not state.telemetry else "📡 Telemetry logging disabled"
         logger.debug(message)
         return
 
     try:
         logger.debug(f"📡 Upload usage telemetry to {constants.telemetry_server}:\n{state.telemetry}")
         for log in state.telemetry:
```

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/main.py` & `khoj_assistant-0.7.2.dev45/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/404.html` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/chat.html` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/chat.html`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,15 @@
                         reader.read().then(({ done, value }) => {
                             if (done) {
                                 return;
                             }
 
                             // Decode message chunk from stream
                             const chunk = decoder.decode(value, { stream: true });
+
                             if (chunk.includes("### compiled references:")) {
                                 const additionalResponse = chunk.split("### compiled references:")[0];
                                 new_response_text.innerHTML += additionalResponse;
 
                                 const rawReference = chunk.split("### compiled references:")[1];
                                 const rawReferenceAsJson = JSON.parse(rawReference);
                                 let polishedReference = rawReferenceAsJson.map((reference, index) => generateReference(reference, index))
```

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/config.html` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/config.html`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
                     <img class="card-icon" src="/static/assets/icons/github.svg" alt="Github">
                     <h3 class="card-title">
                         Github
                         {% if current_config.content_type.github %}
                             <img id="configured-icon-github" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
                         {% endif %}
                     </h3>
-
                 </div>
                 <div class="card-description-row">
                 <p class="card-description">Set repositories for Khoj to index</p>
                 </div>
                 <div class="card-action-row">
                     <a class="card-button" href="/config/content_type/github">
                         {% if current_config.content_type.github %}
@@ -35,14 +34,45 @@
                             Disable
                         </button>
                     </div>
                 {% endif %}
             </div>
             <div class="card">
                 <div class="card-title-row">
+                    <img class="card-icon" src="/static/assets/icons/notion.svg" alt="Notion">
+                    <h3 class="card-title">
+                        Notion
+                        {% if current_config.content_type.notion %}
+                            <img id="configured-icon-notion" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
+                        {% endif %}
+                    </h3>
+                </div>
+                <div class="card-description-row">
+                    <p class="card-description">Configure your settings from Notion</p>
+                </div>
+                <div class="card-action-row">
+                    <a class="card-button" href="/config/content_type/notion">
+                        {% if current_config.content_type.content %}
+                            Update
+                        {% else %}
+                            Setup
+                        {% endif %}
+                        <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M12 5l7 7-7 7"></path></svg>
+                    </a>
+                </div>
+                {% if current_config.content_type.notion %}
+                    <div id="clear-notion" class="card-action-row">
+                        <button class="card-button" onclick="clearContentType('notion')">
+                            Disable
+                        </button>
+                    </div>
+                {% endif %}
+            </div>
+            <div class="card">
+                <div class="card-title-row">
                     <img class="card-icon" src="/static/assets/icons/markdown.svg" alt="markdown">
                     <h3 class="card-title">
                         Markdown
                         {% if current_config.content_type.markdown %}
                             <img id="configured-icon-markdown" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
                         {% endif %}
                     </h3>
@@ -220,70 +250,65 @@
             }
         })
     };
 
     var configure = document.getElementById("configure");
     configure.addEventListener("click", function(event) {
         event.preventDefault();
-        configure.disabled = true;
-        configure.innerHTML = "Configuring...";
-        const csrfToken = document.cookie.split('; ').find(row => row.startsWith('csrftoken'))?.split('=')[1];
-        fetch('/api/update?&client=web', {
-            method: 'GET',
-            headers: {
-                'Content-Type': 'application/json',
-                'X-CSRFToken': csrfToken
-            }
-        })
-        .then(response => response.json())
-        .then(data => {
-            console.log('Success:', data);
-            document.getElementById("status").innerHTML = "Configured successfully!";
-            document.getElementById("status").style.display = "block";
-            configure.disabled = false;
-            configure.innerHTML = "⚙️ Configured";
-        })
-        .catch((error) => {
-            console.error('Error:', error);
-            document.getElementById("status").innerHTML = "Unable to save configuration. Raise issue on Khoj Discord or Github.";
-            document.getElementById("status").style.display = "block";
-            configure.disabled = false;
-            configure.innerHTML = "⚙️ Configure";
-        });
+        updateIndex(
+            force=false,
+            successText="Configured successfully!",
+            errorText="Unable to configure. Raise issue on Khoj <a href='https://github.com/khoj-ai/khoj/issues'>Github</a> or <a href='https://discord.gg/BDgyabRM6e'>Discord</a>.",
+            button=configure,
+            loadingText="Configuring...",
+            emoji="⚙️");
     });
 
     var reinitialize = document.getElementById("reinitialize");
     reinitialize.addEventListener("click", function(event) {
         event.preventDefault();
-        reinitialize.disabled = true;
-        reinitialize.innerHTML = "Reinitializing...";
+        updateIndex(
+            force=true,
+            successText="Reinitialized successfully!",
+            errorText="Unable to reinitialize. Raise issue on Khoj <a href='https://github.com/khoj-ai/khoj/issues'>Github</a> or <a href='https://discord.gg/BDgyabRM6e'>Discord</a>.",
+            button=reinitialize,
+            loadingText="Reinitializing...",
+            emoji="🔄");
+    });
+
+    function updateIndex(force, successText, errorText, button, loadingText, emoji) {
         const csrfToken = document.cookie.split('; ').find(row => row.startsWith('csrftoken'))?.split('=')[1];
-        fetch('/api/update?&client=web&force=True', {
+        button.disabled = true;
+        button.innerHTML = emoji + loadingText;
+        fetch('/api/update?&client=web&force=' + force, {
             method: 'GET',
             headers: {
                 'Content-Type': 'application/json',
                 'X-CSRFToken': csrfToken
             }
         })
         .then(response => response.json())
         .then(data => {
             console.log('Success:', data);
-            document.getElementById("status").innerHTML = "Reinitialized successfully!";
+            if (data.detail != null) {
+                throw new Error(data.detail);
+            }
+            document.getElementById("status").innerHTML = emoji + successText;
             document.getElementById("status").style.display = "block";
-            reinitialize.disabled = false;
-            reinitialize.innerHTML = "🔄 Reinitialized";
+            button.disabled = false;
+            button.innerHTML = '✅ Done!';
         })
         .catch((error) => {
             console.error('Error:', error);
-            document.getElementById("status").innerHTML = "Unable to reinitialize. Raise issue on Khoj Discord or Github.";
+            document.getElementById("status").innerHTML = emoji + errorText
             document.getElementById("status").style.display = "block";
-            reinitialize.disabled = false;
-            reinitialize.innerHTML = "🔄 Reinitialize";
+            button.disabled = false;
+            button.innerHTML = '⚠️ Unsuccessful';
         });
-    });
+    }
 
     // Setup the results count slider
     const resultsCountSlider = document.getElementById('results-count-slider');
     const resultsCountValue = document.getElementById('results-count-value');
 
     // Set the initial value of the slider
     resultsCountValue.textContent = resultsCountSlider.value;
```

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/index.html` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
                         (item.additional.file.includes("issues") && item.additional.file.includes("github.com")) ||
                         (item.additional.file.includes("commit") && item.additional.file.includes("github.com"))
                     )
                 {
                     html += render_markdown(query, [item]);
                 } else if (item.additional.file.endsWith(".pdf")) {
                     html += render_pdf(query, [item]);
+                } else if (item.additional.file.includes("notion.so")) {
+                    html += `<div class="results-notion">` + `<b><a href="${item.additional.file}">${item.additional.heading}</a></b>` + `<p>${item.entry}</p>` + `</div>`;
                 }
             });
             return html;
         }
 
         function render_results(data, query, type) {
             let results = "";
@@ -82,15 +84,15 @@
                 results = render_markdown(query, data);
             } else if (type === "org") {
                 results = render_org(query, data, "org-");
             } else if (type === "image") {
                 results = data.map(render_image).join('');
             } else if (type === "pdf") {
                 results = render_pdf(query, data);
-            } else if (type === "github" || type === "all") {
+            } else if (type === "github" || type === "all" || type === "notion") {
                 results = render_multiple(query, data, type);
             } else {
                 results = data.map((item) => `<div class="results-plugin">` + `<p>${item.entry}</p>` + `</div>`).join("\n")
             }
 
             // Any POST rendering goes here.
 
@@ -123,15 +125,15 @@
             }
 
             // If set query field in url query param on rerank
             if (rerank)
                 setQueryFieldInUrl(query);
 
             // Execute Search and Render Results
-            url = createRequestUrl(query, type, results_count, rerank);
+            url = createRequestUrl(query, type, results_count || 5, rerank);
             fetch(url)
                 .then(response => response.json())
                 .then(data => {
                     console.log(data);
                     document.getElementById("results").innerHTML = render_results(data, query, type);
                 });
 
@@ -343,14 +345,15 @@
             border-radius: 10px;
             border: 1px solid #475569;
         }
         #json {
             white-space: pre-wrap;
         }
         .results-pdf,
+        .results-notion,
         .results-plugin {
             text-align: left;
             white-space: pre-line;
         }
         .results-markdown,
         .results-github {
             text-align: left;
@@ -400,14 +403,15 @@
             width: 20px;
             height: 20px;
             border-radius: 50%;
         }
 
         div#results-error,
         div.results-markdown,
+        div.results-notion,
         div.results-org,
         div.results-pdf {
             text-align: left;
             box-shadow: 2px 2px 2px var(--primary-hover);
             border-radius: 5px;
             padding: 10px;
             margin: 10px 0;
```

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.7.2.dev45/src/khoj/processor/text_to_jsonl.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                     )
                 )
 
         return chunked_entries
 
     @staticmethod
     def mark_entries_for_update(
-        current_entries: List[Entry], previous_entries: List[Entry], key="compiled", logger=None
+        current_entries: List[Entry], previous_entries: List[Entry], key="compiled", logger: logging.Logger = None
     ) -> List[Tuple[int, Entry]]:
         # Hash all current and previous entries to identify new entries
         with timer("Hash previous, current entries", logger):
             current_entry_hashes = list(map(TextToJsonl.hash_func(key), current_entries))
             previous_entry_hashes = list(map(TextToJsonl.hash_func(key), previous_entries))
 
         with timer("Identify, Mark, Combine new, existing entries", logger):
@@ -86,7 +86,12 @@
                 for entry_hash in existing_entry_hashes
             ]
 
             existing_entries_sorted = sorted(existing_entries, key=lambda e: e[0])
             entries_with_ids = existing_entries_sorted + new_entries
 
         return entries_with_ids
+
+    @staticmethod
+    def convert_text_maps_to_jsonl(entries: List[Entry]) -> str:
+        # Convert each entry to JSON and write to JSONL file
+        return "".join([f"{entry.to_json()}\n" for entry in entries])
```

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,15 @@
     # Get Response from GPT
     logger.debug(f"Prompt for GPT: {messages}")
     response = completion_with_backoff(
         messages=messages,
         model_name=model,
         temperature=temperature,
         max_tokens=max_tokens,
-        frequency_penalty=0.2,
-        model_kwargs={"stop": ['"""']},
+        model_kwargs={"stop": ['"""'], "frequency_penalty": 0.2},
         openai_api_key=api_key,
     )
 
     # Extract, Clean Message from GPT's Response
     return str(response.content).replace("\n\n", "")
```

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.7.2.dev45/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.7.2.dev45/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.7.2.dev45/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.7.2.dev45/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.7.2.dev45/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.7.2.dev45/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/routers/api.py` & `khoj_assistant-0.7.2.dev45/src/khoj/routers/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     FullConfig,
     ProcessorConfig,
     SearchConfig,
     SearchResponse,
     TextContentConfig,
     ConversationProcessorConfig,
     GithubContentConfig,
+    NotionContentConfig,
 )
 from khoj.utils.state import SearchType
 from khoj.utils import state, constants
 from khoj.utils.yaml import save_config_to_file_updated_state
 from fastapi.responses import StreamingResponse, Response
 from khoj.routers.helpers import perform_chat_checks, generate_chat_response
 from khoj.processor.conversation.gpt import extract_questions
@@ -41,53 +42,73 @@
 # Initialize Router
 api = APIRouter()
 logger = logging.getLogger(__name__)
 
 # If it's a demo instance, prevent updating any of the configuration.
 if not state.demo:
 
+    def _initialize_config():
+        if state.config is None:
+            state.config = FullConfig()
+            state.config.search_type = SearchConfig.parse_obj(constants.default_config["search-type"])
+
     @api.get("/config/data", response_model=FullConfig)
     def get_config_data():
         return state.config
 
     @api.post("/config/data")
     async def set_config_data(updated_config: FullConfig):
         state.config = updated_config
         with open(state.config_file, "w") as outfile:
             yaml.dump(yaml.safe_load(state.config.json(by_alias=True)), outfile)
             outfile.close()
         return state.config
 
     @api.post("/config/data/content_type/github", status_code=200)
     async def set_content_config_github_data(updated_config: Union[GithubContentConfig, None]):
-        if not state.config:
-            state.config = FullConfig()
-            state.config.search_type = SearchConfig.parse_obj(constants.default_config["search-type"])
+        _initialize_config()
 
         if not state.config.content_type:
             state.config.content_type = ContentConfig(**{"github": updated_config})
         else:
             state.config.content_type.github = updated_config
 
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
 
+    @api.post("/config/data/content_type/notion", status_code=200)
+    async def set_content_config_notion_data(updated_config: Union[NotionContentConfig, None]):
+        _initialize_config()
+
+        if not state.config.content_type:
+            state.config.content_type = ContentConfig(**{"notion": updated_config})
+        else:
+            state.config.content_type.notion = updated_config
+
+        try:
+            save_config_to_file_updated_state()
+            return {"status": "ok"}
+        except Exception as e:
+            return {"status": "error", "message": str(e)}
+
     @api.post("/delete/config/data/content_type/{content_type}", status_code=200)
     async def remove_content_config_data(content_type: str):
         if not state.config or not state.config.content_type:
             return {"status": "ok"}
 
         if state.config.content_type:
             state.config.content_type[content_type] = None
 
         if content_type == "github":
             state.model.github_search = None
+        elif content_type == "notion":
+            state.model.notion_search = None
         elif content_type == "plugins":
             state.model.plugin_search = None
         elif content_type == "pdf":
             state.model.pdf_search = None
         elif content_type == "markdown":
             state.model.markdown_search = None
         elif content_type == "org":
@@ -110,34 +131,31 @@
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
 
     @api.post("/config/data/content_type/{content_type}", status_code=200)
     async def set_content_config_data(content_type: str, updated_config: Union[TextContentConfig, None]):
-        if not state.config:
-            state.config = FullConfig()
-            state.config.search_type = SearchConfig.parse_obj(constants.default_config["search-type"])
+        _initialize_config()
 
         if not state.config.content_type:
             state.config.content_type = ContentConfig(**{content_type: updated_config})
         else:
             state.config.content_type[content_type] = updated_config
 
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
 
     @api.post("/config/data/processor/conversation", status_code=200)
     async def set_processor_conversation_config_data(updated_config: Union[ConversationProcessorConfig, None]):
-        if not state.config:
-            state.config = FullConfig()
-            state.config.search_type = SearchConfig.parse_obj(constants.default_config["search-type"])
+        _initialize_config()
+
         state.config.processor = ProcessorConfig(conversation=updated_config)
         state.processor_config = configure_processor(state.config.processor)
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
@@ -308,14 +326,28 @@
                     question_embedding=encoded_asymmetric_query,
                     rank_results=r or False,
                     score_threshold=score_threshold,
                     dedupe=dedupe or True,
                 )
             ]
 
+        if (t == SearchType.Notion or t == SearchType.All) and state.model.notion_search:
+            # query notion pages
+            search_futures += [
+                executor.submit(
+                    text_search.query,
+                    user_query,
+                    state.model.notion_search,
+                    question_embedding=encoded_asymmetric_query,
+                    rank_results=r or False,
+                    score_threshold=score_threshold,
+                    dedupe=dedupe or True,
+                )
+            ]
+
         # Query across each requested content types in parallel
         with timer("Query took", logger):
             for search_future in concurrent.futures.as_completed(search_futures):
                 if t == SearchType.Image:
                     hits = await search_future.result()
                     output_directory = constants.web_directory / "images"
                     # Collate results
```

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/routers/helpers.py` & `khoj_assistant-0.7.2.dev45/src/khoj/routers/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/routers/web_client.py` & `khoj_assistant-0.7.2.dev45/src/khoj/routers/web_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,36 @@
 
         current_config = json.loads(current_config.json())
 
         return templates.TemplateResponse(
             "content_type_github_input.html", context={"request": request, "current_config": current_config}
         )
 
+    @web_client.get("/config/content_type/notion", response_class=HTMLResponse)
+    def notion_config_page(request: Request):
+        default_copy = constants.default_config.copy()
+        default_notion = default_copy["content-type"]["notion"]  # type: ignore
+
+        default_config = TextContentConfig(
+            compressed_jsonl=default_notion["compressed-jsonl"],
+            embeddings_file=default_notion["embeddings-file"],
+        )
+
+        current_config = (
+            state.config.content_type.notion
+            if state.config and state.config.content_type and state.config.content_type.notion
+            else default_config
+        )
+
+        current_config = json.loads(current_config.json())
+
+        return templates.TemplateResponse(
+            "content_type_notion_input.html", context={"request": request, "current_config": current_config}
+        )
+
     @web_client.get("/config/content_type/{content_type}", response_class=HTMLResponse)
     def content_config_page(request: Request, content_type: str):
         if content_type not in VALID_TEXT_CONTENT_TYPES:
             return templates.TemplateResponse("config.html", context={"request": request})
 
         default_copy = constants.default_config.copy()
         default_content_type = default_copy["content-type"][content_type]  # type: ignore
```

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.7.2.dev45/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.7.2.dev45/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.7.2.dev45/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.7.2.dev45/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/search_type/image_search.py` & `khoj_assistant-0.7.2.dev45/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/search_type/text_search.py` & `khoj_assistant-0.7.2.dev45/src/khoj/search_type/text_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from khoj.search_filter.base_filter import BaseFilter
 
 # Internal Packages
 from khoj.utils import state
 from khoj.utils.helpers import get_absolute_path, is_none_or_empty, resolve_absolute_path, load_model, timer
 from khoj.utils.config import TextSearchModel
 from khoj.utils.models import BaseEncoder
-from khoj.utils.rawconfig import SearchResponse, TextSearchConfig, TextContentConfig, Entry
+from khoj.utils.rawconfig import SearchResponse, TextSearchConfig, TextConfigBase, Entry
 from khoj.utils.jsonl import load_jsonl
 
 
 logger = logging.getLogger(__name__)
 
 
 def initialize_model(search_config: TextSearchConfig):
@@ -155,24 +155,28 @@
 
 def collate_results(hits, entries: List[Entry], count=5) -> List[SearchResponse]:
     return [
         SearchResponse.parse_obj(
             {
                 "entry": entries[hit["corpus_id"]].raw,
                 "score": f"{hit.get('cross-score') or hit.get('score')}",
-                "additional": {"file": entries[hit["corpus_id"]].file, "compiled": entries[hit["corpus_id"]].compiled},
+                "additional": {
+                    "file": entries[hit["corpus_id"]].file,
+                    "compiled": entries[hit["corpus_id"]].compiled,
+                    "heading": entries[hit["corpus_id"]].heading,
+                },
             }
         )
         for hit in hits[0:count]
     ]
 
 
 def setup(
     text_to_jsonl: Type[TextToJsonl],
-    config: TextContentConfig,
+    config: TextConfigBase,
     search_config: TextSearchConfig,
     regenerate: bool,
     filters: List[BaseFilter] = [],
 ) -> TextSearchModel:
     # Initialize Model
     bi_encoder, cross_encoder, top_k = initialize_model(search_config)
 
@@ -182,15 +186,16 @@
         extract_entries(config.compressed_jsonl) if config.compressed_jsonl.exists() and not regenerate else None
     )
     entries_with_indices = text_to_jsonl(config).process(previous_entries or [])
 
     # Extract Updated Entries
     entries = extract_entries(config.compressed_jsonl)
     if is_none_or_empty(entries):
-        raise ValueError(f"No valid entries found in specified files: {config.input_files} or {config.input_filter}")
+        config_params = ", ".join([f"{key}={value}" for key, value in config.dict().items()])
+        raise ValueError(f"No valid entries found in specified files: {config_params}")
     top_k = min(len(entries), top_k)  # top_k hits can't be more than the total entries in corpus
 
     # Compute or Load Embeddings
     config.embeddings_file = resolve_absolute_path(config.embeddings_file)
     corpus_embeddings = compute_embeddings(
         entries_with_indices, bi_encoder, config.embeddings_file, regenerate=regenerate
     )
```

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/utils/cli.py` & `khoj_assistant-0.7.2.dev45/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/utils/config.py` & `khoj_assistant-0.7.2.dev45/src/khoj/utils/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # System Packages
 from __future__ import annotations  # to avoid quoting type hints
 from enum import Enum
 from dataclasses import dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, Dict, List
+from typing import TYPE_CHECKING, Dict, List, Union
 
 # External Packages
 import torch
 
 # Internal Packages
 if TYPE_CHECKING:
     from sentence_transformers import CrossEncoder
@@ -19,14 +19,15 @@
 class SearchType(str, Enum):
     All = "all"
     Org = "org"
     Markdown = "markdown"
     Image = "image"
     Pdf = "pdf"
     Github = "github"
+    Notion = "notion"
 
 
 class ProcessorType(str, Enum):
     Conversation = "conversation"
 
 
 class TextSearchModel:
@@ -54,28 +55,29 @@
         self.image_embeddings = image_embeddings
         self.image_metadata_embeddings = image_metadata_embeddings
         self.image_encoder = image_encoder
 
 
 @dataclass
 class SearchModels:
-    org_search: TextSearchModel = None
-    markdown_search: TextSearchModel = None
-    pdf_search: TextSearchModel = None
-    image_search: ImageSearchModel = None
-    github_search: TextSearchModel = None
-    plugin_search: Dict[str, TextSearchModel] = None
+    org_search: Union[TextSearchModel, None] = None
+    markdown_search: Union[TextSearchModel, None] = None
+    pdf_search: Union[TextSearchModel, None] = None
+    image_search: Union[ImageSearchModel, None] = None
+    github_search: Union[TextSearchModel, None] = None
+    notion_search: Union[TextSearchModel, None] = None
+    plugin_search: Union[Dict[str, TextSearchModel], None] = None
 
 
 class ConversationProcessorConfigModel:
     def __init__(self, processor_config: ConversationProcessorConfig):
         self.openai_api_key = processor_config.openai_api_key
         self.model = processor_config.model
         self.chat_model = processor_config.chat_model
         self.conversation_logfile = Path(processor_config.conversation_logfile)
         self.chat_session: List[str] = []
         self.meta_log: dict = {}
 
 
 @dataclass
 class ProcessorConfigModel:
-    conversation: ConversationProcessorConfigModel = None
+    conversation: Union[ConversationProcessorConfigModel, None] = None
```

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/utils/constants.py` & `khoj_assistant-0.7.2.dev45/src/khoj/utils/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,19 @@
         },
         "github": {
             "pat-token": None,
             "repos": [],
             "compressed-jsonl": "~/.khoj/content/github/github.jsonl.gz",
             "embeddings-file": "~/.khoj/content/github/github_embeddings.pt",
         },
+        "notion": {
+            "token": None,
+            "compressed-jsonl": "~/.khoj/content/notion/notion.jsonl.gz",
+            "embeddings-file": "~/.khoj/content/notion/notion_embeddings.pt",
+        },
     },
     "search-type": {
         "symmetric": {
             "encoder": "sentence-transformers/all-MiniLM-L6-v2",
             "cross-encoder": "cross-encoder/ms-marco-MiniLM-L-6-v2",
             "model_directory": "~/.khoj/search/symmetric/",
         },
```

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/utils/helpers.py` & `khoj_assistant-0.7.2.dev45/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/utils/jsonl.py` & `khoj_assistant-0.7.2.dev45/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/utils/models.py` & `khoj_assistant-0.7.2.dev45/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.7.2.dev45/src/khoj/utils/rawconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 
 
 class GithubContentConfig(TextConfigBase):
     pat_token: str
     repos: List[GithubRepoConfig]
 
 
+class NotionContentConfig(TextConfigBase):
+    token: str
+
+
 class ImageContentConfig(ConfigBase):
     input_directories: Optional[List[Path]]
     input_filter: Optional[List[str]]
     embeddings_file: Path
     use_xmp_metadata: bool
     batch_size: int
 
@@ -73,14 +77,15 @@
 class ContentConfig(ConfigBase):
     org: Optional[TextContentConfig]
     image: Optional[ImageContentConfig]
     markdown: Optional[TextContentConfig]
     pdf: Optional[TextContentConfig]
     github: Optional[GithubContentConfig]
     plugins: Optional[Dict[str, TextContentConfig]]
+    notion: Optional[NotionContentConfig]
 
 
 class TextSearchConfig(ConfigBase):
     encoder: str
     cross_encoder: str
     encoder_type: Optional[str]
     model_directory: Optional[Path]
@@ -144,8 +149,13 @@
         return json.dumps(self.__dict__, ensure_ascii=False)
 
     def __repr__(self) -> str:
         return self.__dict__.__repr__()
 
     @classmethod
     def from_dict(cls, dictionary: dict):
-        return cls(raw=dictionary["raw"], compiled=dictionary["compiled"], file=dictionary.get("file", None))
+        return cls(
+            raw=dictionary["raw"],
+            compiled=dictionary["compiled"],
+            file=dictionary.get("file", None),
+            heading=dictionary.get("heading", None),
+        )
```

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/utils/state.py` & `khoj_assistant-0.7.2.dev45/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/src/khoj/utils/yaml.py` & `khoj_assistant-0.7.2.dev45/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/.gitignore` & `khoj_assistant-0.7.2.dev45/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/LICENSE` & `khoj_assistant-0.7.2.dev45/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/README.md` & `khoj_assistant-0.7.2.dev45/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/pyproject.toml` & `khoj_assistant-0.7.2.dev45/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev44/PKG-INFO` & `khoj_assistant-0.7.2.dev45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.7.2.dev44
+Version: 0.7.2.dev45
 Summary: An AI personal assistant for your Digital Brain
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

