# Comparing `tmp/langdash-1.7.3.tar.gz` & `tmp/langdash-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.7.3.tar", last modified: Sun Jul  9 01:57:44 2023, max compression
+gzip compressed data, was "langdash-1.7.4.tar", last modified: Mon Jul 10 01:52:12 2023, max compression
```

## Comparing `langdash-1.7.3.tar` & `langdash-1.7.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 01:57:44.908830 langdash-1.7.3/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.7.3/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.7.3/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-09 01:57:44.908830 langdash-1.7.3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2712 2023-07-08 22:51:09.000000 langdash-1.7.3/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 01:57:44.904830 langdash-1.7.3/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-09 01:47:46.000000 langdash-1.7.3/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 01:57:44.904830 langdash-1.7.3/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.7.3/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14976 2023-07-09 01:44:13.000000 langdash-1.7.3/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     9394 2023-06-28 07:12:18.000000 langdash-1.7.3/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.7.3/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 01:57:44.900830 langdash-1.7.3/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.7.3/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.7.3/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6738 2023-06-28 07:20:44.000000 langdash-1.7.3/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)     1341 2023-06-28 07:36:19.000000 langdash-1.7.3/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1661 2023-06-28 07:07:44.000000 langdash-1.7.3/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     9137 2023-06-28 07:27:22.000000 langdash-1.7.3/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 01:57:44.908830 langdash-1.7.3/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.7.3/langdash/models/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 01:57:44.908830 langdash-1.7.3/langdash/models/_mixins/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.3/langdash/models/_mixins/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3412 2023-06-21 10:26:00.000000 langdash-1.7.3/langdash/models/_mixins/tensor_based_infer_mixin.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 01:57:44.908830 langdash-1.7.3/langdash/models/_tokenizer/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.3/langdash/models/_tokenizer/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.7.3/langdash/models/_tokenizer/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-07-09 01:44:13.000000 langdash-1.7.3/langdash/models/_tokenizer/bytes_dict_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     2269 2023-06-21 10:26:00.000000 langdash-1.7.3/langdash/models/_tokenizer/hf_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1546 2023-06-22 00:31:04.000000 langdash-1.7.3/langdash/models/_tokenizer/rwkv_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.7.3/langdash/models/_tokenizer/tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     5280 2023-06-27 18:43:45.000000 langdash-1.7.3/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     4932 2023-06-27 18:24:11.000000 langdash-1.7.3/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.7.3/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)    11281 2023-07-09 01:48:13.000000 langdash-1.7.3/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.7.3/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5632 2023-06-27 18:22:06.000000 langdash-1.7.3/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.7.3/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.7.3/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 01:57:44.904830 langdash-1.7.3/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.7.3/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.7.3/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.7.3/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.7.3/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 01:57:44.904830 langdash-1.7.3/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-09 01:57:44.000000 langdash-1.7.3/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1654 2023-07-09 01:57:44.000000 langdash-1.7.3/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-09 01:57:44.000000 langdash-1.7.3/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-09 01:57:44.000000 langdash-1.7.3/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-09 01:57:44.000000 langdash-1.7.3/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-09 01:57:44.908830 langdash-1.7.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.7.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.642570 langdash-1.7.4/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.7.4/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.7.4/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-10 01:52:12.642570 langdash-1.7.4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2712 2023-07-08 22:51:09.000000 langdash-1.7.4/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.638570 langdash-1.7.4/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-10 01:51:24.000000 langdash-1.7.4/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.638570 langdash-1.7.4/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.7.4/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15364 2023-07-10 01:47:58.000000 langdash-1.7.4/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9394 2023-06-28 07:12:18.000000 langdash-1.7.4/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.7.4/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.634570 langdash-1.7.4/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.7.4/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.7.4/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6738 2023-06-28 07:20:44.000000 langdash-1.7.4/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1341 2023-06-28 07:36:19.000000 langdash-1.7.4/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1661 2023-06-28 07:07:44.000000 langdash-1.7.4/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9137 2023-06-28 07:27:22.000000 langdash-1.7.4/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.638570 langdash-1.7.4/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.7.4/langdash/models/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.642570 langdash-1.7.4/langdash/models/_mixins/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.4/langdash/models/_mixins/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3412 2023-06-21 10:26:00.000000 langdash-1.7.4/langdash/models/_mixins/tensor_based_infer_mixin.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.642570 langdash-1.7.4/langdash/models/_tokenizer/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.4/langdash/models/_tokenizer/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.7.4/langdash/models/_tokenizer/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-07-09 01:44:13.000000 langdash-1.7.4/langdash/models/_tokenizer/bytes_dict_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2269 2023-06-21 10:26:00.000000 langdash-1.7.4/langdash/models/_tokenizer/hf_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1546 2023-06-22 00:31:04.000000 langdash-1.7.4/langdash/models/_tokenizer/rwkv_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.7.4/langdash/models/_tokenizer/tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5280 2023-06-27 18:43:45.000000 langdash-1.7.4/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4932 2023-06-27 18:24:11.000000 langdash-1.7.4/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.7.4/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11281 2023-07-09 01:48:13.000000 langdash-1.7.4/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.7.4/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5632 2023-06-27 18:22:06.000000 langdash-1.7.4/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.7.4/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.7.4/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.634570 langdash-1.7.4/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.7.4/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.7.4/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.7.4/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.7.4/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.638570 langdash-1.7.4/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-10 01:52:12.000000 langdash-1.7.4/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1654 2023-07-10 01:52:12.000000 langdash-1.7.4/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-10 01:52:12.000000 langdash-1.7.4/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-10 01:52:12.000000 langdash-1.7.4/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-10 01:52:12.000000 langdash-1.7.4/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-10 01:52:12.642570 langdash-1.7.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.7.4/setup.py
```

### Comparing `langdash-1.7.3/LICENSE.txt` & `langdash-1.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/PKG-INFO` & `langdash-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.7.3
+Version: 1.7.4
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.7.3/README.md` & `langdash-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/chains/chains.py` & `langdash-1.7.4/langdash/chains/chains.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,23 @@
       if isinstance(node, str):
         pp_nodes.append(self._ld.text(node))
       elif isinstance(node, LDFormatArg):
         _preprocess_format_arg(node)
       else:
         pp_nodes.append(node)
 
+    # argument/return checking
+    for node in nodes:
+      if isinstance(node, LDArg):
+        if node._arg not in self._args:
+          raise ValueError(f"'{node._arg}' not found in argument declaration")
+      elif isinstance(node, (LDReturns, LDChoice)):
+        if node._returns not in self._returns:
+          raise ValueError(f"'{node._returns}' not found in return declaration")
+
     # fuse text nodes
     for i in range(len(pp_nodes)):
       pp_node_i = pp_nodes[i]
       if isinstance(pp_node_i, LDText):
         for j in range(i + 1, len(pp_nodes)):
           pp_node_j = pp_nodes[j]
           if not isinstance(pp_node_j, LDText):
```

### Comparing `langdash-1.7.3/langdash/chains/nodes.py` & `langdash-1.7.4/langdash/chains/nodes.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/classify/token_qa.py` & `langdash-1.7.4/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/core.py` & `langdash-1.7.4/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/infer.py` & `langdash-1.7.4/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/llm.py` & `langdash-1.7.4/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/llm_session.py` & `langdash-1.7.4/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/models/_mixins/tensor_based_infer_mixin.py` & `langdash-1.7.4/langdash/models/_mixins/tensor_based_infer_mixin.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/models/_tokenizer/_bpe.py` & `langdash-1.7.4/langdash/models/_tokenizer/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/models/_tokenizer/bytes_dict_tokenizer.py` & `langdash-1.7.4/langdash/models/_tokenizer/bytes_dict_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/models/_tokenizer/hf_tokenizer.py` & `langdash-1.7.4/langdash/models/_tokenizer/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/models/_tokenizer/rwkv_tokenizer.py` & `langdash-1.7.4/langdash/models/_tokenizer/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/models/_tokenizer/tokenizer.py` & `langdash-1.7.4/langdash/models/_tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/models/ctransformers.py` & `langdash-1.7.4/langdash/models/ctransformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/models/llama_cpp.py` & `langdash-1.7.4/langdash/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/models/mock.py` & `langdash-1.7.4/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/models/rwkv_cpp.py` & `langdash-1.7.4/langdash/models/rwkv_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/models/sentence_transformers.py` & `langdash-1.7.4/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/models/transformers.py` & `langdash-1.7.4/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/response.py` & `langdash-1.7.4/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/sampling.py` & `langdash-1.7.4/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/search/embedding_search.py` & `langdash-1.7.4/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/search/engine.py` & `langdash-1.7.4/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash/search/multichoice_search.py` & `langdash-1.7.4/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/langdash.egg-info/PKG-INFO` & `langdash-1.7.4/langdash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.7.3
+Version: 1.7.4
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.7.3/langdash.egg-info/SOURCES.txt` & `langdash-1.7.4/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.7.3/setup.py` & `langdash-1.7.4/setup.py`

 * *Files identical despite different names*

