# Comparing `tmp/UniTok-3.1.8.tar.gz` & `tmp/UniTok-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniTok-3.1.8.tar", last modified: Mon Jul 10 05:28:57 2023, max compression
+gzip compressed data, was "UniTok-3.1.9.tar", last modified: Mon Jul 10 05:40:28 2023, max compression
```

## Comparing `UniTok-3.1.8.tar` & `UniTok-3.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:28:57.110200 UniTok-3.1.8/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-07-10 05:28:57.110082 UniTok-3.1.8/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.1.8/README.md
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:28:57.106563 UniTok-3.1.8/UniTok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.1.8/UniTok/__init__.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:28:57.107864 UniTok-3.1.8/UniTok/analysis/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.1.8/UniTok/analysis/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.1.8/UniTok/analysis/lengths.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.1.8/UniTok/analysis/plot.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.1.8/UniTok/cols.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     3787 2023-04-21 12:19:35.000000 UniTok-3.1.8/UniTok/column.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.1.8/UniTok/global_setting.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     4358 2023-07-10 05:28:17.000000 UniTok-3.1.8/UniTok/meta.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:28:57.109772 UniTok-3.1.8/UniTok/tok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.1.8/UniTok/tok/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      911 2023-04-21 12:17:40.000000 UniTok-3.1.8/UniTok/tok/bert_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.1.8/UniTok/tok/ent_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.1.8/UniTok/tok/id_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1442 2023-04-21 12:17:40.000000 UniTok-3.1.8/UniTok/tok/number_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.1.8/UniTok/tok/seq_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.1.8/UniTok/tok/split_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1697 2023-04-21 12:21:10.000000 UniTok-3.1.8/UniTok/tok/tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     9129 2023-07-10 05:28:17.000000 UniTok-3.1.8/UniTok/unidep.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6665 2023-04-21 13:00:13.000000 UniTok-3.1.8/UniTok/unitok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8788 2023-04-21 12:18:43.000000 UniTok-3.1.8/UniTok/vocab.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1685 2023-07-10 05:17:38.000000 UniTok-3.1.8/UniTok/vocabs.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:28:57.107183 UniTok-3.1.8/UniTok.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-07-10 05:28:57.000000 UniTok-3.1.8/UniTok.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-07-10 05:28:57.000000 UniTok-3.1.8/UniTok.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-07-10 05:28:57.000000 UniTok-3.1.8/UniTok.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-07-10 05:28:57.000000 UniTok-3.1.8/UniTok.egg-info/requires.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-07-10 05:28:57.000000 UniTok-3.1.8/UniTok.egg-info/top_level.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-07-10 05:28:57.110235 UniTok-3.1.8/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      724 2023-07-10 05:28:17.000000 UniTok-3.1.8/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:40:28.445107 UniTok-3.1.9/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-07-10 05:40:28.444973 UniTok-3.1.9/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.1.9/README.md
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:40:28.441275 UniTok-3.1.9/UniTok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.1.9/UniTok/__init__.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:40:28.442533 UniTok-3.1.9/UniTok/analysis/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.1.9/UniTok/analysis/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.1.9/UniTok/analysis/lengths.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.1.9/UniTok/analysis/plot.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.1.9/UniTok/cols.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     3787 2023-04-21 12:19:35.000000 UniTok-3.1.9/UniTok/column.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.1.9/UniTok/global_setting.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     4358 2023-07-10 05:28:17.000000 UniTok-3.1.9/UniTok/meta.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:40:28.444666 UniTok-3.1.9/UniTok/tok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.1.9/UniTok/tok/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      911 2023-04-21 12:17:40.000000 UniTok-3.1.9/UniTok/tok/bert_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.1.9/UniTok/tok/ent_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.1.9/UniTok/tok/id_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1442 2023-04-21 12:17:40.000000 UniTok-3.1.9/UniTok/tok/number_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.1.9/UniTok/tok/seq_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.1.9/UniTok/tok/split_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1697 2023-04-21 12:21:10.000000 UniTok-3.1.9/UniTok/tok/tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     9148 2023-07-10 05:39:24.000000 UniTok-3.1.9/UniTok/unidep.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6665 2023-04-21 13:00:13.000000 UniTok-3.1.9/UniTok/unitok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8788 2023-04-21 12:18:43.000000 UniTok-3.1.9/UniTok/vocab.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1685 2023-07-10 05:17:38.000000 UniTok-3.1.9/UniTok/vocabs.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:40:28.441959 UniTok-3.1.9/UniTok.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-07-10 05:40:28.000000 UniTok-3.1.9/UniTok.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-07-10 05:40:28.000000 UniTok-3.1.9/UniTok.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-07-10 05:40:28.000000 UniTok-3.1.9/UniTok.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-07-10 05:40:28.000000 UniTok-3.1.9/UniTok.egg-info/requires.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-07-10 05:40:28.000000 UniTok-3.1.9/UniTok.egg-info/top_level.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-07-10 05:40:28.445151 UniTok-3.1.9/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      724 2023-07-10 05:40:10.000000 UniTok-3.1.9/setup.py
```

### Comparing `UniTok-3.1.8/PKG-INFO` & `UniTok-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.1.8
+Version: 3.1.9
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.1.8/README.md` & `UniTok-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.8/UniTok/analysis/lengths.py` & `UniTok-3.1.9/UniTok/analysis/lengths.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.8/UniTok/analysis/plot.py` & `UniTok-3.1.9/UniTok/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.8/UniTok/column.py` & `UniTok-3.1.9/UniTok/column.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.8/UniTok/meta.py` & `UniTok-3.1.9/UniTok/meta.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.8/UniTok/tok/bert_tok.py` & `UniTok-3.1.9/UniTok/tok/bert_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.8/UniTok/tok/number_tok.py` & `UniTok-3.1.9/UniTok/tok/number_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.8/UniTok/tok/split_tok.py` & `UniTok-3.1.9/UniTok/tok/split_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.8/UniTok/tok/tok.py` & `UniTok-3.1.9/UniTok/tok/tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.8/UniTok/unidep.py` & `UniTok-3.1.9/UniTok/unidep.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         json.dump(meta_data, open(os.path.join(store_dir, 'meta.data.json'), 'w'), indent=2)
 
     def reset_data(self, data):
         """
         reset data with new data
         """
         self.data = data
-        self._sample_size = len(data[self.id_col])
+        self.sample_size = self._sample_size = len(data[self.id_col])
         self._indexes = list(range(self._sample_size))
         self.cached = False
 
     """
     Deprecated properties and methods
     """
```

### Comparing `UniTok-3.1.8/UniTok/unitok.py` & `UniTok-3.1.9/UniTok/unitok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.8/UniTok/vocab.py` & `UniTok-3.1.9/UniTok/vocab.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.8/UniTok/vocabs.py` & `UniTok-3.1.9/UniTok/vocabs.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.8/UniTok.egg-info/PKG-INFO` & `UniTok-3.1.9/UniTok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.1.8
+Version: 3.1.9
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.1.8/UniTok.egg-info/SOURCES.txt` & `UniTok-3.1.9/UniTok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.8/setup.py` & `UniTok-3.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='UniTok',
-    version='3.1.8',
+    version='3.1.9',
     keywords=['token', 'tokenizer', 'bert'],
     description='Unified Tokenizer',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT Licence',
     url='https://github.com/Jyonn/UnifiedTokenizer',
     author='Jyonn Liu',
```

