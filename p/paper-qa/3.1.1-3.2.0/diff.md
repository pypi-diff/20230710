# Comparing `tmp/paper-qa-3.1.1.tar.gz` & `tmp/paper-qa-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.1.1.tar", last modified: Tue Jun 27 01:29:07 2023, max compression
+gzip compressed data, was "paper-qa-3.2.0.tar", last modified: Mon Jul 10 02:53:41 2023, max compression
```

## Comparing `paper-qa-3.1.1.tar` & `paper-qa-3.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:29:07.568499 paper-qa-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 01:28:22.000000 paper-qa-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-27 01:29:07.568499 paper-qa-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-27 01:28:22.000000 paper-qa-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:29:07.564499 paper-qa-3.1.1/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-27 01:29:07.000000 paper-qa-3.1.1/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 01:29:07.000000 paper-qa-3.1.1/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 01:29:07.000000 paper-qa-3.1.1/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-27 01:29:07.000000 paper-qa-3.1.1/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 01:29:07.000000 paper-qa-3.1.1/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:29:07.568499 paper-qa-3.1.1/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:29:07.568499 paper-qa-3.1.1/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    22564 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 01:29:07.568499 paper-qa-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-27 01:28:22.000000 paper-qa-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:29:07.568499 paper-qa-3.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-06-27 01:28:22.000000 paper-qa-3.1.1/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:41.886588 paper-qa-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 02:52:56.000000 paper-qa-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-10 02:53:41.886588 paper-qa-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-10 02:52:56.000000 paper-qa-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:41.882588 paper-qa-3.2.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-10 02:53:41.000000 paper-qa-3.2.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-10 02:53:41.000000 paper-qa-3.2.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 02:53:41.000000 paper-qa-3.2.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 02:53:41.000000 paper-qa-3.2.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 02:53:41.000000 paper-qa-3.2.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:41.886588 paper-qa-3.2.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:41.886588 paper-qa-3.2.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 02:52:56.000000 paper-qa-3.2.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 02:53:41.886588 paper-qa-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-10 02:52:56.000000 paper-qa-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:41.886588 paper-qa-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-07-10 02:52:56.000000 paper-qa-3.2.0/tests/test_paperqa.py
```

### Comparing `paper-qa-3.1.1/LICENSE` & `paper-qa-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.1/PKG-INFO` & `paper-qa-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.1.1
+Version: 3.2.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.1.1/README.md` & `paper-qa-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.1/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.2.0/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.1.1
+Version: 3.2.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.1.1/paperqa/chains.py` & `paper-qa-3.2.0/paperqa/chains.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.1/paperqa/contrib/zotero.py` & `paper-qa-3.2.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.1/paperqa/docs.py` & `paper-qa-3.2.0/paperqa/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,15 +253,15 @@
                 self.texts_index.add_embeddings(  # type: ignore
                     vec_store_text_and_embeddings,
                     metadatas=[t.dict(exclude={"embeddings", "text"}) for t in texts],
                 )
             except AttributeError:
                 raise ValueError("Need a vector store that supports adding embeddings.")
         if self.doc_index is not None:
-            self.doc_index.add_texts([doc.citation], metadatas=[{"dockey": doc.dockey}])
+            self.doc_index.add_texts([doc.citation], metadatas=[doc.dict()])
         self.docs[doc.dockey] = doc
         self.texts += texts
         self.docnames.add(doc.docname)
         return True
 
     def delete(
         self, name: Optional[str] = None, dockey: Optional[DocKey] = None
@@ -287,15 +287,25 @@
             metadatas = [d.dict() for d in self.docs.values()]
             self.doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
         matches = self.doc_index.max_marginal_relevance_search(
             query, k=k + len(self.deleted_dockeys)
         )
-        matched_docs = [self.docs[m.metadata["dockey"]] for m in matches]
+        # filter the matches
+        matches = [
+            m for m in matches if m.metadata["dockey"] not in self.deleted_dockeys
+        ]
+        try:
+            # for backwards compatibility (old pickled objects)
+            matched_docs = [self.docs[m.metadata["dockey"]] for m in matches]
+        except KeyError:
+            matched_docs = [Doc(**m.metadata) for m in matches]
+        if len(matched_docs) == 0:
+            return set()
         chain = make_chain(
             self.prompts.select, cast(BaseLanguageModel, self.llm), skip_system=True
         )
         papers = [f"{d.docname}: {d.citation}" for d in matched_docs]
         result = await chain.arun(  # type: ignore
             question=query, papers="\n".join(papers), callbacks=get_callbacks("filter")
         )
@@ -368,15 +378,15 @@
         self,
         answer: Answer,
         k: int = 3,
         max_sources: int = 5,
         marginal_relevance: bool = True,
         get_callbacks: CallbackFactory = lambda x: None,
     ) -> Answer:
-        if len(self.docs) == 0:
+        if len(self.docs) == 0 and self.doc_index is None:
             return answer
         if self.texts_index is None:
             self._build_texts_index()
         self.texts_index = cast(VectorStore, self.texts_index)
         _k = k
         if answer.dockey_filter is not None:
             _k = k * 10  # heuristic
```

### Comparing `paper-qa-3.1.1/paperqa/prompts.py` & `paper-qa-3.2.0/paperqa/prompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.1/paperqa/readers.py` & `paper-qa-3.2.0/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.1/paperqa/types.py` & `paper-qa-3.2.0/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.1/paperqa/utils.py` & `paper-qa-3.2.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.1/setup.py` & `paper-qa-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.1/tests/test_paperqa.py` & `paper-qa-3.2.0/tests/test_paperqa.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,16 +191,14 @@
                 question="What date is bring your dog to work in the US?",
                 summary_length="about 20 words",
             ),
             k=3,
             max_sources=1,
         ).context,
     )
-    print(context1)
-    print(context2)
     assert strings_similarity(context1, context2) > 0.75
     # make sure we can query
     docs.query("What date is bring your dog to work in the US?")
 
 
 def test_docs_pickle_no_faiss():
     doc_path = "example.txt"
@@ -584,33 +582,48 @@
     docs = Docs(llm=llm)
     docs.add_url(
         "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day",
         citation="WikiMedia Foundation, 2023, Accessed now",
         dockey="test",
     )
 
-    docs2 = Docs(llm=llm)
+    docs2 = Docs()
     texts = [Text(**dict(t)) for t in docs.texts]
     for t in texts:
         t.embeddings = None
     docs2.add_texts(texts, list(docs.docs.values())[0])
 
     for t1, t2 in zip(docs2.texts, docs.texts):
         assert t1.text == t2.text
         assert np.allclose(t1.embeddings, t2.embeddings, atol=1e-3)
 
     docs2._build_texts_index()
-    print("BUILT NOW")
     # now do it again to test after text index is already built
     llm = OpenAI(client=None, temperature=0.1, model="text-ada-001")
     docs = Docs(llm=llm)
     docs.add_url(
         "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
         citation="WikiMedia Foundation, 2023, Accessed now",
         dockey="test3",
     )
 
     texts = [Text(**dict(t)) for t in docs.texts]
     for t in texts:
         t.embeddings = None
     docs2.add_texts(texts, list(docs.docs.values())[0])
     assert len(docs2.docs) == 2
+
+    docs2.query("What country was Bates Born in?")
+
+
+def test_external_doc_index():
+    docs = Docs()
+    docs.add_url(
+        "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day",
+        citation="WikiMedia Foundation, 2023, Accessed now",
+        dockey="test",
+    )
+    evidence = docs.query(query="What is the date of flag day?", key_filter=True)
+    docs2 = Docs(doc_index=docs.doc_index, texts_index=docs.texts_index)
+    assert len(docs2.docs) == 0
+    evidence = docs2.query("What is the date of flag day?", key_filter=True)
+    assert "February 15" in evidence.context
```

