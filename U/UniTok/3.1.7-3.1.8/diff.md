# Comparing `tmp/UniTok-3.1.7.tar.gz` & `tmp/UniTok-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniTok-3.1.7.tar", last modified: Fri Apr 21 13:00:31 2023, max compression
+gzip compressed data, was "UniTok-3.1.8.tar", last modified: Mon Jul 10 05:28:57 2023, max compression
```

## Comparing `UniTok-3.1.7.tar` & `UniTok-3.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 13:00:31.608036 UniTok-3.1.7/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-21 13:00:31.607920 UniTok-3.1.7/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.1.7/README.md
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 13:00:31.604503 UniTok-3.1.7/UniTok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.1.7/UniTok/__init__.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 13:00:31.605760 UniTok-3.1.7/UniTok/analysis/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.1.7/UniTok/analysis/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.1.7/UniTok/analysis/lengths.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.1.7/UniTok/analysis/plot.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.1.7/UniTok/cols.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     3787 2023-04-21 12:19:35.000000 UniTok-3.1.7/UniTok/column.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.1.7/UniTok/global_setting.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     4288 2023-04-20 08:16:56.000000 UniTok-3.1.7/UniTok/meta.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 13:00:31.607633 UniTok-3.1.7/UniTok/tok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.1.7/UniTok/tok/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      911 2023-04-21 12:17:40.000000 UniTok-3.1.7/UniTok/tok/bert_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.1.7/UniTok/tok/ent_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.1.7/UniTok/tok/id_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1442 2023-04-21 12:17:40.000000 UniTok-3.1.7/UniTok/tok/number_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.1.7/UniTok/tok/seq_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.1.7/UniTok/tok/split_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1697 2023-04-21 12:21:10.000000 UniTok-3.1.7/UniTok/tok/tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8798 2023-04-21 12:56:42.000000 UniTok-3.1.7/UniTok/unidep.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6665 2023-04-21 13:00:13.000000 UniTok-3.1.7/UniTok/unitok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8788 2023-04-21 12:18:43.000000 UniTok-3.1.7/UniTok/vocab.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1532 2023-04-21 12:42:39.000000 UniTok-3.1.7/UniTok/vocabs.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 13:00:31.605142 UniTok-3.1.7/UniTok.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-21 13:00:31.000000 UniTok-3.1.7/UniTok.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-04-21 13:00:31.000000 UniTok-3.1.7/UniTok.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-04-21 13:00:31.000000 UniTok-3.1.7/UniTok.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-04-21 13:00:31.000000 UniTok-3.1.7/UniTok.egg-info/requires.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-04-21 13:00:31.000000 UniTok-3.1.7/UniTok.egg-info/top_level.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-04-21 13:00:31.608067 UniTok-3.1.7/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      724 2023-04-21 13:00:26.000000 UniTok-3.1.7/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:28:57.110200 UniTok-3.1.8/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-07-10 05:28:57.110082 UniTok-3.1.8/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.1.8/README.md
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:28:57.106563 UniTok-3.1.8/UniTok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.1.8/UniTok/__init__.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:28:57.107864 UniTok-3.1.8/UniTok/analysis/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.1.8/UniTok/analysis/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.1.8/UniTok/analysis/lengths.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.1.8/UniTok/analysis/plot.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.1.8/UniTok/cols.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     3787 2023-04-21 12:19:35.000000 UniTok-3.1.8/UniTok/column.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.1.8/UniTok/global_setting.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     4358 2023-07-10 05:28:17.000000 UniTok-3.1.8/UniTok/meta.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:28:57.109772 UniTok-3.1.8/UniTok/tok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.1.8/UniTok/tok/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      911 2023-04-21 12:17:40.000000 UniTok-3.1.8/UniTok/tok/bert_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.1.8/UniTok/tok/ent_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.1.8/UniTok/tok/id_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1442 2023-04-21 12:17:40.000000 UniTok-3.1.8/UniTok/tok/number_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.1.8/UniTok/tok/seq_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.1.8/UniTok/tok/split_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1697 2023-04-21 12:21:10.000000 UniTok-3.1.8/UniTok/tok/tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     9129 2023-07-10 05:28:17.000000 UniTok-3.1.8/UniTok/unidep.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6665 2023-04-21 13:00:13.000000 UniTok-3.1.8/UniTok/unitok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8788 2023-04-21 12:18:43.000000 UniTok-3.1.8/UniTok/vocab.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1685 2023-07-10 05:17:38.000000 UniTok-3.1.8/UniTok/vocabs.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-07-10 05:28:57.107183 UniTok-3.1.8/UniTok.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-07-10 05:28:57.000000 UniTok-3.1.8/UniTok.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-07-10 05:28:57.000000 UniTok-3.1.8/UniTok.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-07-10 05:28:57.000000 UniTok-3.1.8/UniTok.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-07-10 05:28:57.000000 UniTok-3.1.8/UniTok.egg-info/requires.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-07-10 05:28:57.000000 UniTok-3.1.8/UniTok.egg-info/top_level.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-07-10 05:28:57.110235 UniTok-3.1.8/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      724 2023-07-10 05:28:17.000000 UniTok-3.1.8/setup.py
```

### Comparing `UniTok-3.1.7/PKG-INFO` & `UniTok-3.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.1.7
+Version: 3.1.8
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.1.7/README.md` & `UniTok-3.1.8/README.md`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.7/UniTok/analysis/lengths.py` & `UniTok-3.1.8/UniTok/analysis/lengths.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.7/UniTok/analysis/plot.py` & `UniTok-3.1.8/UniTok/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.7/UniTok/column.py` & `UniTok-3.1.8/UniTok/column.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.7/UniTok/meta.py` & `UniTok-3.1.8/UniTok/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,20 @@
         if self.list:
             info['max_length'] = self.max_length
             info['padding'] = self.padding
         return info
 
 
 class Voc:
-    def __init__(self, name, size, cols, store_dir):
+    def __init__(self, name, size, cols, store_dir, vocab=None):
         self.name: str = name
         self.size: int = size
         self.cols: List[Union[Col, str]] = cols
         self.store_dir = store_dir
+        self.vocab = vocab
 
     def __eq__(self, other):
         return self.name == other.name and self.size == other.size
 
     def get_info(self):
         return {
             'size': self.size,
@@ -45,19 +46,21 @@
         cols = self.cols.copy()
         for col in other.cols:
             for _col in cols:
                 if col.name == _col.name:
                     break
             else:
                 cols.append(col)
+
         return Voc(
             name=self.name,
             size=self.size,
             cols=cols,
-            store_dir=self.store_dir
+            store_dir=self.store_dir,
+            vocab=self.vocab
         )
 
 
 class Meta:
     VER = 'UniDep-2.0'
 
     def __init__(self, store_dir):
```

### Comparing `UniTok-3.1.7/UniTok/tok/bert_tok.py` & `UniTok-3.1.8/UniTok/tok/bert_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.7/UniTok/tok/number_tok.py` & `UniTok-3.1.8/UniTok/tok/number_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.7/UniTok/tok/split_tok.py` & `UniTok-3.1.8/UniTok/tok/split_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.7/UniTok/tok/tok.py` & `UniTok-3.1.8/UniTok/tok/tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.7/UniTok/unidep.py` & `UniTok-3.1.8/UniTok/unidep.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,16 @@
         if self.sample_size != self._sample_size:
             self.print('resize sample_size to', self._sample_size)
             self.sample_size = self._sample_size
 
         self.vocabs = Vocabs()
         for vocab_name in self.vocs:
             self.vocabs.append(Vocab(name=vocab_name).load(self.store_dir))
+        for voc in self.vocs:
+            self.vocs[voc].vocab = self.vocabs[voc]
         self.id2index = self.vocabs[self.id_voc.name].o2i
 
         self._indexes = list(range(self.sample_size))
         self.unions = dict()  # type: Dict[str, List[UniDep]]
 
     def print(self, *args, **kwargs):
         """
@@ -218,14 +220,23 @@
         for col_name in data:
             data[col_name] = np.array(data[col_name])
         np.save(os.path.join(store_dir, 'data.npy'), data, allow_pickle=True)
 
         meta_data = self.meta.get_info()
         json.dump(meta_data, open(os.path.join(store_dir, 'meta.data.json'), 'w'), indent=2)
 
+    def reset_data(self, data):
+        """
+        reset data with new data
+        """
+        self.data = data
+        self._sample_size = len(data[self.id_col])
+        self._indexes = list(range(self._sample_size))
+        self.cached = False
+
     """
     Deprecated properties and methods
     """
 
     @property
     def meta_data(self):
         warnings.warn('meta_data is deprecated, '
```

### Comparing `UniTok-3.1.7/UniTok/unitok.py` & `UniTok-3.1.8/UniTok/unitok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.7/UniTok/vocab.py` & `UniTok-3.1.8/UniTok/vocab.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.7/UniTok/vocabs.py` & `UniTok-3.1.8/UniTok/vocabs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import warnings
 
+from .meta import Col, Voc
+
 from .vocab import Vocab
 
 
 class Vocabs(dict):
     def __init__(self):
         super().__init__()
         self.cols = {}
@@ -45,8 +47,12 @@
             cols=self.cols[vocab.name],
         ) for vocab in self.values()}
 
     def __call__(self, name) -> Vocab:
         return self[name]
 
     def __getitem__(self, item) -> Vocab:
+        if isinstance(item, Col):
+            item = item.voc
+        if isinstance(item, Voc):
+            item = item.name
         return super().__getitem__(item)
```

### Comparing `UniTok-3.1.7/UniTok.egg-info/PKG-INFO` & `UniTok-3.1.8/UniTok.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.1.7
+Version: 3.1.8
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.1.7/UniTok.egg-info/SOURCES.txt` & `UniTok-3.1.8/UniTok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.7/setup.py` & `UniTok-3.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='UniTok',
-    version='3.1.7',
+    version='3.1.8',
     keywords=['token', 'tokenizer', 'bert'],
     description='Unified Tokenizer',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT Licence',
     url='https://github.com/Jyonn/UnifiedTokenizer',
     author='Jyonn Liu',
```

