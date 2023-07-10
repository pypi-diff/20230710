# Comparing `tmp/langchain-chatglm-0.0.8.tar.gz` & `tmp/langchain-chatglm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-chatglm-0.0.8.tar", last modified: Mon Jul 10 12:50:33 2023, max compression
+gzip compressed data, was "langchain-chatglm-0.0.9.tar", last modified: Mon Jul 10 14:05:30 2023, max compression
```

## Comparing `langchain-chatglm-0.0.8.tar` & `langchain-chatglm-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 12:50:33.509591 langchain-chatglm-0.0.8/
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1065 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.8/LICENSE
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1616 2023-07-10 12:50:33.509591 langchain-chatglm-0.0.8/PKG-INFO
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1065 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.8/README.md
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 12:50:33.509591 langchain-chatglm-0.0.8/langchain_chatglm/
--rw-r--r--   0 tsai      (1000) tsai      (1000)       67 2023-07-08 07:02:39.000000 langchain-chatglm-0.0.8/langchain_chatglm/__init__.py
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 12:50:33.509591 langchain-chatglm-0.0.8/langchain_chatglm/llms/
--rw-r--r--   0 tsai      (1000) tsai      (1000)       67 2023-07-08 07:02:39.000000 langchain-chatglm-0.0.8/langchain_chatglm/llms/__init__.py
--rw-r--r--   0 tsai      (1000) tsai      (1000)     4980 2023-07-10 12:49:37.000000 langchain-chatglm-0.0.8/langchain_chatglm/llms/chatglm_pipeline.py
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 12:50:33.509591 langchain-chatglm-0.0.8/langchain_chatglm.egg-info/
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1616 2023-07-10 12:50:33.000000 langchain-chatglm-0.0.8/langchain_chatglm.egg-info/PKG-INFO
--rw-r--r--   0 tsai      (1000) tsai      (1000)      344 2023-07-10 12:50:33.000000 langchain-chatglm-0.0.8/langchain_chatglm.egg-info/SOURCES.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)        1 2023-07-10 12:50:33.000000 langchain-chatglm-0.0.8/langchain_chatglm.egg-info/dependency_links.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)       37 2023-07-10 12:50:33.000000 langchain-chatglm-0.0.8/langchain_chatglm.egg-info/requires.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)       18 2023-07-10 12:50:33.000000 langchain-chatglm-0.0.8/langchain_chatglm.egg-info/top_level.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)      690 2023-07-10 12:50:18.000000 langchain-chatglm-0.0.8/pyproject.toml
--rw-r--r--   0 tsai      (1000) tsai      (1000)       38 2023-07-10 12:50:33.509591 langchain-chatglm-0.0.8/setup.cfg
+drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 14:05:30.279529 langchain-chatglm-0.0.9/
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     1065 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.9/LICENSE
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     1813 2023-07-10 14:05:30.279529 langchain-chatglm-0.0.9/PKG-INFO
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     1263 2023-07-10 13:46:05.000000 langchain-chatglm-0.0.9/README.md
+drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 14:05:30.279529 langchain-chatglm-0.0.9/langchain_chatglm/
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       86 2023-07-10 13:39:01.000000 langchain-chatglm-0.0.9/langchain_chatglm/__init__.py
+drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 14:05:30.279529 langchain-chatglm-0.0.9/langchain_chatglm/llms/
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       67 2023-07-08 07:02:39.000000 langchain-chatglm-0.0.9/langchain_chatglm/llms/__init__.py
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     5811 2023-07-10 14:04:55.000000 langchain-chatglm-0.0.9/langchain_chatglm/llms/chatglm_pipeline.py
+drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 14:05:30.279529 langchain-chatglm-0.0.9/langchain_chatglm.egg-info/
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     1813 2023-07-10 14:05:30.000000 langchain-chatglm-0.0.9/langchain_chatglm.egg-info/PKG-INFO
+-rw-r--r--   0 tsai      (1000) tsai      (1000)      344 2023-07-10 14:05:30.000000 langchain-chatglm-0.0.9/langchain_chatglm.egg-info/SOURCES.txt
+-rw-r--r--   0 tsai      (1000) tsai      (1000)        1 2023-07-10 14:05:30.000000 langchain-chatglm-0.0.9/langchain_chatglm.egg-info/dependency_links.txt
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       40 2023-07-10 14:05:30.000000 langchain-chatglm-0.0.9/langchain_chatglm.egg-info/requires.txt
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       18 2023-07-10 14:05:30.000000 langchain-chatglm-0.0.9/langchain_chatglm.egg-info/top_level.txt
+-rw-r--r--   0 tsai      (1000) tsai      (1000)      703 2023-07-10 13:47:13.000000 langchain-chatglm-0.0.9/pyproject.toml
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       38 2023-07-10 14:05:30.279529 langchain-chatglm-0.0.9/setup.cfg
```

### Comparing `langchain-chatglm-0.0.8/LICENSE` & `langchain-chatglm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-chatglm-0.0.8/PKG-INFO` & `langchain-chatglm-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: langchain-chatglm
-Version: 0.0.8
-Summary: esay use ChatGLM in LangChain.
-Author-email: Sim Tsai <13759975+SimTsai@users.noreply.github.com>
-Project-URL: Homepage, https://github.com/SimTsai/langchain_chatglm
-Project-URL: Bug Tracker, https://github.com/SimTsai/langchain_chatglm/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # langchain-ChatGLM
 
 esay use ChatGLM in LangChain.
 
 [ChatGLM2-6B](https://github.com/THUDM/ChatGLM2-6B)
 [langchain](https://github.com/hwchase17/langchain)
 
@@ -51,7 +37,15 @@
 llm_chain = LLMChain(prompt=prompt, llm=llm)
 
 question = "华晨宇和张碧晨是什么关系?"
 
 llm_chain.run(question)
 
 ```
+
+## model_kwargs
+| key | values | remark |
+| --- | ------ | ------ |
+| `"device"` | `"cuda"` | 使用cuda加速 |
+| `"float"` | `True`, `False` | 使用cpu推理  |
+| `"quantize"`| `8` | 量化 |
+
```

### Comparing `langchain-chatglm-0.0.8/langchain_chatglm/llms/chatglm_pipeline.py` & `langchain-chatglm-0.0.9/langchain_chatglm/llms/chatglm_pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Wrapper around ChatGLMP Pipeline APIs."""
 
 from functools import partial
 import importlib.util
 import logging
-from typing import Any, List, Mapping, Optional
+from typing import Any, List, Mapping, Optional, Tuple
 
 from pydantic import Extra
 
 from langchain.callbacks.manager import CallbackManagerForLLMRun
 from langchain.llms.base import LLM
 
 DEFAULT_MODEL_ID = "THUDM/chatglm2-6b"
 
 logger = logging.getLogger(__name__)
 
+
 class ChatGLMPipeline(LLM):
     """Wrapper around ChatGLM Pipeline API.
 
     To use, you should have the ``transformers`` python package installed.
 
     Example using from_model_id:
         .. code-block:: python
@@ -25,17 +26,17 @@
             from langchain.llms import ChatGLM
             hf = ChatGLM.from_model_id(
                 model_id="THUDM/chatglm2-6b",
                 model_kwargs={"trust_remote_code": True, device='cuda'}
             )
     """
 
-    client: Any  #: :meta private:
-    stream_client: Any #: :meta private:
-    tokenizer: Any #: :meta private:
+    model: Any  #: :meta private:
+    tokenizer: Any  # : :meta private:
+    histoty: List[Tuple[str, str]] = []
     model_id: str = DEFAULT_MODEL_ID
     """Model name to use."""
     model_kwargs: Optional[dict] = None
     """Key word arguments passed to the model."""
     streaming: bool = True
     """Whether to stream the results, token by token."""
 
@@ -54,57 +55,68 @@
     ) -> LLM:
         """Construct the pipeline object from model_id and task."""
         try:
             from transformers import (
                 AutoModel,
                 AutoTokenizer,
             )
-            from transformers import pipeline as hf_pipeline
-
         except ImportError:
             raise ValueError(
                 "Could not import transformers python package. "
                 "Please install it with `pip install transformers`."
             )
 
         _model_kwargs = model_kwargs or {}
         tokenizer = AutoTokenizer.from_pretrained(model_id, **_model_kwargs)
 
         try:
-           model = AutoModel.from_pretrained(model_id, **_model_kwargs).cuda()
-           model = model.eval()
+            model = AutoModel.from_pretrained(model_id, **_model_kwargs)
+            if "quantize" in _model_kwargs:
+                model = model.quantize(_model_kwargs["quantize"])
+                _model_kwargs = {
+                    k: v for k, v in _model_kwargs.items() if k != "quantize"
+                }
+            if "device" in _model_kwargs and _model_kwargs["device"] == "cuda":
+                model = model.cuda()
+                _model_kwargs = {
+                    k: v for k, v in _model_kwargs.items() if k != "device"
+                }
+                if importlib.util.find_spec("torch") is not None:
+                    import torch
+
+                    cuda_device_count = torch.cuda.device_count()
+                    if device < -1 or (device >= cuda_device_count):
+                        raise ValueError(
+                            f"Got device=={device}, "
+                            f"device is required to be within [-1, {cuda_device_count})"
+                        )
+                    if device < 0 and cuda_device_count > 0:
+                        logger.warning(
+                            "Device has %d GPUs available. "
+                            "Provide device={deviceId} to `from_model_id` to use available"
+                            "GPUs for execution. deviceId is -1 (default) for CPU and "
+                            "can be a positive integer associated with CUDA device id.",
+                            cuda_device_count,
+                        )
+            if "float" in _model_kwargs and _model_kwargs["float"] == True:
+                model = model.float()
+                _model_kwargs = {
+                    k: v for k, v in _model_kwargs.items() if k != "float"
+                }
+            model = model.eval()
         except ImportError as e:
             raise ValueError(
                 f"Could not load the {model_id} model due to missing dependencies."
             ) from e
-
-        if importlib.util.find_spec("torch") is not None:
-            import torch
-
-            cuda_device_count = torch.cuda.device_count()
-            if device < -1 or (device >= cuda_device_count):
-                raise ValueError(
-                    f"Got device=={device}, "
-                    f"device is required to be within [-1, {cuda_device_count})"
-                )
-            if device < 0 and cuda_device_count > 0:
-                logger.warning(
-                    "Device has %d GPUs available. "
-                    "Provide device={deviceId} to `from_model_id` to use available"
-                    "GPUs for execution. deviceId is -1 (default) for CPU and "
-                    "can be a positive integer associated with CUDA device id.",
-                    cuda_device_count,
-                )
         if "trust_remote_code" in _model_kwargs:
             _model_kwargs = {
                 k: v for k, v in _model_kwargs.items() if k != "trust_remote_code"
             }
         return cls(
-            client=model.chat,
-            stream_client=model.stream_chat,
+            model=model,
             model_id=model_id,
             tokenizer=tokenizer,
             model_kwargs=_model_kwargs,
             **kwargs,
         )
 
     @property
@@ -125,27 +137,29 @@
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> str:
         if self.streaming:
             return self.stream(prompt=prompt, stop=stop, run_manager=run_manager)
         else:
-            response, history = self.client(self.tokenizer, prompt, history=[])
+            response, history = self.model.chat(
+                self.tokenizer, prompt, history=self.histoty, return_past_key_values=True)
             return response
 
     def stream(
         self,
         prompt,
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
     ) -> str:
         current_length = 0
         text_callback = None
         if run_manager:
-                text_callback = partial(run_manager.on_llm_new_token, verbose=self.verbose)
+            text_callback = partial(
+                run_manager.on_llm_new_token, verbose=self.verbose)
         text = ""
-        for response, history, past_key_values in self.stream_client(self.tokenizer, prompt, history=[],return_past_key_values=True):
+        for response, history, past_key_values in self.model.stream_chat(self.tokenizer, prompt, history=self.histoty, return_past_key_values=True):
             if text_callback:
                 text_callback(response[current_length:])
             text += response[current_length:]
             current_length = len(response)
         return text
```

### Comparing `langchain-chatglm-0.0.8/pyproject.toml` & `langchain-chatglm-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [build-system]
 requires = ["setuptools>=68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langchain-chatglm"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Sim Tsai", email="13759975+SimTsai@users.noreply.github.com" },
 ]
 description = "esay use ChatGLM in LangChain."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "pydantic==1.10.11",
-  "langchain==0.0.226"
+  "pydantic<2",
+  "langchain",
+  "transformers",
+  "torch"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/SimTsai/langchain_chatglm"
 "Bug Tracker" = "https://github.com/SimTsai/langchain_chatglm/issues"
```

