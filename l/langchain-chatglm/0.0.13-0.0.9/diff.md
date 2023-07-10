# Comparing `tmp/langchain-chatglm-0.0.13.tar.gz` & `tmp/langchain-chatglm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-chatglm-0.0.13.tar", last modified: Mon Jul 10 14:40:28 2023, max compression
+gzip compressed data, was "langchain-chatglm-0.0.9.tar", last modified: Mon Jul 10 14:05:30 2023, max compression
```

## Comparing `langchain-chatglm-0.0.13.tar` & `langchain-chatglm-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 14:40:28.109503 langchain-chatglm-0.0.13/
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1065 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.13/LICENSE
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1814 2023-07-10 14:40:28.109503 langchain-chatglm-0.0.13/PKG-INFO
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1263 2023-07-10 13:46:05.000000 langchain-chatglm-0.0.13/README.md
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 14:40:28.109503 langchain-chatglm-0.0.13/langchain_chatglm/
--rw-r--r--   0 tsai      (1000) tsai      (1000)       87 2023-07-10 14:39:09.000000 langchain-chatglm-0.0.13/langchain_chatglm/__init__.py
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 14:40:28.109503 langchain-chatglm-0.0.13/langchain_chatglm/llms/
--rw-r--r--   0 tsai      (1000) tsai      (1000)       67 2023-07-08 07:02:39.000000 langchain-chatglm-0.0.13/langchain_chatglm/llms/__init__.py
--rw-r--r--   0 tsai      (1000) tsai      (1000)     6349 2023-07-10 14:38:54.000000 langchain-chatglm-0.0.13/langchain_chatglm/llms/chatglm_pipeline.py
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 14:40:28.109503 langchain-chatglm-0.0.13/langchain_chatglm.egg-info/
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1814 2023-07-10 14:40:28.000000 langchain-chatglm-0.0.13/langchain_chatglm.egg-info/PKG-INFO
--rw-r--r--   0 tsai      (1000) tsai      (1000)      344 2023-07-10 14:40:28.000000 langchain-chatglm-0.0.13/langchain_chatglm.egg-info/SOURCES.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)        1 2023-07-10 14:40:28.000000 langchain-chatglm-0.0.13/langchain_chatglm.egg-info/dependency_links.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)       40 2023-07-10 14:40:28.000000 langchain-chatglm-0.0.13/langchain_chatglm.egg-info/requires.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)       18 2023-07-10 14:40:28.000000 langchain-chatglm-0.0.13/langchain_chatglm.egg-info/top_level.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)      704 2023-07-10 14:39:09.000000 langchain-chatglm-0.0.13/pyproject.toml
--rw-r--r--   0 tsai      (1000) tsai      (1000)       38 2023-07-10 14:40:28.109503 langchain-chatglm-0.0.13/setup.cfg
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

### Comparing `langchain-chatglm-0.0.13/LICENSE` & `langchain-chatglm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-chatglm-0.0.13/PKG-INFO` & `langchain-chatglm-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-chatglm
-Version: 0.0.13
+Version: 0.0.9
 Summary: esay use ChatGLM in LangChain.
 Author-email: Sim Tsai <13759975+SimTsai@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/SimTsai/langchain_chatglm
 Project-URL: Bug Tracker, https://github.com/SimTsai/langchain_chatglm/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `langchain-chatglm-0.0.13/README.md` & `langchain-chatglm-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `langchain-chatglm-0.0.13/langchain_chatglm/llms/chatglm_pipeline.py` & `langchain-chatglm-0.0.9/langchain_chatglm/llms/chatglm_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,26 +64,23 @@
                 "Could not import transformers python package. "
                 "Please install it with `pip install transformers`."
             )
 
         _model_kwargs = model_kwargs or {}
         tokenizer = AutoTokenizer.from_pretrained(model_id, **_model_kwargs)
 
-        def get_model(_model_kwargs):
-            mdl = 0
-            quantize = -1
+        try:
+            model = AutoModel.from_pretrained(model_id, **_model_kwargs)
             if "quantize" in _model_kwargs:
-                quantize = _model_kwargs["quantize"]
+                model = model.quantize(_model_kwargs["quantize"])
                 _model_kwargs = {
                     k: v for k, v in _model_kwargs.items() if k != "quantize"
                 }
-
-            cuda = False
-            if "device" in _model_kwargs and "cuda" == _model_kwargs["device"]:
-                cuda = True
+            if "device" in _model_kwargs and _model_kwargs["device"] == "cuda":
+                model = model.cuda()
                 _model_kwargs = {
                     k: v for k, v in _model_kwargs.items() if k != "device"
                 }
                 if importlib.util.find_spec("torch") is not None:
                     import torch
 
                     cuda_device_count = torch.cuda.device_count()
@@ -96,34 +93,20 @@
                         logger.warning(
                             "Device has %d GPUs available. "
                             "Provide device={deviceId} to `from_model_id` to use available"
                             "GPUs for execution. deviceId is -1 (default) for CPU and "
                             "can be a positive integer associated with CUDA device id.",
                             cuda_device_count,
                         )
-
-            flt = False
             if "float" in _model_kwargs and _model_kwargs["float"] == True:
-                flt = True
+                model = model.float()
                 _model_kwargs = {
                     k: v for k, v in _model_kwargs.items() if k != "float"
                 }
-
-            if quantize > -1 and flt and cuda:
-                mdl = AutoModel.from_pretrained(
-                    model_id, **_model_kwargs).float().quantize(quantize).cuda()
-            elif quantize > -1 and cuda:
-                mdl = AutoModel.from_pretrained(
-                    model_id, **_model_kwargs).quantize(quantize).cuda()
-            elif cuda:
-                mdl = AutoModel.from_pretrained(
-                    model_id, **_model_kwargs).cuda()
-            return mdl.eval()
-        try:
-            model = get_model(_model_kwargs)
+            model = model.eval()
         except ImportError as e:
             raise ValueError(
                 f"Could not load the {model_id} model due to missing dependencies."
             ) from e
         if "trust_remote_code" in _model_kwargs:
             _model_kwargs = {
                 k: v for k, v in _model_kwargs.items() if k != "trust_remote_code"
```

### Comparing `langchain-chatglm-0.0.13/langchain_chatglm.egg-info/PKG-INFO` & `langchain-chatglm-0.0.9/langchain_chatglm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-chatglm
-Version: 0.0.13
+Version: 0.0.9
 Summary: esay use ChatGLM in LangChain.
 Author-email: Sim Tsai <13759975+SimTsai@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/SimTsai/langchain_chatglm
 Project-URL: Bug Tracker, https://github.com/SimTsai/langchain_chatglm/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `langchain-chatglm-0.0.13/pyproject.toml` & `langchain-chatglm-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langchain-chatglm"
-version = "0.0.13"
+version = "0.0.9"
 authors = [
   { name="Sim Tsai", email="13759975+SimTsai@users.noreply.github.com" },
 ]
 description = "esay use ChatGLM in LangChain."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

