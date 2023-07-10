# Comparing `tmp/bnlp_toolkit-3.3.1.tar.gz` & `tmp/bnlp_toolkit-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnlp_toolkit-3.3.1.tar", last modified: Sat Apr 29 03:41:10 2023, max compression
+gzip compressed data, was "bnlp_toolkit-3.3.2.tar", last modified: Mon Jul 10 05:51:39 2023, max compression
```

## Comparing `bnlp_toolkit-3.3.1.tar` & `bnlp_toolkit-3.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.691246 bnlp_toolkit-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-04-29 03:41:10.691246 bnlp_toolkit-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22844 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.687246 bnlp_toolkit-3.3.1/bnlp/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.687246 bnlp_toolkit-3.3.1/bnlp/cleantext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/cleantext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/cleantext/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/cleantext/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.687246 bnlp_toolkit-3.3.1/bnlp/corpus/
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/corpus/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.687246 bnlp_toolkit-3.3.1/bnlp/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/embedding/doc2vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/embedding/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/embedding/glove.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/embedding/word2vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/pos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.687246 bnlp_toolkit-3.3.1/bnlp/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/tokenizer/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/tokenizer/nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/tokenizer/sentencepiece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.691246 bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-04-29 03:41:10.000000 bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-29 03:41:10.000000 bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 03:41:10.000000 bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-29 03:41:10.000000 bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 03:41:10.000000 bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 03:41:10.691246 bnlp_toolkit-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.691246 bnlp_toolkit-3.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.023692 bnlp_toolkit-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-07-10 05:51:39.023692 bnlp_toolkit-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22844 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.019692 bnlp_toolkit-3.3.2/bnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.019692 bnlp_toolkit-3.3.2/bnlp/cleantext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/cleantext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/cleantext/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/cleantext/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.019692 bnlp_toolkit-3.3.2/bnlp/corpus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/corpus/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.019692 bnlp_toolkit-3.3.2/bnlp/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/embedding/doc2vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/embedding/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/embedding/glove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/embedding/word2vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/pos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.019692 bnlp_toolkit-3.3.2/bnlp/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/tokenizer/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/tokenizer/nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/tokenizer/sentencepiece.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.023692 bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-07-10 05:51:39.000000 bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-10 05:51:39.000000 bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 05:51:39.000000 bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-10 05:51:39.000000 bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 05:51:39.000000 bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 05:51:39.023692 bnlp_toolkit-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.023692 bnlp_toolkit-3.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/tests/test.py
```

### Comparing `bnlp_toolkit-3.3.1/LICENSE` & `bnlp_toolkit-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.1/PKG-INFO` & `bnlp_toolkit-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnlp_toolkit
-Version: 3.3.1
+Version: 3.3.2
 Summary: BNLP is a natural language processing toolkit for Bengali Language
 Home-page: https://github.com/sagorbrur/bnlp
 Author: Sagor Sarker
 Author-email: sagorhem3532@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bnlp_toolkit-3.3.1/README.md` & `bnlp_toolkit-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.1/bnlp/cleantext/clean.py` & `bnlp_toolkit-3.3.2/bnlp/cleantext/clean.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.1/bnlp/cleantext/constants.py` & `bnlp_toolkit-3.3.2/bnlp/cleantext/constants.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.1/bnlp/corpus/__init__.py` & `bnlp_toolkit-3.3.2/bnlp/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.1/bnlp/embedding/doc2vec.py` & `bnlp_toolkit-3.3.2/bnlp/embedding/doc2vec.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.1/bnlp/embedding/fasttext.py` & `bnlp_toolkit-3.3.2/bnlp/embedding/fasttext.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.1/bnlp/embedding/glove.py` & `bnlp_toolkit-3.3.2/bnlp/embedding/glove.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.1/bnlp/embedding/word2vec.py` & `bnlp_toolkit-3.3.2/bnlp/embedding/word2vec.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.1/bnlp/ner.py` & `bnlp_toolkit-3.3.2/bnlp/ner.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.1/bnlp/pos.py` & `bnlp_toolkit-3.3.2/bnlp/pos.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.1/bnlp/tokenizer/basic.py` & `bnlp_toolkit-3.3.2/bnlp/tokenizer/basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,17 +66,14 @@
         """Tokenizes a piece of text."""
         text = convert_to_unicode(text)
 
         orig_tokens = whitespace_tokenize(text)
         # print("original tokens: ", orig_tokens)
         split_tokens = []
         for token in orig_tokens:
-            # if self.do_lower_case:
-            #   token = token.lower()
-            #   token = self._run_strip_accents(token)
             split_tokens.extend(self._run_split_on_punc(token))
 
         # print("split tokens: ", split_tokens)
         output_tokens = whitespace_tokenize(" ".join(split_tokens))
         return output_tokens
 
     def _run_strip_accents(self, text):
```

### Comparing `bnlp_toolkit-3.3.1/bnlp/tokenizer/nltk.py` & `bnlp_toolkit-3.3.2/bnlp/tokenizer/nltk.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 try:
     nltk.data.find("tokenizers/punkt")
 except LookupError:
     print("punkt not found. downloading...")
     nltk.download("punkt")
 
+DUMMYTOKEN = "XTEMPTOKEN"
 
 class NLTKTokenizer:
     def word_tokenize(self, text):
         tokens = nltk.word_tokenize(text)
         new_tokens = []
         for token in tokens:
             if token[-1] == "।" and len(token) > 1:
@@ -18,16 +19,16 @@
                 new_tokens.append(token_1)
                 new_tokens.append(token_2)
             else:
                 new_tokens.append(token)
         return new_tokens
 
     def sentence_tokenize(self, text):
-        text = text.replace(".", "<dummy_bangla_token>")  # to deal with abbreviations
+        text = text.replace(".", DUMMYTOKEN)  # to deal with abbreviations
         text = text.replace("।", ".")
         tokens = nltk.tokenize.sent_tokenize(text)
         new_tokens = []
         for token in tokens:
             token = token.replace(".", "।")  # do operation in reverse order
-            token = token.replace("<dummy_bangla_token>", ".")
+            token = token.replace(DUMMYTOKEN, ".")
             new_tokens.append(token)
         return new_tokens
```

### Comparing `bnlp_toolkit-3.3.1/bnlp/tokenizer/sentencepiece.py` & `bnlp_toolkit-3.3.2/bnlp/tokenizer/sentencepiece.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/PKG-INFO` & `bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnlp-toolkit
-Version: 3.3.1
+Version: 3.3.2
 Summary: BNLP is a natural language processing toolkit for Bengali Language
 Home-page: https://github.com/sagorbrur/bnlp
 Author: Sagor Sarker
 Author-email: sagorhem3532@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/SOURCES.txt` & `bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.1/setup.py` & `bnlp_toolkit-3.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 import setuptools
 
 
 setuptools.setup(
     name="bnlp_toolkit",
-    version="3.3.1",
+    version="3.3.2",
     author="Sagor Sarker",
     author_email="sagorhem3532@gmail.com",
     description="BNLP is a natural language processing toolkit for Bengali Language",
     long_description=codecs.open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/sagorbrur/bnlp",
     license="MIT",
```

### Comparing `bnlp_toolkit-3.3.1/tests/test.py` & `bnlp_toolkit-3.3.2/tests/test.py`

 * *Files identical despite different names*

