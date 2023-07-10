# Comparing `tmp/bert-for-sequence-classification-0.0.5.tar.gz` & `tmp/bert-for-sequence-classification-0.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert-for-sequence-classification-0.0.5.tar", last modified: Mon Jul 10 06:58:24 2023, max compression
+gzip compressed data, was "bert-for-sequence-classification-0.0.5a0.tar", last modified: Mon Jul 10 13:42:44 2023, max compression
```

## Comparing `bert-for-sequence-classification-0.0.5.tar` & `bert-for-sequence-classification-0.0.5a0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:24.434451 bert-for-sequence-classification-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-10 06:58:24.434451 bert-for-sequence-classification-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:24.434451 bert-for-sequence-classification-0.0.5/bert_clf/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:24.434451 bert-for-sequence-classification-0.0.5/bert_clf/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/BertCLF.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/early_stopping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:24.434451 bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/BaseDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/PandasDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/SimpleDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/preparing_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/src/training_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/bert_clf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:58:24.434451 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-10 06:58:24.000000 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-10 06:58:24.000000 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:58:24.000000 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 06:58:24.000000 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 06:58:24.000000 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 06:58:24.000000 bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 06:58:24.438451 bert-for-sequence-classification-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-10 06:58:11.000000 bert-for-sequence-classification-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/bert_clf/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/bert_clf/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/BertCLF.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/early_stopping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/BaseDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/PandasDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/SimpleDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/preparing_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/training_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-10 13:42:34.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-10 13:42:44.000000 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-10 13:42:44.000000 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:42:44.000000 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 13:42:44.000000 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 13:42:44.000000 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 13:42:44.000000 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-10 13:42:34.000000 bert-for-sequence-classification-0.0.5a0/setup.py
```

### Comparing `bert-for-sequence-classification-0.0.5/LICENSE` & `bert-for-sequence-classification-0.0.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5/PKG-INFO` & `bert-for-sequence-classification-0.0.5a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-for-sequence-classification
-Version: 0.0.5
+Version: 0.0.5a0
 Summary: Easy fine-tuning for BERT models
 Author: Tatiana Iazykova
 Author-email: tania_yazykova@bk.ru
 Keywords: python,bert,deep learning,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bert-for-sequence-classification-0.0.5/README.md` & `bert-for-sequence-classification-0.0.5a0/README.md`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5/bert_clf/pipeline.py` & `bert-for-sequence-classification-0.0.5a0/bert_clf/pipeline.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5/bert_clf/src/BertCLF.py` & `bert-for-sequence-classification-0.0.5a0/bert_clf/src/BertCLF.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,17 +39,21 @@
 
     def _predict(self, text: str) -> torch.Tensor:
         inputs = self.tokenizer.encode(text, return_tensors="pt", truncation=True)
         outputs = self(inputs.to(self.pretrained_model.device))
         return outputs
 
     def predict(self, text: str) -> str:
-        outputs = self._predict(text=text)
-        pred = outputs.argmax(1).item()
-        pred_text = self.mapper[pred]
+        self.eval()
+        with torch.no_grad():
+            outputs = self._predict(text=text)
+            pred = outputs.argmax(1).item()
+            pred_text = self.mapper[pred]
         return pred_text
 
     def predict_proba(self, text: str) -> Dict[str, float]:
-        outputs = self._predict(text=text)
-        probas = torch.nn.functional.softmax(outputs, dim=1).cpu().numpy().tolist()
-        probas_dict = {self.mapper[i]: proba for i, proba in enumerate(probas)}
+        self.eval()
+        with torch.no_grad():
+            outputs = self._predict(text=text)
+            probas = torch.nn.functional.softmax(outputs, dim=1).cpu().detach().numpy().tolist()[0]
+            probas_dict = {self.mapper[i]: proba for i, proba in enumerate(probas)}
         return probas_dict
```

### Comparing `bert-for-sequence-classification-0.0.5/bert_clf/src/dataset.py` & `bert-for-sequence-classification-0.0.5a0/bert_clf/src/dataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5/bert_clf/src/early_stopping.py` & `bert-for-sequence-classification-0.0.5a0/bert_clf/src/early_stopping.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/BaseDataset.py` & `bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/BaseDataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/PandasDataset.py` & `bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/PandasDataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5/bert_clf/src/pandas_dataset/SimpleDataFrame.py` & `bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/SimpleDataFrame.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5/bert_clf/src/preparing_data_utils.py` & `bert-for-sequence-classification-0.0.5a0/bert_clf/src/preparing_data_utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5/bert_clf/src/training_utils.py` & `bert-for-sequence-classification-0.0.5a0/bert_clf/src/training_utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5/bert_clf/utils.py` & `bert-for-sequence-classification-0.0.5a0/bert_clf/utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/PKG-INFO` & `bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-for-sequence-classification
-Version: 0.0.5
+Version: 0.0.5a0
 Summary: Easy fine-tuning for BERT models
 Author: Tatiana Iazykova
 Author-email: tania_yazykova@bk.ru
 Keywords: python,bert,deep learning,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bert-for-sequence-classification-0.0.5/bert_for_sequence_classification.egg-info/SOURCES.txt` & `bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5/setup.py` & `bert-for-sequence-classification-0.0.5a0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bert-for-sequence-classification",
-    version='0.0.5',
+    version='0.0.5a',
     author="Tatiana Iazykova",
     author_email="tania_yazykova@bk.ru",
     description='Easy fine-tuning for BERT models',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'bert-clf-train = bert_clf.pipeline:main',
```

