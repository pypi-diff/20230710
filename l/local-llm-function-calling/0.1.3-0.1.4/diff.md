# Comparing `tmp/local_llm_function_calling-0.1.3.tar.gz` & `tmp/local_llm_function_calling-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_llm_function_calling-0.1.3.tar", max compression
+gzip compressed data, was "local_llm_function_calling-0.1.4.tar", max compression
```

## Comparing `local_llm_function_calling-0.1.3.tar` & `local_llm_function_calling-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     3105 2023-06-27 19:54:06.411406 local_llm_function_calling-0.1.3/README.md
--rw-r--r--   0        0        0      555 2023-06-27 19:57:49.091938 local_llm_function_calling-0.1.3/local_llm_function_calling/__init__.py
--rw-r--r--   0        0        0     5386 2023-06-27 19:57:39.016004 local_llm_function_calling-0.1.3/local_llm_function_calling/constrainer.py
--rw-r--r--   0        0        0     5256 2023-06-27 19:57:01.459251 local_llm_function_calling-0.1.3/local_llm_function_calling/generator.py
--rw-r--r--   0        0        0     3950 2023-06-27 09:38:19.333497 local_llm_function_calling-0.1.3/local_llm_function_calling/prompter.py
--rw-r--r--   0        0        0      433 2023-07-01 10:56:36.554955 local_llm_function_calling-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3566 1970-01-01 00:00:00.000000 local_llm_function_calling-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-10 14:03:26.088229 local_llm_function_calling-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3418 2023-07-10 13:45:59.047336 local_llm_function_calling-0.1.4/README.md
+-rw-r--r--   0        0        0      555 2023-06-27 19:57:49.091938 local_llm_function_calling-0.1.4/local_llm_function_calling/__init__.py
+-rw-r--r--   0        0        0     5386 2023-06-27 19:57:39.016004 local_llm_function_calling-0.1.4/local_llm_function_calling/constrainer.py
+-rw-r--r--   0        0        0     5256 2023-06-27 19:57:01.459251 local_llm_function_calling-0.1.4/local_llm_function_calling/generator.py
+-rw-r--r--   0        0        0     3950 2023-06-27 09:38:19.333497 local_llm_function_calling-0.1.4/local_llm_function_calling/prompter.py
+-rw-r--r--   0        0        0      750 2023-07-10 14:03:37.311295 local_llm_function_calling-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4235 1970-01-01 00:00:00.000000 local_llm_function_calling-0.1.4/PKG-INFO
```

### Comparing `local_llm_function_calling-0.1.3/README.md` & `local_llm_function_calling-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Local LLM function calling
 
+[![Documentation Status](https://readthedocs.org/projects/local-llm-function-calling/badge/?version=latest)](https://local-llm-function-calling.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/local-llm-function-calling.svg)](https://badge.fury.io/py/local-llm-function-calling)
+
 ## Overview
 
 The `local-llm-function-calling` project is designed to constrain the generation of Hugging Face text generation models by enforcing a JSON schema and facilitating the formulation of prompts for function calls, similar to OpenAI's [function calling](https://openai.com/blog/function-calling-and-other-api-updates) feature, but actually enforcing the schema unlike OpenAI.
 
 The project provides a `Generator` class that allows users to easily generate text while ensuring compliance with the provided prompt and JSON schema. By utilizing the `local-llm-function-calling` library, users can conveniently control the output of text generation models. It uses my own quickly sketched `json-schema-enforcer` project as the enforcer.
 
 ## Features
```

### Comparing `local_llm_function_calling-0.1.3/local_llm_function_calling/__init__.py` & `local_llm_function_calling-0.1.4/local_llm_function_calling/__init__.py`

 * *Files identical despite different names*

### Comparing `local_llm_function_calling-0.1.3/local_llm_function_calling/constrainer.py` & `local_llm_function_calling-0.1.4/local_llm_function_calling/constrainer.py`

 * *Files identical despite different names*

### Comparing `local_llm_function_calling-0.1.3/local_llm_function_calling/generator.py` & `local_llm_function_calling-0.1.4/local_llm_function_calling/generator.py`

 * *Files identical despite different names*

### Comparing `local_llm_function_calling-0.1.3/local_llm_function_calling/prompter.py` & `local_llm_function_calling-0.1.4/local_llm_function_calling/prompter.py`

 * *Files identical despite different names*

### Comparing `local_llm_function_calling-0.1.3/PKG-INFO` & `local_llm_function_calling-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 Metadata-Version: 2.1
 Name: local-llm-function-calling
-Version: 0.1.3
-Summary: 
+Version: 0.1.4
+Summary: A tool for generating function arguments and choosing what function to call with local LLMs
+Home-page: https://github.com/rizerphe/local-llm-function-calling
+License: MIT
+Keywords: llm,jsonschema,huggingface,transformers,local
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: json-schema-enforcer (>=0.1.3,<0.2.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: transformers (>=4.30.2,<5.0.0)
+Project-URL: Documentation, https://local-llm-function-calling.readthedocs.io/
 Description-Content-Type: text/markdown
 
 # Local LLM function calling
 
+[![Documentation Status](https://readthedocs.org/projects/local-llm-function-calling/badge/?version=latest)](https://local-llm-function-calling.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/local-llm-function-calling.svg)](https://badge.fury.io/py/local-llm-function-calling)
+
 ## Overview
 
 The `local-llm-function-calling` project is designed to constrain the generation of Hugging Face text generation models by enforcing a JSON schema and facilitating the formulation of prompts for function calls, similar to OpenAI's [function calling](https://openai.com/blog/function-calling-and-other-api-updates) feature, but actually enforcing the schema unlike OpenAI.
 
 The project provides a `Generator` class that allows users to easily generate text while ensuring compliance with the provided prompt and JSON schema. By utilizing the `local-llm-function-calling` library, users can conveniently control the output of text generation models. It uses my own quickly sketched `json-schema-enforcer` project as the enforcer.
 
 ## Features
```

