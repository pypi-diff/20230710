# Comparing `tmp/rotman_ncs-0.1.0a7-py3-none-any.whl.zip` & `tmp/rotman_ncs-0.1.0a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,23 @@
-Zip file size: 17823 bytes, number of entries: 14
--rw-r--r--  2.0 unx      281 b- defN 23-Jul-10 00:45 ncs/__init__.py
--rw-r--r--  2.0 unx       77 b- defN 23-Jul-10 00:45 ncs/call_strategy/__init__.py
--rw-r--r--  2.0 unx    13714 b- defN 23-Jul-10 00:45 ncs/call_strategy/strategy.py
--rw-r--r--  2.0 unx     2804 b- defN 23-Jul-10 00:45 ncs/data/__init__.py
--rw-r--r--  2.0 unx     1220 b- defN 23-Jul-10 00:45 ncs/data/downloader.py
--rw-r--r--  2.0 unx       58 b- defN 23-Jul-10 00:45 ncs/model/__init__.py
--rw-r--r--  2.0 unx      291 b- defN 23-Jul-10 00:45 ncs/model/config.py
--rw-r--r--  2.0 unx     2737 b- defN 23-Jul-10 00:45 ncs/model/inference.py
--rw-r--r--  2.0 unx     7183 b- defN 23-Jul-10 00:45 ncs/model/train.py
--rw-r--r--  2.0 unx    11355 b- defN 23-Jul-10 00:46 rotman_ncs-0.1.0a7.dist-info/LICENSE
--rw-r--r--  2.0 unx     6876 b- defN 23-Jul-10 00:46 rotman_ncs-0.1.0a7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 00:46 rotman_ncs-0.1.0a7.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Jul-10 00:46 rotman_ncs-0.1.0a7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1114 b- defN 23-Jul-10 00:46 rotman_ncs-0.1.0a7.dist-info/RECORD
-14 files, 47806 bytes uncompressed, 15979 bytes compressed:  66.6%
+Zip file size: 622532 bytes, number of entries: 21
+-rw-r--r--  2.0 unx      281 b- defN 23-Jul-10 04:32 ncs/__init__.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jul-10 04:32 ncs/call_strategy/__init__.py
+-rw-r--r--  2.0 unx   274806 b- defN 23-Jul-10 04:32 ncs/call_strategy/random_action.csv
+-rw-r--r--  2.0 unx    76695 b- defN 23-Jul-10 04:32 ncs/call_strategy/random_strategy_portfolio.parquet
+-rw-r--r--  2.0 unx   149006 b- defN 23-Jul-10 04:32 ncs/call_strategy/random_strategy_portfolio_10d.parquet
+-rw-r--r--  2.0 unx    16686 b- defN 23-Jul-10 04:32 ncs/call_strategy/random_strategy_portfolio_1d.parquet
+-rw-r--r--  2.0 unx    76219 b- defN 23-Jul-10 04:32 ncs/call_strategy/random_strategy_portfolio_5d.parquet
+-rw-r--r--  2.0 unx   279457 b- defN 23-Jul-10 04:32 ncs/call_strategy/spy_action.csv
+-rw-r--r--  2.0 unx    12797 b- defN 23-Jul-10 04:32 ncs/call_strategy/spy_strategy_portfolio.parquet
+-rw-r--r--  2.0 unx    13714 b- defN 23-Jul-10 04:32 ncs/call_strategy/strategy.py
+-rw-r--r--  2.0 unx     2804 b- defN 23-Jul-10 04:32 ncs/data/__init__.py
+-rw-r--r--  2.0 unx     1220 b- defN 23-Jul-10 04:32 ncs/data/downloader.py
+-rw-r--r--  2.0 unx       58 b- defN 23-Jul-10 04:32 ncs/model/__init__.py
+-rw-r--r--  2.0 unx      291 b- defN 23-Jul-10 04:32 ncs/model/config.py
+-rw-r--r--  2.0 unx     2737 b- defN 23-Jul-10 04:32 ncs/model/inference.py
+-rw-r--r--  2.0 unx     7183 b- defN 23-Jul-10 04:32 ncs/model/train.py
+-rw-r--r--  2.0 unx    11355 b- defN 23-Jul-10 04:33 rotman_ncs-0.1.0a8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7552 b- defN 23-Jul-10 04:33 rotman_ncs-0.1.0a8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 04:33 rotman_ncs-0.1.0a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-10 04:33 rotman_ncs-0.1.0a8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1852 b- defN 23-Jul-10 04:33 rotman_ncs-0.1.0a8.dist-info/RECORD
+21 files, 934886 bytes uncompressed, 619498 bytes compressed:  33.7%
```

## zipnote {}

```diff
@@ -1,13 +1,34 @@
 Filename: ncs/__init__.py
 Comment: 
 
 Filename: ncs/call_strategy/__init__.py
 Comment: 
 
+Filename: ncs/call_strategy/random_action.csv
+Comment: 
+
+Filename: ncs/call_strategy/random_strategy_portfolio.parquet
+Comment: 
+
+Filename: ncs/call_strategy/random_strategy_portfolio_10d.parquet
+Comment: 
+
+Filename: ncs/call_strategy/random_strategy_portfolio_1d.parquet
+Comment: 
+
+Filename: ncs/call_strategy/random_strategy_portfolio_5d.parquet
+Comment: 
+
+Filename: ncs/call_strategy/spy_action.csv
+Comment: 
+
+Filename: ncs/call_strategy/spy_strategy_portfolio.parquet
+Comment: 
+
 Filename: ncs/call_strategy/strategy.py
 Comment: 
 
 Filename: ncs/data/__init__.py
 Comment: 
 
 Filename: ncs/data/downloader.py
@@ -21,23 +42,23 @@
 
 Filename: ncs/model/inference.py
 Comment: 
 
 Filename: ncs/model/train.py
 Comment: 
 
-Filename: rotman_ncs-0.1.0a7.dist-info/LICENSE
+Filename: rotman_ncs-0.1.0a8.dist-info/LICENSE
 Comment: 
 
-Filename: rotman_ncs-0.1.0a7.dist-info/METADATA
+Filename: rotman_ncs-0.1.0a8.dist-info/METADATA
 Comment: 
 
-Filename: rotman_ncs-0.1.0a7.dist-info/WHEEL
+Filename: rotman_ncs-0.1.0a8.dist-info/WHEEL
 Comment: 
 
-Filename: rotman_ncs-0.1.0a7.dist-info/top_level.txt
+Filename: rotman_ncs-0.1.0a8.dist-info/top_level.txt
 Comment: 
 
-Filename: rotman_ncs-0.1.0a7.dist-info/RECORD
+Filename: rotman_ncs-0.1.0a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rotman_ncs-0.1.0a7.dist-info/LICENSE` & `rotman_ncs-0.1.0a8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rotman_ncs-0.1.0a7.dist-info/METADATA` & `rotman_ncs-0.1.0a8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotman-ncs
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: UoT Rotman NLP Case Study
 Home-page: https://github.com/colingwuyu/rotman_ncs.git
 Author: Zeyu Colin Wang
 Author-email: colinzeyu.wang@utoronto.ca
 Keywords: NLP,Case Study,UoT,UoT Rotman,Machine Learning,Investing
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -119,8 +119,25 @@
 
 # Generate benchmark strategy report
 ncs.demo_benchmark(strategy='random', holding_period=5)
 ```
 
 The key dataset used in the case study is the `call_statements` DataFrame, which contains unique identifiers (`statement_uid`, `call_uid`), as well as text data (`text`, `clean_text`). The `text` field is original call transcript and the `clean_text` field is processed by several text cleaning steps. Apply different NLP models to convert them into numeric features that can be consumed by the model training functions. These features are then used to inform the investment strategies with the trained model.
 
+## Usage and Examples
+
+Please refer to the following notebooks for detailed examples and usage instructions:
+
+- [TF-IDF Solution Notebook](https://colab.research.google.com/drive/1JYQK1IfBEBkOKRbAnNChC-aZrQsUcfGu?usp=sharing)
+- Word2Vec Solution (Coming Soon)
+- BERT Solution (Coming Soon)
+- LLM (Language Model) Solution (Coming Soon)
+
+These notebooks demonstrate how to utilize different NLP techniques for processing text data and building investment strategies.
+
+Make sure to follow the instructions provided in each notebook for proper setup and execution of the code.
+
+If you have any questions or need further assistance, please feel free to reach out.
+
+Happy coding!
+
 ## Enjoy the Learning and Investing 🥳
```

