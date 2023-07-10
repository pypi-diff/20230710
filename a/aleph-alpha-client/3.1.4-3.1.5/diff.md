# Comparing `tmp/aleph-alpha-client-3.1.4.tar.gz` & `tmp/aleph-alpha-client-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-alpha-client-3.1.4.tar", last modified: Mon Jun 26 09:36:52 2023, max compression
+gzip compressed data, was "aleph-alpha-client-3.1.5.tar", last modified: Mon Jul 10 09:16:12 2023, max compression
```

## Comparing `aleph-alpha-client-3.1.4.tar` & `aleph-alpha-client-3.1.5.tar`

### file list

```diff
@@ -1,44 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:36:52.016419 aleph-alpha-client-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-06-26 09:36:52.016419 aleph-alpha-client-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:36:52.012419 aleph-alpha-client-3.1.4/aleph_alpha_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35123 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/aleph_alpha_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/detokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/aleph_alpha_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:36:52.012419 aleph-alpha-client-3.1.4/aleph_alpha_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-06-26 09:36:51.000000 aleph-alpha-client-3.1.4/aleph_alpha_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-26 09:36:52.000000 aleph-alpha-client-3.1.4/aleph_alpha_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:36:51.000000 aleph-alpha-client-3.1.4/aleph_alpha_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-26 09:36:52.000000 aleph-alpha-client-3.1.4/aleph_alpha_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 09:36:52.000000 aleph-alpha-client-3.1.4/aleph_alpha_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 09:36:52.016419 aleph-alpha-client-3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:36:52.016419 aleph-alpha-client-3.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_detokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 09:36:42.000000 aleph-alpha-client-3.1.4/tests/test_wildcard_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:16:12.354924 aleph-alpha-client-3.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-10 09:16:12.354924 aleph-alpha-client-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:16:12.350924 aleph-alpha-client-3.1.5/aleph_alpha_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34335 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/aleph_alpha_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/detokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:16:12.350924 aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-10 09:16:12.000000 aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-10 09:16:12.000000 aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:16:12.000000 aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-10 09:16:12.000000 aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 09:16:12.000000 aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:16:12.354924 aleph-alpha-client-3.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:16:12.354924 aleph-alpha-client-3.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_detokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_wildcard_import.py
```

### Comparing `aleph-alpha-client-3.1.4/LICENSE` & `aleph-alpha-client-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/PKG-INFO` & `aleph-alpha-client-3.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 3.1.4
+Version: 3.1.5
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aleph-alpha-client-3.1.4/README.md` & `aleph-alpha-client-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client/__init__.py` & `aleph-alpha-client-3.1.5/aleph_alpha_client/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     TargetScore,
     TextPromptItemExplanation,
     TextScore,
     TokenPromptItemExplanation,
     TokenScore,
 )
 from .qa import QaRequest, QaResponse
-from .search import SearchRequest, SearchResponse, SearchResult
 from .summarization import SummarizationRequest, SummarizationResponse
 from .tokenization import TokenizationRequest, TokenizationResponse
 from .utils import load_base64_from_file, load_base64_from_url
 from .version import __version__
 
 __all__ = [
     "AsyncClient",
@@ -73,17 +72,14 @@
     "ImageScore",
     "POOLING_OPTIONS",
     "Prompt",
     "PromptGranularity",
     "QaRequest",
     "QaResponse",
     "QuotaError",
-    "SearchRequest",
-    "SearchResponse",
-    "SearchResult",
     "SemanticEmbeddingRequest",
     "SemanticEmbeddingResponse",
     "SemanticRepresentation",
     "SummarizationRequest",
     "SummarizationResponse",
     "TargetGranularity",
     "TargetPromptItemExplanation",
```

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client/aleph_alpha_client.py` & `aleph-alpha-client-3.1.5/aleph_alpha_client/aleph_alpha_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 )
 from aleph_alpha_client.embedding import (
     EmbeddingRequest,
     EmbeddingResponse,
     SemanticEmbeddingRequest,
     SemanticEmbeddingResponse,
 )
-from aleph_alpha_client.search import SearchRequest, SearchResponse
 
 POOLING_OPTIONS = ["mean", "max", "last_token", "abs_max"]
 RETRY_STATUS_CODES = frozenset({408, 429, 500, 502, 503, 504})
 DEFAULT_REQUEST_TIMEOUT = 305
 
 
 class QuotaError(Exception):
@@ -71,15 +70,14 @@
     TokenizationRequest,
     DetokenizationRequest,
     SemanticEmbeddingRequest,
     QaRequest,
     SummarizationRequest,
     ExplanationRequest,
     ExplanationRequest,
-    SearchRequest,
 ]
 
 
 class Client:
     """
     Construct a client for synchronous requests given a user token
 
@@ -127,15 +125,14 @@
         token: str,
         host: str = "https://api.aleph-alpha.com",
         hosting: Optional[str] = None,
         request_timeout_seconds: int = DEFAULT_REQUEST_TIMEOUT,
         total_retries: int = 8,
         nice: bool = False,
     ) -> None:
-
         if host[-1] != "/":
             host += "/"
         self.host = host
         self.hosting = hosting
         self.request_timeout_seconds = request_timeout_seconds
         self.token = token
         self.nice = nice
@@ -171,15 +168,14 @@
 
     def _post_request(
         self,
         endpoint: str,
         request: AnyRequest,
         model: Optional[str] = None,
     ) -> Dict[str, Any]:
-
         json_body = self._build_json_body(request, model)
 
         query_params = self._build_query_parameters()
 
         response = self.session.post(
             self.host + endpoint,
             json=json_body,
@@ -476,24 +472,14 @@
         response = self._post_request(
             "explain",
             request,
             model,
         )
         return ExplanationResponse.from_json(response)
 
-    def _search(
-        self,
-        request: SearchRequest,
-    ) -> SearchResponse:
-        """
-        For details see https://www.aleph-alpha.com/luminous-explore-a-model-for-world-class-semantic-representation
-        """
-        response = self._post_request("search", request, None)
-        return SearchResponse.from_json(response)
-
     def tokenizer(self, model: str) -> Tokenizer:
         """Returns a Tokenizer instance with the settings that were used to train the model.
 
         Examples:
             >>> tokenizer = client.tokenizer(model="luminous-extended")
             >>> tokenized_prompt = tokenizer.encode("Hello world")
         """
@@ -628,15 +614,14 @@
 
     async def _post_request(
         self,
         endpoint: str,
         request: AnyRequest,
         model: Optional[str] = None,
     ) -> Dict[str, Any]:
-
         json_body = self._build_json_body(request, model)
 
         query_params = self._build_query_parameters()
 
         async with self.session.post(
             self.host + endpoint, json=json_body, params=query_params
         ) as response:
@@ -927,24 +912,14 @@
         response = await self._post_request(
             "explain",
             request,
             model,
         )
         return ExplanationResponse.from_json(response)
 
-    async def _search(
-        self,
-        request: SearchRequest,
-    ) -> SearchResponse:
-        """
-        For details see https://www.aleph-alpha.com/luminous-explore-a-model-for-world-class-semantic-representation
-        """
-        response = await self._post_request("search", request, None)
-        return SearchResponse.from_json(response)
-
     async def tokenizer(self, model: str) -> Tokenizer:
         """Returns a Tokenizer instance with the settings that were used to train the model.
 
         Examples:
             >>> tokenizer = await client.tokenizer(model="luminous-extended")
             >>> tokenized_prompt = tokenizer.encode("Hello world")
         """
```

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client/completion.py` & `aleph-alpha-client-3.1.5/aleph_alpha_client/completion.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client/detokenization.py` & `aleph-alpha-client-3.1.5/aleph_alpha_client/detokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client/document.py` & `aleph-alpha-client-3.1.5/aleph_alpha_client/document.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client/embedding.py` & `aleph-alpha-client-3.1.5/aleph_alpha_client/embedding.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client/evaluation.py` & `aleph-alpha-client-3.1.5/aleph_alpha_client/evaluation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client/explanation.py` & `aleph-alpha-client-3.1.5/aleph_alpha_client/explanation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client/prompt.py` & `aleph-alpha-client-3.1.5/aleph_alpha_client/prompt.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client/qa.py` & `aleph-alpha-client-3.1.5/aleph_alpha_client/qa.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client/summarization.py` & `aleph-alpha-client-3.1.5/aleph_alpha_client/summarization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client/tokenization.py` & `aleph-alpha-client-3.1.5/aleph_alpha_client/tokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client.egg-info/PKG-INFO` & `aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 3.1.4
+Version: 3.1.5
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aleph-alpha-client-3.1.4/aleph_alpha_client.egg-info/SOURCES.txt` & `aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 aleph_alpha_client/detokenization.py
 aleph_alpha_client/document.py
 aleph_alpha_client/embedding.py
 aleph_alpha_client/evaluation.py
 aleph_alpha_client/explanation.py
 aleph_alpha_client/prompt.py
 aleph_alpha_client/qa.py
-aleph_alpha_client/search.py
 aleph_alpha_client/summarization.py
 aleph_alpha_client/tokenization.py
 aleph_alpha_client/utils.py
 aleph_alpha_client/version.py
 aleph_alpha_client.egg-info/PKG-INFO
 aleph_alpha_client.egg-info/SOURCES.txt
 aleph_alpha_client.egg-info/dependency_links.txt
@@ -28,11 +27,10 @@
 tests/test_embed.py
 tests/test_error_handling.py
 tests/test_evaluate.py
 tests/test_explanation.py
 tests/test_image.py
 tests/test_prompt.py
 tests/test_qa.py
-tests/test_search.py
 tests/test_summarize.py
 tests/test_tokenize.py
 tests/test_wildcard_import.py
```

### Comparing `aleph-alpha-client-3.1.4/setup.py` & `aleph-alpha-client-3.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/tests/test_clients.py` & `aleph-alpha-client-3.1.5/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/tests/test_complete.py` & `aleph-alpha-client-3.1.5/tests/test_complete.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/tests/test_detokenize.py` & `aleph-alpha-client-3.1.5/tests/test_detokenize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/tests/test_embed.py` & `aleph-alpha-client-3.1.5/tests/test_embed.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/tests/test_error_handling.py` & `aleph-alpha-client-3.1.5/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/tests/test_evaluate.py` & `aleph-alpha-client-3.1.5/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/tests/test_explanation.py` & `aleph-alpha-client-3.1.5/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/tests/test_image.py` & `aleph-alpha-client-3.1.5/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/tests/test_prompt.py` & `aleph-alpha-client-3.1.5/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/tests/test_qa.py` & `aleph-alpha-client-3.1.5/tests/test_qa.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,58 +8,54 @@
     model_name,
     async_client,
 )
 
 # AsyncClient
 
 
-@pytest.mark.system_test
 async def test_can_qa_with_async_client(async_client: AsyncClient):
     request = QaRequest(
         query="Who likes pizza?",
         documents=[Document.from_text("Andreas likes pizza.")],
     )
 
     response = await async_client.qa(request)
     assert len(response.answers) == 1
     assert response.answers[0].score > 0.0
 
 
 # Client
 
 
-@pytest.mark.system_test
 def test_qa(sync_client: Client):
     # when posting a QA request with a QaRequest object
     request = QaRequest(
         query="Who likes pizza?",
         documents=[Document.from_prompt(["Andreas likes pizza."])],
     )
 
     response = sync_client.qa(request)
 
     # the response should exist and be in the form of a named tuple class
     assert len(response.answers) == 1
 
 
-@pytest.mark.system_test
 def test_qa_no_answer_found(sync_client: Client):
     # when posting a QA request with a QaRequest object
     request = QaRequest(
         query="Who likes pizza?",
         documents=[],
     )
 
     response = sync_client.qa(request)
 
     # the response should exist and be in the form of a named tuple class
     assert len(response.answers) == 0
 
 
-@pytest.mark.system_test
 def test_text(sync_client: Client):
     # when posting an illegal request
     request = QaRequest(
         query="Who likes pizza?",
         documents=[Document.from_text("Andreas likes pizza.")],
     )
```

### Comparing `aleph-alpha-client-3.1.4/tests/test_summarize.py` & `aleph-alpha-client-3.1.5/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.4/tests/test_tokenize.py` & `aleph-alpha-client-3.1.5/tests/test_tokenize.py`

 * *Files identical despite different names*

