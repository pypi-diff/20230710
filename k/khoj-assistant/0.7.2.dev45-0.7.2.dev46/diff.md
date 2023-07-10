# Comparing `tmp/khoj_assistant-0.7.2.dev45.tar.gz` & `tmp/khoj_assistant-0.7.2.dev46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Jul  9 22:29:26 2023, max compression
+gzip compressed data, last modified: Mon Jul 10 05:31:37 2023, max compression
```

## Comparing `khoj_assistant-0.7.2.dev45.tar` & `khoj_assistant-0.7.2.dev46.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/__init__.py
--rw-r--r--   0        0        0    11624 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/configure.py
--rw-r--r--   0        0        0     5304 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1395 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3910 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    17875 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    16101 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6930 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     7322 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0     3401 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/content_type_notion_input.html
--rw-r--r--   0        0        0    19024 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3660 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1813 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0      549 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0   205167 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     1578 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/notion.svg
--rw-r--r--   0        0        0     7946 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4455 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     4824 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     3991 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     8304 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13517 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7454 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0     9295 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/notion/notion_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5397 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    20444 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/routers/api.py
--rw-r--r--   0        0        0      167 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     2895 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/routers/helpers.py
--rw-r--r--   0        0        0     5524 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7566 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11237 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2040 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2571 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2710 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6889 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4338 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/LICENSE
--rw-r--r--   0        0        0    24572 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/README.md
--rw-r--r--   0        0        0     2792 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/pyproject.toml
--rw-r--r--   0        0        0    26937 2023-07-09 22:29:26.000000 khoj_assistant-0.7.2.dev45/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/__init__.py
+-rw-r--r--   0        0        0    11624 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/configure.py
+-rw-r--r--   0        0        0     5304 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     5152 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    18248 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    16101 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6930 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     7322 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0     3401 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/content_type_notion_input.html
+-rw-r--r--   0        0        0    19406 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3660 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1921 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0      549 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0   205167 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     1578 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/notion.svg
+-rw-r--r--   0        0        0     7946 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4455 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     4824 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     3991 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     8304 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13517 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0     9295 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/notion/notion_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5397 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    20444 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/routers/api.py
+-rw-r--r--   0        0        0      167 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     2895 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/routers/helpers.py
+-rw-r--r--   0        0        0     5524 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7566 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11237 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2040 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2571 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2710 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6889 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4338 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/LICENSE
+-rw-r--r--   0        0        0    24572 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/README.md
+-rw-r--r--   0        0        0     2792 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/pyproject.toml
+-rw-r--r--   0        0        0    26937 2023-07-10 05:31:37.000000 khoj_assistant-0.7.2.dev46/PKG-INFO
```

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/configure.py` & `khoj_assistant-0.7.2.dev46/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/main.py` & `khoj_assistant-0.7.2.dev46/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/404.html` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/base_config.html`

 * *Files 24% similar despite different names*

```diff
@@ -5,33 +5,74 @@
         <meta name="viewport" content="width=device-width, initial-scale=1.0 maximum-scale=1.0">
         <link rel="icon" type="image/png" sizes="128x128" href="/static/assets/icons/favicon-128x128.png">
         <title>Khoj - Settings</title>
         <link rel="stylesheet" href="/static/assets/pico.min.css">
         <link rel="stylesheet" href="/static/assets/khoj.css">
     </head>
     <body class="khoj-configure">
-        <div class="khoj-header">
-            <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
-            <nav class="khoj-nav">
-                <a href="/chat">Chat</a>
-                <a href="/">Search</a>
-                <a class="khoj-nav-selected" href="/config">Settings</a>
-            </nav>
+        <div class="khoj-header-wrapper">
+            <div class="filler"></div>
+            <div class="khoj-header">
+                <a class="khoj-logo" href="https://lantern.khoj.dev" target="_blank">
+                    <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
+                </a>
+                <nav class="khoj-nav">
+                    <a class="khoj-nav" href="/chat">Chat</a>
+                    <a class="khoj-nav" href="/">Search</a>
+                    <a class="khoj-nav khoj-nav-selected" href="/config">Settings</a>
+                </nav>
+            </div>
+            <div class="filler"></div>
         </div>
         <div class=”content”>
             {% block content %}
             {% endblock %}
         </div>
     </body>
     <style>
         html, body {
             width: 100%;
             margin: 0;
             padding: 0;
         }
+        @media only screen and (max-width: 600px) {
+            body {
+                display: grid;
+                grid-template-columns: 1fr;
+                grid-template-rows: 1fr auto auto auto minmax(80px, 100%);
+            }
+            body > * {
+                grid-column: 1;
+            }
+
+            div.filler {
+                display: none;
+            }
+
+            div.khoj-header {
+                display: grid;
+                grid-template-columns: 1fr 1fr;
+                padding: 0;
+                margin-bottom: 8px;
+                margin-top: 8px;
+                padding-top: 8px;
+            }
+
+            body.khoj-configure {
+                padding: 0;
+            }
+        }
+
+        img.khoj-logo {
+            max-width: none!important;
+        }
+        div.khoj-header-wrapper{
+            display: grid;
+            grid-template-columns: 1fr min(70vw, 100%) 1fr;
+        }
         .page {
             display: grid;
             grid-auto-flow: row;
             gap: 32px;
         }
         .section {
             display: grid;
```

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/chat.html` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/chat.html`

 * *Files 1% similar despite different names*

```diff
@@ -177,27 +177,27 @@
                         </p>
                     </a>
                     <input type="text" id="khoj-banner-email" placeholder="email" class="khoj-banner-email"></input>
                     <button id="khoj-banner-submit" class="khoj-banner-button">Submit</button>
                 </div>
             {% endif %}
             {% if demo %}
-                <a href="https://khoj.dev" target="_blank">
+                <a class="khoj-logo" href="https://khoj.dev" target="_blank">
                     <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
                 </a>
             {% else %}
-                <a href="https://lantern.khoj.dev" target="_blank">
+                <a class="khoj-logo" href="https://lantern.khoj.dev" target="_blank">
                     <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
                 </a>
             {% endif %}
             <nav class="khoj-nav">
-                <a class="khoj-nav-selected" href="/chat">Chat</a>
-                <a href="/">Search</a>
+                <a class="khoj-nav khoj-nav-selected" href="/chat">Chat</a>
+                <a class="khoj-nav" href="/">Search</a>
                 {% if not demo %}
-                    <a href="/config">Settings</a>
+                    <a class="khoj-nav" href="/config">Settings</a>
                 {% endif %}
             </nav>
         </div>
 
         <!-- Chat Body -->
         <div id="chat-body"></div>
 
@@ -360,14 +360,26 @@
                 padding: 0;
                 margin: 4px;
                 grid-template-columns: auto;
             }
             a.khoj-banner {
                 display: block;
             }
+
+            div.khoj-header {
+                display: grid;
+                grid-template-columns: 1fr 1fr;
+                padding: 0;
+                margin-bottom: 8px;
+                margin-top: 8px;
+            }
+
+            nav.khoj-nav {
+                grid-gap: 0px;
+            }
         }
         @media only screen and (min-width: 600px) {
             body {
                 grid-template-columns: auto min(70vw, 100%) auto;
                 grid-template-rows: auto minmax(80px, 100%) auto;
             }
             body > * {
```

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/config.html` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/content_type_notion_input.html` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/content_type_notion_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/index.html` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -234,18 +234,18 @@
                 </a>
             {% else %}
                 <a class="khoj-logo" href="https://lantern.khoj.dev" target="_blank">
                     <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
                 </a>
             {% endif %}
             <nav class="khoj-nav">
-                <a href="/chat">Chat</a>
-                <a class="khoj-nav-selected" href="/">Search</a>
+                <a class="khoj-nav" href="/chat">Chat</a>
+                <a class="khoj-nav khoj-nav-selected" href="/">Search</a>
                 {% if not demo %}
-                    <a href="/config">Settings</a>
+                    <a class="khoj-nav" href="/config">Settings</a>
                 {% endif %}
             </nav>
         </div>
 
         <!--Add Text Box To Enter Query, Trigger Incremental Search OnChange -->
         <input type="text" id="query" class="option" onkeyup=incrementalSearch(event) autofocus="autofocus" placeholder="What is the meaning of life?">
 
@@ -266,18 +266,32 @@
 
     <style>
         @media only screen and (max-width: 600px) {
             body {
                 display: grid;
                 grid-template-columns: 1fr;
                 grid-template-rows: 1fr auto auto auto minmax(80px, 100%);
+                font-size: small!important;
             }
             body > * {
                 grid-column: 1;
             }
+
+            div.khoj-header {
+                display: grid;
+                grid-template-columns: 1fr 1fr;
+                padding: 0;
+                margin-bottom: 8px;
+                margin-top: 8px;
+            }
+
+            nav.khoj-nav {
+                grid-gap: 0px;
+            }
+
         }
         @media only screen and (min-width: 600px) {
             body {
                 display: grid;
                 grid-template-columns: 1fr min(70vw, 100%) 1fr;
                 grid-template-rows: 1fr auto auto auto minmax(80px, 100%);
                 padding-top: 60vw;
```

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/khoj.css`

 * *Files 6% similar despite different names*

```diff
@@ -37,25 +37,36 @@
 .khoj-configure {
     display: grid;
     grid-template-columns: 1fr;
     padding: 0 24px;
 }
 .khoj-header {
     display: grid;
-    grid-auto-flow: row;
+    grid-auto-flow: column;
     gap: 20px;
     padding: 16px 0;
     margin: 0 0 16px 0;
 }
-.khoj-nav {
+
+nav.khoj-nav {
     display: grid;
     grid-auto-flow: column;
     grid-gap: 32px;
-    justify-self: center;
+    justify-self: right;
+}
+
+a.khoj-nav {
+    display: flex;
+    align-items: center;
+}
+
+a.khoj-logo {
+    justify-self: left;
 }
+
 .khoj-nav a {
     color: #333;
     text-decoration: none;
     font-size: 20px;
     font-weight: normal;
     padding: 8px;
     border-radius: 4px;
@@ -64,10 +75,10 @@
 .khoj-nav a:hover {
     background-color: var(--primary-hover);
 }
 .khoj-nav-selected {
     background-color: var(--primary);
 }
 img.khoj-logo {
-    width: min(60vw, 150px);
+    width: min(60vw, 100px);
     justify-self: center;
 }
```

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/notion.svg` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/notion.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.7.2.dev46/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.7.2.dev46/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.7.2.dev46/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.7.2.dev46/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.7.2.dev46/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.7.2.dev46/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/processor/notion/notion_to_jsonl.py` & `khoj_assistant-0.7.2.dev46/src/khoj/processor/notion/notion_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.7.2.dev46/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.7.2.dev46/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.7.2.dev46/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/routers/api.py` & `khoj_assistant-0.7.2.dev46/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/routers/helpers.py` & `khoj_assistant-0.7.2.dev46/src/khoj/routers/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/routers/web_client.py` & `khoj_assistant-0.7.2.dev46/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.7.2.dev46/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.7.2.dev46/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.7.2.dev46/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.7.2.dev46/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/search_type/image_search.py` & `khoj_assistant-0.7.2.dev46/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/search_type/text_search.py` & `khoj_assistant-0.7.2.dev46/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/utils/cli.py` & `khoj_assistant-0.7.2.dev46/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/utils/config.py` & `khoj_assistant-0.7.2.dev46/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/utils/constants.py` & `khoj_assistant-0.7.2.dev46/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/utils/helpers.py` & `khoj_assistant-0.7.2.dev46/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/utils/jsonl.py` & `khoj_assistant-0.7.2.dev46/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/utils/models.py` & `khoj_assistant-0.7.2.dev46/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.7.2.dev46/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/utils/state.py` & `khoj_assistant-0.7.2.dev46/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/src/khoj/utils/yaml.py` & `khoj_assistant-0.7.2.dev46/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/.gitignore` & `khoj_assistant-0.7.2.dev46/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/LICENSE` & `khoj_assistant-0.7.2.dev46/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/README.md` & `khoj_assistant-0.7.2.dev46/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/pyproject.toml` & `khoj_assistant-0.7.2.dev46/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev45/PKG-INFO` & `khoj_assistant-0.7.2.dev46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.7.2.dev45
+Version: 0.7.2.dev46
 Summary: An AI personal assistant for your Digital Brain
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

