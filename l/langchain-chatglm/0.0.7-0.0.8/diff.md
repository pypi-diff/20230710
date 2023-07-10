# Comparing `tmp/langchain-chatglm-0.0.7.tar.gz` & `tmp/langchain-chatglm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-chatglm-0.0.7.tar", last modified: Sat Jul  8 07:05:42 2023, max compression
+gzip compressed data, was "langchain-chatglm-0.0.8.tar", last modified: Mon Jul 10 12:50:33 2023, max compression
```

## Comparing `langchain-chatglm-0.0.7.tar` & `langchain-chatglm-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-08 07:05:42.899317 langchain-chatglm-0.0.7/
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1065 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.7/LICENSE
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1616 2023-07-08 07:05:42.899317 langchain-chatglm-0.0.7/PKG-INFO
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1065 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.7/README.md
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-08 07:05:42.889317 langchain-chatglm-0.0.7/langchain_chatglm/
--rw-r--r--   0 tsai      (1000) tsai      (1000)       67 2023-07-08 07:02:39.000000 langchain-chatglm-0.0.7/langchain_chatglm/__init__.py
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-08 07:05:42.899317 langchain-chatglm-0.0.7/langchain_chatglm/llms/
--rw-r--r--   0 tsai      (1000) tsai      (1000)       67 2023-07-08 07:02:39.000000 langchain-chatglm-0.0.7/langchain_chatglm/llms/__init__.py
--rw-r--r--   0 tsai      (1000) tsai      (1000)     4973 2023-07-08 07:05:18.000000 langchain-chatglm-0.0.7/langchain_chatglm/llms/chatglm_pipeline.py
-drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-08 07:05:42.889317 langchain-chatglm-0.0.7/langchain_chatglm.egg-info/
--rw-r--r--   0 tsai      (1000) tsai      (1000)     1616 2023-07-08 07:05:42.000000 langchain-chatglm-0.0.7/langchain_chatglm.egg-info/PKG-INFO
--rw-r--r--   0 tsai      (1000) tsai      (1000)      344 2023-07-08 07:05:42.000000 langchain-chatglm-0.0.7/langchain_chatglm.egg-info/SOURCES.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)        1 2023-07-08 07:05:42.000000 langchain-chatglm-0.0.7/langchain_chatglm.egg-info/dependency_links.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)       37 2023-07-08 07:05:42.000000 langchain-chatglm-0.0.7/langchain_chatglm.egg-info/requires.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)       18 2023-07-08 07:05:42.000000 langchain-chatglm-0.0.7/langchain_chatglm.egg-info/top_level.txt
--rw-r--r--   0 tsai      (1000) tsai      (1000)      690 2023-07-08 07:05:36.000000 langchain-chatglm-0.0.7/pyproject.toml
--rw-r--r--   0 tsai      (1000) tsai      (1000)       38 2023-07-08 07:05:42.899317 langchain-chatglm-0.0.7/setup.cfg
+drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 12:50:33.509591 langchain-chatglm-0.0.8/
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     1065 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.8/LICENSE
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     1616 2023-07-10 12:50:33.509591 langchain-chatglm-0.0.8/PKG-INFO
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     1065 2023-07-07 23:39:43.000000 langchain-chatglm-0.0.8/README.md
+drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 12:50:33.509591 langchain-chatglm-0.0.8/langchain_chatglm/
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       67 2023-07-08 07:02:39.000000 langchain-chatglm-0.0.8/langchain_chatglm/__init__.py
+drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 12:50:33.509591 langchain-chatglm-0.0.8/langchain_chatglm/llms/
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       67 2023-07-08 07:02:39.000000 langchain-chatglm-0.0.8/langchain_chatglm/llms/__init__.py
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     4980 2023-07-10 12:49:37.000000 langchain-chatglm-0.0.8/langchain_chatglm/llms/chatglm_pipeline.py
+drwxr-xr-x   0 tsai      (1000) tsai      (1000)        0 2023-07-10 12:50:33.509591 langchain-chatglm-0.0.8/langchain_chatglm.egg-info/
+-rw-r--r--   0 tsai      (1000) tsai      (1000)     1616 2023-07-10 12:50:33.000000 langchain-chatglm-0.0.8/langchain_chatglm.egg-info/PKG-INFO
+-rw-r--r--   0 tsai      (1000) tsai      (1000)      344 2023-07-10 12:50:33.000000 langchain-chatglm-0.0.8/langchain_chatglm.egg-info/SOURCES.txt
+-rw-r--r--   0 tsai      (1000) tsai      (1000)        1 2023-07-10 12:50:33.000000 langchain-chatglm-0.0.8/langchain_chatglm.egg-info/dependency_links.txt
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       37 2023-07-10 12:50:33.000000 langchain-chatglm-0.0.8/langchain_chatglm.egg-info/requires.txt
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       18 2023-07-10 12:50:33.000000 langchain-chatglm-0.0.8/langchain_chatglm.egg-info/top_level.txt
+-rw-r--r--   0 tsai      (1000) tsai      (1000)      690 2023-07-10 12:50:18.000000 langchain-chatglm-0.0.8/pyproject.toml
+-rw-r--r--   0 tsai      (1000) tsai      (1000)       38 2023-07-10 12:50:33.509591 langchain-chatglm-0.0.8/setup.cfg
```

### Comparing `langchain-chatglm-0.0.7/LICENSE` & `langchain-chatglm-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-chatglm-0.0.7/PKG-INFO` & `langchain-chatglm-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-chatglm
-Version: 0.0.7
+Version: 0.0.8
 Summary: esay use ChatGLM in LangChain.
 Author-email: Sim Tsai <13759975+SimTsai@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/SimTsai/langchain_chatglm
 Project-URL: Bug Tracker, https://github.com/SimTsai/langchain_chatglm/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `langchain-chatglm-0.0.7/README.md` & `langchain-chatglm-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `langchain-chatglm-0.0.7/langchain_chatglm/llms/chatglm_pipeline.py` & `langchain-chatglm-0.0.8/langchain_chatglm/llms/chatglm_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                 "Please install it with `pip install transformers`."
             )
 
         _model_kwargs = model_kwargs or {}
         tokenizer = AutoTokenizer.from_pretrained(model_id, **_model_kwargs)
 
         try:
-           model = AutoModel.from_pretrained(model_id, **_model_kwargs)
+           model = AutoModel.from_pretrained(model_id, **_model_kwargs).cuda()
            model = model.eval()
         except ImportError as e:
             raise ValueError(
                 f"Could not load the {model_id} model due to missing dependencies."
             ) from e
 
         if importlib.util.find_spec("torch") is not None:
```

### Comparing `langchain-chatglm-0.0.7/langchain_chatglm.egg-info/PKG-INFO` & `langchain-chatglm-0.0.8/langchain_chatglm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-chatglm
-Version: 0.0.7
+Version: 0.0.8
 Summary: esay use ChatGLM in LangChain.
 Author-email: Sim Tsai <13759975+SimTsai@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/SimTsai/langchain_chatglm
 Project-URL: Bug Tracker, https://github.com/SimTsai/langchain_chatglm/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `langchain-chatglm-0.0.7/pyproject.toml` & `langchain-chatglm-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langchain-chatglm"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Sim Tsai", email="13759975+SimTsai@users.noreply.github.com" },
 ]
 description = "esay use ChatGLM in LangChain."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

