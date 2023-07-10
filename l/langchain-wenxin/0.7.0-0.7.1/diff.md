# Comparing `tmp/langchain_wenxin-0.7.0.tar.gz` & `tmp/langchain_wenxin-0.7.1.tar.gz`

## Comparing `langchain_wenxin-0.7.0.tar` & `langchain_wenxin-0.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0    14049 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/examples/Langchain_wenxin_retrieval_qa_compared.ipynb
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/src/langchain_wenxin/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/src/langchain_wenxin/__init__.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/src/langchain_wenxin/chat_models.py
--rw-r--r--   0        0        0    17115 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/src/langchain_wenxin/llms.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/src/langchain_wenxin/retrievers.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/integration_tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/integration_tests/chat_models/__init__.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/integration_tests/chat_models/test_wenxin.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/integration_tests/llms/__init__.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/integration_tests/llms/test_wenxin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/tools/__init__.py
--rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/tests/tools/test_callbacks.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/README.md
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0    14049 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/examples/Langchain_wenxin_retrieval_qa_compared.ipynb
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/src/langchain_wenxin/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/src/langchain_wenxin/__init__.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/src/langchain_wenxin/chat_models.py
+-rw-r--r--   0        0        0    17115 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/src/langchain_wenxin/llms.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/src/langchain_wenxin/retrievers.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/tests/integration_tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/tests/integration_tests/chat_models/__init__.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/tests/integration_tests/chat_models/test_wenxin.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/tests/integration_tests/llms/__init__.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/tests/integration_tests/llms/test_wenxin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/tests/tools/__init__.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/tests/tools/test_callbacks.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/README.md
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 langchain_wenxin-0.7.1/PKG-INFO
```

### Comparing `langchain_wenxin-0.7.0/examples/Langchain_wenxin_retrieval_qa_compared.ipynb` & `langchain_wenxin-0.7.1/examples/Langchain_wenxin_retrieval_qa_compared.ipynb`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.7.0/src/langchain_wenxin/chat_models.py` & `langchain_wenxin-0.7.1/src/langchain_wenxin/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.7.0/src/langchain_wenxin/llms.py` & `langchain_wenxin-0.7.1/src/langchain_wenxin/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.7.0/src/langchain_wenxin/retrievers.py` & `langchain_wenxin-0.7.1/src/langchain_wenxin/retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.7.0/tests/integration_tests/chat_models/test_wenxin.py` & `langchain_wenxin-0.7.1/tests/integration_tests/chat_models/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.7.0/tests/integration_tests/llms/test_wenxin.py` & `langchain_wenxin-0.7.1/tests/integration_tests/llms/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.7.0/tests/tools/test_callbacks.py` & `langchain_wenxin-0.7.1/tests/tools/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.7.0/.gitignore` & `langchain_wenxin-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.7.0/LICENSE.txt` & `langchain_wenxin-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.7.0/README.md` & `langchain_wenxin-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.7.0/pyproject.toml` & `langchain_wenxin-0.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,17 @@
   "requests",
   "sseclient-py",
   "numpy",
   "aiohttp",
 ]
 
 [project.urls]
-Documentation = "https://github.com/unknown/langchain-wenxin#readme"
-Issues = "https://github.com/unknown/langchain-wenxin/issues"
-Source = "https://github.com/unknown/langchain-wenxin"
+Documentation = "https://github.com/ninehills/langchain-wenxin#readme"
+Issues = "https://github.com/ninehills/langchain-wenxin/issues"
+Source = "https://github.com/ninehills/langchain-wenxin"
 
 [tool.hatch.version]
 path = "src/langchain_wenxin/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
```

### Comparing `langchain_wenxin-0.7.0/PKG-INFO` & `langchain_wenxin-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: langchain-wenxin
-Version: 0.7.0
-Project-URL: Documentation, https://github.com/unknown/langchain-wenxin#readme
-Project-URL: Issues, https://github.com/unknown/langchain-wenxin/issues
-Project-URL: Source, https://github.com/unknown/langchain-wenxin
+Version: 0.7.1
+Project-URL: Documentation, https://github.com/ninehills/langchain-wenxin#readme
+Project-URL: Issues, https://github.com/ninehills/langchain-wenxin/issues
+Project-URL: Source, https://github.com/ninehills/langchain-wenxin
 Author-email: Tao Yang <swulling@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

