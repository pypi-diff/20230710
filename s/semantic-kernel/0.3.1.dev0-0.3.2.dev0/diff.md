# Comparing `tmp/semantic_kernel-0.3.1.dev0.tar.gz` & `tmp/semantic_kernel-0.3.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.3.1.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.3.2.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.3.1.dev0.tar` & `semantic_kernel-0.3.2.dev0.tar`

### file list

```diff
@@ -1,92 +1,96 @@
--rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.955726 semantic_kernel-0.3.1.dev0/pip/README.md
--rw-r--r--   0        0        0      927 2023-06-12 17:06:53.335469 semantic_kernel-0.3.1.dev0/pyproject.toml
--rw-r--r--   0        0        0     1227 2023-05-08 23:38:10.959435 semantic_kernel-0.3.1.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0      719 2023-05-25 17:48:21.153018 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.983569 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/ai_exception.py
--rw-r--r--   0        0        0     1792 2023-06-12 17:06:53.338448 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1235 2023-06-12 17:06:53.340338 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1405 2023-06-12 17:06:53.340916 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-30 18:57:02.986074 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      352 2023-04-30 18:57:02.986678 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     6161 2023-06-12 17:06:53.341797 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.960592 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      892 2023-04-30 18:57:02.988571 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.030156 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.032300 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.034473 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     8467 2023-06-12 17:06:53.342528 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     5504 2023-06-12 17:06:53.343178 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.041646 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1616 2023-06-12 17:06:53.344173 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      182 2023-05-18 17:32:52.334054 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    15268 2023-06-08 17:22:29.422161 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4402 2023-06-08 17:22:29.423786 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0    11295 2023-06-12 17:06:53.345249 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0      691 2023-05-19 18:06:11.089827 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.044314 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
--rw-r--r--   0        0        0     2072 2023-04-13 23:12:46.166679 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.780276 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/http_skill.py
--rw-r--r--   0        0        0     3164 2023-05-15 18:12:57.045974 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/math_skill.py
--rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.194344 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2403 2023-04-13 23:12:46.167467 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     7502 2023-06-08 17:22:29.425604 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0    27810 2023-06-12 17:06:53.346838 semantic_kernel-0.3.1.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     1626 2023-04-30 18:57:02.993735 semantic_kernel-0.3.1.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      160 2023-04-13 23:12:46.173418 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2544 2023-06-08 17:22:29.427355 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     3708 2023-06-08 17:22:29.428125 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     2014 2023-05-19 23:02:13.063945 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1272 2023-06-08 17:22:29.429766 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6295 2023-06-08 17:22:29.430728 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1298 2023-06-08 17:22:29.431397 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.047968 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.782347 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.199808 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.064609 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-13 23:12:46.179530 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.160748 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    15915 2023-05-08 23:26:29.698891 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.999492 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      158 2023-05-08 23:38:10.963774 semantic_kernel-0.3.1.dev0/semantic_kernel/planning/__init__.py
--rw-r--r--   0        0        0     7287 2023-05-25 17:48:21.156811 semantic_kernel-0.3.1.dev0/semantic_kernel/planning/basic_planner.py
--rw-r--r--   0        0        0      396 2023-05-08 23:26:29.700122 semantic_kernel-0.3.1.dev0/semantic_kernel/planning/plan.py
--rw-r--r--   0        0        0      932 2023-05-19 23:02:13.065230 semantic_kernel-0.3.1.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      694 2023-06-05 21:39:19.138269 semantic_kernel-0.3.1.dev0/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.182583 semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.203325 semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-13 23:12:46.183441 semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4525 2023-06-12 17:06:53.347832 semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-14 00:51:57.204455 semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-14 00:51:57.205241 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.205757 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     2199 2023-06-12 17:06:53.350203 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.206300 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.206885 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.207475 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-13 23:12:46.187552 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-14 00:51:57.208334 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.208951 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-13 23:12:46.188719 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.189034 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      830 2023-04-14 00:51:57.209567 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-14 00:51:57.210164 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000489 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.192355 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-13 23:12:46.192840 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.211524 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.193631 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.212261 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.194683 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.212967 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-13 23:12:46.195769 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.196165 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-13 23:12:46.196572 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.196999 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      473 2023-04-30 18:57:03.001133 semantic_kernel-0.3.1.dev0/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      667 2023-04-30 18:57:03.001562 semantic_kernel-0.3.1.dev0/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     6467 2023-05-15 18:12:57.049895 semantic_kernel-0.3.1.dev0/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      403 2023-04-13 23:12:46.197533 semantic_kernel-0.3.1.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     1643 2023-06-08 17:22:29.433328 semantic_kernel-0.3.1.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-13 23:12:46.198404 semantic_kernel-0.3.1.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.198764 semantic_kernel-0.3.1.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 semantic_kernel-0.3.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.000000 semantic_kernel-0.3.2.dev0/pip/README.md
+-rw-r--r--   0        0        0     1040 2023-07-10 20:42:43.199828 semantic_kernel-0.3.2.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1301 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0      719 2023-05-25 17:48:21.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0        0        0     1792 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1235 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1405 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-30 18:57:02.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      352 2023-04-30 18:57:02.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     6161 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      892 2023-04-30 18:57:02.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     8467 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     5504 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1616 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      182 2023-05-18 17:32:52.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    15268 2023-06-08 17:22:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4402 2023-06-08 17:22:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      190 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    14867 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0     1154 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0    11295 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0      691 2023-05-19 18:06:11.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
+-rw-r--r--   0        0        0     2082 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     3171 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/math_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2413 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     7860 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0      629 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/wait_skill.py
+-rw-r--r--   0        0        0    27810 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     1626 2023-04-30 18:57:02.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      160 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2544 2023-06-08 17:22:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     3708 2023-06-08 17:22:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     2014 2023-05-19 23:02:13.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1272 2023-06-08 17:22:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6354 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1298 2023-06-08 17:22:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    16088 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      158 2023-05-08 23:38:10.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/planning/__init__.py
+-rw-r--r--   0        0        0     7538 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/planning/basic_planner.py
+-rw-r--r--   0        0        0      396 2023-05-08 23:26:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/planning/plan.py
+-rw-r--r--   0        0        0      932 2023-05-19 23:02:13.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      694 2023-06-05 21:39:19.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4525 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     2199 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      830 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      473 2023-04-30 18:57:03.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-30 18:57:03.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8440 2023-07-10 20:40:59.227169 semantic_kernel-0.3.2.dev0/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      403 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2574 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 semantic_kernel-0.3.2.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.3.1.dev0/pip/README.md` & `semantic_kernel-0.3.2.dev0/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/pyproject.toml` & `semantic_kernel-0.3.2.dev0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.3.1.dev"
+version = "0.3.2.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.24.2"
 openai = "^0.27.0"
 aiofiles = "^23.1.0"
 python-dotenv = "1.0.0"
+regex = "^2023.6.3"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "2.21.0"
+pre-commit = "3.3.3"
 black = {version = "23.3.0", allow-prereleases = true}
 ipykernel = "^6.21.1"
-pytest = "7.2.0"
-ruff = "0.0.257"
+pytest = "7.4.0"
+ruff = "0.0.277"
 pytest-asyncio = "0.21.0"
 
-
 [tool.poetry.group.hugging_face.dependencies]
 transformers = "^4.28.1"
 sentence-transformers = "^2.2.2"
 torch = "2.0.0"
 
 [tool.poetry.group.chromadb.dependencies]
 chromadb = "^0.3.23"
 
 
 [tool.poetry.group.weaviate.dependencies]
 weaviate-client = "^3.18.0"
 
+[tool.poetry.group.pinecone.dependencies]
+pinecone-client = "^2.2.2"
+
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
+select = ["E", "F", "I"]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,21 +13,23 @@
 from semantic_kernel.semantic_functions.semantic_function_config import (
     SemanticFunctionConfig,
 )
 from semantic_kernel.utils.null_logger import NullLogger
 from semantic_kernel.utils.settings import (
     azure_openai_settings_from_dot_env,
     openai_settings_from_dot_env,
+    pinecone_settings_from_dot_env,
 )
 
 __all__ = [
     "Kernel",
     "NullLogger",
     "openai_settings_from_dot_env",
     "azure_openai_settings_from_dot_env",
+    "pinecone_settings_from_dot_env",
     "PromptTemplateConfig",
     "PromptTemplate",
     "ChatPromptTemplate",
     "SemanticFunctionConfig",
     "ContextVariables",
     "SKFunctionBase",
     "SKContext",
```

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/__init__.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/ai_exception.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/chat_request_settings.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/complete_request_settings.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/__init__.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/conversation_summary_skill.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/conversation_summary_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class FileIOSkill:
     """
     Description: Read and write from a file.
 
     Usage:
-        kernel.import_skill("file", FileIOSkill());
+        kernel.import_skill(FileIOSkill(), skill_name="file")
 
     Examples:
 
     {{file.readAsync $path }} => "hello world"
     {{file.writeAsync}}
     """
```

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/http_skill.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/http_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/math_skill.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/math_skill.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class MathSkill:
     """
     Description: MathSkill provides a set of functions to make Math calculations.
 
     Usage:
-        kernel.import_skill("math", new MathSkill())
+        kernel.import_skill(MathSkill(), skill_name="math")
 
     Examples:
         {{math.Add}}         => Returns the sum of initial_value_text and Amount (provided in the SKContext)
     """
 
     @sk_function(
         description="Adds value to a value",
```

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class TextSkill:
     """
     TextSkill provides a set of functions to manipulate strings.
 
     Usage:
-        kernel.import_skill("text", TextSkill());
+        kernel.import_skill(TextSkill(), skill_name="text")
 
     Examples:
         SKContext["input"] = "  hello world  "
         {{text.trim $input}} => "hello world"
 
         SKContext["input"] = "  hello world  "
         {{text.trimStart $input} => "hello world  "
```

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 
 class TimeSkill:
     """
     Description: TimeSkill provides a set of functions
                  to get the current time and date.
 
     Usage:
-        kernel.import_skill("time", TimeSkill())
+        kernel.import_skill(TimeSkill(), skill_name="time")
 
     Examples:
         {{time.date}}            => Sunday, 12 January, 2031
         {{time.today}}           => Sunday, 12 January, 2031
+        {{time.iso_date}}        => 2031-01-12
         {{time.now}}             => Sunday, January 12, 2031 9:15 PM
         {{time.utcNow}}          => Sunday, January 13, 2031 5:15 AM
         {{time.time}}            => 09:15:07 PM
         {{time.year}}            => 2031
         {{time.month}}           => January
         {{time.monthNumber}}     => 01
         {{time.day}}             => 12
@@ -51,14 +52,25 @@
         Get the current date
 
         Example:
             {{time.today}} => Sunday, 12 January, 2031
         """
         return self.date()
 
+    @sk_function(description="Get the current date in iso format.")
+    def iso_date(self) -> str:
+        """
+        Get the current date in iso format
+
+        Example:
+            {{time.iso_date}} => 2031-01-12
+        """
+        today = datetime.date.today()
+        return today.isoformat()
+
     @sk_function(description="Get the current date and time in the local time zone")
     def now(self) -> str:
         """
         Get the current date and time in the local time zone"
 
         Example:
             {{time.now}} => Sunday, January 12, 2031 9:15 PM
```

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,17 @@
         """
         # TODO: not the best place to create collection, but will address this behavior together with .NET SK
         if not await self._storage.does_collection_exist_async(
             collection_name=collection
         ):
             await self._storage.create_collection_async(collection_name=collection)
 
-        embedding = await self._embeddings_generator.generate_embeddings_async([text])
+        embedding = (
+            await self._embeddings_generator.generate_embeddings_async([text])
+        )[0]
         data = MemoryRecord.local_record(
             id=id,
             text=text,
             description=description,
             additional_metadata=additional_metadata,
             embedding=embedding,
         )
@@ -90,15 +92,17 @@
         """
         # TODO: not the best place to create collection, but will address this behavior together with .NET SK
         if not await self._storage.does_collection_exist_async(
             collection_name=collection
         ):
             await self._storage.create_collection_async(collection_name=collection)
 
-        embedding = await self._embeddings_generator.generate_embeddings_async([text])
+        embedding = (
+            await self._embeddings_generator.generate_embeddings_async([text])
+        )[0]
         data = MemoryRecord.reference_record(
             external_id=external_id,
             source_name=external_source_name,
             description=description,
             additional_metadata=additional_metadata,
             embedding=embedding,
         )
@@ -138,17 +142,17 @@
             limit {int} -- The maximum number of results to return. (default: {1})
             min_relevance_score {float} -- The minimum relevance score to return. (default: {0.0})
             with_embeddings {bool} -- Whether to return the embeddings of the results. (default: {False})
 
         Returns:
             List[MemoryQueryResult] -- The list of MemoryQueryResult found.
         """
-        query_embedding = await self._embeddings_generator.generate_embeddings_async(
-            [query]
-        )
+        query_embedding = (
+            await self._embeddings_generator.generate_embeddings_async([query])
+        )[0]
         results = await self._storage.get_nearest_matches_async(
             collection_name=collection,
             embedding=query_embedding,
             limit=limit,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embeddings,
         )
```

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import asyncio
+import platform
+import sys
 import threading
 from enum import Enum
 from logging import Logger
 from typing import Any, Callable, List, Optional, cast
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import (
     ChatCompletionClientBase,
@@ -32,14 +34,17 @@
 from semantic_kernel.skill_definition.function_view import FunctionView
 from semantic_kernel.skill_definition.parameter_view import ParameterView
 from semantic_kernel.skill_definition.read_only_skill_collection_base import (
     ReadOnlySkillCollectionBase,
 )
 from semantic_kernel.utils.null_logger import NullLogger
 
+if platform.system() == "Windows" and sys.version_info >= (3, 8, 0):
+    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+
 
 class SKFunction(SKFunctionBase):
     """
     Semantic Kernel function.
     """
 
     _parameters: List[ParameterView]
```

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/planning/basic_planner.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/planning/basic_planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 """A basic JSON-based planner for the Python Semantic Kernel"""
 import json
 
+import regex
+
 from semantic_kernel.kernel import Kernel
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.planning.plan import Plan
 
 PROMPT = """
 You are a planner for the Semantic Kernel.
 Your job is to create a properly formatted JSON plan step by step, to satisfy the goal given.
@@ -183,15 +185,21 @@
         return Plan(prompt=prompt, goal=goal, plan=generated_plan)
 
     async def execute_plan_async(self, plan: Plan, kernel: Kernel) -> str:
         """
         Given a plan, execute each of the functions within the plan
         from start to finish and output the result.
         """
-        generated_plan = json.loads(plan.generated_plan.result)
+
+        # Filter out good JSON from the result in case additional text is present
+        json_regex = r"\{(?:[^{}]|(?R))*\}"
+        generated_plan_string = regex.search(
+            json_regex, plan.generated_plan.result
+        ).group()
+        generated_plan = json.loads(generated_plan_string)
 
         context = ContextVariables()
         context["input"] = generated_plan["input"]
         subtasks = generated_plan["subtasks"]
 
         for subtask in subtasks:
             skill_name, function_name = subtask["function"].split(".")
```

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/utils/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from typing import Optional, Tuple
+
 from dotenv import dotenv_values
 
 
 def openai_settings_from_dot_env() -> Tuple[str, Optional[str]]:
     """
     Reads the OpenAI API key and organization ID from the .env file.
 
@@ -43,7 +44,35 @@
             deployment is not None
         ), "Azure OpenAI deployment name not found in .env file"
 
     assert api_key is not None, "Azure OpenAI API key not found in .env file"
     assert endpoint is not None, "Azure OpenAI endpoint not found in .env file"
 
     return deployment or "", api_key, endpoint
+
+
+def pinecone_settings_from_dot_env() -> Tuple[str, Optional[str]]:
+    """
+    Reads the Pinecone API key and Environment from the .env file.
+    Returns:
+        Tuple[str, str]: The Pinecone API key, the Pinecone Environment
+    """
+
+    api_key, environment = None, None
+    with open(".env", "r") as f:
+        lines = f.readlines()
+
+        for line in lines:
+            if line.startswith("PINECONE_API_KEY"):
+                parts = line.split("=")[1:]
+                api_key = "=".join(parts).strip().strip('"')
+                continue
+
+            if line.startswith("PINECONE_ENVIRONMENT"):
+                parts = line.split("=")[1:]
+                environment = "=".join(parts).strip().strip('"')
+                continue
+
+    assert api_key is not None, "Pinecone API key not found in .env file"
+    assert environment is not None, "Pinecone environment not found in .env file"
+
+    return api_key, environment
```

### Comparing `semantic_kernel-0.3.1.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.3.2.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.1.dev0/PKG-INFO` & `semantic_kernel-0.3.2.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.3.1.dev0
+Version: 0.3.2.dev0
 Summary: 
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: openai (>=0.27.0,<0.28.0)
 Requires-Dist: python-dotenv (==1.0.0)
+Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # About Semantic Kernel
 
 **Semantic Kernel (SK)** is a lightweight SDK enabling integration of AI Large
 Language Models (LLMs) with conventional programming languages. The SK
 extensible programming model combines natural language **semantic functions**,
```

