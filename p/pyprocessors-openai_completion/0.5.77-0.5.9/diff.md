# Comparing `tmp/pyprocessors_openai_completion-0.5.77.tar.gz` & `tmp/pyprocessors-openai_completion-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors_openai_completion-0.5.77.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyprocessors-openai_completion-0.5.9.tar", last modified: Wed Feb 15 16:28:15 2023, max compression
```

## Comparing `pyprocessors_openai_completion-0.5.77.tar` & `pyprocessors-openai_completion-0.5.9.tar`

### file list

```diff
@@ -1,35 +1,14 @@
--rw-r--r--   0        0        0       97 2023-06-07 12:04:27.485906 pyprocessors_openai_completion-0.5.77/.dockerignore
--rw-r--r--   0        0        0      147 2023-06-07 12:04:27.486906 pyprocessors_openai_completion-0.5.77/.gitignore
--rw-r--r--   0        0        0      448 2023-06-07 12:04:27.487906 pyprocessors_openai_completion-0.5.77/Dockerfile
--rw-r--r--   0        0        0    10227 2023-06-07 12:04:27.488906 pyprocessors_openai_completion-0.5.77/Jenkinsfile
--rw-r--r--   0        0        0      380 2023-06-07 12:04:27.489906 pyprocessors_openai_completion-0.5.77/README.md
--rw-r--r--   0        0        0     1559 2023-06-07 12:04:27.490906 pyprocessors_openai_completion-0.5.77/bumpversion.py
--rw-r--r--   0        0        0       56 2023-07-10 10:11:14.190472 pyprocessors_openai_completion-0.5.77/pyprocessors_openai_completion/__init__.py
--rw-r--r--   0        0        0    12287 2023-07-10 10:08:41.551112 pyprocessors_openai_completion-0.5.77/pyprocessors_openai_completion/openai_completion.py
--rw-r--r--   0        0        0     1923 2023-06-07 12:04:27.493906 pyprocessors_openai_completion-0.5.77/pyprocessors_openai_completion/retry_limit.py
--rw-r--r--   0        0        0     2594 2023-06-07 12:04:27.494906 pyprocessors_openai_completion-0.5.77/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 12:04:27.494906 pyprocessors_openai_completion-0.5.77/tests/__init__.py
--rw-r--r--   0        0        0      674 2023-06-07 12:04:27.496906 pyprocessors_openai_completion-0.5.77/tests/data/complexdoc.json
--rw-r--r--   0        0        0     3992 2023-06-07 12:04:27.498906 pyprocessors_openai_completion-0.5.77/tests/data/en_davinci-instruct-beta.json
--rw-r--r--   0        0        0     4868 2023-06-07 12:04:27.498906 pyprocessors_openai_completion-0.5.77/tests/data/en_gpt-3.5-turbo.json
--rw-r--r--   0        0        0     4716 2023-06-07 12:04:27.499906 pyprocessors_openai_completion-0.5.77/tests/data/en_gpt-4.json
--rw-r--r--   0        0        0     4141 2023-06-07 12:04:27.500906 pyprocessors_openai_completion-0.5.77/tests/data/en_text-ada-001.json
--rw-r--r--   0        0        0     3914 2023-06-07 12:04:27.500906 pyprocessors_openai_completion-0.5.77/tests/data/en_text-babbage-001.json
--rw-r--r--   0        0        0     4187 2023-06-07 12:04:27.501906 pyprocessors_openai_completion-0.5.77/tests/data/en_text-curie-001.json
--rw-r--r--   0        0        0     4182 2023-06-07 12:04:27.502906 pyprocessors_openai_completion-0.5.77/tests/data/en_text-davinci-003.json
--rw-r--r--   0        0        0     2202 2023-06-07 12:04:27.502906 pyprocessors_openai_completion-0.5.77/tests/data/fr_davinci-instruct-beta.json
--rw-r--r--   0        0        0     3207 2023-06-07 12:04:27.503907 pyprocessors_openai_completion-0.5.77/tests/data/fr_gpt-3.5-turbo.json
--rw-r--r--   0        0        0     2560 2023-06-07 12:04:27.504907 pyprocessors_openai_completion-0.5.77/tests/data/fr_gpt-4.json
--rw-r--r--   0        0        0     2295 2023-06-07 12:04:27.505906 pyprocessors_openai_completion-0.5.77/tests/data/fr_text-ada-001.json
--rw-r--r--   0        0        0     1699 2023-06-07 12:04:27.506907 pyprocessors_openai_completion-0.5.77/tests/data/fr_text-babbage-001.json
--rw-r--r--   0        0        0     1823 2023-06-07 12:04:27.506907 pyprocessors_openai_completion-0.5.77/tests/data/fr_text-curie-001.json
--rw-r--r--   0        0        0     2366 2023-06-07 12:04:27.507907 pyprocessors_openai_completion-0.5.77/tests/data/fr_text-davinci-003.json
--rw-r--r--   0        0        0     8421 2023-06-07 12:04:27.508907 pyprocessors_openai_completion-0.5.77/tests/data/jinjadocs.json
--rw-r--r--   0        0        0    13529 2023-06-07 12:04:27.508907 pyprocessors_openai_completion-0.5.77/tests/data/jinjadocs_preserve_entities.json
--rw-r--r--   0        0        0    14427 2023-06-07 12:04:27.509907 pyprocessors_openai_completion-0.5.77/tests/data/jinjadocs_substitute_entities.json
--rw-r--r--   0        0        0     5070 2023-06-07 12:04:27.510907 pyprocessors_openai_completion-0.5.77/tests/data/question_segments.json
--rw-r--r--   0        0        0     1219 2023-06-07 12:04:27.510907 pyprocessors_openai_completion-0.5.77/tests/data/question_segments_answer.json
--rw-r--r--   0        0        0    10702 2023-06-07 12:19:46.483369 pyprocessors_openai_completion-0.5.77/tests/test_openai_completion.py
--rw-r--r--   0        0        0      951 2023-06-07 12:04:27.512907 pyprocessors_openai_completion-0.5.77/tox.ini
--rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 pyprocessors_openai_completion-0.5.77/setup.py
--rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 pyprocessors_openai_completion-0.5.77/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-02-15 15:56:35.737007 pyprocessors-openai_completion-0.5.9/.dockerignore
+-rw-r--r--   0        0        0      147 2023-02-15 15:56:35.738007 pyprocessors-openai_completion-0.5.9/.gitignore
+-rw-r--r--   0        0        0      448 2023-02-15 15:56:35.739007 pyprocessors-openai_completion-0.5.9/Dockerfile
+-rw-r--r--   0        0        0    10227 2023-02-15 16:21:10.683489 pyprocessors-openai_completion-0.5.9/Jenkinsfile
+-rw-r--r--   0        0        0      380 2023-02-15 15:56:35.741007 pyprocessors-openai_completion-0.5.9/README.md
+-rw-r--r--   0        0        0     1559 2023-02-15 15:56:35.742007 pyprocessors-openai_completion-0.5.9/bumpversion.py
+-rw-r--r--   0        0        0       55 2023-02-15 16:28:13.706505 pyprocessors-openai_completion-0.5.9/pyprocessors_openai_completion/__init__.py
+-rw-r--r--   0        0        0     8400 2023-02-15 16:25:55.699911 pyprocessors-openai_completion-0.5.9/pyprocessors_openai_completion/openai_completion.py
+-rw-r--r--   0        0        0     2556 2023-02-15 15:56:35.744007 pyprocessors-openai_completion-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-15 15:56:35.745007 pyprocessors-openai_completion-0.5.9/tests/__init__.py
+-rw-r--r--   0        0        0     5320 2023-02-15 16:15:56.148298 pyprocessors-openai_completion-0.5.9/tests/test_openai_completion.py
+-rw-r--r--   0        0        0      951 2023-02-15 16:25:55.699911 pyprocessors-openai_completion-0.5.9/tox.ini
+-rw-r--r--   0        0        0     1309 1970-01-01 00:00:00.000000 pyprocessors-openai_completion-0.5.9/setup.py
+-rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 pyprocessors-openai_completion-0.5.9/PKG-INFO
```

### Comparing `pyprocessors_openai_completion-0.5.77/Jenkinsfile` & `pyprocessors-openai_completion-0.5.9/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.77/bumpversion.py` & `pyprocessors-openai_completion-0.5.9/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.77/pyprocessors_openai_completion/openai_completion.py` & `pyprocessors-openai_completion-0.5.9/pyprocessors_openai_completion/openai_completion.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,282 +1,185 @@
-import inspect
+import collections
 import os
 from enum import Enum
 from functools import lru_cache
 from string import Template
 from typing import List, cast, Type
 
-import jinja2
 import openai
 from pydantic import Field, BaseModel
+from pymultirole_plugins.util import comma_separated_to_list
 from pymultirole_plugins.v1.processor import ProcessorParameters, ProcessorBase
 from pymultirole_plugins.v1.schema import Document, AltText
 
-from .retry_limit import api_retry
-
 
 class OpenAIModel(str, Enum):
-    gpt_4 = "gpt-4"
-    gpt_3_5_turbo = "gpt-3.5-turbo"
+    davinci_instruct_beta = "davinci-instruct-beta"
     text_davinci_003 = "text-davinci-003"
     text_curie_001 = "text-curie-001"
     text_babbage_001 = "text-babbage-001"
     text_ada_001 = "text-ada-001"
-    davinci_instruct_beta = "davinci-instruct-beta"
-
-
-class TemplateLanguage(str, Enum):
-    none = "none"
-    string = "string"
-    jinja2 = "jinja2"
 
 
 class OpenAICompletionParameters(ProcessorParameters):
     model: OpenAIModel = Field(
-        OpenAIModel.gpt_3_5_turbo,
-        description="""The [OpenAI model](https://platform.openai.com/docs/models) used for completion. Options currently available:</br>
-                        <li>`gpt_4` - More capable than any GPT-3.5 model, able to do more complex tasks, and optimized for chat. Will be updated with our latest model iteration.
-                        <li>`gpt-3.5-turbo` - Most capable GPT-3.5 model and optimized for chat at 1/10th the cost of text-davinci-003. Will be updated with our latest model iteration.
+        OpenAIModel.davinci_instruct_beta,
+        description="""The [OpenAI model](https://help.openai.com/en/articles/5832130-what-s-changed-with-engine-names-and-best-practices) used for completion. Options currently available:</br>
+                        <li>`davinci-instruct-beta` - older Instruct GPT-3 model
                         <li>`text-davinci-003` - Most capable GPT-3 model. Can do any task the other models can do, often with higher quality, longer output and better instruction-following.
                         <li>`text-curie-001` - Very capable, but faster and lower cost than Davinci.
                         <li>`text-babbage-001` - Capable of straightforward tasks, very fast, and lower cost.
                         <li>`text-ada-001` - Capable of very simple tasks, usually the fastest model in the GPT-3 series, and lowest cost.
-                        <li>`davinci-instruct-beta` - older Instruct GPT-3 model.
                         """,
     )
     max_tokens: int = Field(
         256,
         description="""The maximum number of tokens to generate in the completion.
     The token count of your prompt plus max_tokens cannot exceed the model's context length.
     Most models have a context length of 2048 tokens (except for the newest models, which support 4096).""",
     )
     temperature: float = Field(
         1.0,
         description="""What sampling temperature to use, between 0 and 2.
     Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic.
     We generally recommend altering this or `top_p` but not both.""",
-        extra="advanced",
     )
     top_p: int = Field(
         1,
         description="""An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass.
     So 0.1 means only the tokens comprising the top 10% probability mass are considered.
     We generally recommend altering this or `temperature` but not both.""",
-        extra="advanced",
     )
     n: int = Field(
         1,
         description="""How many completions to generate for each prompt.
     Note: Because this parameter generates many completions, it can quickly consume your token quota.
     Use carefully and ensure that you have reasonable settings for `max_tokens`.""",
-        extra="advanced",
     )
     best_of: int = Field(
         1,
         description="""Generates best_of completions server-side and returns the "best" (the one with the highest log probability per token).
     Results cannot be streamed.
     When used with `n`, `best_of` controls the number of candidate completions and `n` specifies how many to return – `best_of` must be greater than `n`.
     Use carefully and ensure that you have reasonable settings for `max_tokens`.""",
-        extra="advanced",
     )
     presence_penalty: float = Field(
         0.0,
         description="""Number between -2.0 and 2.0.
     Positive values penalize new tokens based on whether they appear in the text so far, increasing the model's likelihood to talk about new topics.""",
-        extra="advanced",
     )
     frequency_penalty: float = Field(
         0.0,
         description="""Number between -2.0 and 2.0.
     Positive values penalize new tokens based on their existing frequency in the text so far, decreasing the model's likelihood to repeat the same line verbatim.""",
-        extra="advanced",
     )
-    prompt: str = Field(
-        "$text",
-        description="""Contains the prompt as a template string, templates can be:
-         <li>a simple (python template string)[https://docs.python.org/3/library/string.html#template-strings]<br/>
-         where the document elements can be substituted using `$based`-syntax<br/>
-         `$text` to be substituted by the document text<br/>
-         `$title` to be substituted by the document title
-         <li>a more complex (jinja2 template)[https://jinja.palletsprojects.com/en/3.1.x/]
-         where the document is injected as `doc` and can be used in jinja2 variables like<br/>
-         `{{ doc.text }}` to be substituted by the document text etc...""",
-        extra="multiline",
+    prompt_altText: str = Field(
+        None,
+        description="""<li>If defined: contains the prompt as an alternative text of the input document (can be a template string containing `$text` to be substituted by the document text),
+        <li>if not takes the text of the input document as prompt.""",
     )
     completion_altText: str = Field(
         None,
         description="""<li>If defined: generates the completion as an alternative text of the input document,
     <li>if not: replace the text of the input document.""",
     )
 
 
-# SUPPORTED_LANGUAGES = "de,en,es,fr,it,nl,pt"
+SUPPORTED_LANGUAGES = "de,en,es,fr,it,nl,pt"
 
 
 # noqa: E501
 class OpenAICompletionProcessor(ProcessorBase):
     __doc__ = """Generate text using [OpenAI Text Completion](https://platform.openai.com/docs/guides/completion) API
-    You input some text as a prompt, and the model will generate a text completion that attempts to match whatever context or pattern you gave it."""
+    You input some text as a prompt, and the model will generate a text completion that attempts to match whatever context or pattern you gave it.
+    #languages:""" + SUPPORTED_LANGUAGES
 
     def process(
-        self, documents: List[Document], parameters: ProcessorParameters
+            self, documents: List[Document], parameters: ProcessorParameters
     ) -> List[Document]:
-        # supported_languages = comma_separated_to_list(SUPPORTED_LANGUAGES)
+        supported_languages = comma_separated_to_list(SUPPORTED_LANGUAGES)
         openai = get_openai()
         params: OpenAICompletionParameters = cast(
             OpenAICompletionParameters, parameters
         )
         try:
-            templ, prompt_templ = get_template(params)
 
             for document in documents:
-                # lang = document_language(document, None)
-                # if lang is None or lang not in supported_languages:
-                #     raise AttributeError(
-                #         f"Metadata language {lang} is required and must be in {SUPPORTED_LANGUAGES}"
-                #     )
+                lang = document_language(document, None)
+                if lang is None or lang not in supported_languages:
+                    raise AttributeError(
+                        f"Metadata language {lang} is required and must be in {SUPPORTED_LANGUAGES}"
+                    )
                 altTexts = document.altTexts or []
-
-                if templ == TemplateLanguage.string:
-                    flatten_doc = flatten_document(document)
-                    prompt = prompt_templ.safe_substitute(flatten_doc)
-                elif templ == TemplateLanguage.jinja2:
-                    prompt = prompt_templ.render(doc=document)
-                else:
-                    prompt = prompt_templ
-
-                if params.model in [OpenAIModel.gpt_4, OpenAIModel.gpt_3_5_turbo]:
-                    response = openai_chat_completion(openai,
-                                                      model=params.model.value,
-                                                      messages=[{"role": "user", "content": prompt}],
-                                                      max_tokens=params.max_tokens,
-                                                      temperature=params.temperature,
-                                                      top_p=params.top_p,
-                                                      n=params.n,
-                                                      frequency_penalty=params.frequency_penalty,
-                                                      presence_penalty=params.presence_penalty,
-                                                      )
-                    completion = "\n".join(
-                        r.message["content"] for r in response["choices"]
+                prompt = document.text
+                if params.prompt_altText is not None and len(
+                        params.prompt_altText.strip()
+                ):
+                    prompt_altText = next(
+                        (
+                            alt
+                            for alt in altTexts
+                            if alt.name == params.prompt_altText.strip()
+                        ),
+                        None,
                     )
-                else:
-                    response = openai_completion(openai,
-                                                 model=params.model.value,
-                                                 prompt=prompt,
-                                                 max_tokens=params.max_tokens,
-                                                 temperature=params.temperature,
-                                                 top_p=params.top_p,
-                                                 n=params.n,
-                                                 frequency_penalty=params.frequency_penalty,
-                                                 presence_penalty=params.presence_penalty,
-                                                 best_of=params.best_of,
-                                                 )
-                    completion = "\n".join(r["text"] for r in response["choices"])
+                    if prompt_altText is not None:
+                        prompt = prompt_altText.text
+                        if "$" in prompt:
+                            prompt_templ = Template(prompt)
+                            flatten_doc = flatten(document.dict())
+                            prompt = prompt_templ.safe_substitute(flatten_doc)
+
+                response = openai.Completion.create(
+                    model=params.model.value,
+                    prompt=prompt,
+                    max_tokens=params.max_tokens,
+                    temperature=params.temperature,
+                    top_p=params.top_p,
+                    n=params.n,
+                    frequency_penalty=params.frequency_penalty,
+                    presence_penalty=params.presence_penalty,
+                    best_of=params.best_of,
+                )
+                completion = "\n".join(r["text"] for r in response["choices"])
                 if params.completion_altText is not None and len(
-                    params.completion_altText
+                        params.completion_altText
                 ):
                     altTexts.append(
                         AltText(name=params.completion_altText, text=completion)
                     )
                     document.altTexts = altTexts
                 else:
                     document.text = completion
                     document.sentences = []
-                    document.annotations = []
-                    document.categories = []
+                    document.annotations = None
+                    document.categories = None
         except BaseException as err:
             raise err
         return documents
 
     @classmethod
     def get_model(cls) -> Type[BaseModel]:
         return OpenAICompletionParameters
 
 
-# def flatten(d, parent_key="", sep="_"):
-#     items = []
-#     for k, v in d.items():
-#         new_key = parent_key + sep + k if parent_key else k
-#         if isinstance(v, collections.MutableMapping):
-#             items.extend(flatten(v, new_key, sep=sep).items())
-#         else:
-#             items.append((new_key, v))
-#     return dict(items)
-
-
-def flatten_document(doc: Document):
-    y = doc.dict()
-    out = {}
-
-    def flatten(x, name=""):
-
-        # If the Nested key-value
-        # pair is of dict type
-        if type(x) is dict:
-
-            for a in x:
-                flatten(x[a], name + a + "_")
-
-        # If the Nested key-value
-        # pair is of list type
-        elif type(x) is list:
-
-            i = 0
-
-            for a in x:
-                flatten(a, name + str(i) + "_")
-                i += 1
+def flatten(d, parent_key="", sep="."):
+    items = []
+    for k, v in d.items():
+        new_key = parent_key + sep + k if parent_key else k
+        if isinstance(v, collections.MutableMapping):
+            items.extend(flatten(v, new_key, sep=sep).items())
         else:
-            out[name[:-1]] = x
-
-    flatten(y)
-    return out
+            items.append((new_key, v))
+    return dict(items)
 
 
 def document_language(doc: Document, default: str = None):
     if doc.metadata is not None and "language" in doc.metadata:
         return doc.metadata["language"]
     return default
 
 
-def get_template(params: OpenAICompletionParameters, default: str = None):
-    if "$" in params.prompt:
-        prompt_templ = Template(params.prompt)
-        return TemplateLanguage.string, prompt_templ
-    elif "{{" in params.prompt:
-        environment = get_jinja2_env()
-        prompt_dedented = inspect.cleandoc(params.prompt)
-        prompt_templ = environment.from_string(prompt_dedented)
-        return TemplateLanguage.jinja2, prompt_templ
-    return TemplateLanguage.none, params.prompt
-
-
-@api_retry(max_call_number=3000, max_call_number_interval=60)
-def openai_completion(openai, **kwargs):
-    response = openai.Completion.create(**kwargs)
-    return response
-
-
-@api_retry(max_call_number=3500, max_call_number_interval=60)
-def openai_chat_completion(openai, **kwargs):
-    response = openai.ChatCompletion.create(**kwargs)
-    return response
-
-
 @lru_cache(maxsize=None)
 def get_openai():
     openai.api_key = os.getenv("OPENAI_API_KEY")
-    OPENAI_API_TYPE = os.getenv("OPENAI_API_TYPE", None)
-    if OPENAI_API_TYPE is not None:
-        openai.type = OPENAI_API_TYPE
-    OPENAI_API_BASE = os.getenv("OPENAI_API_BASE", None)
-    if OPENAI_API_BASE is not None:
-        openai.api_base = OPENAI_API_BASE
-    OPENAI_API_VERSION = os.getenv("OPENAI_API_VERSION", None)
-    if OPENAI_API_VERSION is not None:
-        openai.api_version = OPENAI_API_VERSION
     return openai
-
-
-@lru_cache(maxsize=None)
-def get_jinja2_env():
-    return jinja2.Environment(extensions=["jinja2.ext.do"])
```

### Comparing `pyprocessors_openai_completion-0.5.77/pyproject.toml` & `pyprocessors-openai_completion-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 requires = [
     "pymultirole-plugins>=0.5.0,<0.6.0",
-    "openai>=0.27.0",
-    "Jinja2",
-    "tenacity"
+    "openai"
 ]
 dist-name = "pyprocessors-openai_completion"
 description-file = "README.md"
 requires-python = ">=3.8"
 
 [tool.flit.entrypoints."pyprocessors.plugins"]
 openai_completion = "pyprocessors_openai_completion.openai_completion:OpenAICompletionProcessor"
```

### Comparing `pyprocessors_openai_completion-0.5.77/tox.ini` & `pyprocessors-openai_completion-0.5.9/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.77/setup.py` & `pyprocessors-openai_completion-0.5.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 packages = \
 ['pyprocessors_openai_completion']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pymultirole-plugins>=0.5.0,<0.6.0', 'openai>=0.27.0', 'Jinja2', 'tenacity']
+['pymultirole-plugins>=0.5.0,<0.6.0', 'openai']
 
 extras_require = \
 {'dev': ['flit', 'pre-commit', 'bump2version'],
  'docs': ['sphinx',
           'sphinx-rtd-theme',
           'm2r2',
           'sphinxcontrib.apidoc',
@@ -30,15 +30,15 @@
           'flask==2.1.3']}
 
 entry_points = \
 {'pyprocessors.plugins': ['openai_completion = '
                           'pyprocessors_openai_completion.openai_completion:OpenAICompletionProcessor']}
 
 setup(name='pyprocessors-openai_completion',
-      version='0.5.77',
+      version='0.5.9',
       description='OpenAICompletion processor',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `pyprocessors_openai_completion-0.5.77/PKG-INFO` & `pyprocessors-openai_completion-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-openai_completion
-Version: 0.5.77
+Version: 0.5.9
 Summary: OpenAICompletion processor
 Home-page: https://kairntech.com/
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -23,17 +23,15 @@
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: pymultirole-plugins>=0.5.0,<0.6.0
-Requires-Dist: openai>=0.27.0
-Requires-Dist: Jinja2
-Requires-Dist: tenacity
+Requires-Dist: openai
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: bump2version ; extra == "dev"
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Requires-Dist: m2r2 ; extra == "docs"
 Requires-Dist: sphinxcontrib.apidoc ; extra == "docs"
```

