# Comparing `tmp/bert-for-sequence-classification-0.0.4.tar.gz` & `tmp/bert-for-sequence-classification-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert-for-sequence-classification-0.0.4.tar", last modified: Thu Oct 13 19:52:55 2022, max compression
+gzip compressed data, was "bert-for-sequence-classification-0.0.5.tar", last modified: Mon Jul 10 06:58:24 2023, max compression
```

## Comparing `bert-for-sequence-classification-0.0.4.tar` & `bert-for-sequence-classification-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:52:55.579445 bert-for-sequence-classification-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3042 2022-10-13 19:52:55.579445 bert-for-sequence-classification-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2567 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:52:55.575446 bert-for-sequence-classification-0.0.4/bert_clf/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/bert_clf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3669 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/bert_clf/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:52:55.575446 bert-for-sequence-classification-0.0.4/bert_clf/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/bert_clf/src/BertCLF.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/bert_clf/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/bert_clf/src/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/bert_clf/src/early_stopping.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:52:55.575446 bert-for-sequence-classification-0.0.4/bert_clf/src/pandas_dataset/
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/bert_clf/src/pandas_dataset/BaseDataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2808 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/bert_clf/src/pandas_dataset/PandasDataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1884 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/bert_clf/src/pandas_dataset/SimpleDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/bert_clf/src/pandas_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4696 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/bert_clf/src/preparing_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7725 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/bert_clf/src/training_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/bert_clf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:52:55.579445 bert-for-sequence-classification-0.0.4/bert_for_sequence_classification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3042 2022-10-13 19:52:55.000000 bert-for-sequence-classification-0.0.4/bert_for_sequence_classification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-10-13 19:52:55.000000 bert-for-sequence-classification-0.0.4/bert_for_sequence_classification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 19:52:55.000000 bert-for-sequence-classification-0.0.4/bert_for_sequence_classification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-13 19:52:55.000000 bert-for-sequence-classification-0.0.4/bert_for_sequence_classification.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-13 19:52:55.000000 bert-for-sequence-classification-0.0.4/bert_for_sequence_classification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-13 19:52:55.000000 bert-for-sequence-classification-0.0.4/bert_for_sequence_classification.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-10-13 19:52:55.579445 bert-for-sequence-classification-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-10-13 19:52:44.000000 bert-for-sequence-classification-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:24.434451 bert-for-sequence-classification-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-10 06:58:24.434451 bert-for-sequence-classification-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:24.434451 bert-for-sequence-classification-0.0.5/bert_clf/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:24.434451 bert-for-sequence-classification-0.0.5/bert_clf/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/BertCLF.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/early_stopping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:24.434451 bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/BaseDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/PandasDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/SimpleDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/preparing_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/training_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:24.434451 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-10 06:58:24.000000 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-10 06:58:24.000000 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:58:24.000000 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 06:58:24.000000 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 06:58:24.000000 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 06:58:24.000000 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 06:58:24.438451 bert-for-sequence-classification-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/setup.py
```

### Comparing `bert-for-sequence-classification-0.0.4/LICENSE` & `bert-for-sequence-classification-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.4/PKG-INFO` & `bert-for-sequence-classification-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-for-sequence-classification
-Version: 0.0.4
+Version: 0.0.5
 Summary: Easy fine-tuning for BERT models
 Author: Tatiana Iazykova
 Author-email: tania_yazykova@bk.ru
 Keywords: python,bert,deep learning,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bert-for-sequence-classification-0.0.4/README.md` & `bert-for-sequence-classification-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.4/bert_clf/pipeline.py` & `bert-for-sequence-classification-0.0.5/bert_clf/pipeline.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.4/bert_clf/src/BertCLF.py` & `bert-for-sequence-classification-0.0.5/bert_clf/src/BertCLF.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         dense_outputs = self.fc(self.drop(hidden[:, 0]))
         outputs = self.act(dense_outputs)
 
         return outputs
 
     def _predict(self, text: str) -> torch.Tensor:
         inputs = self.tokenizer.encode(text, return_tensors="pt", truncation=True)
-        outputs = self(inputs)
+        outputs = self(inputs.to(self.pretrained_model.device))
         return outputs
 
     def predict(self, text: str) -> str:
         outputs = self._predict(text=text)
         pred = outputs.argmax(1).item()
         pred_text = self.mapper[pred]
         return pred_text
```

### Comparing `bert-for-sequence-classification-0.0.4/bert_clf/src/dataset.py` & `bert-for-sequence-classification-0.0.5/bert_clf/src/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 import torch
 from typing import List, Union, Tuple, Any
 import numpy as np
-from transformers.tokenization_utils_base import PreTrainedTokenizerBase
+from transformers import PreTrainedTokenizerBase
 
 
 class Dataset(torch.utils.data.Dataset):
 
     def __init__(
             self,
-            tokenizer: PreTrainedTokenizerBase,
-            maxlen: int,
             texts: Union[List[str], np.ndarray],
             targets: Union[List[Any], np.ndarray]
     ):
-        self.tokenizer = tokenizer
-        self.texts = [torch.LongTensor(self.tokenizer.encode(
-            t,
-            truncation=True,
-            max_length=maxlen
-        )) for t in texts]
-        self.texts = torch.nn.utils.rnn.pad_sequence(self.texts, batch_first=True,
-                                                     padding_value=self.tokenizer.pad_token_id)
 
+        self.texts = texts
+        self.targets = targets
         self.length = len(texts)
 
-        self.target = torch.LongTensor(targets)
-
     def __len__(self) -> int:
         return self.length
 
     def __getitem__(self, index: int) -> Tuple[torch.LongTensor, torch.LongTensor]:
         ids = self.texts[index]
-        y = self.target[index]
+        y = self.targets[index]
 
         return ids, y
+
+
+class Collator():
+
+    def __init__(self, maxlen: int, tokenizer: PreTrainedTokenizerBase):
+        self.tokenizer = tokenizer
+        self.maxlen = maxlen
+
+    def collate(self, batch: Tuple[List[str], List[int]]) -> Tuple[torch.LongTensor, torch.LongTensor]:
+        texts, targets = zip(*batch)
+
+        texts = self.tokenizer(
+            list(texts), max_length=self.maxlen, truncation=True, padding=True, return_tensors='pt')
+        targets = torch.LongTensor(targets)
+
+        return texts['input_ids'], targets
```

### Comparing `bert-for-sequence-classification-0.0.4/bert_clf/src/early_stopping.py` & `bert-for-sequence-classification-0.0.5/bert_clf/src/early_stopping.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.4/bert_clf/src/pandas_dataset/BaseDataset.py` & `bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/BaseDataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.4/bert_clf/src/pandas_dataset/PandasDataset.py` & `bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/PandasDataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.4/bert_clf/src/pandas_dataset/SimpleDataFrame.py` & `bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/SimpleDataFrame.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.4/bert_clf/src/preparing_data_utils.py` & `bert-for-sequence-classification-0.0.5/bert_clf/src/preparing_data_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 from bert_clf.src.pandas_dataset.PandasDataset import PandasDataset
 from bert_clf.src.pandas_dataset.SimpleDataFrame import SimpleDataFrame
 from typing import Dict, Any, List, Tuple, Optional, Union
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
-from bert_clf.src.dataset import Dataset
+from bert_clf.src.dataset import Dataset, Collator
 import torch
 import warnings
 
 
 def prepare_data(
         config: Dict[str, Dict[str, Any]],
 ) -> Tuple[Dict[int, str], List[str], List[str], List[int], List[int]]:
@@ -100,33 +100,33 @@
     :param valid_targets: list of targets for texts selected for evaluation
     :param config:  config with all the necessary information to set up a model
 
     :return: Dataloader  objects for bert_clf and evaluatuon
     """
 
     training_set = Dataset(
-        tokenizer=tokenizer,
         texts=train_texts,
         targets=train_targets,
-        maxlen=config['transformer_model']['maxlen']
     )
 
+    collator = Collator(maxlen=config['transformer_model']['maxlen'], tokenizer=tokenizer)
+
     training_generator = torch.utils.data.DataLoader(
         training_set,
         batch_size=config['transformer_model']['batch_size'],
-        shuffle=config['transformer_model']['shuffle']
+        shuffle=config['transformer_model']['shuffle'],
+        collate_fn=collator.collate
     )
 
     valid_set = Dataset(
-        tokenizer=tokenizer,
         texts=valid_texts,
         targets=valid_targets,
-        maxlen=config['transformer_model']['maxlen']
     )
 
     valid_generator = torch.utils.data.DataLoader(
         valid_set,
         batch_size=config['transformer_model']['batch_size'],
-        shuffle=config['transformer_model']['shuffle']
+        shuffle=config['transformer_model']['shuffle'],
+        collate_fn=collator.collate
     )
 
     return training_generator, valid_generator
```

### Comparing `bert-for-sequence-classification-0.0.4/bert_clf/src/training_utils.py` & `bert-for-sequence-classification-0.0.5/bert_clf/src/training_utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.4/bert_clf/utils.py` & `bert-for-sequence-classification-0.0.5/bert_clf/utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.4/bert_for_sequence_classification.egg-info/PKG-INFO` & `bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-for-sequence-classification
-Version: 0.0.4
+Version: 0.0.5
 Summary: Easy fine-tuning for BERT models
 Author: Tatiana Iazykova
 Author-email: tania_yazykova@bk.ru
 Keywords: python,bert,deep learning,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bert-for-sequence-classification-0.0.4/bert_for_sequence_classification.egg-info/SOURCES.txt` & `bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.4/setup.py` & `bert-for-sequence-classification-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bert-for-sequence-classification",
-    version='0.0.4',
+    version='0.0.5',
     author="Tatiana Iazykova",
     author_email="tania_yazykova@bk.ru",
     description='Easy fine-tuning for BERT models',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'bert-clf-train = bert_clf.pipeline:main',
```

