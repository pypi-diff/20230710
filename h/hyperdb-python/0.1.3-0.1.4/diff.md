# Comparing `tmp/hyperdb-python-0.1.3.tar.gz` & `tmp/hyperdb-python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdb-python-0.1.3.tar", last modified: Fri May  5 03:06:37 2023, max compression
+gzip compressed data, was "hyperdb-python-0.1.4.tar", last modified: Mon Jul 10 00:34:47 2023, max compression
```

## Comparing `hyperdb-python-0.1.3.tar` & `hyperdb-python-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-05-05 03:06:37.204128 hyperdb-python-0.1.3/
--rw-r--r--   0 jdagdelen   (501) staff       (20)     1070 2023-04-16 06:27:54.000000 hyperdb-python-0.1.3/LICENSE
--rw-r--r--   0 jdagdelen   (501) staff       (20)     3141 2023-05-05 03:06:37.203943 hyperdb-python-0.1.3/PKG-INFO
--rw-r--r--   0 jdagdelen   (501) staff       (20)     2485 2023-05-05 03:06:29.000000 hyperdb-python-0.1.3/README.md
-drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-05-05 03:06:37.202419 hyperdb-python-0.1.3/hyperdb/
--rw-r--r--   0 jdagdelen   (501) staff       (20)       22 2023-04-16 07:55:26.000000 hyperdb-python-0.1.3/hyperdb/__init__.py
--rw-r--r--   0 jdagdelen   (501) staff       (20)     1733 2023-05-05 03:06:29.000000 hyperdb-python-0.1.3/hyperdb/galaxy_brain_math_shit.py
--rw-r--r--   0 jdagdelen   (501) staff       (20)     4887 2023-05-05 03:06:29.000000 hyperdb-python-0.1.3/hyperdb/hyperdb.py
-drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-05-05 03:06:37.203279 hyperdb-python-0.1.3/hyperdb_python.egg-info/
--rw-r--r--   0 jdagdelen   (501) staff       (20)     3141 2023-05-05 03:06:37.000000 hyperdb-python-0.1.3/hyperdb_python.egg-info/PKG-INFO
--rw-r--r--   0 jdagdelen   (501) staff       (20)      343 2023-05-05 03:06:37.000000 hyperdb-python-0.1.3/hyperdb_python.egg-info/SOURCES.txt
--rw-r--r--   0 jdagdelen   (501) staff       (20)        1 2023-05-05 03:06:37.000000 hyperdb-python-0.1.3/hyperdb_python.egg-info/dependency_links.txt
--rw-r--r--   0 jdagdelen   (501) staff       (20)       13 2023-05-05 03:06:37.000000 hyperdb-python-0.1.3/hyperdb_python.egg-info/requires.txt
--rw-r--r--   0 jdagdelen   (501) staff       (20)       14 2023-05-05 03:06:37.000000 hyperdb-python-0.1.3/hyperdb_python.egg-info/top_level.txt
--rw-r--r--   0 jdagdelen   (501) staff       (20)       38 2023-05-05 03:06:37.204179 hyperdb-python-0.1.3/setup.cfg
--rw-r--r--   0 jdagdelen   (501) staff       (20)      937 2023-05-05 03:06:12.000000 hyperdb-python-0.1.3/setup.py
-drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-05-05 03:06:37.203722 hyperdb-python-0.1.3/tests/
--rw-r--r--   0 jdagdelen   (501) staff       (20)        0 2023-05-05 03:06:29.000000 hyperdb-python-0.1.3/tests/__init__.py
--rw-r--r--   0 jdagdelen   (501) staff       (20)      498 2023-05-05 03:06:29.000000 hyperdb-python-0.1.3/tests/test_galaxy_brain_math_shit.py
+drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-07-10 00:34:47.279130 hyperdb-python-0.1.4/
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     1070 2023-07-10 00:31:39.000000 hyperdb-python-0.1.4/LICENSE
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     3142 2023-07-10 00:34:47.278953 hyperdb-python-0.1.4/PKG-INFO
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     2486 2023-07-10 00:31:39.000000 hyperdb-python-0.1.4/README.md
+drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-07-10 00:34:47.277720 hyperdb-python-0.1.4/hyperdb/
+-rw-r--r--   0 jdagdelen   (501) staff       (20)       22 2023-07-10 00:31:39.000000 hyperdb-python-0.1.4/hyperdb/__init__.py
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     1849 2023-07-10 00:31:39.000000 hyperdb-python-0.1.4/hyperdb/galaxy_brain_math_shit.py
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     5707 2023-07-10 00:31:39.000000 hyperdb-python-0.1.4/hyperdb/hyperdb.py
+drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-07-10 00:34:47.278522 hyperdb-python-0.1.4/hyperdb_python.egg-info/
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     3142 2023-07-10 00:34:47.000000 hyperdb-python-0.1.4/hyperdb_python.egg-info/PKG-INFO
+-rw-r--r--   0 jdagdelen   (501) staff       (20)      343 2023-07-10 00:34:47.000000 hyperdb-python-0.1.4/hyperdb_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jdagdelen   (501) staff       (20)        1 2023-07-10 00:34:47.000000 hyperdb-python-0.1.4/hyperdb_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jdagdelen   (501) staff       (20)       13 2023-07-10 00:34:47.000000 hyperdb-python-0.1.4/hyperdb_python.egg-info/requires.txt
+-rw-r--r--   0 jdagdelen   (501) staff       (20)       14 2023-07-10 00:34:47.000000 hyperdb-python-0.1.4/hyperdb_python.egg-info/top_level.txt
+-rw-r--r--   0 jdagdelen   (501) staff       (20)       38 2023-07-10 00:34:47.279180 hyperdb-python-0.1.4/setup.cfg
+-rw-r--r--   0 jdagdelen   (501) staff       (20)      937 2023-07-10 00:34:45.000000 hyperdb-python-0.1.4/setup.py
+drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-07-10 00:34:47.278759 hyperdb-python-0.1.4/tests/
+-rw-r--r--   0 jdagdelen   (501) staff       (20)        0 2023-07-10 00:31:39.000000 hyperdb-python-0.1.4/tests/__init__.py
+-rw-r--r--   0 jdagdelen   (501) staff       (20)      498 2023-07-10 00:31:39.000000 hyperdb-python-0.1.4/tests/test_galaxy_brain_math_shit.py
```

### Comparing `hyperdb-python-0.1.3/LICENSE` & `hyperdb-python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperdb-python-0.1.3/PKG-INFO` & `hyperdb-python-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdb-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: A hyper-fast local vector database for use with LLM Agents.
 Home-page: https://github.com/jdagdelen/hyperdb
 Author: John Dagdelen
 Author-email: jjdagdelen@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 # HyperDB
 <div>
 <img src="https://github.com/jdagdelen/hyperDB/blob/main/_static/logo.png?raw=true" width="400" alt="HyperDB Logo">
 </div>
 
 A hyper-fast local vector database for use with LLM Agents. 
 
-Want to invest? [Now accepting SAFEs ($35M cap minimum.)](https://www.youtube.com/watch?v=QH2-TGUlwu4)
+Want to invest? [Now accepting SAFEs ($135M cap minimum.)](https://www.youtube.com/watch?v=QH2-TGUlwu4)
 
 Join the [HyperDBiscord](https://discord.gg/8YQzexAA)
 
 ## Advantages
 * Simple interface compatible with _all_ large language model agents. 
 * Highly optimized C++ backend vector store with HW accelerated operations via MKL BLAS. 
 * Enables users to index documents with advanced features such as _ids_ and _metadata_.
```

### Comparing `hyperdb-python-0.1.3/README.md` & `hyperdb-python-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # HyperDB
 <div>
 <img src="https://github.com/jdagdelen/hyperDB/blob/main/_static/logo.png?raw=true" width="400" alt="HyperDB Logo">
 </div>
 
 A hyper-fast local vector database for use with LLM Agents. 
 
-Want to invest? [Now accepting SAFEs ($35M cap minimum.)](https://www.youtube.com/watch?v=QH2-TGUlwu4)
+Want to invest? [Now accepting SAFEs ($135M cap minimum.)](https://www.youtube.com/watch?v=QH2-TGUlwu4)
 
 Join the [HyperDBiscord](https://discord.gg/8YQzexAA)
 
 ## Advantages
 * Simple interface compatible with _all_ large language model agents. 
 * Highly optimized C++ backend vector store with HW accelerated operations via MKL BLAS. 
 * Enables users to index documents with advanced features such as _ids_ and _metadata_.
```

### Comparing `hyperdb-python-0.1.3/hyperdb/galaxy_brain_math_shit.py` & `hyperdb-python-0.1.4/hyperdb/galaxy_brain_math_shit.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 def get_norm_vector(vector):
     if len(vector.shape) == 1:
         return vector / np.linalg.norm(vector)
     else:
         return vector / np.linalg.norm(vector, axis=1)[:, np.newaxis]
 
+def dot_product(vectors, query_vector):
+    similarities = np.dot(vectors, query_vector.T)
+    return similarities
+
 def cosine_similarity(vectors, query_vector):
     norm_vectors = get_norm_vector(vectors)
     norm_query_vector = get_norm_vector(query_vector)
     similarities = np.dot(norm_vectors, norm_query_vector.T)
     return similarities
 
 def euclidean_metric(vectors, query_vector, get_similarity_score=True):
```

### Comparing `hyperdb-python-0.1.3/hyperdb/hyperdb.py` & `hyperdb-python-0.1.4/hyperdb/hyperdb.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,135 @@
+import gzip
 import pickle
+
 import numpy as np
-import gzip
 import openai
-from hyperdb.galaxy_brain_math_shit import cosine_similarity, euclidean_metric, derridaean_similarity, adams_similarity, hyper_SVM_ranking_algorithm_sort
+
+from hyperdb.galaxy_brain_math_shit import (
+    dot_product,
+    adams_similarity,
+    cosine_similarity,
+    derridaean_similarity,
+    euclidean_metric,
+    hyper_SVM_ranking_algorithm_sort,
+)
+
+MAX_BATCH_SIZE = 2048  # OpenAI batch endpoint max size https://github.com/openai/openai-python/blob/main/openai/embeddings_utils.py#L43
+
 
 def get_embedding(documents, key=None, model="text-embedding-ada-002"):
     """Default embedding function that uses OpenAI Embeddings."""
     if isinstance(documents, list):
         if isinstance(documents[0], dict):
             texts = []
             if isinstance(key, str):
                 if "." in key:
                     key_chain = key.split(".")
-                else: 
+                else:
                     key_chain = [key]
                 for doc in documents:
                     for key in key_chain:
                         doc = doc[key]
                     texts.append(doc.replace("\n", " "))
             elif key is None:
                 for doc in documents:
                     text = ", ".join([f"{key}: {value}" for key, value in doc.items()])
                     texts.append(text)
         elif isinstance(documents[0], str):
             texts = documents
-    response = openai.Embedding.create(input=texts, model=model)
-    return [np.array(item["embedding"]) for item in response["data"]]
+    batches = [
+        texts[i : i + MAX_BATCH_SIZE] for i in range(0, len(texts), MAX_BATCH_SIZE)
+    ]
+    embeddings = []
+    for batch in batches:
+        response = openai.Embedding.create(input=batch, model=model)
+        embeddings.extend(np.array(item["embedding"]) for item in response["data"])
+    return embeddings
 
 
 class HyperDB:
-    def __init__(self, documents=None, key=None, embedding_function=None, similarity_metric="cosine"):
+    def __init__(
+        self,
+        documents=None,
+        vectors=None,
+        key=None,
+        embedding_function=None,
+        similarity_metric="cosine",
+    ):
         documents = documents or []
         self.documents = []
-        self.embedding_function = embedding_function or (lambda docs: get_embedding(docs, key=key))
         self.vectors = None
-        self.add_documents(documents)
-        if similarity_metric.__contains__("cosine"):
+        self.embedding_function = embedding_function or (
+            lambda docs: get_embedding(docs, key=key)
+        )
+        if vectors is not None:
+            self.vectors = vectors
+            self.documents = documents
+        else:
+            self.add_documents(documents)
+
+        if similarity_metric.__contains__("dot"):
+            self.similarity_metric = dot_product
+        elif similarity_metric.__contains__("cosine"):
             self.similarity_metric = cosine_similarity
         elif similarity_metric.__contains__("euclidean"):
             self.similarity_metric = euclidean_metric
         elif similarity_metric.__contains__("derrida"):
             self.similarity_metric = derridaean_similarity
         elif similarity_metric.__contains__("adams"):
             self.similarity_metric = adams_similarity
         else:
-            raise Exception("Similarity metric not supported. Please use either 'cosine', 'euclidean', 'adams', or 'derrida'.")
+            raise Exception(
+                "Similarity metric not supported. Please use either 'dot', 'cosine', 'euclidean', 'adams', or 'derrida'."
+            )
 
     def dict(self, vectors=False):
         if vectors:
-            return [{
-                "document": document,
-                "vector": vector.tolist(),
-                "index": index
-            } for index, (document, vector) in enumerate(zip(self.documents, self.vectors))]
-        return [{"document": document, "index": index} for index, document in enumerate(self.documents)]
+            return [
+                {"document": document, "vector": vector.tolist(), "index": index}
+                for index, (document, vector) in enumerate(
+                    zip(self.documents, self.vectors)
+                )
+            ]
+        return [
+            {"document": document, "index": index}
+            for index, document in enumerate(self.documents)
+        ]
 
     def add(self, documents, vectors=None):
         if not isinstance(documents, list):
             return self.add_document(documents, vectors)
         self.add_documents(documents, vectors)
 
-    def add_document(self, document, vector=None):
-        vector = vector or self.embedding_function([document])[0]
+    def add_document(self, document: dict, vector=None):
+        vector = (
+            vector if vector is not None else self.embedding_function([document])[0]
+        )
         if self.vectors is None:
             self.vectors = np.empty((0, len(vector)), dtype=np.float32)
         elif len(vector) != self.vectors.shape[1]:
             raise ValueError("All vectors must have the same length.")
         self.vectors = np.vstack([self.vectors, vector]).astype(np.float32)
         self.documents.append(document)
 
     def remove_document(self, index):
         self.vectors = np.delete(self.vectors, index, axis=0)
         self.documents.pop(index)
 
     def add_documents(self, documents, vectors=None):
         if not documents:
             return
-        vectors = vectors or np.array(self.embedding_function(documents)).astype(np.float32)
+        vectors = vectors or np.array(self.embedding_function(documents)).astype(
+            np.float32
+        )
         for vector, document in zip(vectors, documents):
             self.add_document(document, vector)
 
     def save(self, storage_file):
-        data = {
-            "vectors": self.vectors,
-            "documents": self.documents
-        }
+        data = {"vectors": self.vectors, "documents": self.documents}
         if storage_file.endswith(".gz"):
             with gzip.open(storage_file, "wb") as f:
                 pickle.dump(data, f)
         else:
             with open(storage_file, "wb") as f:
                 pickle.dump(data, f)
 
@@ -101,15 +142,14 @@
                 data = pickle.load(f)
         self.vectors = data["vectors"].astype(np.float32)
         self.documents = data["documents"]
 
     def query(self, query_text, top_k=5, return_similarities=True):
         query_vector = self.embedding_function([query_text])[0]
         ranked_results, similarities = hyper_SVM_ranking_algorithm_sort(
-            self.vectors,
-            query_vector,
-            top_k=top_k,
-            metric=self.similarity_metric
+            self.vectors, query_vector, top_k=top_k, metric=self.similarity_metric
         )
         if return_similarities:
-            return list(zip([self.documents[index] for index in ranked_results], similarities))
+            return list(
+                zip([self.documents[index] for index in ranked_results], similarities)
+            )
         return [self.documents[index] for index in ranked_results]
```

### Comparing `hyperdb-python-0.1.3/hyperdb_python.egg-info/PKG-INFO` & `hyperdb-python-0.1.4/hyperdb_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdb-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: A hyper-fast local vector database for use with LLM Agents.
 Home-page: https://github.com/jdagdelen/hyperdb
 Author: John Dagdelen
 Author-email: jjdagdelen@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 # HyperDB
 <div>
 <img src="https://github.com/jdagdelen/hyperDB/blob/main/_static/logo.png?raw=true" width="400" alt="HyperDB Logo">
 </div>
 
 A hyper-fast local vector database for use with LLM Agents. 
 
-Want to invest? [Now accepting SAFEs ($35M cap minimum.)](https://www.youtube.com/watch?v=QH2-TGUlwu4)
+Want to invest? [Now accepting SAFEs ($135M cap minimum.)](https://www.youtube.com/watch?v=QH2-TGUlwu4)
 
 Join the [HyperDBiscord](https://discord.gg/8YQzexAA)
 
 ## Advantages
 * Simple interface compatible with _all_ large language model agents. 
 * Highly optimized C++ backend vector store with HW accelerated operations via MKL BLAS. 
 * Enables users to index documents with advanced features such as _ids_ and _metadata_.
```

### Comparing `hyperdb-python-0.1.3/setup.py` & `hyperdb-python-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="hyperdb-python",
-    version="0.1.3",
+    version="0.1.4",
     author="John Dagdelen",
     author_email="jjdagdelen@gmail.com",
     description="A hyper-fast local vector database for use with LLM Agents.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jdagdelen/hyperdb",
     packages=find_packages(),
```

